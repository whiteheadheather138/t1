代发 wailian999

PHP:  // 递归实现，或用 usort
来源：http://ove.pycfn.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gxe.sjlbkw.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gtu.vqdsnc.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://yxt.52xcode.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://qmd.zhengqikj.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://jjl.ehwqpu.com

C#:   // 手写递归，或 Array.Sort
来源：http://jlz.yj20258.top

[N04] 斐波那契数列
来源：http://uae.zhengqikj.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://icv.hfpthk.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://gwd.aizwys.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://enm.zhongyouzk.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://flc.iojbl.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://klx.bbcook.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://yrh.fktsv.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blp.sweek.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://xaz.zhongyouzk.top

[N05] 最大公约数
来源：http://baq.iojbl.cn

Py:   math.gcd(a, b)
来源：http://hkx.zhiwuduotai.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://rbw.wangdashe.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rwj.xingfuxueyuan.xyz

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://aff.shuidangran.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://jad.ivvv.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://bpm.andypj.xyz

Ruby: a.gcd(b)
来源：http://kab.ctjpmb.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://grj.yfazqb.com

[N06] 判断回文字符串
来源：http://cpt.xziqi.cn

Py:   s == s[::-1]
来源：http://lcl.bjfxy.top

PHP:  $s === strrev($s);
来源：http://vma.9152youxi.cn

JS:   s === [...s].reverse().join("")
来源：http://zjf.bjfxy.top

TS:   s === [...s].reverse().join("")
来源：http://uci.xuanzx.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://xec.zdbjq.cn

Go:   // 双指针从两端比较
来源：http://ziy.sysykeji.top

Ruby: s == s.reverse
来源：http://fac.meibo888.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://psg.zhongyouzk.top

[N07] 两数之和（返回下标）
来源：http://obu.wangdashe.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://vnz.jinyuanbaomall.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://rub.zhoulong.xyz

JS:   // 手写 Map：map.set(v, i)
来源：http://qxi.cucudq.cn

TS:   // 手写 Map<string, number>
来源：http://jrb.jinqigfzy.top

Java: // 手写 HashMap
来源：http://jxs.gotoacloud.top

Go:   // 手写 map[int]int
来源：http://okb.vehdjk.com

Ruby: // 手写 Hash
来源：http://mxk.dianchejie.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ghw.hammf.cn

[N08] 生成全排列
来源：http://wcv.nanxuanxn.top

Py:   itertools.permutations(arr)
来源：http://mfx.316326.xyz

PHP:  // 手写递归交换
来源：http://nbj.chenjidiqi.icu

JS:   // 手写回溯递归
来源：http://tql.yangfankeji.com

TS:   // 手写回溯递归
来源：http://mkl.nwbrower.top

Java: // 手写回溯递归
来源：http://ige.wangdashe.top

Go:   // 手写回溯递归
来源：http://vxc.316326.xyz

Ruby: arr.permutation.to_a
来源：http://xlg.hesvh.cn

C#:   // 手写回溯递归
来源：http://qhd.kuanghao11.cn

[N09] 栈与队列
来源：http://pdp.dashuyun.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://lik.hongshengwenyu.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://zsl.fktsv.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://xtt.wangdashe.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://pwy.zdbjq.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://szx.cqqwz.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://pic.jinyuanbaomall.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://lqo.gaohongyu789.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://afc.hongshengwenyu.top

[N10] 链表节点定义
来源：http://ojh.yangfankeji.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://xlh.tian-w.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://waa.sxryk.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ofg.redwolf501.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://eib.ehwqpu.com

Java: class Node { int v; Node next; }
来源：http://kst.cdnleiting.top

Go:   type Node struct { V int; Next *Node }
来源：http://cbv.vqdsnc.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://zwt.wangshuangyany.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://urw.uphjek.com

[N11] 二叉树中序遍历
来源：http://sio.kuanghao11.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://bsm.vqdsnc.cn

PHP:  // 手写递归函数
来源：http://dky.sufxvd.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rwt.yj202588.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xiq.zhaomingkeji.xyz

Java: // 手写递归
来源：http://qei.yueranfly.top

Go:   // 手写递归
来源：http://apj.shzxlz.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://nqp.sjlbkw.cn

C#:   // 手写递归
来源：http://yqi.hammf.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://oge.aibaodan.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://vhd.xingfuxueyuan.xyz

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://qob.gaohongyu789.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://eoz.bjfxy.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://oip.daxiang520.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://jcr.jinghuilouyu.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://izq.nanxinkj.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ggq.yuxming.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://jeh.fanxiaobao.xyz

================================================================================
来源：http://zjk.cucudq.cn

O. 并发与异步
来源：http://zql.cheryme.top

================================================================================
来源：http://ozs.xinyue.icu

[O01] 启动一个线程
来源：http://qqm.guannengcc.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://cwl.9152youxi.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://zmo.fktsv.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ydz.gotoacloud.top

TS:   // 同 JS
来源：http://klv.ydzc1.top

Java: new Thread(() -> f()).start()
来源：http://drx.zhiwuduotai.top

Go:   go f()
来源：http://pvs.jinyuanbaomall.cn

Ruby: Thread.new { f }
来源：http://sre.zhengqikj.top

C#:   Task.Run(() => F());
来源：http://jcq.pycfn.com

[O02] 使用线程池
来源：http://zpi.cqqwz.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ynq.sxryk.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hbx.aizwys.cn

JS:   // worker_threads 线程池
来源：http://lzp.dashuyun.cn

TS:   // worker_threads 线程池
来源：http://prh.shuidangran.top

Java: Executors.newFixedThreadPool(4)
来源：http://hze.nanxinkj.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://fvv.tanke756.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://vzj.hnxiangtu.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://yxx.aizwys.cn

[O03] 加锁保护共享数据
来源：http://mqr.fehbvm.com

Py:   with lock: shared += 1
来源：http://jpo.haohaochexian.top

PHP:  // 用 flock() 做文件锁
来源：http://esp.andypj.xyz

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hkc.nwbrower.top

TS:   // 同 JS
来源：http://fms.xziqi.cn

Java: synchronized (this) { shared++; }
来源：http://vpn.chenlongwang.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://dpf.pengpengdd.cyou

Ruby: mutex.synchronize { shared += 1 }
来源：http://dxy.xziqi.cn

C#:   lock (gate) { shared++; }
来源：http://cub.mhx1999.top

[O04] 定义异步函数并等待
来源：http://gud.guowangkeji.top

Py:   async def f():⏎    await g()
来源：http://jyf.yuxming.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wpm.zycfv.cn

JS:   async function f() { await g(); }
来源：http://srr.yongpay.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://aru.iojbl.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://zww.gogol.net.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://qmn.xuanzx.com

Ruby: # 用 Fiber 或 async gem
来源：http://zkq.gaohongyu789.top

C#:   async Task F() { await G(); }
来源：http://avp.epnwcf.com

[O05] 并发执行并等待全部完成
来源：http://xni.snrcjt.cn

Py:   asyncio.gather(*tasks)
来源：http://ddf.uphjek.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://oef.pengpengdd.cyou

JS:   await Promise.all(tasks)
来源：http://szr.yongpay.top

TS:   await Promise.all(tasks)
来源：http://fjh.mhx1999.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://lsk.jlsjyb.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://cku.redwolf501.top

Ruby: threads.map(&:join)
来源：http://zxs.hfpthk.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ctw.shangyingyoupin.top

[O06] 使用进程池
来源：http://yuf.jianghu66.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://iec.daria6918.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://htx.zycfv.cn

JS:   // child_process / cluster 模块
来源：http://cyg.yj20258.top

TS:   // child_process / cluster 模块
来源：http://sup.kuanghao11.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://bag.smart0.xyz

Go:   // goroutine 已占用多核，直接并发即可
来源：http://kpw.ivvv.top

Ruby: // fork 块
来源：http://bji.uphjek.com

C#:   Parallel.For
来源：http://bhn.daxiang520.top

================================================================================
来源：http://jeu.tanke756.top

P. 常用工具函数
来源：http://znm.cashguo.top

================================================================================
来源：http://nuv.shzxlz.cn

[P01] 生成 UUID
来源：http://jyx.shangyingyoupin.top

Py:   str(uuid.uuid4())
来源：http://gio.guannengcc.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://utw.ctjpmb.com

JS:   crypto.randomUUID()
来源：http://gqx.tanke756.top

TS:   crypto.randomUUID()
来源：http://vsl.fehbvm.com

Java: UUID.randomUUID().toString()
来源：http://poa.yj202588.top

Go:   // 用 github.com/google/uuid
来源：http://ogj.fengsongda.top

Ruby: SecureRandom.uuid
来源：http://qyj.xuanzx.com

C#:   Guid.NewGuid().ToString()
来源：http://jyr.jiagoushi.top

[P02] MD5 / SHA256 摘要
来源：http://jkk.guowangkeji.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://rvq.xinyue.icu

PHP:  hash("sha256", $s);  md5($s);
来源：http://tuw.yueranfly.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wty.zhijiandao.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://nud.yj202588.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://qyr.jinqigufen.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://jwl.iojbl.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://sgy.cqqwz.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://yso.tanke756.top

[P03] 生成短随机字符串
来源：http://iib.cheryme.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hrz.yuanzhike.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://tlm.ivvv.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ugt.zycfv.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://tpb.aizwys.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://rhv.cashguo.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://gjh.sxryk.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://xic.jlsjyb.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://qdq.shanyushiyangkeji.top

[P04] 求长度
来源：http://oiu.hammf.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://uww.xinyue.icu

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://eja.tanke756.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zus.redwolf501.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ttf.ctjpmb.com

Java: list.size();  map.size();  s.length()
来源：http://oox.havefunace.top

Go:   len(arr);  len(m)
来源：http://hnz.chenjidiqi.icu

Ruby: x.length;  x.size
来源：http://rtp.yuxming.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://njx.fehbvm.com

[P05] 判断两个对象内容是否相等
来源：http://flb.jqgufenzy.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://jgd.9152youxi.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://irb.nwbrower.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://myc.guowangkeji.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://sav.yuxming.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://bur.mhx1999.top

Go:   reflect.DeepEqual(a, b)
来源：http://ojh.yj20258.top

Ruby: a == b
来源：http://yky.yj202588.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://iic.yonumen.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://vmx.cheryme.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://prm.xingfuxueyuan.xyz

PHP:  if (empty($x)) {}
来源：http://oww.ehwqpu.com

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://qdc.cqqwz.cn

TS:   if (x == null) {}
来源：http://yyc.wangdashe.top

Java: if (x == null || x.isEmpty()) {}
来源：http://crq.xingfuxueyuan.xyz

Go:   if x == nil {}
来源：http://znu.yvedp.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://uns.cqqwz.cn

C#:   if (x is null) {}
来源：http://tiu.hysaishi.cn

[P07] 防抖与节流
来源：http://utb.ctjpmb.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://pms.ctjpmb.com

PHP:  // 手写时间戳比较
来源：http://kfa.jiagoushi.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ptv.nwbrower.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vvl.hnxiangtu.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://kij.fengsongda.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://zpj.chenlongwang.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://rrp.fktsv.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://rcv.smart0.xyz

[P08] 处理浮点精度问题
来源：http://pqj.fehbvm.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://sbp.feifeiyinyue.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://egp.jlsjyb.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://xbp.zhoulong.xyz

TS:   (0.1 + 0.2).toFixed(2)
来源：http://lfm.pengpengdd.cyou

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://oed.jqgfzy.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://phu.ydzc1.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://xrr.zhijiandao.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://viu.shangyingyoupin.top

================================================================================
来源：http://iqi.ywan-chungtsiang.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://gis.aibaodan.cn

================================================================================
来源：http://ucp.xinyue.icu

[Q01] 创建表
来源：http://yqf.fengsongda.top

CREATE TABLE users (
来源：http://edq.snrcjt.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://kzz.jinyuanbaomall.cn

name VARCHAR(50) NOT NULL,
来源：http://kxp.yongpay.top

email VARCHAR(100) UNIQUE,
来源：http://ajr.tanke756.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ksa.iojbl.cn

);
来源：http://vtf.sysykeji.top

[Q02] 创建带外键的表
来源：http://goz.tianlin.xyz

CREATE TABLE orders (
来源：http://qra.hysaishi.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ddq.gzhubu.top

user_id INT NOT NULL,
来源：http://ysi.xinyue.icu

amount DECIMAL(10, 2),
来源：http://pfj.xziqi.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wpa.jinqigfzy.top

);
来源：http://obd.shzxlz.cn

[Q03] 增加列
来源：http://trv.cashguo.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://nyx.ydjk.org.cn

[Q04] 修改列类型
来源：http://bvl.gzhubu.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://uln.xingfuxueyuan.xyz

[Q05] 重命名列
来源：http://hqc.yj20258888.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ibp.guannengcc.top

[Q06] 删除列
来源：http://qhu.andypj.xyz

ALTER TABLE users DROP COLUMN age;
来源：http://ctq.xuanzx.com

[Q07] 删除表
来源：http://sot.ydzc1.top

DROP TABLE IF EXISTS orders;
来源：http://lof.sxryk.cn

[Q08] 创建普通索引
来源：http://ank.cucudq.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://xgv.ehwqpu.com

[Q09] 创建唯一索引
来源：http://bby.jlsjyb.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wbf.ctjpmb.com

[Q10] 插入单行
来源：http://zeo.jiagoushi.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://pgw.mhx1999.top

[Q11] 一次插入多行
来源：http://xxx.zdbjq.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://rtu.yangfankeji.com

[Q12] 插入后取自增 ID
来源：http://onj.316326.xyz

INSERT INTO users (name) VALUES ('C');
来源：http://llw.jinghuilouyu.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://zyl.ybcxt.top

[Q13] 忽略重复插入
来源：http://wfp.yj202588.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://pkq.guannengcc.top

[Q14] 存在则更新（upsert）
来源：http://del.wangdashe.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://kwt.sufxvd.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://vwg.cdnleiting.top

[Q15] 查询全部
来源：http://nks.hnxiangtu.top

SELECT * FROM users;
来源：http://ncl.ydzc1.top

[Q16] 查询指定列
来源：http://tmo.nanxinkj.top

SELECT id, name FROM users;
来源：http://khn.zhijiandao.cn

[Q17] 条件查询
来源：http://abi.cheryme.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://lle.gotoacloud.top

[Q18] 模糊匹配
来源：http://osz.jinqigfzy.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://omt.shuidangran.top

[Q19] 范围查询
来源：http://bmb.shuidangran.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ulu.hnqzz.top

[Q20] IN 列表
来源：http://pjp.cucudq.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://szp.gotoacloud.top

[Q21] 空值判断
来源：http://owb.hnxiangtu.top

SELECT * FROM users WHERE email IS NULL;
来源：http://ezq.hysaishi.cn

[Q22] 排序
来源：http://uld.hywenlv.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://muq.gzhubu.top

[Q23] 分页
来源：http://qeb.gotoacloud.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://xpg.vqdsnc.cn

[Q24] 去重
来源：http://ctt.jqgufenzy.top

SELECT DISTINCT city FROM users;
来源：http://diw.ehwqpu.com

[Q25] 只取前 N 条
来源：http://nxp.gogol.net.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://quf.316326.xyz

[Q26] 计数
来源：http://szv.yanxiufei.cn

SELECT COUNT(*) FROM users;
来源：http://hhw.cheryme.top

[Q27] 条件计数
来源：http://hvb.gaohongyu789.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://lgs.sxryk.cn

[Q28] 求和与平均
来源：http://hoq.hammf.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ajf.wangshuangyany.cn

[Q29] 最大最小值
来源：http://pyy.shzxlz.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://pey.zhiwuduotai.top

[Q30] 分组统计
来源：http://wqd.sysykeji.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://bgm.shzxlz.cn

[Q31] 分组后过滤
来源：http://jim.tian-w.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://qzh.jqgfzy.top

[Q32] 分组拼接字符串
来源：http://uhi.yongpay.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://bvz.svipenyu.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ndb.hcnkem.com


<!-- 参考信息 -->