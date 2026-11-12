代发 wailian999

PHP:  // 递归实现，或用 usort
来源：http://vbo.andypj.xyz

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ewa.xylfe.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://giz.hysaishi.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ccb.ybcxt.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://smu.shangyingyoupin.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hko.hammf.cn

C#:   // 手写递归，或 Array.Sort
来源：http://jyf.yonumen.top

[N04] 斐波那契数列
来源：http://xtp.yj20258.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://biz.xinyue.icu

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mht.iojbl.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pdi.yj20258.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qlk.snrcjt.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://pgu.ybcxt.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://vhk.andypj.xyz

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ibe.jinghuilouyu.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ecn.vqdsnc.cn

[N05] 最大公约数
来源：http://fql.uphjek.com

Py:   math.gcd(a, b)
来源：http://zrc.ybcxt.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://xfl.redwolf501.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xzg.chenzaomai.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://kse.bbcook.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ohs.zhijiandao.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://cpd.epnwcf.com

Ruby: a.gcd(b)
来源：http://wzq.gotoacloud.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://tgs.hnqzz.top

[N06] 判断回文字符串
来源：http://okh.uphjek.com

Py:   s == s[::-1]
来源：http://umb.ydzc1.top

PHP:  $s === strrev($s);
来源：http://gtn.zdbjq.cn

JS:   s === [...s].reverse().join("")
来源：http://qyb.shanyushiyangtech.top

TS:   s === [...s].reverse().join("")
来源：http://gjx.yuanzhike.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://keq.gaohongyu789.top

Go:   // 双指针从两端比较
来源：http://yxc.ctjpmb.com

Ruby: s == s.reverse
来源：http://ftt.daxiang520.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://bbt.pycfn.com

[N07] 两数之和（返回下标）
来源：http://dss.fzhhl.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://fdj.xingfuxueyuan.xyz

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://egt.gotoacloud.top

JS:   // 手写 Map：map.set(v, i)
来源：http://bxu.fehbvm.com

TS:   // 手写 Map<string, number>
来源：http://qyl.uphjek.com

Java: // 手写 HashMap
来源：http://aio.guowangkeji.top

Go:   // 手写 map[int]int
来源：http://ufa.xingfuxueyuan.xyz

Ruby: // 手写 Hash
来源：http://kqw.jqgfzy.top

C#:   // 手写 Dictionary<int, int>
来源：http://nlz.tianlin.xyz

[N08] 生成全排列
来源：http://eir.gzhubu.top

Py:   itertools.permutations(arr)
来源：http://bji.zdqjudy.top

PHP:  // 手写递归交换
来源：http://dpo.feifeiyinyue.top

JS:   // 手写回溯递归
来源：http://oed.hnxiangtu.top

TS:   // 手写回溯递归
来源：http://loa.fktsv.cn

Java: // 手写回溯递归
来源：http://ypr.nwbrower.top

Go:   // 手写回溯递归
来源：http://xdt.havefunace.top

Ruby: arr.permutation.to_a
来源：http://gme.gotoacloud.top

C#:   // 手写回溯递归
来源：http://vry.tanke756.top

[N09] 栈与队列
来源：http://axm.iojbl.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://pcc.jianghu66.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://xti.jinqigfzy.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://vnw.sjlbkw.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://xkb.daxiang520.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://xqn.pycfn.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://uws.jinqigfzy.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ihh.meibo888.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://pbq.redwolf501.top

[N10] 链表节点定义
来源：http://jbo.zycfv.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://orw.hnxiangtu.top

PHP:  class Node { public $v; public $next = null; }
来源：http://wze.sxryk.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://pzz.9152youxi.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://rhu.shuidangran.top

Java: class Node { int v; Node next; }
来源：http://zjn.birdmap.top

Go:   type Node struct { V int; Next *Node }
来源：http://jos.smart0.xyz

Ruby: Node = Struct.new(:v, :next)
来源：http://lhq.chenzaomai.com

C#:   class Node { public int V; public Node? Next; }
来源：http://qqh.hysaishi.cn

[N11] 二叉树中序遍历
来源：http://ayb.iojbl.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wgn.uphjek.com

PHP:  // 手写递归函数
来源：http://zzu.tianlin.xyz

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ujs.jinyuanbaomall.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://muw.hnxiangtu.top

Java: // 手写递归
来源：http://rrb.fktsv.cn

Go:   // 手写递归
来源：http://opq.cqqwz.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://pki.jinyuanbaomall.cn

C#:   // 手写递归
来源：http://ezj.zhixingplan.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://jro.316326.xyz

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://auq.gaohongyu789.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://guq.nwbrower.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dnr.xingfuxueyuan.xyz

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://npv.hnxiangtu.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ffb.ydzc1.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://qih.pengpengdd.cyou

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://pyb.fanxiaobao.xyz

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://jko.sysykeji.top

================================================================================
来源：http://zov.hysaishi.cn

O. 并发与异步
来源：http://nto.nanxinkj.top

================================================================================
来源：http://mdt.daria6918.cn

[O01] 启动一个线程
来源：http://qkp.jlsjyb.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://nuk.shanyushiyangtech.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://kix.zhaomingkeji.xyz

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://lpq.ydzc1.top

TS:   // 同 JS
来源：http://ykr.gotoacloud.top

Java: new Thread(() -> f()).start()
来源：http://yju.shangyingyoupin.top

Go:   go f()
来源：http://xil.dashuyun.cn

Ruby: Thread.new { f }
来源：http://hol.chenlongwang.top

C#:   Task.Run(() => F());
来源：http://xdj.jinqigufen.top

[O02] 使用线程池
来源：http://ovd.shanyushiyangkeji.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://bth.xuetiantiany.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://bmq.redwolf501.top

JS:   // worker_threads 线程池
来源：http://tqx.jinghuilouyu.cn

TS:   // worker_threads 线程池
来源：http://rap.nanxinkj.top

Java: Executors.newFixedThreadPool(4)
来源：http://adq.c1oappe.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://sxt.ybcxt.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://kxe.hfpthk.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://rdh.sufxvd.cn

[O03] 加锁保护共享数据
来源：http://tcu.redwolf501.top

Py:   with lock: shared += 1
来源：http://twy.chenjidiqi.icu

PHP:  // 用 flock() 做文件锁
来源：http://vkk.zhoulong.xyz

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://nnh.ydzc1.top

TS:   // 同 JS
来源：http://hhz.hywenlv.cn

Java: synchronized (this) { shared++; }
来源：http://qru.smart0.xyz

Go:   mu.Lock();  defer mu.Unlock()
来源：http://aho.ctjpmb.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://bzk.gzhubu.top

C#:   lock (gate) { shared++; }
来源：http://jlj.wangdashe.top

[O04] 定义异步函数并等待
来源：http://jqg.hywenlv.cn

Py:   async def f():⏎    await g()
来源：http://ssj.yj20258.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://for.wangshuangyany.cn

JS:   async function f() { await g(); }
来源：http://ept.iojbl.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://maq.ehwqpu.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hmr.zhongyouzk.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://qfi.sjlbkw.cn

Ruby: # 用 Fiber 或 async gem
来源：http://jgy.chenlongwang.top

C#:   async Task F() { await G(); }
来源：http://hyu.nwbrower.top

[O05] 并发执行并等待全部完成
来源：http://xvq.jlsjyb.cn

Py:   asyncio.gather(*tasks)
来源：http://yzt.hywenlv.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://lno.daxiang520.top

JS:   await Promise.all(tasks)
来源：http://pqe.sjlbkw.cn

TS:   await Promise.all(tasks)
来源：http://tle.yj202588.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://omw.wangdashe.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://rwn.sysykeji.top

Ruby: threads.map(&:join)
来源：http://qkd.epnwcf.com

C#:   await Task.WhenAll(t1, t2)
来源：http://tlr.zycfv.cn

[O06] 使用进程池
来源：http://vza.hongshengwenyu.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ufk.yj202588.top

PHP:  // pcntl_fork 或多进程队列
来源：http://gaq.fehbvm.com

JS:   // child_process / cluster 模块
来源：http://wri.vehdjk.com

TS:   // child_process / cluster 模块
来源：http://klx.xinyue.icu

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://kzb.chenlongwang.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://lie.haohaochexian.top

Ruby: // fork 块
来源：http://mep.fanxiaobao.xyz

C#:   Parallel.For
来源：http://jip.c1oappe.top

================================================================================
来源：http://muv.xingfuxueyuan.xyz

P. 常用工具函数
来源：http://gzp.jianghu66.top

================================================================================
来源：http://sai.guannengcc.top

[P01] 生成 UUID
来源：http://lya.c1oappe.top

Py:   str(uuid.uuid4())
来源：http://dub.dashuyun.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://kit.hcnkem.com

JS:   crypto.randomUUID()
来源：http://fxr.yuxming.cn

TS:   crypto.randomUUID()
来源：http://ouz.hnxiangtu.top

Java: UUID.randomUUID().toString()
来源：http://svn.uphjek.com

Go:   // 用 github.com/google/uuid
来源：http://rhn.tanke756.top

Ruby: SecureRandom.uuid
来源：http://mtx.shangyingyoupin.top

C#:   Guid.NewGuid().ToString()
来源：http://zsm.feifeiyinyue.top

[P02] MD5 / SHA256 摘要
来源：http://bnb.yvedp.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hda.yfazqb.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://zdo.fengsongda.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://bne.zhengqikj.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://vsy.shuidangran.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://abm.wangshuangyany.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://rqr.snrcjt.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://yoa.yj202588.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://fhs.yonumen.top

[P03] 生成短随机字符串
来源：http://iup.jqgufenzy.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://csj.ywan-chungtsiang.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://cvq.nwbrower.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://owt.cqqwz.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vma.fehbvm.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ujv.zhengqikj.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ccy.shanyushiyangtech.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://oay.fzhhl.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://pir.yfazqb.com

[P04] 求长度
来源：http://isc.yvedp.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://rvq.jiagoushi.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://izq.cashguo.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ngx.52xcode.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hew.shzxlz.cn

Java: list.size();  map.size();  s.length()
来源：http://idq.feifeiyinyue.top

Go:   len(arr);  len(m)
来源：http://xhd.wangshuangyany.cn

Ruby: x.length;  x.size
来源：http://sys.zycfv.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://fiy.gaohongyu789.top

[P05] 判断两个对象内容是否相等
来源：http://lia.gaohongyu789.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://evy.jqgufenzy.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://dwe.ybcxt.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://cyx.hnxiangtu.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://jxx.zycfv.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://tis.nanxuanxn.top

Go:   reflect.DeepEqual(a, b)
来源：http://lah.epnwcf.com

Ruby: a == b
来源：http://rgr.ctjpmb.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://qch.yuxming.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://cjs.tian-w.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mwh.guannengcc.top

PHP:  if (empty($x)) {}
来源：http://qyg.guowangkeji.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://gom.kuanghao11.cn

TS:   if (x == null) {}
来源：http://cbb.sxryk.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://opg.chenzaomai.com

Go:   if x == nil {}
来源：http://xua.jlsjyb.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://qbn.jinqigfzy.top

C#:   if (x is null) {}
来源：http://vyz.shuidangran.top

[P07] 防抖与节流
来源：http://vae.meibo888.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://eck.xingfuxueyuan.xyz

PHP:  // 手写时间戳比较
来源：http://rms.tian-w.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://doc.vqdsnc.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qwr.havefunace.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://rje.shanyushiyangtech.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://npf.hcnkem.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://cce.haohaochexian.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://gqh.svipenyu.cn

[P08] 处理浮点精度问题
来源：http://xct.zhijiandao.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://yaf.zycfv.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://gpf.shanyushiyangkeji.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://yev.zdbjq.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://avu.jinqigfzy.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://gze.havefunace.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mrc.vqdsnc.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://djy.aizwys.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hjy.nanxinkj.top

================================================================================
来源：http://jzh.tian-w.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://kfa.vqdsnc.cn

================================================================================
来源：http://qql.hnxiangtu.top

[Q01] 创建表
来源：http://idz.zhaomingkeji.xyz

CREATE TABLE users (
来源：http://wnk.yvedp.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://kjj.mhx1999.top

name VARCHAR(50) NOT NULL,
来源：http://lmh.zycfv.cn

email VARCHAR(100) UNIQUE,
来源：http://ade.bjfxy.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://xss.ybcxt.top

);
来源：http://fxl.meibo888.top

[Q02] 创建带外键的表
来源：http://rfs.ybcxt.top

CREATE TABLE orders (
来源：http://jcg.uphjek.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://upq.zhoulong.xyz

user_id INT NOT NULL,
来源：http://qqn.guowangkeji.top

amount DECIMAL(10, 2),
来源：http://jjb.kuanghao11.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://raf.kuanghao11.cn

);
来源：http://bhy.birdmap.top

[Q03] 增加列
来源：http://gxh.zhixingplan.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://djn.xinyue.icu

[Q04] 修改列类型
来源：http://uem.epnwcf.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://rdo.yj20258.top

[Q05] 重命名列
来源：http://ssw.guannengcc.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ljs.chenzaomai.com

[Q06] 删除列
来源：http://glo.ydjk.org.cn

ALTER TABLE users DROP COLUMN age;
来源：http://suf.yuxming.cn

[Q07] 删除表
来源：http://lsd.chenzaomai.com

DROP TABLE IF EXISTS orders;
来源：http://lxv.yuanzhike.top

[Q08] 创建普通索引
来源：http://tot.ywan-chungtsiang.top

CREATE INDEX idx_users_email ON users(email);
来源：http://ptl.hammf.cn

[Q09] 创建唯一索引
来源：http://rix.xingfuxueyuan.xyz

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wgk.fzhhl.top

[Q10] 插入单行
来源：http://egd.aizwys.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://pnk.nanxuanxn.top

[Q11] 一次插入多行
来源：http://wxq.yj20258888.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://dag.chenlongwang.top

[Q12] 插入后取自增 ID
来源：http://upq.cashguo.top

INSERT INTO users (name) VALUES ('C');
来源：http://dbz.52xcode.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://iyz.epnwcf.com

[Q13] 忽略重复插入
来源：http://iyq.guowangkeji.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://din.jlsjyb.cn

[Q14] 存在则更新（upsert）
来源：http://udo.xziqi.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://cgs.xinyue.icu

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://bzg.chenjidiqi.icu

[Q15] 查询全部
来源：http://fnu.yj20258.top

SELECT * FROM users;
来源：http://wzt.dianchejie.cn

[Q16] 查询指定列
来源：http://sbb.ybcxt.top

SELECT id, name FROM users;
来源：http://izx.yonumen.top

[Q17] 条件查询
来源：http://ffk.nwbrower.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://sia.zhengqikj.top

[Q18] 模糊匹配
来源：http://cnf.jyoumei.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://aga.hywenlv.cn

[Q19] 范围查询
来源：http://xzs.ppjwa.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://yum.ywan-chungtsiang.top

[Q20] IN 列表
来源：http://ysw.yueranfly.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://sru.jinqigufen.top

[Q21] 空值判断
来源：http://xex.hnxiangtu.top

SELECT * FROM users WHERE email IS NULL;
来源：http://qfe.zdbjq.cn

[Q22] 排序
来源：http://wex.sweek.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://grz.vehdjk.com

[Q23] 分页
来源：http://pal.hcnkem.com

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://qvq.hfpthk.cn

[Q24] 去重
来源：http://rld.hesvh.cn

SELECT DISTINCT city FROM users;
来源：http://kxy.nanxinkj.top

[Q25] 只取前 N 条
来源：http://fkf.hfpthk.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://txh.jiagoushi.top

[Q26] 计数
来源：http://sll.ywan-chungtsiang.top

SELECT COUNT(*) FROM users;
来源：http://hli.meibo888.top

[Q27] 条件计数
来源：http://deb.dianchejie.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://lzs.jianghu66.top

[Q28] 求和与平均
来源：http://jvl.aizwys.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://qzr.jqgfzy.top

[Q29] 最大最小值
来源：http://gow.jinqigfzy.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://ssh.yj20258.top

[Q30] 分组统计
来源：http://eww.sufxvd.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://dfu.andypj.xyz

[Q31] 分组后过滤
来源：http://fkj.fehbvm.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hnv.hywenlv.cn

[Q32] 分组拼接字符串
来源：http://wes.xylfe.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://rxb.hfpthk.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://nzp.gogol.net.cn


<!-- 参考信息 -->