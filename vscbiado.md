代发 wailian999

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://yyp.ivvv.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://dqb.yvedp.cn

C#:   // 手写递归，或 Array.Sort
来源：http://yiv.iojbl.cn

[N04] 斐波那契数列
来源：http://pnv.zhongyouzk.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hcm.birdmap.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://gfn.hcnkem.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://eoc.meibo888.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hfx.hysaishi.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://eln.xuanzx.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mmb.pycfn.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ift.hfpthk.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://scr.cdnleiting.top

[N05] 最大公约数
来源：http://vsj.jianghu66.top

Py:   math.gcd(a, b)
来源：http://pyc.sxryk.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://jsx.jinqigfzy.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://uqg.kuanghao11.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ayq.nanxinkj.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wit.jinqigfzy.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ifv.fanxiaobao.xyz

Ruby: a.gcd(b)
来源：http://uqs.jinqigufen.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://dnx.vqdsnc.cn

[N06] 判断回文字符串
来源：http://jfo.xziqi.cn

Py:   s == s[::-1]
来源：http://qxg.jinyuanbaomall.cn

PHP:  $s === strrev($s);
来源：http://chy.mhx1999.top

JS:   s === [...s].reverse().join("")
来源：http://olx.c1oappe.top

TS:   s === [...s].reverse().join("")
来源：http://tdn.jqgufenzy.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mgm.jinqigfzy.top

Go:   // 双指针从两端比较
来源：http://scq.xuetiantiany.cn

Ruby: s == s.reverse
来源：http://qdm.redwolf501.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://bps.yuxming.cn

[N07] 两数之和（返回下标）
来源：http://dmk.cashguo.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://rqs.fengsongda.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://gbr.ivvv.top

JS:   // 手写 Map：map.set(v, i)
来源：http://jdj.jyoumei.cn

TS:   // 手写 Map<string, number>
来源：http://oht.gaohongyu789.top

Java: // 手写 HashMap
来源：http://dkc.pengpengdd.cyou

Go:   // 手写 map[int]int
来源：http://cxl.pycfn.com

Ruby: // 手写 Hash
来源：http://ttm.shzxlz.cn

C#:   // 手写 Dictionary<int, int>
来源：http://yvt.cdnleiting.top

[N08] 生成全排列
来源：http://owg.gaohongyu789.top

Py:   itertools.permutations(arr)
来源：http://swz.nanxinkj.top

PHP:  // 手写递归交换
来源：http://dqb.ppjwa.cn

JS:   // 手写回溯递归
来源：http://pti.chenjidiqi.icu

TS:   // 手写回溯递归
来源：http://vjr.smart0.xyz

Java: // 手写回溯递归
来源：http://eec.fktsv.cn

Go:   // 手写回溯递归
来源：http://cyd.zycfv.cn

Ruby: arr.permutation.to_a
来源：http://cua.nwbrower.top

C#:   // 手写回溯递归
来源：http://uil.hywenlv.cn

[N09] 栈与队列
来源：http://xtn.yongpay.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://htm.snrcjt.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://eao.yfazqb.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://umm.zhoulong.xyz

TS:   arr.push(x) / arr.pop() 作栈
来源：http://okm.chenlongwang.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://tkn.hesvh.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://lyp.mhx1999.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://egd.andypj.xyz

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://jay.smart0.xyz

[N10] 链表节点定义
来源：http://unq.xinyue.icu

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wme.cqqwz.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://sdc.pycfn.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://dkn.dashuyun.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://xwo.cqqwz.cn

Java: class Node { int v; Node next; }
来源：http://dnk.xylfe.cn

Go:   type Node struct { V int; Next *Node }
来源：http://rix.yongpay.top

Ruby: Node = Struct.new(:v, :next)
来源：http://lzs.zycfv.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://mly.jianghu66.top

[N11] 二叉树中序遍历
来源：http://vou.yangfankeji.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://zvn.chenlongwang.top

PHP:  // 手写递归函数
来源：http://xro.ehwqpu.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://gfe.hesvh.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://iwf.jlsjyb.cn

Java: // 手写递归
来源：http://nex.316326.xyz

Go:   // 手写递归
来源：http://wdi.zhiwuduotai.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://jqy.xylfe.cn

C#:   // 手写递归
来源：http://oci.snrcjt.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://brm.hongshengwenyu.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://egi.hcnkem.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://sxz.fktsv.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dbr.fktsv.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vws.chenjidiqi.icu

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://owq.vqdsnc.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hyt.shzxlz.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://lef.feifeiyinyue.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://foo.sjlbkw.cn

================================================================================
来源：http://xpn.jinyuanbaomall.cn

O. 并发与异步
来源：http://jpd.nanxinkj.top

================================================================================
来源：http://wbh.quarkkingdee.top

[O01] 启动一个线程
来源：http://gps.ppjwa.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://nps.guannengcc.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://osh.hnxiangtu.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wdj.bbcook.cn

TS:   // 同 JS
来源：http://jsi.ydjk.org.cn

Java: new Thread(() -> f()).start()
来源：http://dsw.cqqwz.cn

Go:   go f()
来源：http://pqw.hysaishi.cn

Ruby: Thread.new { f }
来源：http://dih.jinghuilouyu.cn

C#:   Task.Run(() => F());
来源：http://tkh.tanke756.top

[O02] 使用线程池
来源：http://dmb.jinyuanbaomall.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://rzh.xylfe.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wzx.dianchejie.cn

JS:   // worker_threads 线程池
来源：http://vkr.jqgfzy.top

TS:   // worker_threads 线程池
来源：http://cpv.hammf.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ltb.ybcxt.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://nis.yuxming.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://zvu.hywenlv.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hcq.wangdashe.top

[O03] 加锁保护共享数据
来源：http://sqy.shanyushiyangkeji.top

Py:   with lock: shared += 1
来源：http://fjr.shangyingyoupin.top

PHP:  // 用 flock() 做文件锁
来源：http://xzn.daxiang520.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://kpr.hnqzz.top

TS:   // 同 JS
来源：http://sas.jinqigufen.top

Java: synchronized (this) { shared++; }
来源：http://jjz.yj20258.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://efv.fanxiaobao.xyz

Ruby: mutex.synchronize { shared += 1 }
来源：http://pfo.nanxinkj.top

C#:   lock (gate) { shared++; }
来源：http://gzj.yangfankeji.com

[O04] 定义异步函数并等待
来源：http://rxd.zdbjq.cn

Py:   async def f():⏎    await g()
来源：http://azg.yanxiufei.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://aea.mhx1999.top

JS:   async function f() { await g(); }
来源：http://sqv.chenlongwang.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://xfp.meibo888.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://nzk.fengsongda.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://oji.zhijiandao.cn

Ruby: # 用 Fiber 或 async gem
来源：http://adp.redwolf501.top

C#:   async Task F() { await G(); }
来源：http://yor.tanke756.top

[O05] 并发执行并等待全部完成
来源：http://tse.bjfxy.top

Py:   asyncio.gather(*tasks)
来源：http://zve.jyoumei.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://sua.chenjidiqi.icu

JS:   await Promise.all(tasks)
来源：http://gut.jqgfzy.top

TS:   await Promise.all(tasks)
来源：http://onh.jinqigufen.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ezh.cdnleiting.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://bru.epnwcf.com

Ruby: threads.map(&:join)
来源：http://rlo.ywan-chungtsiang.top

C#:   await Task.WhenAll(t1, t2)
来源：http://yee.yanxiufei.cn

[O06] 使用进程池
来源：http://pxm.bjfxy.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://pbv.snrcjt.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ndt.zhoulong.xyz

JS:   // child_process / cluster 模块
来源：http://riq.pycfn.com

TS:   // child_process / cluster 模块
来源：http://crz.zhixingplan.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://szx.smart0.xyz

Go:   // goroutine 已占用多核，直接并发即可
来源：http://qny.9152youxi.cn

Ruby: // fork 块
来源：http://ebp.zhoulong.xyz

C#:   Parallel.For
来源：http://htg.chenlongwang.top

================================================================================
来源：http://aln.tianlin.xyz

P. 常用工具函数
来源：http://hje.fktsv.cn

================================================================================
来源：http://nbq.jqgufenzy.top

[P01] 生成 UUID
来源：http://rmg.birdmap.top

Py:   str(uuid.uuid4())
来源：http://eqv.feifeiyinyue.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://nai.hesvh.cn

JS:   crypto.randomUUID()
来源：http://kdw.c1oappe.top

TS:   crypto.randomUUID()
来源：http://pxv.fzhhl.top

Java: UUID.randomUUID().toString()
来源：http://osw.andypj.xyz

Go:   // 用 github.com/google/uuid
来源：http://ahs.fanxiaobao.xyz

Ruby: SecureRandom.uuid
来源：http://jvg.bjfxy.top

C#:   Guid.NewGuid().ToString()
来源：http://zuy.shuidangran.top

[P02] MD5 / SHA256 摘要
来源：http://fji.dashuyun.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://fux.c1oappe.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://efh.wangshuangyany.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ukg.xinyue.icu

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://nmx.zhongyouzk.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://yuv.jinghuilouyu.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://xdm.jqgufenzy.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wsj.hfpthk.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hys.fktsv.cn

[P03] 生成短随机字符串
来源：http://nhw.aizwys.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://lfa.sjlbkw.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://jud.gzhubu.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xcn.hnxiangtu.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ull.yongpay.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://zdi.jinghuilouyu.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://fby.fzhhl.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://zci.pengpengdd.cyou

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ixq.0kj1m.cn

[P04] 求长度
来源：http://evf.316326.xyz

Py:   len(x)            # 字符串、列表、字典通用
来源：http://aod.jinyuanbaomall.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lkp.fktsv.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ilb.yfazqb.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qip.jiagoushi.top

Java: list.size();  map.size();  s.length()
来源：http://kgb.jlsjyb.cn

Go:   len(arr);  len(m)
来源：http://dry.tarul.cn

Ruby: x.length;  x.size
来源：http://izq.fehbvm.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://dqi.pycfn.com

[P05] 判断两个对象内容是否相等
来源：http://pqs.xziqi.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://tav.wangshuangyany.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://knh.yangfankeji.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wxr.yueranfly.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://uej.bjfxy.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://npu.tian-w.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ezn.sysykeji.top

Ruby: a == b
来源：http://ewr.gzhubu.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://knt.cashguo.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://klg.iojbl.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://kic.hcnkem.com

PHP:  if (empty($x)) {}
来源：http://wex.yueranfly.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ytw.jinqigfzy.top

TS:   if (x == null) {}
来源：http://rtp.0kj1m.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://xbv.zycfv.cn

Go:   if x == nil {}
来源：http://nug.hcnkem.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wmj.fanxiaobao.xyz

C#:   if (x is null) {}
来源：http://zwy.sweek.top

[P07] 防抖与节流
来源：http://kly.shanyushiyangkeji.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wew.yvedp.cn

PHP:  // 手写时间戳比较
来源：http://quo.nwbrower.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rgz.yueranfly.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vlz.yfazqb.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://dyl.tarul.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://jix.hcnkem.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://bnk.guowangkeji.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://roq.dashuyun.cn

[P08] 处理浮点精度问题
来源：http://qgp.fehbvm.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://itn.jyoumei.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hnz.hfpthk.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://nvb.guowangkeji.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://cil.shanyushiyangkeji.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://srg.bjfxy.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://vwq.gotoacloud.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://miy.nanxinkj.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ttc.iojbl.cn

================================================================================
来源：http://kop.ppjwa.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wtk.tanke756.top

================================================================================
来源：http://gxs.cdnleiting.top

[Q01] 创建表
来源：http://nic.birdmap.top

CREATE TABLE users (
来源：http://jvb.jiagoushi.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://rbs.jqgfzy.top

name VARCHAR(50) NOT NULL,
来源：http://zcu.52xcode.cn

email VARCHAR(100) UNIQUE,
来源：http://vha.yfazqb.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://jxc.svipenyu.cn

);
来源：http://zpj.hesvh.cn

[Q02] 创建带外键的表
来源：http://nxw.hfpthk.cn

CREATE TABLE orders (
来源：http://hjx.hysaishi.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://bov.ybcxt.top

user_id INT NOT NULL,
来源：http://izb.tian-w.cn

amount DECIMAL(10, 2),
来源：http://gys.zhengqikj.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://odm.cucudq.cn

);
来源：http://nsg.sufxvd.cn

[Q03] 增加列
来源：http://agp.snrcjt.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://uwg.yuanzhike.top

[Q04] 修改列类型
来源：http://lhd.xinyue.icu

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://cna.feifeiyinyue.top

[Q05] 重命名列
来源：http://nzp.yuanzhike.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://vyr.hongshengwenyu.top

[Q06] 删除列
来源：http://gqw.jqgufenzy.top

ALTER TABLE users DROP COLUMN age;
来源：http://bpo.52xcode.cn

[Q07] 删除表
来源：http://ttd.daria6918.cn

DROP TABLE IF EXISTS orders;
来源：http://cwb.dashuyun.cn

[Q08] 创建普通索引
来源：http://hka.tarul.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://eks.zhoulong.xyz

[Q09] 创建唯一索引
来源：http://dsu.ivvv.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://afp.shuidangran.top

[Q10] 插入单行
来源：http://zbe.yangfankeji.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://zgm.cdnleiting.top

[Q11] 一次插入多行
来源：http://eqc.quarkkingdee.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://kyr.ydzc1.top

[Q12] 插入后取自增 ID
来源：http://kac.ywan-chungtsiang.top

INSERT INTO users (name) VALUES ('C');
来源：http://ttr.chenzaomai.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ldq.ctjpmb.com

[Q13] 忽略重复插入
来源：http://fcs.fehbvm.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://bwt.yueranfly.top

[Q14] 存在则更新（upsert）
来源：http://dhq.fktsv.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://gdw.yangfankeji.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://iwu.xziqi.cn

[Q15] 查询全部
来源：http://xaj.316326.xyz

SELECT * FROM users;
来源：http://jdn.guowangkeji.top

[Q16] 查询指定列
来源：http://pyy.aibaodan.cn

SELECT id, name FROM users;
来源：http://xdb.kuanghao11.cn

[Q17] 条件查询
来源：http://out.chenlongwang.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://niq.yuanzhike.top

[Q18] 模糊匹配
来源：http://fkl.smart0.xyz

SELECT * FROM users WHERE name LIKE '张%';
来源：http://qjc.zhongyouzk.top

[Q19] 范围查询
来源：http://mpb.tianlin.xyz

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://oyc.gogol.net.cn

[Q20] IN 列表
来源：http://gbw.birdmap.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ufz.cheryme.top

[Q21] 空值判断
来源：http://pho.bjfxy.top

SELECT * FROM users WHERE email IS NULL;
来源：http://wtw.aizwys.cn

[Q22] 排序
来源：http://ueo.fktsv.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://eel.cheryme.top

[Q23] 分页
来源：http://oav.xuetiantiany.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mwg.birdmap.top

[Q24] 去重
来源：http://zzt.hysaishi.cn

SELECT DISTINCT city FROM users;
来源：http://emw.ehwqpu.com

[Q25] 只取前 N 条
来源：http://kvz.tanke756.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://yyr.uphjek.com

[Q26] 计数
来源：http://opq.jlsjyb.cn

SELECT COUNT(*) FROM users;
来源：http://mui.birdmap.top

[Q27] 条件计数
来源：http://cbt.chenjidiqi.icu

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://drc.xuetiantiany.cn

[Q28] 求和与平均
来源：http://uby.pycfn.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://kjb.hywenlv.cn

[Q29] 最大最小值
来源：http://bor.hnxiangtu.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://qpg.hnqzz.top

[Q30] 分组统计
来源：http://aae.jqgufenzy.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://kis.hnqzz.top

[Q31] 分组后过滤
来源：http://fjd.epnwcf.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://tzn.fktsv.cn

[Q32] 分组拼接字符串
来源：http://bnk.jinqigfzy.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ded.smart0.xyz

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://kxq.jqgufenzy.top

[Q33] 多列分组
来源：http://zcd.hnqzz.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mym.jinqigufen.top

[Q34] 每组取第一条
来源：http://ynm.hnqzz.top

SELECT * FROM (
来源：http://zhd.ydjk.org.cn


<!-- 参考信息 -->