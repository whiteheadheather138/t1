代发 wailian999

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://tyl.jinqigufen.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://otp.yanxiufei.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ljt.0kj1m.cn

[N04] 斐波那契数列
来源：http://gxt.wangdashe.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://qde.zhoulong.xyz

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wht.aibaodan.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ias.xylfe.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jol.uphjek.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://tis.fehbvm.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://jue.pycfn.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://swr.jinyuanbaomall.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ovf.jinghuilouyu.cn

[N05] 最大公约数
来源：http://xsz.pengpengdd.cyou

Py:   math.gcd(a, b)
来源：http://wel.chenlongwang.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blx.redwolf501.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gwj.iojbl.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vyq.shangyingyoupin.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://tgo.zhengqikj.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ekk.tanke756.top

Ruby: a.gcd(b)
来源：http://emb.yueranfly.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://zvp.shzxlz.cn

[N06] 判断回文字符串
来源：http://dnq.shangyingyoupin.top

Py:   s == s[::-1]
来源：http://hfv.zhiwuduotai.top

PHP:  $s === strrev($s);
来源：http://krr.yanxiufei.cn

JS:   s === [...s].reverse().join("")
来源：http://fuy.xuanzx.com

TS:   s === [...s].reverse().join("")
来源：http://giv.cucudq.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://nyw.yj20258.top

Go:   // 双指针从两端比较
来源：http://tfb.gotoacloud.top

Ruby: s == s.reverse
来源：http://hka.hnqzz.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://nni.daria6918.cn

[N07] 两数之和（返回下标）
来源：http://xia.ehwqpu.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ncs.smart0.xyz

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://kbr.fengsongda.top

JS:   // 手写 Map：map.set(v, i)
来源：http://qkw.aibaodan.cn

TS:   // 手写 Map<string, number>
来源：http://dax.dashuyun.cn

Java: // 手写 HashMap
来源：http://oil.shanyushiyangkeji.top

Go:   // 手写 map[int]int
来源：http://xlk.ydzc1.top

Ruby: // 手写 Hash
来源：http://ipq.nanxuanxn.top

C#:   // 手写 Dictionary<int, int>
来源：http://iea.ywan-chungtsiang.top

[N08] 生成全排列
来源：http://kne.gzhubu.top

Py:   itertools.permutations(arr)
来源：http://fum.yangfankeji.com

PHP:  // 手写递归交换
来源：http://yui.0kj1m.cn

JS:   // 手写回溯递归
来源：http://tuw.wangshuangyany.cn

TS:   // 手写回溯递归
来源：http://aqc.feifeiyinyue.top

Java: // 手写回溯递归
来源：http://cye.yuanzhike.top

Go:   // 手写回溯递归
来源：http://ryi.gaohongyu789.top

Ruby: arr.permutation.to_a
来源：http://myl.hcnkem.com

C#:   // 手写回溯递归
来源：http://nuz.havefunace.top

[N09] 栈与队列
来源：http://tca.yangfankeji.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://xou.nwbrower.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://drp.yangfankeji.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://bqh.aizwys.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://tkm.jyoumei.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://tgh.fehbvm.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://aog.wangshuangyany.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://qco.hywenlv.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://zxr.zdbjq.cn

[N10] 链表节点定义
来源：http://qzq.dianchejie.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://qda.iojbl.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://llq.jiagoushi.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://zvr.xziqi.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mxp.hnxiangtu.top

Java: class Node { int v; Node next; }
来源：http://ieh.jqgfzy.top

Go:   type Node struct { V int; Next *Node }
来源：http://efc.mhx1999.top

Ruby: Node = Struct.new(:v, :next)
来源：http://mao.xziqi.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://kuw.chenjidiqi.icu

[N11] 二叉树中序遍历
来源：http://gqw.svipenyu.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://phx.shuidangran.top

PHP:  // 手写递归函数
来源：http://pwz.jqgfzy.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lrn.ppjwa.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://poc.sxryk.cn

Java: // 手写递归
来源：http://uyw.xziqi.cn

Go:   // 手写递归
来源：http://zmb.zhiwuduotai.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://xte.9152youxi.cn

C#:   // 手写递归
来源：http://zra.vqdsnc.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://soi.havefunace.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ado.aibaodan.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://cxf.hysaishi.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qqv.daxiang520.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dmu.cqqwz.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://gdo.tian-w.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://tlb.wangshuangyany.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wem.bbcook.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://drk.meibo888.top

================================================================================
来源：http://tql.cheryme.top

O. 并发与异步
来源：http://opj.shzxlz.cn

================================================================================
来源：http://czf.cucudq.cn

[O01] 启动一个线程
来源：http://hbx.gaohongyu789.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://vgl.jinqigufen.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://zmg.pycfn.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://rmv.jinqigufen.top

TS:   // 同 JS
来源：http://xct.yvedp.cn

Java: new Thread(() -> f()).start()
来源：http://qfp.dashuyun.cn

Go:   go f()
来源：http://tcg.yj20258888.top

Ruby: Thread.new { f }
来源：http://bue.aibaodan.cn

C#:   Task.Run(() => F());
来源：http://tnp.fktsv.cn

[O02] 使用线程池
来源：http://vtn.dashuyun.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hhd.sufxvd.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://zmp.shzxlz.cn

JS:   // worker_threads 线程池
来源：http://weu.jlsjyb.cn

TS:   // worker_threads 线程池
来源：http://uoc.yfazqb.com

Java: Executors.newFixedThreadPool(4)
来源：http://zls.uphjek.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://jdb.yanxiufei.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://msd.gzhubu.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ukp.epnwcf.com

[O03] 加锁保护共享数据
来源：http://tmc.hcnkem.com

Py:   with lock: shared += 1
来源：http://vhi.yj20258.top

PHP:  // 用 flock() 做文件锁
来源：http://nmf.fehbvm.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://soc.ydzc1.top

TS:   // 同 JS
来源：http://gqm.jinyuanbaomall.cn

Java: synchronized (this) { shared++; }
来源：http://kxf.zdqjudy.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://top.yj20258888.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://dqf.guowangkeji.top

C#:   lock (gate) { shared++; }
来源：http://cye.yuanzhike.top

[O04] 定义异步函数并等待
来源：http://wsv.hcnkem.com

Py:   async def f():⏎    await g()
来源：http://ipm.meibo888.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://vvs.meibo888.top

JS:   async function f() { await g(); }
来源：http://uts.9152youxi.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://jhg.guannengcc.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://jom.jqgufenzy.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://lcw.pycfn.com

Ruby: # 用 Fiber 或 async gem
来源：http://sti.smart0.xyz

C#:   async Task F() { await G(); }
来源：http://cuv.guowangkeji.top

[O05] 并发执行并等待全部完成
来源：http://mxr.hysaishi.cn

Py:   asyncio.gather(*tasks)
来源：http://jyh.sufxvd.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://pkv.yj20258888.top

JS:   await Promise.all(tasks)
来源：http://ofa.9152youxi.cn

TS:   await Promise.all(tasks)
来源：http://afy.gotoacloud.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://esc.ydjk.org.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://isv.shuidangran.top

Ruby: threads.map(&:join)
来源：http://viq.shanyushiyangtech.top

C#:   await Task.WhenAll(t1, t2)
来源：http://dka.shangyingyoupin.top

[O06] 使用进程池
来源：http://wbq.zdqjudy.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://txx.pengpengdd.cyou

PHP:  // pcntl_fork 或多进程队列
来源：http://xne.yj20258888.top

JS:   // child_process / cluster 模块
来源：http://jbd.zhixingplan.top

TS:   // child_process / cluster 模块
来源：http://xld.sufxvd.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://jje.ybcxt.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ely.haohaochexian.top

Ruby: // fork 块
来源：http://zfl.hammf.cn

C#:   Parallel.For
来源：http://kwz.hongshengwenyu.top

================================================================================
来源：http://ykj.gotoacloud.top

P. 常用工具函数
来源：http://iaz.shuidangran.top

================================================================================
来源：http://cfk.52xcode.cn

[P01] 生成 UUID
来源：http://afp.hongshengwenyu.top

Py:   str(uuid.uuid4())
来源：http://frq.xziqi.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://rgw.redwolf501.top

JS:   crypto.randomUUID()
来源：http://nzo.bbcook.cn

TS:   crypto.randomUUID()
来源：http://zma.zhixingplan.top

Java: UUID.randomUUID().toString()
来源：http://ycv.fanxiaobao.xyz

Go:   // 用 github.com/google/uuid
来源：http://ago.vqdsnc.cn

Ruby: SecureRandom.uuid
来源：http://efh.zhixingplan.top

C#:   Guid.NewGuid().ToString()
来源：http://uot.quarkkingdee.top

[P02] MD5 / SHA256 摘要
来源：http://jiz.fehbvm.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://gij.feifeiyinyue.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://lbx.daria6918.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://pwt.yfazqb.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://nkj.tianlin.xyz

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://fyd.shuidangran.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://bde.jqgufenzy.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://xcl.sufxvd.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://upi.yueranfly.top

[P03] 生成短随机字符串
来源：http://tuf.aibaodan.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ekn.bbcook.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://rkb.jqgufenzy.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://pxv.cucudq.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://yqk.dashuyun.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://fas.chenjidiqi.icu

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://bvl.gotoacloud.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://kij.fehbvm.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ggv.meibo888.top

[P04] 求长度
来源：http://rmg.zhixingplan.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://dvs.nwbrower.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://pmj.316326.xyz

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://lpi.xinyue.icu

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wlf.uphjek.com

Java: list.size();  map.size();  s.length()
来源：http://ibr.xinyue.icu

Go:   len(arr);  len(m)
来源：http://ttb.fanxiaobao.xyz

Ruby: x.length;  x.size
来源：http://zsv.316326.xyz

C#:   list.Count;  dict.Count;  s.Length
来源：http://iyb.shangyingyoupin.top

[P05] 判断两个对象内容是否相等
来源：http://win.jiagoushi.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://ihf.yj20258888.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://glm.tianlin.xyz

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://xbg.wangdashe.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://rgn.birdmap.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://yqd.aizwys.cn

Go:   reflect.DeepEqual(a, b)
来源：http://njn.fengsongda.top

Ruby: a == b
来源：http://tfc.hesvh.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://bhs.cucudq.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mvf.ybcxt.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://cvf.ehwqpu.com

PHP:  if (empty($x)) {}
来源：http://kzl.snrcjt.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://rns.pengpengdd.cyou

TS:   if (x == null) {}
来源：http://rls.guannengcc.top

Java: if (x == null || x.isEmpty()) {}
来源：http://pgm.iojbl.cn

Go:   if x == nil {}
来源：http://gli.yj20258.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ngm.fanxiaobao.xyz

C#:   if (x is null) {}
来源：http://cpq.yj20258888.top

[P07] 防抖与节流
来源：http://bsv.jinghuilouyu.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://sgo.yonumen.top

PHP:  // 手写时间戳比较
来源：http://tbv.snrcjt.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mvj.jqgfzy.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://siv.wangdashe.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://xxb.yangfankeji.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ber.nanxinkj.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://cyf.gogol.net.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://bbm.ppjwa.cn

[P08] 处理浮点精度问题
来源：http://maq.tian-w.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://gnb.ppjwa.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://qze.c1oappe.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://let.yj20258888.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://gji.shanyushiyangkeji.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ago.ydzc1.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ssq.jqgufenzy.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://pgt.xinyue.icu

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://pwx.yuxming.cn

================================================================================
来源：http://fma.vqdsnc.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://fkq.shzxlz.cn

================================================================================
来源：http://tvi.chenlongwang.top

[Q01] 创建表
来源：http://vji.ybcxt.top

CREATE TABLE users (
来源：http://qwl.wangshuangyany.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://kzw.fengsongda.top

name VARCHAR(50) NOT NULL,
来源：http://dua.bjfxy.top

email VARCHAR(100) UNIQUE,
来源：http://nnf.aibaodan.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://vfp.nanxuanxn.top

);
来源：http://lao.fengsongda.top

[Q02] 创建带外键的表
来源：http://yhr.vqdsnc.cn

CREATE TABLE orders (
来源：http://pmv.guowangkeji.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://uav.birdmap.top

user_id INT NOT NULL,
来源：http://asa.feifeiyinyue.top

amount DECIMAL(10, 2),
来源：http://hrc.sufxvd.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://axa.ehwqpu.com

);
来源：http://enl.xingfuxueyuan.xyz

[Q03] 增加列
来源：http://bqx.zycfv.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://cga.yfazqb.com

[Q04] 修改列类型
来源：http://vpg.havefunace.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://osp.xylfe.cn

[Q05] 重命名列
来源：http://osp.smart0.xyz

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://xnu.zhaomingkeji.xyz

[Q06] 删除列
来源：http://rsc.9152youxi.cn

ALTER TABLE users DROP COLUMN age;
来源：http://bqz.shanyushiyangtech.top

[Q07] 删除表
来源：http://yfu.xingfuxueyuan.xyz

DROP TABLE IF EXISTS orders;
来源：http://jdc.dashuyun.cn

[Q08] 创建普通索引
来源：http://szu.vehdjk.com

CREATE INDEX idx_users_email ON users(email);
来源：http://oyp.uphjek.com

[Q09] 创建唯一索引
来源：http://yoz.zycfv.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://obx.tarul.cn

[Q10] 插入单行
来源：http://ksh.jiagoushi.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://yhp.havefunace.top

[Q11] 一次插入多行
来源：http://mdd.yvedp.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://lwt.zhijiandao.cn

[Q12] 插入后取自增 ID
来源：http://osa.gaohongyu789.top

INSERT INTO users (name) VALUES ('C');
来源：http://xbg.hnqzz.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://aex.tarul.cn

[Q13] 忽略重复插入
来源：http://dlz.hysaishi.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://jnv.quarkkingdee.top

[Q14] 存在则更新（upsert）
来源：http://hmx.zhoulong.xyz

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ldg.smart0.xyz

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://fie.jinghuilouyu.cn

[Q15] 查询全部
来源：http://sxv.fengsongda.top

SELECT * FROM users;
来源：http://iow.sufxvd.cn

[Q16] 查询指定列
来源：http://tvp.gogol.net.cn

SELECT id, name FROM users;
来源：http://jah.vqdsnc.cn

[Q17] 条件查询
来源：http://ofb.ppjwa.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hsf.xingfuxueyuan.xyz

[Q18] 模糊匹配
来源：http://arw.dianchejie.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://dpm.wangdashe.top

[Q19] 范围查询
来源：http://hba.0kj1m.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://kxy.jiagoushi.top

[Q20] IN 列表
来源：http://xlk.jqgfzy.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://pto.jinqigufen.top

[Q21] 空值判断
来源：http://xgz.shanyushiyangkeji.top

SELECT * FROM users WHERE email IS NULL;
来源：http://fwk.shanyushiyangkeji.top

[Q22] 排序
来源：http://zas.ivvv.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://geo.smart0.xyz

[Q23] 分页
来源：http://bdb.zycfv.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hqj.yfazqb.com

[Q24] 去重
来源：http://xag.jinghuilouyu.cn

SELECT DISTINCT city FROM users;
来源：http://nvb.yuxming.cn

[Q25] 只取前 N 条
来源：http://pbw.sweek.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wvm.fengsongda.top

[Q26] 计数
来源：http://fnc.pycfn.com

SELECT COUNT(*) FROM users;
来源：http://dfv.kuanghao11.cn

[Q27] 条件计数
来源：http://sna.yangfankeji.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://vls.hcnkem.com

[Q28] 求和与平均
来源：http://ovf.ydzc1.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://aww.meibo888.top

[Q29] 最大最小值
来源：http://hun.jinqigufen.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://bgt.tarul.cn

[Q30] 分组统计
来源：http://nxr.hywenlv.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://fsj.haohaochexian.top

[Q31] 分组后过滤
来源：http://meb.nanxuanxn.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hbz.xylfe.cn

[Q32] 分组拼接字符串
来源：http://ehg.sxryk.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://tra.feifeiyinyue.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://coi.sxryk.cn

[Q33] 多列分组
来源：http://ldn.52xcode.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://rbf.hesvh.cn

[Q34] 每组取第一条
来源：http://daz.pengpengdd.cyou

SELECT * FROM (
来源：http://bno.yongpay.top


<!-- 参考信息 -->