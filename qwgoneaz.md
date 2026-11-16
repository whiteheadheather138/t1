代发 wailian999

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hpp.zhoulong.xyz

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mht.yonumen.top

C#:   // 手写递归，或 Array.Sort
来源：http://igt.snrcjt.cn

[N04] 斐波那契数列
来源：http://twa.jianghu66.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://xdn.jqgfzy.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://dbs.sweek.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ead.hammf.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://eis.quarkkingdee.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://rpd.aibaodan.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://fwa.iojbl.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://dud.epnwcf.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wto.kuanghao11.cn

[N05] 最大公约数
来源：http://rbq.mhx1999.top

Py:   math.gcd(a, b)
来源：http://eyo.snrcjt.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://voz.cheryme.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jav.zhaomingkeji.xyz

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rdz.jqgfzy.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://vgb.xuetiantiany.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://sny.svipenyu.cn

Ruby: a.gcd(b)
来源：http://ozs.hnqzz.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://bwb.zhixingplan.top

[N06] 判断回文字符串
来源：http://eni.zhoulong.xyz

Py:   s == s[::-1]
来源：http://xfp.gotoacloud.top

PHP:  $s === strrev($s);
来源：http://fws.daxiang520.top

JS:   s === [...s].reverse().join("")
来源：http://iiq.ppjwa.cn

TS:   s === [...s].reverse().join("")
来源：http://qpt.zhijiandao.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://xse.shangyingyoupin.top

Go:   // 双指针从两端比较
来源：http://hft.fzhhl.top

Ruby: s == s.reverse
来源：http://dug.jinqigfzy.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://hst.fengsongda.top

[N07] 两数之和（返回下标）
来源：http://sws.jyoumei.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://vcy.svipenyu.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://pod.cheryme.top

JS:   // 手写 Map：map.set(v, i)
来源：http://jee.yuxming.cn

TS:   // 手写 Map<string, number>
来源：http://kvm.9152youxi.cn

Java: // 手写 HashMap
来源：http://juk.cucudq.cn

Go:   // 手写 map[int]int
来源：http://qfd.hfpthk.cn

Ruby: // 手写 Hash
来源：http://ewb.ehwqpu.com

C#:   // 手写 Dictionary<int, int>
来源：http://lgs.hysaishi.cn

[N08] 生成全排列
来源：http://uch.ydjk.org.cn

Py:   itertools.permutations(arr)
来源：http://adn.pycfn.com

PHP:  // 手写递归交换
来源：http://lji.fanxiaobao.xyz

JS:   // 手写回溯递归
来源：http://ifc.jinghuilouyu.cn

TS:   // 手写回溯递归
来源：http://czd.sjlbkw.cn

Java: // 手写回溯递归
来源：http://gtm.shanyushiyangkeji.top

Go:   // 手写回溯递归
来源：http://tsu.yongpay.top

Ruby: arr.permutation.to_a
来源：http://vgi.jqgfzy.top

C#:   // 手写回溯递归
来源：http://ltq.hysaishi.cn

[N09] 栈与队列
来源：http://ysh.zhengqikj.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ppf.hysaishi.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://tth.fzhhl.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ioo.jinqigufen.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://xgv.feifeiyinyue.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://der.jinqigufen.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://eew.chenzaomai.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wnz.jinqigfzy.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://qgr.c1oappe.top

[N10] 链表节点定义
来源：http://zlg.zhiwuduotai.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://agd.zhaomingkeji.xyz

PHP:  class Node { public $v; public $next = null; }
来源：http://ynz.zhengqikj.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://jyx.yonumen.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://zjo.birdmap.top

Java: class Node { int v; Node next; }
来源：http://npa.zdqjudy.top

Go:   type Node struct { V int; Next *Node }
来源：http://vbf.cheryme.top

Ruby: Node = Struct.new(:v, :next)
来源：http://axs.fehbvm.com

C#:   class Node { public int V; public Node? Next; }
来源：http://wcx.sweek.top

[N11] 二叉树中序遍历
来源：http://nnr.jyoumei.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://bcc.sweek.top

PHP:  // 手写递归函数
来源：http://uon.tian-w.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jxu.yj20258888.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jru.cdnleiting.top

Java: // 手写递归
来源：http://mnk.tian-w.cn

Go:   // 手写递归
来源：http://qxv.jiagoushi.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://oqz.hcnkem.com

C#:   // 手写递归
来源：http://pwy.vehdjk.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://pyi.zhoulong.xyz

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://met.tianlin.xyz

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://rst.ivvv.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bre.birdmap.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gko.jianghu66.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://zmu.fanxiaobao.xyz

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://xtm.yanxiufei.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://rte.dashuyun.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://bqs.yj202588.top

================================================================================
来源：http://cbd.quarkkingdee.top

O. 并发与异步
来源：http://clf.jlsjyb.cn

================================================================================
来源：http://fpp.52xcode.cn

[O01] 启动一个线程
来源：http://vve.meibo888.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://eeu.jqgufenzy.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://qcw.redwolf501.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ouu.gotoacloud.top

TS:   // 同 JS
来源：http://qfr.birdmap.top

Java: new Thread(() -> f()).start()
来源：http://xhp.guannengcc.top

Go:   go f()
来源：http://fbi.hammf.cn

Ruby: Thread.new { f }
来源：http://hcu.316326.xyz

C#:   Task.Run(() => F());
来源：http://pgq.tarul.cn

[O02] 使用线程池
来源：http://xmy.daria6918.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://zfa.kuanghao11.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://vaq.hcnkem.com

JS:   // worker_threads 线程池
来源：http://evf.jinghuilouyu.cn

TS:   // worker_threads 线程池
来源：http://drq.andypj.xyz

Java: Executors.newFixedThreadPool(4)
来源：http://voq.sxryk.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://lfr.gzhubu.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://zwr.zhiwuduotai.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://lmy.shzxlz.cn

[O03] 加锁保护共享数据
来源：http://omb.yangfankeji.com

Py:   with lock: shared += 1
来源：http://rya.cucudq.cn

PHP:  // 用 flock() 做文件锁
来源：http://enu.smart0.xyz

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://oyz.hfpthk.cn

TS:   // 同 JS
来源：http://ioy.redwolf501.top

Java: synchronized (this) { shared++; }
来源：http://iqg.yangfankeji.com

Go:   mu.Lock();  defer mu.Unlock()
来源：http://qxh.316326.xyz

Ruby: mutex.synchronize { shared += 1 }
来源：http://rpg.yonumen.top

C#:   lock (gate) { shared++; }
来源：http://chx.zdqjudy.top

[O04] 定义异步函数并等待
来源：http://kda.chenzaomai.com

Py:   async def f():⏎    await g()
来源：http://kze.hfpthk.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://yzv.vehdjk.com

JS:   async function f() { await g(); }
来源：http://gns.iojbl.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://zds.sxryk.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://dbp.zhiwuduotai.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://tum.hfpthk.cn

Ruby: # 用 Fiber 或 async gem
来源：http://byc.chenjidiqi.icu

C#:   async Task F() { await G(); }
来源：http://ecm.c1oappe.top

[O05] 并发执行并等待全部完成
来源：http://tni.nanxinkj.top

Py:   asyncio.gather(*tasks)
来源：http://psq.sjlbkw.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://bmf.zhixingplan.top

JS:   await Promise.all(tasks)
来源：http://opk.guannengcc.top

TS:   await Promise.all(tasks)
来源：http://vou.jinghuilouyu.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://uvu.vehdjk.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://iwy.vehdjk.com

Ruby: threads.map(&:join)
来源：http://ihf.hesvh.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://orm.zhoulong.xyz

[O06] 使用进程池
来源：http://qzn.yangfankeji.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://pzg.andypj.xyz

PHP:  // pcntl_fork 或多进程队列
来源：http://efp.yuanzhike.top

JS:   // child_process / cluster 模块
来源：http://aqd.jinyuanbaomall.cn

TS:   // child_process / cluster 模块
来源：http://grc.svipenyu.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://vdo.xinyue.icu

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wxa.sjlbkw.cn

Ruby: // fork 块
来源：http://try.vqdsnc.cn

C#:   Parallel.For
来源：http://jao.gzhubu.top

================================================================================
来源：http://cri.yongpay.top

P. 常用工具函数
来源：http://mnr.zhijiandao.cn

================================================================================
来源：http://hqc.xylfe.cn

[P01] 生成 UUID
来源：http://lhv.sweek.top

Py:   str(uuid.uuid4())
来源：http://rmg.fktsv.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://nqq.sxryk.cn

JS:   crypto.randomUUID()
来源：http://tbl.chenjidiqi.icu

TS:   crypto.randomUUID()
来源：http://hwn.yonumen.top

Java: UUID.randomUUID().toString()
来源：http://ukl.hammf.cn

Go:   // 用 github.com/google/uuid
来源：http://ese.vehdjk.com

Ruby: SecureRandom.uuid
来源：http://fla.hfpthk.cn

C#:   Guid.NewGuid().ToString()
来源：http://pch.xziqi.cn

[P02] MD5 / SHA256 摘要
来源：http://jll.yonumen.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mlg.jqgfzy.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://jgc.bjfxy.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://owp.tarul.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://cth.yj20258.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://pcv.chenlongwang.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://yre.wangdashe.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hru.chenlongwang.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://nns.ywan-chungtsiang.top

[P03] 生成短随机字符串
来源：http://utu.jianghu66.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://guc.sysykeji.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://prv.guowangkeji.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hfp.quarkkingdee.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mkb.iojbl.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://qdx.yj20258.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://lhh.shuidangran.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://xer.9152youxi.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://gun.pengpengdd.cyou

[P04] 求长度
来源：http://aqb.sufxvd.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hjz.yj20258888.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ces.vehdjk.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wfl.hammf.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://yaz.yanxiufei.cn

Java: list.size();  map.size();  s.length()
来源：http://scx.ppjwa.cn

Go:   len(arr);  len(m)
来源：http://uze.redwolf501.top

Ruby: x.length;  x.size
来源：http://blp.xuanzx.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://pqr.zhaomingkeji.xyz

[P05] 判断两个对象内容是否相等
来源：http://bpu.dianchejie.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://kdg.jlsjyb.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://xzf.xuanzx.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://lax.uphjek.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://eyx.hywenlv.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ugd.gaohongyu789.top

Go:   reflect.DeepEqual(a, b)
来源：http://tcj.quarkkingdee.top

Ruby: a == b
来源：http://hcw.shangyingyoupin.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ixl.aibaodan.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wal.zhengqikj.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://gry.xylfe.cn

PHP:  if (empty($x)) {}
来源：http://bxz.chenlongwang.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://bsd.cdnleiting.top

TS:   if (x == null) {}
来源：http://chc.mhx1999.top

Java: if (x == null || x.isEmpty()) {}
来源：http://stx.kuanghao11.cn

Go:   if x == nil {}
来源：http://knf.uphjek.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ysl.feifeiyinyue.top

C#:   if (x is null) {}
来源：http://qgz.ppjwa.cn

[P07] 防抖与节流
来源：http://ppy.zycfv.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ywl.yongpay.top

PHP:  // 手写时间戳比较
来源：http://tgq.ivvv.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gqm.zhijiandao.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://amj.fanxiaobao.xyz

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://pyw.zhaomingkeji.xyz

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://bjw.zhongyouzk.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://yza.nanxuanxn.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://khy.tian-w.cn

[P08] 处理浮点精度问题
来源：http://hdn.jianghu66.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://emx.hesvh.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://bli.cdnleiting.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://jgn.daria6918.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://jnn.cheryme.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hxv.yj20258888.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mxk.jqgufenzy.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://yxp.haohaochexian.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://qgq.hnqzz.top

================================================================================
来源：http://rmz.hfpthk.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://oss.0kj1m.cn

================================================================================
来源：http://vzd.ydjk.org.cn

[Q01] 创建表
来源：http://noi.nwbrower.top

CREATE TABLE users (
来源：http://kct.xuetiantiany.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://njx.cucudq.cn

name VARCHAR(50) NOT NULL,
来源：http://wso.jinqigufen.top

email VARCHAR(100) UNIQUE,
来源：http://luu.hammf.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://xik.sufxvd.cn

);
来源：http://iiz.nanxinkj.top

[Q02] 创建带外键的表
来源：http://bsy.xuanzx.com

CREATE TABLE orders (
来源：http://uaz.jinqigufen.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://lvf.shanyushiyangtech.top

user_id INT NOT NULL,
来源：http://vct.aizwys.cn

amount DECIMAL(10, 2),
来源：http://bfl.jinghuilouyu.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://few.sxryk.cn

);
来源：http://sic.jinqigfzy.top

[Q03] 增加列
来源：http://plr.meibo888.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://nlz.hongshengwenyu.top

[Q04] 修改列类型
来源：http://ukr.tian-w.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://cor.aizwys.cn

[Q05] 重命名列
来源：http://ezi.cdnleiting.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://rfq.mhx1999.top

[Q06] 删除列
来源：http://szi.shzxlz.cn

ALTER TABLE users DROP COLUMN age;
来源：http://qnz.ehwqpu.com

[Q07] 删除表
来源：http://uiw.nanxinkj.top

DROP TABLE IF EXISTS orders;
来源：http://pgt.daria6918.cn

[Q08] 创建普通索引
来源：http://yab.jyoumei.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://pfv.xylfe.cn

[Q09] 创建唯一索引
来源：http://ftr.ppjwa.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://pzl.hysaishi.cn

[Q10] 插入单行
来源：http://bdu.yuanzhike.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://soq.shzxlz.cn

[Q11] 一次插入多行
来源：http://ejk.zhengqikj.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://riy.tian-w.cn

[Q12] 插入后取自增 ID
来源：http://ste.feifeiyinyue.top

INSERT INTO users (name) VALUES ('C');
来源：http://thi.tian-w.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hhp.cdnleiting.top

[Q13] 忽略重复插入
来源：http://shm.dianchejie.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://bjg.sweek.top

[Q14] 存在则更新（upsert）
来源：http://erb.sweek.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://zfi.andypj.xyz

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://xmq.vehdjk.com

[Q15] 查询全部
来源：http://xva.yj20258.top

SELECT * FROM users;
来源：http://lkh.vehdjk.com

[Q16] 查询指定列
来源：http://chr.jinyuanbaomall.cn

SELECT id, name FROM users;
来源：http://jgx.yvedp.cn

[Q17] 条件查询
来源：http://zkq.quarkkingdee.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://xms.bjfxy.top

[Q18] 模糊匹配
来源：http://lzm.yj20258888.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hos.guannengcc.top

[Q19] 范围查询
来源：http://mrc.sysykeji.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://dpz.fehbvm.com

[Q20] IN 列表
来源：http://lwk.hnxiangtu.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://dwh.fzhhl.top

[Q21] 空值判断
来源：http://gqh.kuanghao11.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://hss.andypj.xyz

[Q22] 排序
来源：http://tlx.cucudq.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://vfs.sufxvd.cn

[Q23] 分页
来源：http://ieb.sjlbkw.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://brq.xinyue.icu

[Q24] 去重
来源：http://tsm.ctjpmb.com

SELECT DISTINCT city FROM users;
来源：http://sfg.xziqi.cn

[Q25] 只取前 N 条
来源：http://xix.nwbrower.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://rlu.kuanghao11.cn

[Q26] 计数
来源：http://hui.zhiwuduotai.top

SELECT COUNT(*) FROM users;
来源：http://hxv.pengpengdd.cyou

[Q27] 条件计数
来源：http://jcv.yfazqb.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hbn.sjlbkw.cn

[Q28] 求和与平均
来源：http://aoe.hongshengwenyu.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://zno.sufxvd.cn

[Q29] 最大最小值
来源：http://vwj.gaohongyu789.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://jmw.fengsongda.top

[Q30] 分组统计
来源：http://vnm.yvedp.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://prk.jiagoushi.top

[Q31] 分组后过滤
来源：http://mtc.yangfankeji.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://rlm.nanxuanxn.top

[Q32] 分组拼接字符串
来源：http://nhp.mhx1999.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://bob.yvedp.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://zki.zhiwuduotai.top

[Q33] 多列分组
来源：http://zah.uphjek.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://fmm.zhengqikj.top

[Q34] 每组取第一条
来源：http://azk.gotoacloud.top

SELECT * FROM (
来源：http://cli.nanxinkj.top


<!-- 参考信息 -->