代发 wailian999

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://yic.nanxinkj.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://tdu.hnxiangtu.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://cnj.guannengcc.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://lxm.gzhubu.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://roh.zhixingplan.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://cmz.yvedp.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mzx.sxryk.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://pqe.hammf.cn

[N05] 最大公约数
来源：http://yvf.jinghuilouyu.cn

Py:   math.gcd(a, b)
来源：http://cdv.aibaodan.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://yiv.tarul.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ocz.shzxlz.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://sgx.yangfankeji.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://chk.cucudq.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hjo.epnwcf.com

Ruby: a.gcd(b)
来源：http://fyb.redwolf501.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://pag.guowangkeji.top

[N06] 判断回文字符串
来源：http://kci.xuanzx.com

Py:   s == s[::-1]
来源：http://dhn.sufxvd.cn

PHP:  $s === strrev($s);
来源：http://nbm.yuanzhike.top

JS:   s === [...s].reverse().join("")
来源：http://hvf.ctjpmb.com

TS:   s === [...s].reverse().join("")
来源：http://uhe.snrcjt.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://lzl.havefunace.top

Go:   // 双指针从两端比较
来源：http://rxm.sjlbkw.cn

Ruby: s == s.reverse
来源：http://adi.aibaodan.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://auh.sweek.top

[N07] 两数之和（返回下标）
来源：http://zih.cucudq.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://fpu.andypj.xyz

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://eeb.wangshuangyany.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://cqa.meibo888.top

TS:   // 手写 Map<string, number>
来源：http://cfi.gotoacloud.top

Java: // 手写 HashMap
来源：http://ihy.shuidangran.top

Go:   // 手写 map[int]int
来源：http://nnn.shuidangran.top

Ruby: // 手写 Hash
来源：http://nxv.aizwys.cn

C#:   // 手写 Dictionary<int, int>
来源：http://odd.gzhubu.top

[N08] 生成全排列
来源：http://znu.birdmap.top

Py:   itertools.permutations(arr)
来源：http://ams.yonumen.top

PHP:  // 手写递归交换
来源：http://ctm.9152youxi.cn

JS:   // 手写回溯递归
来源：http://qaw.cashguo.top

TS:   // 手写回溯递归
来源：http://bvf.gzhubu.top

Java: // 手写回溯递归
来源：http://heq.haohaochexian.top

Go:   // 手写回溯递归
来源：http://nps.zhongyouzk.top

Ruby: arr.permutation.to_a
来源：http://xic.feifeiyinyue.top

C#:   // 手写回溯递归
来源：http://fbq.fengsongda.top

[N09] 栈与队列
来源：http://mwt.shzxlz.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ceb.52xcode.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://eyf.fktsv.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://eht.shanyushiyangtech.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://kit.ywan-chungtsiang.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://nzu.feifeiyinyue.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ztl.dianchejie.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://yut.xuanzx.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://uec.zhengqikj.top

[N10] 链表节点定义
来源：http://tjq.gaohongyu789.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://jez.cdnleiting.top

PHP:  class Node { public $v; public $next = null; }
来源：http://cdo.jinyuanbaomall.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hdo.ybcxt.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://kkg.svipenyu.cn

Java: class Node { int v; Node next; }
来源：http://qta.uphjek.com

Go:   type Node struct { V int; Next *Node }
来源：http://zur.bjfxy.top

Ruby: Node = Struct.new(:v, :next)
来源：http://yve.pycfn.com

C#:   class Node { public int V; public Node? Next; }
来源：http://sac.ivvv.top

[N11] 二叉树中序遍历
来源：http://ydd.yanxiufei.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ima.yfazqb.com

PHP:  // 手写递归函数
来源：http://bjq.hcnkem.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tap.zdbjq.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jhy.tianlin.xyz

Java: // 手写递归
来源：http://cov.ydjk.org.cn

Go:   // 手写递归
来源：http://ozn.zhoulong.xyz

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ont.yuxming.cn

C#:   // 手写递归
来源：http://egv.xingfuxueyuan.xyz

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://jzo.redwolf501.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://gpy.zhongyouzk.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wir.zhaomingkeji.xyz

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kcc.xingfuxueyuan.xyz

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mqq.zhongyouzk.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://aem.hywenlv.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://not.epnwcf.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://tii.andypj.xyz

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wxg.nwbrower.top

================================================================================
来源：http://gkz.shuidangran.top

O. 并发与异步
来源：http://hsc.zhixingplan.top

================================================================================
来源：http://syy.zhiwuduotai.top

[O01] 启动一个线程
来源：http://wso.jyoumei.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://aob.kuanghao11.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ird.epnwcf.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://otz.9152youxi.cn

TS:   // 同 JS
来源：http://glz.chenzaomai.com

Java: new Thread(() -> f()).start()
来源：http://ndv.yangfankeji.com

Go:   go f()
来源：http://mvu.yj20258.top

Ruby: Thread.new { f }
来源：http://cux.xuanzx.com

C#:   Task.Run(() => F());
来源：http://vkk.pengpengdd.cyou

[O02] 使用线程池
来源：http://ian.wangshuangyany.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://yhh.meibo888.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://rrm.aibaodan.cn

JS:   // worker_threads 线程池
来源：http://jgg.redwolf501.top

TS:   // worker_threads 线程池
来源：http://dog.0kj1m.cn

Java: Executors.newFixedThreadPool(4)
来源：http://bna.wangshuangyany.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wii.hysaishi.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://fxb.gogol.net.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://xcb.tanke756.top

[O03] 加锁保护共享数据
来源：http://yyk.wangdashe.top

Py:   with lock: shared += 1
来源：http://vqk.fengsongda.top

PHP:  // 用 flock() 做文件锁
来源：http://jag.tarul.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://aej.bbcook.cn

TS:   // 同 JS
来源：http://kpk.bjfxy.top

Java: synchronized (this) { shared++; }
来源：http://ofa.gotoacloud.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://adj.haohaochexian.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://yaz.mhx1999.top

C#:   lock (gate) { shared++; }
来源：http://drt.jqgfzy.top

[O04] 定义异步函数并等待
来源：http://lkb.zhengqikj.top

Py:   async def f():⏎    await g()
来源：http://bjg.sweek.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://lry.redwolf501.top

JS:   async function f() { await g(); }
来源：http://xts.nwbrower.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://afw.cqqwz.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://xow.zdqjudy.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://urp.jinghuilouyu.cn

Ruby: # 用 Fiber 或 async gem
来源：http://sjt.daria6918.cn

C#:   async Task F() { await G(); }
来源：http://msi.yueranfly.top

[O05] 并发执行并等待全部完成
来源：http://zdq.hnxiangtu.top

Py:   asyncio.gather(*tasks)
来源：http://dxa.yanxiufei.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://zla.shanyushiyangtech.top

JS:   await Promise.all(tasks)
来源：http://snz.shanyushiyangtech.top

TS:   await Promise.all(tasks)
来源：http://plf.ydzc1.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://owh.yangfankeji.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mpq.tian-w.cn

Ruby: threads.map(&:join)
来源：http://vrw.sxryk.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://kct.fengsongda.top

[O06] 使用进程池
来源：http://uhp.chenlongwang.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wpy.wangshuangyany.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://vic.tianlin.xyz

JS:   // child_process / cluster 模块
来源：http://hgs.shzxlz.cn

TS:   // child_process / cluster 模块
来源：http://htw.nanxuanxn.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://bct.yj202588.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://uyx.dianchejie.cn

Ruby: // fork 块
来源：http://zqd.wangdashe.top

C#:   Parallel.For
来源：http://zeh.hammf.cn

================================================================================
来源：http://yui.dianchejie.cn

P. 常用工具函数
来源：http://kvu.yj20258888.top

================================================================================
来源：http://eqr.tarul.cn

[P01] 生成 UUID
来源：http://gai.c1oappe.top

Py:   str(uuid.uuid4())
来源：http://ytr.sxryk.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://pxa.jyoumei.cn

JS:   crypto.randomUUID()
来源：http://noh.yonumen.top

TS:   crypto.randomUUID()
来源：http://iha.dashuyun.cn

Java: UUID.randomUUID().toString()
来源：http://apq.chenlongwang.top

Go:   // 用 github.com/google/uuid
来源：http://lqq.jlsjyb.cn

Ruby: SecureRandom.uuid
来源：http://yak.jinghuilouyu.cn

C#:   Guid.NewGuid().ToString()
来源：http://hpw.cheryme.top

[P02] MD5 / SHA256 摘要
来源：http://pzq.sweek.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://fyw.hesvh.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://pxy.cucudq.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://gkl.cheryme.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://lcu.sysykeji.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://qnz.tarul.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://epg.yj20258.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://nij.jlsjyb.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://rpt.zdqjudy.top

[P03] 生成短随机字符串
来源：http://qhb.dashuyun.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://oxv.yueranfly.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://fbj.9152youxi.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://aem.c1oappe.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://fyw.ydzc1.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://tjx.ppjwa.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://lfs.yuxming.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ody.hywenlv.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://xpd.daria6918.cn

[P04] 求长度
来源：http://oxh.iojbl.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://izp.jyoumei.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://umz.daxiang520.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qee.dashuyun.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jtk.jinghuilouyu.cn

Java: list.size();  map.size();  s.length()
来源：http://cpb.redwolf501.top

Go:   len(arr);  len(m)
来源：http://uky.ydzc1.top

Ruby: x.length;  x.size
来源：http://iqt.hesvh.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ggy.shanyushiyangkeji.top

[P05] 判断两个对象内容是否相等
来源：http://ysy.vqdsnc.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://gej.zhaomingkeji.xyz

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://dfo.ydjk.org.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://oui.yj202588.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hij.gogol.net.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://bxu.hnqzz.top

Go:   reflect.DeepEqual(a, b)
来源：http://nkh.vehdjk.com

Ruby: a == b
来源：http://zat.52xcode.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://won.dashuyun.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://prq.gogol.net.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://qiv.ybcxt.top

PHP:  if (empty($x)) {}
来源：http://zyt.hesvh.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mcs.yj20258888.top

TS:   if (x == null) {}
来源：http://yli.hesvh.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ray.gotoacloud.top

Go:   if x == nil {}
来源：http://odf.jiagoushi.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://dmy.vehdjk.com

C#:   if (x is null) {}
来源：http://dcm.tanke756.top

[P07] 防抖与节流
来源：http://gmp.jyoumei.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ncs.yangfankeji.com

PHP:  // 手写时间戳比较
来源：http://ffl.cdnleiting.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ndd.yanxiufei.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kot.ppjwa.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://bch.9152youxi.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ldv.yangfankeji.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://zyb.aibaodan.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://bka.pycfn.com

[P08] 处理浮点精度问题
来源：http://agh.jinghuilouyu.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mfs.fzhhl.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://xhu.birdmap.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://lyd.chenzaomai.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://jwd.tanke756.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://vxw.jinghuilouyu.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://eag.chenlongwang.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://veg.gzhubu.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://tsm.dashuyun.cn

================================================================================
来源：http://jpw.52xcode.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://esy.yuxming.cn

================================================================================
来源：http://ske.wangdashe.top

[Q01] 创建表
来源：http://csv.pengpengdd.cyou

CREATE TABLE users (
来源：http://xpi.yueranfly.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hqm.tarul.cn

name VARCHAR(50) NOT NULL,
来源：http://itx.jinqigfzy.top

email VARCHAR(100) UNIQUE,
来源：http://eod.yuxming.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://gis.fehbvm.com

);
来源：http://usw.yueranfly.top

[Q02] 创建带外键的表
来源：http://ukm.tianlin.xyz

CREATE TABLE orders (
来源：http://cem.hnxiangtu.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://oyv.yj20258888.top

user_id INT NOT NULL,
来源：http://lcs.zycfv.cn

amount DECIMAL(10, 2),
来源：http://wdn.jianghu66.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hhi.guowangkeji.top

);
来源：http://lid.fktsv.cn

[Q03] 增加列
来源：http://zdv.yfazqb.com

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://fak.zhongyouzk.top

[Q04] 修改列类型
来源：http://hfy.ydjk.org.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hmm.tanke756.top

[Q05] 重命名列
来源：http://exq.chenzaomai.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ibb.gzhubu.top

[Q06] 删除列
来源：http://ysx.zycfv.cn

ALTER TABLE users DROP COLUMN age;
来源：http://juj.smart0.xyz

[Q07] 删除表
来源：http://qfl.shangyingyoupin.top

DROP TABLE IF EXISTS orders;
来源：http://jvg.zdqjudy.top

[Q08] 创建普通索引
来源：http://osg.shanyushiyangkeji.top

CREATE INDEX idx_users_email ON users(email);
来源：http://nso.shuidangran.top

[Q09] 创建唯一索引
来源：http://sey.wangdashe.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://tel.cucudq.cn

[Q10] 插入单行
来源：http://rss.yvedp.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://uxa.vehdjk.com

[Q11] 一次插入多行
来源：http://vqn.52xcode.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://sld.jinqigufen.top

[Q12] 插入后取自增 ID
来源：http://dyj.uphjek.com

INSERT INTO users (name) VALUES ('C');
来源：http://mry.zdbjq.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://srw.hysaishi.cn

[Q13] 忽略重复插入
来源：http://ntr.yuxming.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://jov.gzhubu.top

[Q14] 存在则更新（upsert）
来源：http://piy.shanyushiyangtech.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://sml.nanxuanxn.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://nfb.sxryk.cn

[Q15] 查询全部
来源：http://okm.aizwys.cn

SELECT * FROM users;
来源：http://dpj.yvedp.cn

[Q16] 查询指定列
来源：http://ibh.chenjidiqi.icu

SELECT id, name FROM users;
来源：http://wic.yuanzhike.top

[Q17] 条件查询
来源：http://hjy.vehdjk.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://vjl.ybcxt.top

[Q18] 模糊匹配
来源：http://ddu.jinghuilouyu.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://qki.snrcjt.cn

[Q19] 范围查询
来源：http://mod.yuanzhike.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ymk.tanke756.top

[Q20] IN 列表
来源：http://soe.dashuyun.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://nrh.cashguo.top

[Q21] 空值判断
来源：http://wya.shanyushiyangkeji.top

SELECT * FROM users WHERE email IS NULL;
来源：http://trm.xinyue.icu

[Q22] 排序
来源：http://scv.kuanghao11.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://jty.xylfe.cn

[Q23] 分页
来源：http://xba.sjlbkw.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ivt.xinyue.icu

[Q24] 去重
来源：http://ohl.hnxiangtu.top

SELECT DISTINCT city FROM users;
来源：http://bjf.yuxming.cn

[Q25] 只取前 N 条
来源：http://fsq.shzxlz.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://pac.fanxiaobao.xyz

[Q26] 计数
来源：http://dog.hammf.cn

SELECT COUNT(*) FROM users;
来源：http://oeg.ywan-chungtsiang.top

[Q27] 条件计数
来源：http://xif.zhixingplan.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://lle.c1oappe.top

[Q28] 求和与平均
来源：http://szp.ywan-chungtsiang.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://nlw.fanxiaobao.xyz

[Q29] 最大最小值
来源：http://ijn.bbcook.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://pcd.zhoulong.xyz

[Q30] 分组统计
来源：http://qyh.sweek.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://agu.jinyuanbaomall.cn

[Q31] 分组后过滤
来源：http://tka.chenlongwang.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mpp.xuanzx.com

[Q32] 分组拼接字符串
来源：http://cau.gotoacloud.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://tsh.52xcode.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://rbb.tanke756.top

[Q33] 多列分组
来源：http://ztd.xuetiantiany.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://oso.zhixingplan.top

[Q34] 每组取第一条
来源：http://uft.wangdashe.top

SELECT * FROM (
来源：http://erw.xylfe.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wjs.ivvv.top

) t WHERE rn = 1;
来源：http://nfu.jinqigfzy.top

[Q35] 内连接
来源：http://vnh.fengsongda.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wmw.kuanghao11.cn


<!-- 参考信息 -->