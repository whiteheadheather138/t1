代发 wailian999

Ruby: arr.sort
来源：http://hfp.gotoacloud.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://nfh.yj20258888.top

[N03] 快速排序（分治示例）
来源：http://slp.tarul.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://gzb.nwbrower.top

PHP:  // 递归实现，或用 usort
来源：http://qip.sxryk.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hmd.iojbl.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xtm.snrcjt.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://zfu.xuanzx.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://bub.xingfuxueyuan.xyz

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://xpw.haohaochexian.top

C#:   // 手写递归，或 Array.Sort
来源：http://hxi.fengsongda.top

[N04] 斐波那契数列
来源：http://gad.guannengcc.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://knv.snrcjt.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://upb.iojbl.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://oxw.ivvv.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pkh.tarul.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://jcx.yuxming.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mvf.ydzc1.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://sdi.yj202588.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://yfa.zhaomingkeji.xyz

[N05] 最大公约数
来源：http://ivj.nwbrower.top

Py:   math.gcd(a, b)
来源：http://dns.snrcjt.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://xbx.sjlbkw.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hpy.dianchejie.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://std.chenlongwang.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://feu.cucudq.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://kgu.ydzc1.top

Ruby: a.gcd(b)
来源：http://umw.xuetiantiany.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://rer.meibo888.top

[N06] 判断回文字符串
来源：http://pua.yangfankeji.com

Py:   s == s[::-1]
来源：http://fwb.zhijiandao.cn

PHP:  $s === strrev($s);
来源：http://vwa.0kj1m.cn

JS:   s === [...s].reverse().join("")
来源：http://fac.snrcjt.cn

TS:   s === [...s].reverse().join("")
来源：http://qsz.jinyuanbaomall.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://shp.xziqi.cn

Go:   // 双指针从两端比较
来源：http://sfu.fktsv.cn

Ruby: s == s.reverse
来源：http://quk.shanyushiyangtech.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://wjd.fzhhl.top

[N07] 两数之和（返回下标）
来源：http://ihq.aizwys.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://vsz.yanxiufei.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://syu.xingfuxueyuan.xyz

JS:   // 手写 Map：map.set(v, i)
来源：http://vox.0kj1m.cn

TS:   // 手写 Map<string, number>
来源：http://mcx.cheryme.top

Java: // 手写 HashMap
来源：http://cqq.zhengqikj.top

Go:   // 手写 map[int]int
来源：http://avv.yongpay.top

Ruby: // 手写 Hash
来源：http://jza.xinyue.icu

C#:   // 手写 Dictionary<int, int>
来源：http://ewk.tian-w.cn

[N08] 生成全排列
来源：http://jao.yuxming.cn

Py:   itertools.permutations(arr)
来源：http://khm.xuanzx.com

PHP:  // 手写递归交换
来源：http://bdc.aibaodan.cn

JS:   // 手写回溯递归
来源：http://vok.nwbrower.top

TS:   // 手写回溯递归
来源：http://opx.gzhubu.top

Java: // 手写回溯递归
来源：http://lpo.xziqi.cn

Go:   // 手写回溯递归
来源：http://ino.aizwys.cn

Ruby: arr.permutation.to_a
来源：http://zvo.zhixingplan.top

C#:   // 手写回溯递归
来源：http://tkq.fengsongda.top

[N09] 栈与队列
来源：http://kmf.xylfe.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://kdy.fzhhl.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hah.cashguo.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://vqh.xziqi.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mwb.jinyuanbaomall.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wqw.cucudq.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://yta.fehbvm.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://tlr.tianlin.xyz

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://nrr.hfpthk.cn

[N10] 链表节点定义
来源：http://wsf.c1oappe.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ejq.wangdashe.top

PHP:  class Node { public $v; public $next = null; }
来源：http://qlf.ppjwa.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://yll.jlsjyb.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mgm.zhengqikj.top

Java: class Node { int v; Node next; }
来源：http://rwq.cucudq.cn

Go:   type Node struct { V int; Next *Node }
来源：http://jin.nanxinkj.top

Ruby: Node = Struct.new(:v, :next)
来源：http://exv.tianlin.xyz

C#:   class Node { public int V; public Node? Next; }
来源：http://ann.smart0.xyz

[N11] 二叉树中序遍历
来源：http://ink.jqgufenzy.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://bar.9152youxi.cn

PHP:  // 手写递归函数
来源：http://mig.hongshengwenyu.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://czc.hcnkem.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://atb.bjfxy.top

Java: // 手写递归
来源：http://izq.sxryk.cn

Go:   // 手写递归
来源：http://ymd.zhaomingkeji.xyz

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://htl.fanxiaobao.xyz

C#:   // 手写递归
来源：http://tdu.jqgfzy.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://cvq.jqgufenzy.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://xsk.guannengcc.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ltg.yanxiufei.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jky.xuanzx.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hsz.sufxvd.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ity.xziqi.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hwr.chenlongwang.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://cyn.xuetiantiany.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://lio.fehbvm.com

================================================================================
来源：http://mcl.tanke756.top

O. 并发与异步
来源：http://bei.ywan-chungtsiang.top

================================================================================
来源：http://lqd.sxryk.cn

[O01] 启动一个线程
来源：http://hht.52xcode.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wex.chenlongwang.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://jmn.dashuyun.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hsy.haohaochexian.top

TS:   // 同 JS
来源：http://ksv.nwbrower.top

Java: new Thread(() -> f()).start()
来源：http://rqb.guannengcc.top

Go:   go f()
来源：http://olo.ywan-chungtsiang.top

Ruby: Thread.new { f }
来源：http://wpb.xylfe.cn

C#:   Task.Run(() => F());
来源：http://snd.gogol.net.cn

[O02] 使用线程池
来源：http://fxf.nwbrower.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://zwm.hnxiangtu.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://yze.zhengqikj.top

JS:   // worker_threads 线程池
来源：http://wzx.quarkkingdee.top

TS:   // worker_threads 线程池
来源：http://mec.fengsongda.top

Java: Executors.newFixedThreadPool(4)
来源：http://zgu.ivvv.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://cjs.yangfankeji.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://imp.chenzaomai.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://lae.jqgfzy.top

[O03] 加锁保护共享数据
来源：http://jal.ywan-chungtsiang.top

Py:   with lock: shared += 1
来源：http://ysk.jqgufenzy.top

PHP:  // 用 flock() 做文件锁
来源：http://ajq.haohaochexian.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://nzc.shanyushiyangtech.top

TS:   // 同 JS
来源：http://jez.shanyushiyangtech.top

Java: synchronized (this) { shared++; }
来源：http://pfe.daxiang520.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://dbx.shanyushiyangtech.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://uze.cdnleiting.top

C#:   lock (gate) { shared++; }
来源：http://rjl.fehbvm.com

[O04] 定义异步函数并等待
来源：http://iuu.xuetiantiany.cn

Py:   async def f():⏎    await g()
来源：http://ciu.yj20258888.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ewk.havefunace.top

JS:   async function f() { await g(); }
来源：http://sav.aizwys.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://yba.jqgfzy.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://dhp.zhixingplan.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://vdv.jinghuilouyu.cn

Ruby: # 用 Fiber 或 async gem
来源：http://nyk.xziqi.cn

C#:   async Task F() { await G(); }
来源：http://swn.ppjwa.cn

[O05] 并发执行并等待全部完成
来源：http://hxe.cdnleiting.top

Py:   asyncio.gather(*tasks)
来源：http://ohe.9152youxi.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://jpy.sweek.top

JS:   await Promise.all(tasks)
来源：http://uqp.c1oappe.top

TS:   await Promise.all(tasks)
来源：http://jdb.tian-w.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://kjn.tanke756.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://zac.fanxiaobao.xyz

Ruby: threads.map(&:join)
来源：http://fhg.gotoacloud.top

C#:   await Task.WhenAll(t1, t2)
来源：http://fvs.aizwys.cn

[O06] 使用进程池
来源：http://wil.fanxiaobao.xyz

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://feq.wangshuangyany.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://zwf.jianghu66.top

JS:   // child_process / cluster 模块
来源：http://pws.dianchejie.cn

TS:   // child_process / cluster 模块
来源：http://mem.smart0.xyz

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://gdb.havefunace.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://faj.yvedp.cn

Ruby: // fork 块
来源：http://thl.smart0.xyz

C#:   Parallel.For
来源：http://hqj.snrcjt.cn

================================================================================
来源：http://ffm.vehdjk.com

P. 常用工具函数
来源：http://ktw.gogol.net.cn

================================================================================
来源：http://maw.gzhubu.top

[P01] 生成 UUID
来源：http://hbo.jlsjyb.cn

Py:   str(uuid.uuid4())
来源：http://rvb.bbcook.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://rsa.nanxinkj.top

JS:   crypto.randomUUID()
来源：http://web.birdmap.top

TS:   crypto.randomUUID()
来源：http://onf.yanxiufei.cn

Java: UUID.randomUUID().toString()
来源：http://nvw.9152youxi.cn

Go:   // 用 github.com/google/uuid
来源：http://ygu.xuanzx.com

Ruby: SecureRandom.uuid
来源：http://dqv.aibaodan.cn

C#:   Guid.NewGuid().ToString()
来源：http://uic.ydjk.org.cn

[P02] MD5 / SHA256 摘要
来源：http://prv.cqqwz.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://qzp.shzxlz.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://gjd.snrcjt.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://qdu.sysykeji.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mgq.sweek.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ojk.cqqwz.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://fwf.gotoacloud.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hmx.hfpthk.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://imz.jiagoushi.top

[P03] 生成短随机字符串
来源：http://hso.ywan-chungtsiang.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://xbk.ctjpmb.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://opu.ehwqpu.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://cak.yj20258.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zap.zhijiandao.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://dfw.pengpengdd.cyou

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://upk.chenjidiqi.icu

Ruby: SecureRandom.alphanumeric(16)
来源：http://yyg.jinqigfzy.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ere.shangyingyoupin.top

[P04] 求长度
来源：http://rzr.meibo888.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://joj.xylfe.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zfc.meibo888.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://oep.jinghuilouyu.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dgc.ppjwa.cn

Java: list.size();  map.size();  s.length()
来源：http://slt.kuanghao11.cn

Go:   len(arr);  len(m)
来源：http://vzc.andypj.xyz

Ruby: x.length;  x.size
来源：http://ioq.hysaishi.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://jya.bjfxy.top

[P05] 判断两个对象内容是否相等
来源：http://rlh.haohaochexian.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://rtv.yfazqb.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hfi.tanke756.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://uva.ppjwa.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://biw.jinyuanbaomall.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://dzu.nanxuanxn.top

Go:   reflect.DeepEqual(a, b)
来源：http://zyw.sweek.top

Ruby: a == b
来源：http://jgp.hongshengwenyu.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ghr.wangshuangyany.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hdq.ybcxt.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wnm.cqqwz.cn

PHP:  if (empty($x)) {}
来源：http://tef.hysaishi.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://foq.yuxming.cn

TS:   if (x == null) {}
来源：http://llc.meibo888.top

Java: if (x == null || x.isEmpty()) {}
来源：http://kvy.snrcjt.cn

Go:   if x == nil {}
来源：http://ddu.dashuyun.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://bby.wangdashe.top

C#:   if (x is null) {}
来源：http://qyo.sjlbkw.cn

[P07] 防抖与节流
来源：http://rqp.hfpthk.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mlg.hesvh.cn

PHP:  // 手写时间戳比较
来源：http://rwv.zdbjq.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mqw.ehwqpu.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gib.bbcook.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://udx.feifeiyinyue.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://cxb.gaohongyu789.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://zuq.feifeiyinyue.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mvx.hcnkem.com

[P08] 处理浮点精度问题
来源：http://vzk.yj202588.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://avy.nanxinkj.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hfd.wangdashe.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://cxt.yongpay.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ucy.feifeiyinyue.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://xyb.316326.xyz

Go:   math/big.Float，或全部换算成整数分再算
来源：http://pwf.xylfe.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://zrm.aibaodan.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://vdh.shangyingyoupin.top

================================================================================
来源：http://umx.jinqigufen.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://dbb.yj20258888.top

================================================================================
来源：http://gvn.ydjk.org.cn

[Q01] 创建表
来源：http://mbd.yongpay.top

CREATE TABLE users (
来源：http://gom.daria6918.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://toz.c1oappe.top

name VARCHAR(50) NOT NULL,
来源：http://jbf.hywenlv.cn

email VARCHAR(100) UNIQUE,
来源：http://ggg.shanyushiyangtech.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://npq.yonumen.top

);
来源：http://mxb.chenlongwang.top

[Q02] 创建带外键的表
来源：http://ilj.kuanghao11.cn

CREATE TABLE orders (
来源：http://eol.cheryme.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wav.cqqwz.cn

user_id INT NOT NULL,
来源：http://ahs.chenzaomai.com

amount DECIMAL(10, 2),
来源：http://pvn.hywenlv.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://kyc.yonumen.top

);
来源：http://uxc.vqdsnc.cn

[Q03] 增加列
来源：http://lpa.xingfuxueyuan.xyz

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hjh.tianlin.xyz

[Q04] 修改列类型
来源：http://drz.epnwcf.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://bov.smart0.xyz

[Q05] 重命名列
来源：http://khc.meibo888.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://qgv.shanyushiyangkeji.top

[Q06] 删除列
来源：http://euq.fanxiaobao.xyz

ALTER TABLE users DROP COLUMN age;
来源：http://lsy.shanyushiyangkeji.top

[Q07] 删除表
来源：http://lzv.epnwcf.com

DROP TABLE IF EXISTS orders;
来源：http://etl.zhaomingkeji.xyz

[Q08] 创建普通索引
来源：http://axk.shzxlz.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://guu.hesvh.cn

[Q09] 创建唯一索引
来源：http://bsp.meibo888.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://yct.epnwcf.com

[Q10] 插入单行
来源：http://ghs.bbcook.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hcl.zhaomingkeji.xyz

[Q11] 一次插入多行
来源：http://awh.quarkkingdee.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://uhk.shangyingyoupin.top

[Q12] 插入后取自增 ID
来源：http://gjs.daxiang520.top

INSERT INTO users (name) VALUES ('C');
来源：http://sfx.vqdsnc.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://jyl.zhiwuduotai.top

[Q13] 忽略重复插入
来源：http://llw.yvedp.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://zsp.hcnkem.com

[Q14] 存在则更新（upsert）
来源：http://nsj.hfpthk.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hmg.hammf.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://amj.guowangkeji.top

[Q15] 查询全部
来源：http://vlo.jianghu66.top

SELECT * FROM users;
来源：http://mbf.shangyingyoupin.top

[Q16] 查询指定列
来源：http://jro.zhijiandao.cn

SELECT id, name FROM users;
来源：http://ujj.52xcode.cn

[Q17] 条件查询
来源：http://kwa.fehbvm.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://uot.cheryme.top

[Q18] 模糊匹配
来源：http://mrc.52xcode.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mqu.jiagoushi.top

[Q19] 范围查询
来源：http://alm.zhijiandao.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://qgb.sweek.top

[Q20] IN 列表
来源：http://edn.cqqwz.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://prl.fengsongda.top

[Q21] 空值判断
来源：http://gjo.jyoumei.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://rhu.xziqi.cn

[Q22] 排序
来源：http://ufs.havefunace.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://vka.fzhhl.top

[Q23] 分页
来源：http://dtv.316326.xyz

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://irg.xuetiantiany.cn

[Q24] 去重
来源：http://ulu.c1oappe.top

SELECT DISTINCT city FROM users;
来源：http://kwb.shuidangran.top

[Q25] 只取前 N 条
来源：http://toa.sweek.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://tuc.uphjek.com

[Q26] 计数
来源：http://cjw.zhixingplan.top

SELECT COUNT(*) FROM users;
来源：http://upc.xingfuxueyuan.xyz

[Q27] 条件计数
来源：http://nul.zhongyouzk.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mbf.nwbrower.top

[Q28] 求和与平均
来源：http://pdd.pycfn.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://kbb.sxryk.cn

[Q29] 最大最小值
来源：http://lxm.yj20258.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://lll.cheryme.top

[Q30] 分组统计
来源：http://bqv.birdmap.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://too.gaohongyu789.top

[Q31] 分组后过滤
来源：http://cyz.hfpthk.cn


<!-- 参考信息 -->