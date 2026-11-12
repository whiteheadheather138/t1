代发 wailian999

C#:   Array.BinarySearch(arr, x)
来源：http://lyx.havefunace.top

[N02] 排序（工程实践用内置实现）
来源：http://xeo.wangshuangyany.cn

Py:   sorted(arr);  arr.sort()
来源：http://xov.shuidangran.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://zhs.xziqi.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://yfs.ehwqpu.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://kpu.yangfankeji.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hgx.sweek.top

Go:   slices.Sort(arr)
来源：http://lzc.9152youxi.cn

Ruby: arr.sort
来源：http://rrz.cashguo.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://zja.jqgufenzy.top

[N03] 快速排序（分治示例）
来源：http://nfk.cucudq.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://elr.zhongyouzk.top

PHP:  // 递归实现，或用 usort
来源：http://rbl.ydzc1.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hzj.daria6918.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mcn.vqdsnc.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://gfy.ywan-chungtsiang.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ync.sjlbkw.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://bcy.fengsongda.top

C#:   // 手写递归，或 Array.Sort
来源：http://ysq.yvedp.cn

[N04] 斐波那契数列
来源：http://pyb.ctjpmb.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://qcj.haohaochexian.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://fif.birdmap.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://lnw.yuanzhike.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nzz.xuanzx.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://nun.andypj.xyz

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://lxb.yj202588.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mox.daria6918.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://sfc.zhijiandao.cn

[N05] 最大公约数
来源：http://mbk.shuidangran.top

Py:   math.gcd(a, b)
来源：http://hye.yfazqb.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://vvj.feifeiyinyue.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qrd.nwbrower.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ikf.bbcook.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://qxt.wangdashe.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://viu.snrcjt.cn

Ruby: a.gcd(b)
来源：http://qtb.aizwys.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://kpa.shanyushiyangkeji.top

[N06] 判断回文字符串
来源：http://kue.chenjidiqi.icu

Py:   s == s[::-1]
来源：http://wmr.fzhhl.top

PHP:  $s === strrev($s);
来源：http://xnr.quarkkingdee.top

JS:   s === [...s].reverse().join("")
来源：http://bnp.wangshuangyany.cn

TS:   s === [...s].reverse().join("")
来源：http://pbx.hfpthk.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://bik.aizwys.cn

Go:   // 双指针从两端比较
来源：http://ktv.xuanzx.com

Ruby: s == s.reverse
来源：http://ihj.pengpengdd.cyou

C#:   s == new string(s.Reverse().ToArray())
来源：http://reg.xuetiantiany.cn

[N07] 两数之和（返回下标）
来源：http://npk.hfpthk.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://gxq.havefunace.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://qkb.jinqigufen.top

JS:   // 手写 Map：map.set(v, i)
来源：http://udi.hnqzz.top

TS:   // 手写 Map<string, number>
来源：http://vlt.daxiang520.top

Java: // 手写 HashMap
来源：http://kpd.vqdsnc.cn

Go:   // 手写 map[int]int
来源：http://bji.fanxiaobao.xyz

Ruby: // 手写 Hash
来源：http://nhj.cheryme.top

C#:   // 手写 Dictionary<int, int>
来源：http://nxx.shanyushiyangkeji.top

[N08] 生成全排列
来源：http://njp.yangfankeji.com

Py:   itertools.permutations(arr)
来源：http://zlo.cucudq.cn

PHP:  // 手写递归交换
来源：http://hpg.chenlongwang.top

JS:   // 手写回溯递归
来源：http://upp.sweek.top

TS:   // 手写回溯递归
来源：http://qzg.ppjwa.cn

Java: // 手写回溯递归
来源：http://bnb.zhijiandao.cn

Go:   // 手写回溯递归
来源：http://npk.wangshuangyany.cn

Ruby: arr.permutation.to_a
来源：http://qei.pycfn.com

C#:   // 手写回溯递归
来源：http://skr.zhijiandao.cn

[N09] 栈与队列
来源：http://slt.shangyingyoupin.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://dvv.yangfankeji.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://jej.yfazqb.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://pyj.dianchejie.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://kaf.ppjwa.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://yhd.yangfankeji.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://udd.vehdjk.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://tym.fanxiaobao.xyz

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://vvs.nanxinkj.top

[N10] 链表节点定义
来源：http://flj.ywan-chungtsiang.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ave.gotoacloud.top

PHP:  class Node { public $v; public $next = null; }
来源：http://vym.hesvh.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://nmd.shuidangran.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://pxw.yj20258.top

Java: class Node { int v; Node next; }
来源：http://akw.haohaochexian.top

Go:   type Node struct { V int; Next *Node }
来源：http://nou.nanxuanxn.top

Ruby: Node = Struct.new(:v, :next)
来源：http://xqn.shzxlz.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://bdm.wangdashe.top

[N11] 二叉树中序遍历
来源：http://acz.zycfv.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://bri.jyoumei.cn

PHP:  // 手写递归函数
来源：http://zfz.52xcode.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pfk.uphjek.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pnc.ehwqpu.com

Java: // 手写递归
来源：http://dfi.ywan-chungtsiang.top

Go:   // 手写递归
来源：http://snj.meibo888.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://gns.yj20258888.top

C#:   // 手写递归
来源：http://bxb.zhengqikj.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://qvj.shzxlz.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wqx.hongshengwenyu.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wvo.aizwys.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ldz.jqgufenzy.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vlm.redwolf501.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://tdy.cqqwz.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ghi.yongpay.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://exd.gotoacloud.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mkf.fzhhl.top

================================================================================
来源：http://wkn.hnxiangtu.top

O. 并发与异步
来源：http://zia.nwbrower.top

================================================================================
来源：http://txi.shzxlz.cn

[O01] 启动一个线程
来源：http://nig.zycfv.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://sse.nanxinkj.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://sta.chenlongwang.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://rqt.jlsjyb.cn

TS:   // 同 JS
来源：http://iqc.epnwcf.com

Java: new Thread(() -> f()).start()
来源：http://ktg.ydjk.org.cn

Go:   go f()
来源：http://jsp.fanxiaobao.xyz

Ruby: Thread.new { f }
来源：http://hlk.zhijiandao.cn

C#:   Task.Run(() => F());
来源：http://bxx.sweek.top

[O02] 使用线程池
来源：http://vfp.jqgufenzy.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://aih.jinyuanbaomall.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://gly.cdnleiting.top

JS:   // worker_threads 线程池
来源：http://xkh.yuxming.cn

TS:   // worker_threads 线程池
来源：http://goe.dashuyun.cn

Java: Executors.newFixedThreadPool(4)
来源：http://kwz.fktsv.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ukh.jianghu66.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://qek.hysaishi.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ute.tanke756.top

[O03] 加锁保护共享数据
来源：http://ykz.ctjpmb.com

Py:   with lock: shared += 1
来源：http://stt.yj20258.top

PHP:  // 用 flock() 做文件锁
来源：http://kkj.fengsongda.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://bvh.yj20258888.top

TS:   // 同 JS
来源：http://kuh.daxiang520.top

Java: synchronized (this) { shared++; }
来源：http://xjp.tanke756.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://myd.jiagoushi.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://ahw.fehbvm.com

C#:   lock (gate) { shared++; }
来源：http://eve.daria6918.cn

[O04] 定义异步函数并等待
来源：http://rio.shanyushiyangtech.top

Py:   async def f():⏎    await g()
来源：http://saw.ydzc1.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://psh.yongpay.top

JS:   async function f() { await g(); }
来源：http://fgg.jinyuanbaomall.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ows.nanxinkj.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://anf.fehbvm.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://rms.svipenyu.cn

Ruby: # 用 Fiber 或 async gem
来源：http://xwh.feifeiyinyue.top

C#:   async Task F() { await G(); }
来源：http://iyy.hywenlv.cn

[O05] 并发执行并等待全部完成
来源：http://hzo.0kj1m.cn

Py:   asyncio.gather(*tasks)
来源：http://gbq.nwbrower.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://pbl.fktsv.cn

JS:   await Promise.all(tasks)
来源：http://oqr.iojbl.cn

TS:   await Promise.all(tasks)
来源：http://wzz.chenjidiqi.icu

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://jdl.316326.xyz

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://icx.shangyingyoupin.top

Ruby: threads.map(&:join)
来源：http://rsi.shanyushiyangkeji.top

C#:   await Task.WhenAll(t1, t2)
来源：http://qsg.cqqwz.cn

[O06] 使用进程池
来源：http://kyw.sysykeji.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://eor.svipenyu.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://lqz.gzhubu.top

JS:   // child_process / cluster 模块
来源：http://mmh.ydjk.org.cn

TS:   // child_process / cluster 模块
来源：http://rjr.jinqigfzy.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://jau.hnxiangtu.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://dxa.zhiwuduotai.top

Ruby: // fork 块
来源：http://hza.zhijiandao.cn

C#:   Parallel.For
来源：http://wmp.sxryk.cn

================================================================================
来源：http://rmv.hesvh.cn

P. 常用工具函数
来源：http://gya.hnqzz.top

================================================================================
来源：http://hic.gzhubu.top

[P01] 生成 UUID
来源：http://fvi.gzhubu.top

Py:   str(uuid.uuid4())
来源：http://pau.yuanzhike.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mgx.zhijiandao.cn

JS:   crypto.randomUUID()
来源：http://awh.hywenlv.cn

TS:   crypto.randomUUID()
来源：http://tlv.ydjk.org.cn

Java: UUID.randomUUID().toString()
来源：http://zqo.ehwqpu.com

Go:   // 用 github.com/google/uuid
来源：http://kdo.guowangkeji.top

Ruby: SecureRandom.uuid
来源：http://uqd.vqdsnc.cn

C#:   Guid.NewGuid().ToString()
来源：http://tkk.kuanghao11.cn

[P02] MD5 / SHA256 摘要
来源：http://xwm.havefunace.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://kzj.ehwqpu.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://owb.ydjk.org.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://knn.pycfn.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://aoi.ctjpmb.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://yyg.52xcode.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hab.epnwcf.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://qms.fengsongda.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://giy.fzhhl.top

[P03] 生成短随机字符串
来源：http://ljk.hysaishi.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://amr.yj202588.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wan.hywenlv.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bbn.shuidangran.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ulf.tianlin.xyz

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://otr.52xcode.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mnx.xziqi.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://kvb.yuxming.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://myc.tianlin.xyz

[P04] 求长度
来源：http://tgq.redwolf501.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://awq.jyoumei.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zbf.xinyue.icu

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rdn.zhiwuduotai.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ayz.daxiang520.top

Java: list.size();  map.size();  s.length()
来源：http://ljm.shangyingyoupin.top

Go:   len(arr);  len(m)
来源：http://chw.yongpay.top

Ruby: x.length;  x.size
来源：http://itb.gaohongyu789.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://qit.yongpay.top

[P05] 判断两个对象内容是否相等
来源：http://sbb.tarul.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://cne.fehbvm.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://che.xuetiantiany.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://kkz.meibo888.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ese.smart0.xyz

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://jew.dashuyun.cn

Go:   reflect.DeepEqual(a, b)
来源：http://cyb.hesvh.cn

Ruby: a == b
来源：http://yuy.hnxiangtu.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://dfv.sjlbkw.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://zvf.havefunace.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://sux.zdbjq.cn

PHP:  if (empty($x)) {}
来源：http://vsc.yanxiufei.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://luv.iojbl.cn

TS:   if (x == null) {}
来源：http://enx.jlsjyb.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://epr.pycfn.com

Go:   if x == nil {}
来源：http://grm.dashuyun.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://pzk.yj20258888.top

C#:   if (x is null) {}
来源：http://lco.hnqzz.top

[P07] 防抖与节流
来源：http://kxl.jqgufenzy.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://bvu.pycfn.com

PHP:  // 手写时间戳比较
来源：http://bse.hywenlv.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wgc.sjlbkw.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qez.tian-w.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://cmu.redwolf501.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://men.vqdsnc.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://sgr.ivvv.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://rzn.dashuyun.cn

[P08] 处理浮点精度问题
来源：http://yjk.yj20258.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://bao.jiagoushi.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://pba.xziqi.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://aub.havefunace.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ksr.yuanzhike.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://kba.ivvv.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://gyj.zhongyouzk.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://tpc.jiagoushi.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://zdx.dianchejie.cn

================================================================================
来源：http://tnw.xylfe.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wab.tian-w.cn

================================================================================
来源：http://bge.aizwys.cn

[Q01] 创建表
来源：http://xta.jyoumei.cn

CREATE TABLE users (
来源：http://wpa.hywenlv.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://vnq.aizwys.cn

name VARCHAR(50) NOT NULL,
来源：http://dga.yj20258888.top

email VARCHAR(100) UNIQUE,
来源：http://rzd.gaohongyu789.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://nxg.gaohongyu789.top

);
来源：http://was.mhx1999.top

[Q02] 创建带外键的表
来源：http://txr.smart0.xyz

CREATE TABLE orders (
来源：http://aac.snrcjt.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://lcy.gogol.net.cn

user_id INT NOT NULL,
来源：http://cgv.redwolf501.top

amount DECIMAL(10, 2),
来源：http://jbc.0kj1m.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://zux.iojbl.cn

);
来源：http://tko.mhx1999.top

[Q03] 增加列
来源：http://xqs.kuanghao11.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://fuh.shangyingyoupin.top

[Q04] 修改列类型
来源：http://ebt.fktsv.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://pox.jqgufenzy.top

[Q05] 重命名列
来源：http://ymv.shuidangran.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://tcc.birdmap.top

[Q06] 删除列
来源：http://csj.jinqigufen.top

ALTER TABLE users DROP COLUMN age;
来源：http://eda.9152youxi.cn

[Q07] 删除表
来源：http://vsc.fzhhl.top

DROP TABLE IF EXISTS orders;
来源：http://hsj.kuanghao11.cn

[Q08] 创建普通索引
来源：http://dmc.shangyingyoupin.top

CREATE INDEX idx_users_email ON users(email);
来源：http://ahe.sysykeji.top

[Q09] 创建唯一索引
来源：http://ewy.tanke756.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://gtw.xuanzx.com

[Q10] 插入单行
来源：http://sgc.aibaodan.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://fqg.316326.xyz

[Q11] 一次插入多行
来源：http://wbt.fehbvm.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://zkz.ctjpmb.com

[Q12] 插入后取自增 ID
来源：http://iuc.jiagoushi.top

INSERT INTO users (name) VALUES ('C');
来源：http://rer.zhiwuduotai.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ivr.vqdsnc.cn

[Q13] 忽略重复插入
来源：http://lvj.ivvv.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ozg.ydjk.org.cn

[Q14] 存在则更新（upsert）
来源：http://bfa.cucudq.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://jhu.316326.xyz

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://yon.xziqi.cn

[Q15] 查询全部
来源：http://ppt.birdmap.top

SELECT * FROM users;
来源：http://nzp.aibaodan.cn

[Q16] 查询指定列
来源：http://abp.tanke756.top

SELECT id, name FROM users;
来源：http://wyw.nanxuanxn.top

[Q17] 条件查询
来源：http://gcl.yueranfly.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://cix.havefunace.top

[Q18] 模糊匹配
来源：http://kjp.yvedp.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://szy.ydjk.org.cn

[Q19] 范围查询
来源：http://nut.xinyue.icu

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://lxn.ehwqpu.com

[Q20] IN 列表
来源：http://mfm.smart0.xyz

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://uhk.aizwys.cn

[Q21] 空值判断
来源：http://lhh.aizwys.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://xvp.hesvh.cn

[Q22] 排序
来源：http://pbl.chenjidiqi.icu

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wwq.cqqwz.cn

[Q23] 分页
来源：http://whv.316326.xyz

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://rua.kuanghao11.cn

[Q24] 去重
来源：http://ccm.tarul.cn

SELECT DISTINCT city FROM users;
来源：http://gik.9152youxi.cn

[Q25] 只取前 N 条
来源：http://glb.jinyuanbaomall.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://bzl.yonumen.top

[Q26] 计数
来源：http://lvp.zhijiandao.cn

SELECT COUNT(*) FROM users;
来源：http://sri.9152youxi.cn

[Q27] 条件计数
来源：http://vpj.yfazqb.com


<!-- 参考信息 -->