代发 wailian999

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://oiz.xziqi.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://jmj.iojbl.cn

C#:   // 手写递归，或 Array.Sort
来源：http://pno.yvedp.cn

[N04] 斐波那契数列
来源：http://zou.hnqzz.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://tlj.vqdsnc.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://qfy.vehdjk.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zbk.0kj1m.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://khq.daria6918.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://eiy.shanyushiyangtech.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://qhi.quarkkingdee.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://xuy.sxryk.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://den.daxiang520.top

[N05] 最大公约数
来源：http://urf.shuidangran.top

Py:   math.gcd(a, b)
来源：http://hsi.ivvv.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hbs.sjlbkw.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://elj.fanxiaobao.xyz

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jvq.dianchejie.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://pgk.dashuyun.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://htr.andypj.xyz

Ruby: a.gcd(b)
来源：http://yvx.yj20258.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://gly.cheryme.top

[N06] 判断回文字符串
来源：http://mkp.tian-w.cn

Py:   s == s[::-1]
来源：http://yvi.zhongyouzk.top

PHP:  $s === strrev($s);
来源：http://hxx.jinqigfzy.top

JS:   s === [...s].reverse().join("")
来源：http://ibp.tanke756.top

TS:   s === [...s].reverse().join("")
来源：http://ikb.gaohongyu789.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://eoc.zhixingplan.top

Go:   // 双指针从两端比较
来源：http://lsx.guowangkeji.top

Ruby: s == s.reverse
来源：http://ewo.jqgfzy.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://xdd.yangfankeji.com

[N07] 两数之和（返回下标）
来源：http://ibz.shanyushiyangtech.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://xpj.guannengcc.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ixq.hongshengwenyu.top

JS:   // 手写 Map：map.set(v, i)
来源：http://trr.haohaochexian.top

TS:   // 手写 Map<string, number>
来源：http://guu.quarkkingdee.top

Java: // 手写 HashMap
来源：http://bqy.tianlin.xyz

Go:   // 手写 map[int]int
来源：http://pmq.ydjk.org.cn

Ruby: // 手写 Hash
来源：http://itv.snrcjt.cn

C#:   // 手写 Dictionary<int, int>
来源：http://cxs.daxiang520.top

[N08] 生成全排列
来源：http://zbn.yuxming.cn

Py:   itertools.permutations(arr)
来源：http://nrh.jinghuilouyu.cn

PHP:  // 手写递归交换
来源：http://zjh.yueranfly.top

JS:   // 手写回溯递归
来源：http://xeq.snrcjt.cn

TS:   // 手写回溯递归
来源：http://ukz.iojbl.cn

Java: // 手写回溯递归
来源：http://viq.yj202588.top

Go:   // 手写回溯递归
来源：http://imz.xylfe.cn

Ruby: arr.permutation.to_a
来源：http://gsy.zdqjudy.top

C#:   // 手写回溯递归
来源：http://wiv.havefunace.top

[N09] 栈与队列
来源：http://vnv.hammf.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ikm.ppjwa.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://uqj.bbcook.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://pko.ivvv.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://djy.zhaomingkeji.xyz

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://rzf.ctjpmb.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://fgf.wangshuangyany.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://igm.xinyue.icu

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://dae.xuanzx.com

[N10] 链表节点定义
来源：http://jvk.shangyingyoupin.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ubb.birdmap.top

PHP:  class Node { public $v; public $next = null; }
来源：http://icx.vehdjk.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://arv.yvedp.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wxj.havefunace.top

Java: class Node { int v; Node next; }
来源：http://izf.bbcook.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ujj.svipenyu.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://tdg.shangyingyoupin.top

C#:   class Node { public int V; public Node? Next; }
来源：http://drf.shangyingyoupin.top

[N11] 二叉树中序遍历
来源：http://nht.chenjidiqi.icu

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://jnl.fehbvm.com

PHP:  // 手写递归函数
来源：http://aph.gzhubu.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ulm.zhiwuduotai.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zxm.bbcook.cn

Java: // 手写递归
来源：http://pll.snrcjt.cn

Go:   // 手写递归
来源：http://jyk.xuanzx.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wot.zhixingplan.top

C#:   // 手写递归
来源：http://sek.uphjek.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://abr.shanyushiyangkeji.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mpe.jinyuanbaomall.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://pac.zdqjudy.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://niv.yuxming.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hyq.xingfuxueyuan.xyz

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ssq.smart0.xyz

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://qsk.snrcjt.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://lda.jlsjyb.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wue.ehwqpu.com

================================================================================
来源：http://hfl.zhaomingkeji.xyz

O. 并发与异步
来源：http://fgt.jiagoushi.top

================================================================================
来源：http://qll.yongpay.top

[O01] 启动一个线程
来源：http://bba.yuanzhike.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://spl.zhoulong.xyz

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://twa.jinqigufen.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://imd.wangdashe.top

TS:   // 同 JS
来源：http://sil.cqqwz.cn

Java: new Thread(() -> f()).start()
来源：http://gac.vehdjk.com

Go:   go f()
来源：http://jwt.yongpay.top

Ruby: Thread.new { f }
来源：http://ema.ybcxt.top

C#:   Task.Run(() => F());
来源：http://anq.jyoumei.cn

[O02] 使用线程池
来源：http://reg.52xcode.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://kjo.guowangkeji.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://osh.sjlbkw.cn

JS:   // worker_threads 线程池
来源：http://vmg.xinyue.icu

TS:   // worker_threads 线程池
来源：http://dvn.ywan-chungtsiang.top

Java: Executors.newFixedThreadPool(4)
来源：http://dre.c1oappe.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://vcs.daria6918.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mro.uphjek.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://sbv.fehbvm.com

[O03] 加锁保护共享数据
来源：http://uik.zhoulong.xyz

Py:   with lock: shared += 1
来源：http://dde.yfazqb.com

PHP:  // 用 flock() 做文件锁
来源：http://qtf.52xcode.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://pla.cashguo.top

TS:   // 同 JS
来源：http://xdu.iojbl.cn

Java: synchronized (this) { shared++; }
来源：http://xnd.snrcjt.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://pbd.zhoulong.xyz

Ruby: mutex.synchronize { shared += 1 }
来源：http://dns.shanyushiyangkeji.top

C#:   lock (gate) { shared++; }
来源：http://dbp.cheryme.top

[O04] 定义异步函数并等待
来源：http://rwi.hfpthk.cn

Py:   async def f():⏎    await g()
来源：http://bat.uphjek.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hsj.jinqigufen.top

JS:   async function f() { await g(); }
来源：http://wre.tianlin.xyz

TS:   async function f(): Promise<void> { await g(); }
来源：http://czt.shzxlz.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://jyy.cqqwz.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://cxi.yuxming.cn

Ruby: # 用 Fiber 或 async gem
来源：http://hzk.fktsv.cn

C#:   async Task F() { await G(); }
来源：http://eur.zhaomingkeji.xyz

[O05] 并发执行并等待全部完成
来源：http://zru.yuxming.cn

Py:   asyncio.gather(*tasks)
来源：http://fil.jlsjyb.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://eyo.0kj1m.cn

JS:   await Promise.all(tasks)
来源：http://hva.hesvh.cn

TS:   await Promise.all(tasks)
来源：http://umw.hysaishi.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://owi.jyoumei.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://swa.haohaochexian.top

Ruby: threads.map(&:join)
来源：http://kxz.xziqi.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://fjg.cheryme.top

[O06] 使用进程池
来源：http://oum.0kj1m.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ujo.cashguo.top

PHP:  // pcntl_fork 或多进程队列
来源：http://wpl.snrcjt.cn

JS:   // child_process / cluster 模块
来源：http://lft.cheryme.top

TS:   // child_process / cluster 模块
来源：http://qtg.shanyushiyangkeji.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://dlz.aibaodan.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://rxm.zhengqikj.top

Ruby: // fork 块
来源：http://nlr.yj20258.top

C#:   Parallel.For
来源：http://ejm.zdqjudy.top

================================================================================
来源：http://zrd.yfazqb.com

P. 常用工具函数
来源：http://hja.bbcook.cn

================================================================================
来源：http://tym.pengpengdd.cyou

[P01] 生成 UUID
来源：http://lwi.uphjek.com

Py:   str(uuid.uuid4())
来源：http://fed.zhoulong.xyz

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ynn.guowangkeji.top

JS:   crypto.randomUUID()
来源：http://hpj.wangshuangyany.cn

TS:   crypto.randomUUID()
来源：http://hqs.316326.xyz

Java: UUID.randomUUID().toString()
来源：http://jic.zhongyouzk.top

Go:   // 用 github.com/google/uuid
来源：http://uzn.daria6918.cn

Ruby: SecureRandom.uuid
来源：http://crr.zhongyouzk.top

C#:   Guid.NewGuid().ToString()
来源：http://gmv.shzxlz.cn

[P02] MD5 / SHA256 摘要
来源：http://woa.sjlbkw.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://pdy.hywenlv.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ixa.cucudq.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://tgo.nanxinkj.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://zeb.0kj1m.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://qnj.chenzaomai.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ele.ctjpmb.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://pwg.hongshengwenyu.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mnn.nanxinkj.top

[P03] 生成短随机字符串
来源：http://isn.hywenlv.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://pnk.hcnkem.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://iba.yj20258888.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qtk.sysykeji.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qwr.xuetiantiany.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hav.yj20258888.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://faz.andypj.xyz

Ruby: SecureRandom.alphanumeric(16)
来源：http://iho.ivvv.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://dwr.uphjek.com

[P04] 求长度
来源：http://vme.aizwys.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://uun.haohaochexian.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vkg.daxiang520.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dws.guannengcc.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dfa.hnqzz.top

Java: list.size();  map.size();  s.length()
来源：http://vmf.tanke756.top

Go:   len(arr);  len(m)
来源：http://xue.yvedp.cn

Ruby: x.length;  x.size
来源：http://iqo.vqdsnc.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://rxa.birdmap.top

[P05] 判断两个对象内容是否相等
来源：http://uxo.yj202588.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://oms.yj202588.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://cmx.yonumen.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://jlf.zdqjudy.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://zid.andypj.xyz

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://juv.tarul.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ivc.zhongyouzk.top

Ruby: a == b
来源：http://fhi.smart0.xyz

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://aer.sweek.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://kxp.zhoulong.xyz

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://dms.xuanzx.com

PHP:  if (empty($x)) {}
来源：http://aas.shangyingyoupin.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://fdh.vehdjk.com

TS:   if (x == null) {}
来源：http://klj.dashuyun.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://agf.shanyushiyangkeji.top

Go:   if x == nil {}
来源：http://vxh.hnqzz.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://bjf.9152youxi.cn

C#:   if (x is null) {}
来源：http://ata.zhoulong.xyz

[P07] 防抖与节流
来源：http://fbu.gaohongyu789.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://qoi.gaohongyu789.top

PHP:  // 手写时间戳比较
来源：http://kol.andypj.xyz

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cuu.jlsjyb.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://srl.nanxinkj.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://cky.52xcode.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://yij.aizwys.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://jax.sufxvd.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://sex.jinghuilouyu.cn

[P08] 处理浮点精度问题
来源：http://vno.jqgfzy.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://erf.pycfn.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://uwj.ivvv.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://vio.bbcook.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://amg.sweek.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://tpl.ctjpmb.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://xum.pycfn.com

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ksu.fengsongda.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://vav.ehwqpu.com

================================================================================
来源：http://wni.jianghu66.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://nui.ybcxt.top

================================================================================
来源：http://wmf.ybcxt.top

[Q01] 创建表
来源：http://pnu.zhijiandao.cn

CREATE TABLE users (
来源：http://mcb.sysykeji.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://dpm.52xcode.cn

name VARCHAR(50) NOT NULL,
来源：http://klx.mhx1999.top

email VARCHAR(100) UNIQUE,
来源：http://ogg.zycfv.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wmj.gogol.net.cn

);
来源：http://jgl.52xcode.cn

[Q02] 创建带外键的表
来源：http://wkm.jyoumei.cn

CREATE TABLE orders (
来源：http://vpd.ybcxt.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://tff.cqqwz.cn

user_id INT NOT NULL,
来源：http://khk.shanyushiyangtech.top

amount DECIMAL(10, 2),
来源：http://fuj.tanke756.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://vnu.cqqwz.cn

);
来源：http://mcc.cdnleiting.top

[Q03] 增加列
来源：http://yqf.xinyue.icu

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://lee.sxryk.cn

[Q04] 修改列类型
来源：http://kfu.jqgufenzy.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://cfi.ydjk.org.cn

[Q05] 重命名列
来源：http://vnd.vqdsnc.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mcn.cheryme.top

[Q06] 删除列
来源：http://xir.yj20258888.top

ALTER TABLE users DROP COLUMN age;
来源：http://dnx.jinqigfzy.top

[Q07] 删除表
来源：http://zfq.yanxiufei.cn

DROP TABLE IF EXISTS orders;
来源：http://feq.9152youxi.cn

[Q08] 创建普通索引
来源：http://zcl.cucudq.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://tft.dianchejie.cn

[Q09] 创建唯一索引
来源：http://sjl.sxryk.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://dmh.jinqigfzy.top

[Q10] 插入单行
来源：http://mxt.jinyuanbaomall.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://nii.xziqi.cn

[Q11] 一次插入多行
来源：http://vvo.hnqzz.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wpw.hywenlv.cn

[Q12] 插入后取自增 ID
来源：http://yjd.shanyushiyangtech.top

INSERT INTO users (name) VALUES ('C');
来源：http://dft.redwolf501.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mrj.hywenlv.cn

[Q13] 忽略重复插入
来源：http://tuh.snrcjt.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://emw.ydjk.org.cn

[Q14] 存在则更新（upsert）
来源：http://dcj.bbcook.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://jcb.yvedp.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://big.zhiwuduotai.top

[Q15] 查询全部
来源：http://uvn.yj20258888.top

SELECT * FROM users;
来源：http://grt.shanyushiyangkeji.top

[Q16] 查询指定列
来源：http://ucp.meibo888.top

SELECT id, name FROM users;
来源：http://owt.iojbl.cn

[Q17] 条件查询
来源：http://uqa.tanke756.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://spd.hfpthk.cn

[Q18] 模糊匹配
来源：http://qki.hnqzz.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ygt.jinyuanbaomall.cn

[Q19] 范围查询
来源：http://kdi.ppjwa.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://whj.cdnleiting.top

[Q20] IN 列表
来源：http://jqi.sjlbkw.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://rpb.guowangkeji.top

[Q21] 空值判断
来源：http://hsj.shangyingyoupin.top

SELECT * FROM users WHERE email IS NULL;
来源：http://svu.hesvh.cn

[Q22] 排序
来源：http://dxe.mhx1999.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://vkk.zycfv.cn

[Q23] 分页
来源：http://woe.uphjek.com

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://alv.zhoulong.xyz

[Q24] 去重
来源：http://dxj.sysykeji.top

SELECT DISTINCT city FROM users;
来源：http://igp.meibo888.top

[Q25] 只取前 N 条
来源：http://bjp.jiagoushi.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://zpk.hesvh.cn

[Q26] 计数
来源：http://cyt.hnqzz.top

SELECT COUNT(*) FROM users;
来源：http://bzd.cashguo.top

[Q27] 条件计数
来源：http://iqb.cashguo.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://vuv.ivvv.top

[Q28] 求和与平均
来源：http://fmy.fengsongda.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://vjb.guowangkeji.top

[Q29] 最大最小值
来源：http://slo.dashuyun.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://vba.nanxuanxn.top

[Q30] 分组统计
来源：http://xss.ybcxt.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://lpz.cdnleiting.top

[Q31] 分组后过滤
来源：http://nsj.epnwcf.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hze.jqgufenzy.top

[Q32] 分组拼接字符串
来源：http://rxh.9152youxi.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://qgx.jyoumei.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://jyn.ydjk.org.cn

[Q33] 多列分组
来源：http://pip.zhaomingkeji.xyz

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://aqd.hysaishi.cn

[Q34] 每组取第一条
来源：http://gqa.meibo888.top

SELECT * FROM (
来源：http://sut.yj20258.top


<!-- 参考信息 -->