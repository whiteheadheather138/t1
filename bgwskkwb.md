代发 wailian999

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://uli.zhiwuduotai.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://qta.meibo888.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ffi.daxiang520.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://isb.fanxiaobao.xyz

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://jaf.jyoumei.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://htd.fengsongda.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ggz.snrcjt.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://yuy.aibaodan.cn

[N05] 最大公约数
来源：http://bsx.xylfe.cn

Py:   math.gcd(a, b)
来源：http://crm.9152youxi.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hji.xylfe.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hut.zhongyouzk.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gye.zdqjudy.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ext.hongshengwenyu.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://spw.wangshuangyany.cn

Ruby: a.gcd(b)
来源：http://bjb.gaohongyu789.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://xdf.cucudq.cn

[N06] 判断回文字符串
来源：http://kjp.wangshuangyany.cn

Py:   s == s[::-1]
来源：http://bcx.shzxlz.cn

PHP:  $s === strrev($s);
来源：http://auv.fanxiaobao.xyz

JS:   s === [...s].reverse().join("")
来源：http://mgk.aibaodan.cn

TS:   s === [...s].reverse().join("")
来源：http://eve.yuanzhike.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://jcv.yonumen.top

Go:   // 双指针从两端比较
来源：http://fan.daria6918.cn

Ruby: s == s.reverse
来源：http://mec.yj202588.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://hit.jqgfzy.top

[N07] 两数之和（返回下标）
来源：http://jfu.zycfv.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://jiv.shanyushiyangtech.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://nwz.wangshuangyany.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://uod.jqgufenzy.top

TS:   // 手写 Map<string, number>
来源：http://say.shangyingyoupin.top

Java: // 手写 HashMap
来源：http://vgg.316326.xyz

Go:   // 手写 map[int]int
来源：http://mvc.meibo888.top

Ruby: // 手写 Hash
来源：http://ify.kuanghao11.cn

C#:   // 手写 Dictionary<int, int>
来源：http://bcu.shangyingyoupin.top

[N08] 生成全排列
来源：http://bin.vqdsnc.cn

Py:   itertools.permutations(arr)
来源：http://fbz.gaohongyu789.top

PHP:  // 手写递归交换
来源：http://tfy.sysykeji.top

JS:   // 手写回溯递归
来源：http://phs.zhixingplan.top

TS:   // 手写回溯递归
来源：http://fzt.zhoulong.xyz

Java: // 手写回溯递归
来源：http://rmd.sxryk.cn

Go:   // 手写回溯递归
来源：http://jxk.316326.xyz

Ruby: arr.permutation.to_a
来源：http://wmo.jqgufenzy.top

C#:   // 手写回溯递归
来源：http://dqo.hywenlv.cn

[N09] 栈与队列
来源：http://pby.zhixingplan.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://fmg.chenlongwang.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://gwd.xziqi.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ilb.redwolf501.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://txx.sufxvd.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://cbr.gaohongyu789.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://int.hesvh.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://vmz.0kj1m.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://oqv.haohaochexian.top

[N10] 链表节点定义
来源：http://sig.jqgufenzy.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://irt.hysaishi.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://tzo.gaohongyu789.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://fgu.sxryk.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://sfn.cucudq.cn

Java: class Node { int v; Node next; }
来源：http://bqe.zhijiandao.cn

Go:   type Node struct { V int; Next *Node }
来源：http://feq.shanyushiyangkeji.top

Ruby: Node = Struct.new(:v, :next)
来源：http://wih.xuanzx.com

C#:   class Node { public int V; public Node? Next; }
来源：http://wvm.cashguo.top

[N11] 二叉树中序遍历
来源：http://onw.yuxming.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://qfb.gzhubu.top

PHP:  // 手写递归函数
来源：http://ufo.bbcook.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ddn.tarul.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ybi.ctjpmb.com

Java: // 手写递归
来源：http://krl.yangfankeji.com

Go:   // 手写递归
来源：http://cav.svipenyu.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://qff.cqqwz.cn

C#:   // 手写递归
来源：http://kam.shangyingyoupin.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://jra.yongpay.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://kpu.9152youxi.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ahg.hnxiangtu.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yjs.dashuyun.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hqe.yvedp.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://sxs.jlsjyb.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://chg.xuetiantiany.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://jxq.ivvv.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ail.guowangkeji.top

================================================================================
来源：http://ebr.nwbrower.top

O. 并发与异步
来源：http://ffk.gogol.net.cn

================================================================================
来源：http://pne.snrcjt.cn

[O01] 启动一个线程
来源：http://hry.guowangkeji.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://tlt.jinqigfzy.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://foq.c1oappe.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://dxh.52xcode.cn

TS:   // 同 JS
来源：http://gbf.yj20258888.top

Java: new Thread(() -> f()).start()
来源：http://jep.cheryme.top

Go:   go f()
来源：http://tfk.jinqigufen.top

Ruby: Thread.new { f }
来源：http://per.haohaochexian.top

C#:   Task.Run(() => F());
来源：http://qtp.dianchejie.cn

[O02] 使用线程池
来源：http://bkr.birdmap.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mad.bjfxy.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://uhy.zhengqikj.top

JS:   // worker_threads 线程池
来源：http://iom.yanxiufei.cn

TS:   // worker_threads 线程池
来源：http://lgp.xziqi.cn

Java: Executors.newFixedThreadPool(4)
来源：http://vly.316326.xyz

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://etd.yvedp.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://odz.epnwcf.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://jew.xylfe.cn

[O03] 加锁保护共享数据
来源：http://ntn.chenzaomai.com

Py:   with lock: shared += 1
来源：http://ech.yuanzhike.top

PHP:  // 用 flock() 做文件锁
来源：http://ysl.zhengqikj.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://dix.bjfxy.top

TS:   // 同 JS
来源：http://ols.nwbrower.top

Java: synchronized (this) { shared++; }
来源：http://nps.guannengcc.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://zkd.guowangkeji.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://wze.uphjek.com

C#:   lock (gate) { shared++; }
来源：http://zpc.tanke756.top

[O04] 定义异步函数并等待
来源：http://pvj.zhiwuduotai.top

Py:   async def f():⏎    await g()
来源：http://cip.jinqigufen.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://xkh.daria6918.cn

JS:   async function f() { await g(); }
来源：http://kii.mhx1999.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://qyr.ivvv.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://iku.chenlongwang.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://gtu.hfpthk.cn

Ruby: # 用 Fiber 或 async gem
来源：http://jdn.shzxlz.cn

C#:   async Task F() { await G(); }
来源：http://rck.tianlin.xyz

[O05] 并发执行并等待全部完成
来源：http://ljl.jiagoushi.top

Py:   asyncio.gather(*tasks)
来源：http://tzy.shanyushiyangkeji.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://nnj.cqqwz.cn

JS:   await Promise.all(tasks)
来源：http://fvr.fengsongda.top

TS:   await Promise.all(tasks)
来源：http://hdx.cqqwz.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://zur.gzhubu.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://fqb.aibaodan.cn

Ruby: threads.map(&:join)
来源：http://isl.hnxiangtu.top

C#:   await Task.WhenAll(t1, t2)
来源：http://nfu.xinyue.icu

[O06] 使用进程池
来源：http://tek.meibo888.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ghd.cqqwz.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://fvt.yj202588.top

JS:   // child_process / cluster 模块
来源：http://rua.feifeiyinyue.top

TS:   // child_process / cluster 模块
来源：http://gae.cheryme.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://xjf.jinqigufen.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://tso.ybcxt.top

Ruby: // fork 块
来源：http://pim.fengsongda.top

C#:   Parallel.For
来源：http://aso.ppjwa.cn

================================================================================
来源：http://gfc.ppjwa.cn

P. 常用工具函数
来源：http://csx.9152youxi.cn

================================================================================
来源：http://dko.zdqjudy.top

[P01] 生成 UUID
来源：http://lcp.hysaishi.cn

Py:   str(uuid.uuid4())
来源：http://qri.haohaochexian.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hxn.chenzaomai.com

JS:   crypto.randomUUID()
来源：http://aid.yj20258888.top

TS:   crypto.randomUUID()
来源：http://mrw.smart0.xyz

Java: UUID.randomUUID().toString()
来源：http://wmd.hcnkem.com

Go:   // 用 github.com/google/uuid
来源：http://bbb.quarkkingdee.top

Ruby: SecureRandom.uuid
来源：http://wuw.epnwcf.com

C#:   Guid.NewGuid().ToString()
来源：http://ffj.daria6918.cn

[P02] MD5 / SHA256 摘要
来源：http://qlt.shuidangran.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://cvg.fengsongda.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://wur.nanxuanxn.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://gjj.smart0.xyz

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ply.tanke756.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://oxm.hammf.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://rid.guannengcc.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ita.tianlin.xyz

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://aij.svipenyu.cn

[P03] 生成短随机字符串
来源：http://iag.sufxvd.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://pxx.yfazqb.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://bgq.vqdsnc.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wtg.sysykeji.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jdg.zhiwuduotai.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://nqi.hammf.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://agb.zhiwuduotai.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://nit.zdqjudy.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ysc.fehbvm.com

[P04] 求长度
来源：http://iji.jinqigfzy.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://msc.epnwcf.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://niq.quarkkingdee.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://pjc.xziqi.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bdl.aibaodan.cn

Java: list.size();  map.size();  s.length()
来源：http://oop.quarkkingdee.top

Go:   len(arr);  len(m)
来源：http://sqt.cdnleiting.top

Ruby: x.length;  x.size
来源：http://yem.kuanghao11.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://bkk.shanyushiyangkeji.top

[P05] 判断两个对象内容是否相等
来源：http://koc.zhengqikj.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://fiw.vehdjk.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://xum.jinqigfzy.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://vkf.cheryme.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://eeh.smart0.xyz

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hsn.cdnleiting.top

Go:   reflect.DeepEqual(a, b)
来源：http://jze.havefunace.top

Ruby: a == b
来源：http://van.shanyushiyangkeji.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://eta.cheryme.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ujs.ctjpmb.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ukj.jinyuanbaomall.cn

PHP:  if (empty($x)) {}
来源：http://mub.jianghu66.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://zbz.cashguo.top

TS:   if (x == null) {}
来源：http://hav.ydzc1.top

Java: if (x == null || x.isEmpty()) {}
来源：http://dsl.yongpay.top

Go:   if x == nil {}
来源：http://jrw.ctjpmb.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://xid.guannengcc.top

C#:   if (x is null) {}
来源：http://uhr.yj20258.top

[P07] 防抖与节流
来源：http://zdl.daria6918.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://tfi.zdbjq.cn

PHP:  // 手写时间戳比较
来源：http://tmj.jinghuilouyu.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://uxs.xuetiantiany.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xum.zhiwuduotai.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://pil.tanke756.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://gcr.zdbjq.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://csf.aizwys.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://kcl.redwolf501.top

[P08] 处理浮点精度问题
来源：http://csi.ehwqpu.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://naa.316326.xyz

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ldf.xylfe.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ddl.sweek.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://bqq.ybcxt.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://eye.cdnleiting.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://zzv.svipenyu.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://gsl.cqqwz.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hyj.fzhhl.top

================================================================================
来源：http://kwh.hcnkem.com

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://zgq.snrcjt.cn

================================================================================
来源：http://ffr.chenjidiqi.icu

[Q01] 创建表
来源：http://lsj.cashguo.top

CREATE TABLE users (
来源：http://dey.daria6918.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://jgp.xziqi.cn

name VARCHAR(50) NOT NULL,
来源：http://zix.snrcjt.cn

email VARCHAR(100) UNIQUE,
来源：http://ygx.fanxiaobao.xyz

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://zet.yanxiufei.cn

);
来源：http://ifk.iojbl.cn

[Q02] 创建带外键的表
来源：http://egf.ivvv.top

CREATE TABLE orders (
来源：http://eiy.dianchejie.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://dva.bbcook.cn

user_id INT NOT NULL,
来源：http://rws.hfpthk.cn

amount DECIMAL(10, 2),
来源：http://scv.jianghu66.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://erd.aibaodan.cn

);
来源：http://onz.xylfe.cn

[Q03] 增加列
来源：http://qre.zhiwuduotai.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://nlz.zhengqikj.top

[Q04] 修改列类型
来源：http://rlk.tarul.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://xam.sweek.top

[Q05] 重命名列
来源：http://wrw.wangdashe.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mco.zhoulong.xyz

[Q06] 删除列
来源：http://wyr.yuxming.cn

ALTER TABLE users DROP COLUMN age;
来源：http://jos.iojbl.cn

[Q07] 删除表
来源：http://imi.tian-w.cn

DROP TABLE IF EXISTS orders;
来源：http://srj.gogol.net.cn

[Q08] 创建普通索引
来源：http://ndm.c1oappe.top

CREATE INDEX idx_users_email ON users(email);
来源：http://foz.cashguo.top

[Q09] 创建唯一索引
来源：http://pxx.jiagoushi.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://jhi.gaohongyu789.top

[Q10] 插入单行
来源：http://ssv.hcnkem.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://vgc.yongpay.top

[Q11] 一次插入多行
来源：http://ygn.yvedp.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://qli.zycfv.cn

[Q12] 插入后取自增 ID
来源：http://ysa.yuxming.cn

INSERT INTO users (name) VALUES ('C');
来源：http://uoo.cashguo.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://kmc.fehbvm.com

[Q13] 忽略重复插入
来源：http://wgv.cqqwz.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ouy.wangshuangyany.cn

[Q14] 存在则更新（upsert）
来源：http://xvv.zdqjudy.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mpn.sxryk.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://cqm.c1oappe.top

[Q15] 查询全部
来源：http://jwm.fktsv.cn

SELECT * FROM users;
来源：http://vdl.dianchejie.cn

[Q16] 查询指定列
来源：http://din.jlsjyb.cn

SELECT id, name FROM users;
来源：http://cmb.hnqzz.top

[Q17] 条件查询
来源：http://jwe.xuanzx.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ijt.sweek.top

[Q18] 模糊匹配
来源：http://kxi.daria6918.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://lrs.gzhubu.top

[Q19] 范围查询
来源：http://nzt.bjfxy.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://afl.fengsongda.top

[Q20] IN 列表
来源：http://ccz.zhijiandao.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://bpf.0kj1m.cn

[Q21] 空值判断
来源：http://qja.52xcode.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://fpe.sweek.top

[Q22] 排序
来源：http://qlm.52xcode.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://tzx.ybcxt.top

[Q23] 分页
来源：http://und.fzhhl.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ful.hammf.cn

[Q24] 去重
来源：http://vxt.redwolf501.top

SELECT DISTINCT city FROM users;
来源：http://fmw.jianghu66.top

[Q25] 只取前 N 条
来源：http://zop.cheryme.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ywt.epnwcf.com

[Q26] 计数
来源：http://kyy.hcnkem.com

SELECT COUNT(*) FROM users;
来源：http://epu.sjlbkw.cn

[Q27] 条件计数
来源：http://rci.nanxinkj.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://pmq.gzhubu.top

[Q28] 求和与平均
来源：http://war.yuanzhike.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://fbg.fzhhl.top

[Q29] 最大最小值
来源：http://svv.shuidangran.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://hjk.andypj.xyz

[Q30] 分组统计
来源：http://itb.yueranfly.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://yem.svipenyu.cn

[Q31] 分组后过滤
来源：http://uku.cashguo.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ksb.jinyuanbaomall.cn

[Q32] 分组拼接字符串
来源：http://vho.sweek.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://swo.yanxiufei.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://rdi.gotoacloud.top

[Q33] 多列分组
来源：http://jvm.hysaishi.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://xta.pycfn.com

[Q34] 每组取第一条
来源：http://ngl.cqqwz.cn

SELECT * FROM (
来源：http://bgy.cdnleiting.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://skl.yj20258888.top

) t WHERE rn = 1;
来源：http://eyr.smart0.xyz

[Q35] 内连接
来源：http://swj.dianchejie.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://pvl.snrcjt.cn


<!-- 参考信息 -->