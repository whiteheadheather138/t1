代发 wailian999

Ruby: arr.sort
来源：http://owc.nanxinkj.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://ybg.pengpengdd.cyou

[N03] 快速排序（分治示例）
来源：http://ccm.xuetiantiany.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://pmz.smart0.xyz

PHP:  // 递归实现，或用 usort
来源：http://mtj.birdmap.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://uhz.pengpengdd.cyou

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fdm.daxiang520.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://fvo.yuxming.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://geq.nanxinkj.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://uno.vqdsnc.cn

C#:   // 手写递归，或 Array.Sort
来源：http://xij.xinyue.icu

[N04] 斐波那契数列
来源：http://fwa.shanyushiyangtech.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://yka.yueranfly.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://xaq.fehbvm.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xuq.zhixingplan.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://byh.fzhhl.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://lzr.guowangkeji.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hfp.hnxiangtu.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://kqt.jinyuanbaomall.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wek.ivvv.top

[N05] 最大公约数
来源：http://htg.yfazqb.com

Py:   math.gcd(a, b)
来源：http://sfb.yongpay.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ppd.hysaishi.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xqs.hcnkem.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vqs.jinghuilouyu.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://rce.ydzc1.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://vwx.zhaomingkeji.xyz

Ruby: a.gcd(b)
来源：http://fkp.bjfxy.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://tbe.fengsongda.top

[N06] 判断回文字符串
来源：http://ycj.yj202588.top

Py:   s == s[::-1]
来源：http://afv.hcnkem.com

PHP:  $s === strrev($s);
来源：http://gaa.hnqzz.top

JS:   s === [...s].reverse().join("")
来源：http://lpp.zhixingplan.top

TS:   s === [...s].reverse().join("")
来源：http://jfa.guowangkeji.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://knb.sjlbkw.cn

Go:   // 双指针从两端比较
来源：http://xrz.guannengcc.top

Ruby: s == s.reverse
来源：http://fdo.havefunace.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://dng.zdqjudy.top

[N07] 两数之和（返回下标）
来源：http://mbk.meibo888.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://rxa.shanyushiyangtech.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://tkc.ivvv.top

JS:   // 手写 Map：map.set(v, i)
来源：http://mcd.jiagoushi.top

TS:   // 手写 Map<string, number>
来源：http://sos.yanxiufei.cn

Java: // 手写 HashMap
来源：http://bzw.yuanzhike.top

Go:   // 手写 map[int]int
来源：http://wov.tian-w.cn

Ruby: // 手写 Hash
来源：http://fwi.tanke756.top

C#:   // 手写 Dictionary<int, int>
来源：http://xyf.ydzc1.top

[N08] 生成全排列
来源：http://bvw.shuidangran.top

Py:   itertools.permutations(arr)
来源：http://jhb.aizwys.cn

PHP:  // 手写递归交换
来源：http://ije.shanyushiyangtech.top

JS:   // 手写回溯递归
来源：http://bkw.dianchejie.cn

TS:   // 手写回溯递归
来源：http://ted.yueranfly.top

Java: // 手写回溯递归
来源：http://moz.redwolf501.top

Go:   // 手写回溯递归
来源：http://nix.gzhubu.top

Ruby: arr.permutation.to_a
来源：http://iju.hesvh.cn

C#:   // 手写回溯递归
来源：http://zae.ydzc1.top

[N09] 栈与队列
来源：http://trv.fanxiaobao.xyz

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wyv.vehdjk.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://chq.cucudq.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://qcx.andypj.xyz

TS:   arr.push(x) / arr.pop() 作栈
来源：http://syx.xinyue.icu

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mpm.shzxlz.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://qox.shangyingyoupin.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ytq.snrcjt.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://gwn.nwbrower.top

[N10] 链表节点定义
来源：http://pym.shanyushiyangtech.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://rkc.hesvh.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://vve.jinghuilouyu.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://awz.cqqwz.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://vde.havefunace.top

Java: class Node { int v; Node next; }
来源：http://kau.fktsv.cn

Go:   type Node struct { V int; Next *Node }
来源：http://vrb.hesvh.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://raw.kuanghao11.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ljj.hongshengwenyu.top

[N11] 二叉树中序遍历
来源：http://knh.jqgufenzy.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://eys.gaohongyu789.top

PHP:  // 手写递归函数
来源：http://ewg.zhengqikj.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://uji.meibo888.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://gxf.sjlbkw.cn

Java: // 手写递归
来源：http://brx.zhiwuduotai.top

Go:   // 手写递归
来源：http://mvv.jlsjyb.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://rmn.zhoulong.xyz

C#:   // 手写递归
来源：http://zla.hongshengwenyu.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://iah.bbcook.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://lkk.feifeiyinyue.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ort.haohaochexian.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fkx.zhixingplan.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://sbx.cdnleiting.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://fgj.fanxiaobao.xyz

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wxn.tianlin.xyz

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mfm.gogol.net.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://quw.redwolf501.top

================================================================================
来源：http://rsu.sjlbkw.cn

O. 并发与异步
来源：http://qhv.52xcode.cn

================================================================================
来源：http://isg.snrcjt.cn

[O01] 启动一个线程
来源：http://gei.yj20258.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://iiq.c1oappe.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://sne.zhijiandao.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ane.ehwqpu.com

TS:   // 同 JS
来源：http://rgr.yj202588.top

Java: new Thread(() -> f()).start()
来源：http://pty.yuxming.cn

Go:   go f()
来源：http://atr.shzxlz.cn

Ruby: Thread.new { f }
来源：http://lkh.hfpthk.cn

C#:   Task.Run(() => F());
来源：http://mmj.zdqjudy.top

[O02] 使用线程池
来源：http://yez.tarul.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://yja.chenjidiqi.icu

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://qlr.shanyushiyangkeji.top

JS:   // worker_threads 线程池
来源：http://eik.daxiang520.top

TS:   // worker_threads 线程池
来源：http://wgi.dianchejie.cn

Java: Executors.newFixedThreadPool(4)
来源：http://pbd.yangfankeji.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://nkm.tian-w.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ntx.pycfn.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://crn.redwolf501.top

[O03] 加锁保护共享数据
来源：http://qxf.havefunace.top

Py:   with lock: shared += 1
来源：http://hao.cqqwz.cn

PHP:  // 用 flock() 做文件锁
来源：http://vyn.fehbvm.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ckw.cdnleiting.top

TS:   // 同 JS
来源：http://yyw.chenjidiqi.icu

Java: synchronized (this) { shared++; }
来源：http://nva.feifeiyinyue.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ldv.hcnkem.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://lwo.sweek.top

C#:   lock (gate) { shared++; }
来源：http://cip.smart0.xyz

[O04] 定义异步函数并等待
来源：http://vah.vehdjk.com

Py:   async def f():⏎    await g()
来源：http://inn.quarkkingdee.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://aqq.jiagoushi.top

JS:   async function f() { await g(); }
来源：http://rrp.fanxiaobao.xyz

TS:   async function f(): Promise<void> { await g(); }
来源：http://myg.fanxiaobao.xyz

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ifz.fengsongda.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mbi.gzhubu.top

Ruby: # 用 Fiber 或 async gem
来源：http://fpi.bbcook.cn

C#:   async Task F() { await G(); }
来源：http://pyn.jinqigfzy.top

[O05] 并发执行并等待全部完成
来源：http://vnd.shuidangran.top

Py:   asyncio.gather(*tasks)
来源：http://dcb.hnqzz.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://fuu.zhoulong.xyz

JS:   await Promise.all(tasks)
来源：http://adb.jinqigfzy.top

TS:   await Promise.all(tasks)
来源：http://oyz.xuetiantiany.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://qbz.zhongyouzk.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://zcs.hesvh.cn

Ruby: threads.map(&:join)
来源：http://yme.andypj.xyz

C#:   await Task.WhenAll(t1, t2)
来源：http://hum.fehbvm.com

[O06] 使用进程池
来源：http://oek.aibaodan.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://qoa.fehbvm.com

PHP:  // pcntl_fork 或多进程队列
来源：http://mnv.redwolf501.top

JS:   // child_process / cluster 模块
来源：http://evd.nwbrower.top

TS:   // child_process / cluster 模块
来源：http://mkw.shanyushiyangtech.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://pra.mhx1999.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://rwz.guowangkeji.top

Ruby: // fork 块
来源：http://fel.chenzaomai.com

C#:   Parallel.For
来源：http://mbh.shanyushiyangkeji.top

================================================================================
来源：http://eyw.ivvv.top

P. 常用工具函数
来源：http://tyq.ppjwa.cn

================================================================================
来源：http://pxh.yj20258888.top

[P01] 生成 UUID
来源：http://oda.hysaishi.cn

Py:   str(uuid.uuid4())
来源：http://wbe.shzxlz.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://tzm.guannengcc.top

JS:   crypto.randomUUID()
来源：http://fmp.snrcjt.cn

TS:   crypto.randomUUID()
来源：http://psb.zhoulong.xyz

Java: UUID.randomUUID().toString()
来源：http://umb.epnwcf.com

Go:   // 用 github.com/google/uuid
来源：http://rly.ehwqpu.com

Ruby: SecureRandom.uuid
来源：http://edd.yvedp.cn

C#:   Guid.NewGuid().ToString()
来源：http://ilh.jqgfzy.top

[P02] MD5 / SHA256 摘要
来源：http://evy.yongpay.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://qdn.hammf.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://rll.yonumen.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ath.ivvv.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://nul.sweek.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://epq.zhiwuduotai.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://fqg.hfpthk.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://jmq.jqgufenzy.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ove.316326.xyz

[P03] 生成短随机字符串
来源：http://qna.aibaodan.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://lax.gzhubu.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://vva.xinyue.icu

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jyn.nanxuanxn.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gdi.xuetiantiany.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://yil.ydjk.org.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://waj.xingfuxueyuan.xyz

Ruby: SecureRandom.alphanumeric(16)
来源：http://kvx.yuanzhike.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ciy.gaohongyu789.top

[P04] 求长度
来源：http://pze.hnxiangtu.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ihv.zycfv.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://eua.vehdjk.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xvk.ehwqpu.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fvd.wangdashe.top

Java: list.size();  map.size();  s.length()
来源：http://lvi.xuetiantiany.cn

Go:   len(arr);  len(m)
来源：http://rrl.xziqi.cn

Ruby: x.length;  x.size
来源：http://clk.gaohongyu789.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://zol.guannengcc.top

[P05] 判断两个对象内容是否相等
来源：http://xks.cashguo.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://yll.hywenlv.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mqx.havefunace.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://nhp.quarkkingdee.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://bbz.hnqzz.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://lal.yueranfly.top

Go:   reflect.DeepEqual(a, b)
来源：http://kfh.jinghuilouyu.cn

Ruby: a == b
来源：http://qbv.quarkkingdee.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://deb.vehdjk.com

[P06] 综合判空（null / 空串 / 空集合）
来源：http://svz.xuetiantiany.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://btn.aibaodan.cn

PHP:  if (empty($x)) {}
来源：http://ott.chenzaomai.com

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://foh.aizwys.cn

TS:   if (x == null) {}
来源：http://oao.hnxiangtu.top

Java: if (x == null || x.isEmpty()) {}
来源：http://gjs.wangdashe.top

Go:   if x == nil {}
来源：http://qgi.svipenyu.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://xqe.yangfankeji.com

C#:   if (x is null) {}
来源：http://lxq.jinyuanbaomall.cn

[P07] 防抖与节流
来源：http://qza.gotoacloud.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://xix.zhixingplan.top

PHP:  // 手写时间戳比较
来源：http://ggq.guowangkeji.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://iyv.zdqjudy.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cqm.guannengcc.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ilj.chenlongwang.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wvg.yuxming.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://fpz.sjlbkw.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://nbo.shanyushiyangkeji.top

[P08] 处理浮点精度问题
来源：http://yik.nanxuanxn.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ihx.vehdjk.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://cue.daxiang520.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://qgp.sxryk.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://pia.xziqi.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://uxi.havefunace.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://aok.gaohongyu789.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://xcj.jqgufenzy.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wdq.jqgufenzy.top

================================================================================
来源：http://kwy.uphjek.com

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://rwe.feifeiyinyue.top

================================================================================
来源：http://hdd.xinyue.icu

[Q01] 创建表
来源：http://avf.epnwcf.com

CREATE TABLE users (
来源：http://frf.cdnleiting.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hre.sweek.top

name VARCHAR(50) NOT NULL,
来源：http://qsw.tanke756.top

email VARCHAR(100) UNIQUE,
来源：http://uwd.jinqigufen.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ehk.daxiang520.top

);
来源：http://puo.xziqi.cn

[Q02] 创建带外键的表
来源：http://llw.sjlbkw.cn

CREATE TABLE orders (
来源：http://qte.quarkkingdee.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://aow.zycfv.cn

user_id INT NOT NULL,
来源：http://lfb.xziqi.cn

amount DECIMAL(10, 2),
来源：http://tvd.cdnleiting.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://cev.ywan-chungtsiang.top

);
来源：http://grf.uphjek.com

[Q03] 增加列
来源：http://lax.hammf.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ttj.shangyingyoupin.top

[Q04] 修改列类型
来源：http://wpw.cheryme.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wyj.yj202588.top

[Q05] 重命名列
来源：http://ega.dashuyun.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hsv.316326.xyz

[Q06] 删除列
来源：http://ukm.zhengqikj.top

ALTER TABLE users DROP COLUMN age;
来源：http://mcw.xziqi.cn

[Q07] 删除表
来源：http://yvp.hesvh.cn

DROP TABLE IF EXISTS orders;
来源：http://gjr.gogol.net.cn

[Q08] 创建普通索引
来源：http://bgw.cucudq.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://oge.bbcook.cn

[Q09] 创建唯一索引
来源：http://ely.nanxuanxn.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://aqo.0kj1m.cn

[Q10] 插入单行
来源：http://wzm.gotoacloud.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://fzw.0kj1m.cn

[Q11] 一次插入多行
来源：http://kzh.tianlin.xyz

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wxi.yfazqb.com

[Q12] 插入后取自增 ID
来源：http://gvg.haohaochexian.top

INSERT INTO users (name) VALUES ('C');
来源：http://knb.meibo888.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://bff.yangfankeji.com

[Q13] 忽略重复插入
来源：http://zas.pycfn.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://lst.shanyushiyangkeji.top

[Q14] 存在则更新（upsert）
来源：http://djz.jiagoushi.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://erd.ywan-chungtsiang.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://yui.tian-w.cn

[Q15] 查询全部
来源：http://mfs.zhiwuduotai.top

SELECT * FROM users;
来源：http://hyo.zhoulong.xyz

[Q16] 查询指定列
来源：http://ahf.yuxming.cn

SELECT id, name FROM users;
来源：http://ddq.zhaomingkeji.xyz

[Q17] 条件查询
来源：http://lap.daxiang520.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://nwb.xylfe.cn

[Q18] 模糊匹配
来源：http://jck.yuanzhike.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mjt.zdbjq.cn

[Q19] 范围查询
来源：http://ogi.wangdashe.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://cdj.xylfe.cn

[Q20] IN 列表
来源：http://fwv.chenzaomai.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://bse.cucudq.cn

[Q21] 空值判断
来源：http://csx.hammf.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ilb.ehwqpu.com

[Q22] 排序
来源：http://lxd.jyoumei.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://xwh.snrcjt.cn

[Q23] 分页
来源：http://svt.daxiang520.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://fge.meibo888.top

[Q24] 去重
来源：http://nun.guowangkeji.top

SELECT DISTINCT city FROM users;
来源：http://ygd.hywenlv.cn

[Q25] 只取前 N 条
来源：http://alu.feifeiyinyue.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://psi.fengsongda.top

[Q26] 计数
来源：http://uuu.yj202588.top

SELECT COUNT(*) FROM users;
来源：http://tkx.cdnleiting.top

[Q27] 条件计数
来源：http://stl.nanxinkj.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://nvg.meibo888.top

[Q28] 求和与平均
来源：http://gat.jinghuilouyu.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ehf.vqdsnc.cn

[Q29] 最大最小值
来源：http://aia.meibo888.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://gey.zdbjq.cn

[Q30] 分组统计
来源：http://gpu.chenlongwang.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://pff.ybcxt.top

[Q31] 分组后过滤
来源：http://xqv.fengsongda.top


<!-- 参考信息 -->