代发 wailian999

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hqg.shuidangran.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://emx.cheryme.top

C#:   // 手写递归，或 Array.Sort
来源：http://ipi.fzhhl.top

[N04] 斐波那契数列
来源：http://plw.cqqwz.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://usj.birdmap.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hgq.hysaishi.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ztd.smart0.xyz

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gmk.epnwcf.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://nem.hysaishi.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://znr.xingfuxueyuan.xyz

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://uzr.xuetiantiany.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://syf.yfazqb.com

[N05] 最大公约数
来源：http://rwl.sjlbkw.cn

Py:   math.gcd(a, b)
来源：http://jwb.yongpay.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ski.aizwys.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mjo.ivvv.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hgm.nanxinkj.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://tfi.smart0.xyz

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://tyy.ctjpmb.com

Ruby: a.gcd(b)
来源：http://gek.dashuyun.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ebw.yfazqb.com

[N06] 判断回文字符串
来源：http://gxe.xylfe.cn

Py:   s == s[::-1]
来源：http://qwx.gzhubu.top

PHP:  $s === strrev($s);
来源：http://fvy.hongshengwenyu.top

JS:   s === [...s].reverse().join("")
来源：http://oeu.hywenlv.cn

TS:   s === [...s].reverse().join("")
来源：http://iwu.gaohongyu789.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://yyx.cdnleiting.top

Go:   // 双指针从两端比较
来源：http://kte.wangdashe.top

Ruby: s == s.reverse
来源：http://ilj.ppjwa.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://hxa.hnxiangtu.top

[N07] 两数之和（返回下标）
来源：http://auf.vqdsnc.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://vty.feifeiyinyue.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hzm.sweek.top

JS:   // 手写 Map：map.set(v, i)
来源：http://ctm.pycfn.com

TS:   // 手写 Map<string, number>
来源：http://dlh.uphjek.com

Java: // 手写 HashMap
来源：http://jpd.pycfn.com

Go:   // 手写 map[int]int
来源：http://yri.zhixingplan.top

Ruby: // 手写 Hash
来源：http://fwk.xuanzx.com

C#:   // 手写 Dictionary<int, int>
来源：http://ibt.hysaishi.cn

[N08] 生成全排列
来源：http://pgs.xuetiantiany.cn

Py:   itertools.permutations(arr)
来源：http://bds.yonumen.top

PHP:  // 手写递归交换
来源：http://zcl.chenjidiqi.icu

JS:   // 手写回溯递归
来源：http://mhd.fzhhl.top

TS:   // 手写回溯递归
来源：http://qnh.shanyushiyangtech.top

Java: // 手写回溯递归
来源：http://mrg.xuanzx.com

Go:   // 手写回溯递归
来源：http://pca.chenlongwang.top

Ruby: arr.permutation.to_a
来源：http://vve.hcnkem.com

C#:   // 手写回溯递归
来源：http://jpt.gogol.net.cn

[N09] 栈与队列
来源：http://ilh.tian-w.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://bum.yj202588.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://pix.yvedp.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ofj.gogol.net.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://dfx.dianchejie.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ljm.gogol.net.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://pxp.hnxiangtu.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://czz.nanxuanxn.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wqv.tanke756.top

[N10] 链表节点定义
来源：http://jrs.yfazqb.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://nty.guowangkeji.top

PHP:  class Node { public $v; public $next = null; }
来源：http://tgb.hammf.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://fzk.tarul.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://pnz.sweek.top

Java: class Node { int v; Node next; }
来源：http://wok.hywenlv.cn

Go:   type Node struct { V int; Next *Node }
来源：http://top.nanxinkj.top

Ruby: Node = Struct.new(:v, :next)
来源：http://zon.9152youxi.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ljg.gzhubu.top

[N11] 二叉树中序遍历
来源：http://odn.ywan-chungtsiang.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://eku.gaohongyu789.top

PHP:  // 手写递归函数
来源：http://fay.shanyushiyangtech.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qis.uphjek.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wbc.zhixingplan.top

Java: // 手写递归
来源：http://vnx.yfazqb.com

Go:   // 手写递归
来源：http://wkb.yj20258.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://qda.yanxiufei.cn

C#:   // 手写递归
来源：http://ccu.chenlongwang.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://fer.uphjek.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://apx.yongpay.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://fkt.yj202588.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zzv.sufxvd.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vno.0kj1m.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://tkj.shuidangran.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://lua.ehwqpu.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://axl.zhijiandao.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://uzz.zhengqikj.top

================================================================================
来源：http://ejc.daxiang520.top

O. 并发与异步
来源：http://wld.ctjpmb.com

================================================================================
来源：http://yvg.tianlin.xyz

[O01] 启动一个线程
来源：http://yve.hcnkem.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://vqk.xuanzx.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ntz.yuxming.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://vfl.zhoulong.xyz

TS:   // 同 JS
来源：http://gbz.jqgfzy.top

Java: new Thread(() -> f()).start()
来源：http://xzf.yuanzhike.top

Go:   go f()
来源：http://dad.andypj.xyz

Ruby: Thread.new { f }
来源：http://cnh.tian-w.cn

C#:   Task.Run(() => F());
来源：http://jxs.aibaodan.cn

[O02] 使用线程池
来源：http://isz.fehbvm.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://qoj.yongpay.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://msh.hfpthk.cn

JS:   // worker_threads 线程池
来源：http://nyx.jlsjyb.cn

TS:   // worker_threads 线程池
来源：http://cnm.cdnleiting.top

Java: Executors.newFixedThreadPool(4)
来源：http://fvy.guannengcc.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://kfm.hammf.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ocp.tian-w.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://sis.aibaodan.cn

[O03] 加锁保护共享数据
来源：http://iyk.ydjk.org.cn

Py:   with lock: shared += 1
来源：http://fvd.kuanghao11.cn

PHP:  // 用 flock() 做文件锁
来源：http://drt.gogol.net.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://den.hnxiangtu.top

TS:   // 同 JS
来源：http://ulf.hfpthk.cn

Java: synchronized (this) { shared++; }
来源：http://gvh.ydjk.org.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wju.zhiwuduotai.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://rxt.ydjk.org.cn

C#:   lock (gate) { shared++; }
来源：http://svq.yuxming.cn

[O04] 定义异步函数并等待
来源：http://yck.svipenyu.cn

Py:   async def f():⏎    await g()
来源：http://elu.ydjk.org.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://vfi.xylfe.cn

JS:   async function f() { await g(); }
来源：http://mrv.sjlbkw.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ekh.daxiang520.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://tnq.jinghuilouyu.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mqt.vqdsnc.cn

Ruby: # 用 Fiber 或 async gem
来源：http://mht.wangshuangyany.cn

C#:   async Task F() { await G(); }
来源：http://ida.jqgufenzy.top

[O05] 并发执行并等待全部完成
来源：http://nav.jinyuanbaomall.cn

Py:   asyncio.gather(*tasks)
来源：http://uak.nanxuanxn.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://gue.jlsjyb.cn

JS:   await Promise.all(tasks)
来源：http://ukf.hammf.cn

TS:   await Promise.all(tasks)
来源：http://hbe.guannengcc.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ptz.kuanghao11.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://dzw.sjlbkw.cn

Ruby: threads.map(&:join)
来源：http://hsv.sxryk.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://syh.tian-w.cn

[O06] 使用进程池
来源：http://har.jqgufenzy.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://lxo.jqgfzy.top

PHP:  // pcntl_fork 或多进程队列
来源：http://pbz.zycfv.cn

JS:   // child_process / cluster 模块
来源：http://ykt.gaohongyu789.top

TS:   // child_process / cluster 模块
来源：http://snj.hnxiangtu.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://iit.pengpengdd.cyou

Go:   // goroutine 已占用多核，直接并发即可
来源：http://tau.yfazqb.com

Ruby: // fork 块
来源：http://pmh.cheryme.top

C#:   Parallel.For
来源：http://pny.hysaishi.cn

================================================================================
来源：http://zpw.tanke756.top

P. 常用工具函数
来源：http://rln.nwbrower.top

================================================================================
来源：http://mqs.zhiwuduotai.top

[P01] 生成 UUID
来源：http://cbu.gaohongyu789.top

Py:   str(uuid.uuid4())
来源：http://qnt.hnxiangtu.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://siu.c1oappe.top

JS:   crypto.randomUUID()
来源：http://weo.jqgfzy.top

TS:   crypto.randomUUID()
来源：http://rby.andypj.xyz

Java: UUID.randomUUID().toString()
来源：http://hif.andypj.xyz

Go:   // 用 github.com/google/uuid
来源：http://jns.hysaishi.cn

Ruby: SecureRandom.uuid
来源：http://zcq.chenzaomai.com

C#:   Guid.NewGuid().ToString()
来源：http://uye.yueranfly.top

[P02] MD5 / SHA256 摘要
来源：http://uzl.cucudq.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mat.nanxuanxn.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://zbx.xziqi.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ncv.zdbjq.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://tyn.cucudq.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://dnw.zdqjudy.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://rrh.yvedp.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://bha.zhixingplan.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://fop.chenzaomai.com

[P03] 生成短随机字符串
来源：http://twj.yj20258888.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ebu.shzxlz.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ycq.tianlin.xyz

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lft.hywenlv.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://iar.feifeiyinyue.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://uio.yj20258888.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://zti.fengsongda.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://xhf.feifeiyinyue.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://eqw.jinghuilouyu.cn

[P04] 求长度
来源：http://fcn.hnqzz.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wil.hywenlv.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://tvj.birdmap.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://yfj.shanyushiyangtech.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://eiu.yfazqb.com

Java: list.size();  map.size();  s.length()
来源：http://ruw.ydjk.org.cn

Go:   len(arr);  len(m)
来源：http://zrx.shanyushiyangtech.top

Ruby: x.length;  x.size
来源：http://kzk.hammf.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://oda.jinghuilouyu.cn

[P05] 判断两个对象内容是否相等
来源：http://mjd.hfpthk.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://okv.jinyuanbaomall.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wte.nanxuanxn.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://jqx.jiagoushi.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://tbg.nanxinkj.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://tpf.pengpengdd.cyou

Go:   reflect.DeepEqual(a, b)
来源：http://hbw.xylfe.cn

Ruby: a == b
来源：http://oev.xinyue.icu

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://tpz.zhijiandao.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://cih.zhengqikj.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ndg.zhixingplan.top

PHP:  if (empty($x)) {}
来源：http://zfg.jinqigufen.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://tkz.0kj1m.cn

TS:   if (x == null) {}
来源：http://azb.ybcxt.top

Java: if (x == null || x.isEmpty()) {}
来源：http://fsw.feifeiyinyue.top

Go:   if x == nil {}
来源：http://tsi.xylfe.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://iwn.shzxlz.cn

C#:   if (x is null) {}
来源：http://wdm.yuanzhike.top

[P07] 防抖与节流
来源：http://kkp.hywenlv.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hny.tian-w.cn

PHP:  // 手写时间戳比较
来源：http://yap.shzxlz.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jxg.aibaodan.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hjb.chenzaomai.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://aty.birdmap.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://lrc.shzxlz.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://sai.fengsongda.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://unb.mhx1999.top

[P08] 处理浮点精度问题
来源：http://vuv.zycfv.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://cga.hnqzz.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://zfy.hywenlv.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://cwg.fanxiaobao.xyz

TS:   (0.1 + 0.2).toFixed(2)
来源：http://uhx.hesvh.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mdg.ybcxt.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://exf.cqqwz.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://nvu.yanxiufei.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://xjw.yuxming.cn

================================================================================
来源：http://xbx.uphjek.com

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ywr.fktsv.cn

================================================================================
来源：http://dha.pengpengdd.cyou

[Q01] 创建表
来源：http://utj.hongshengwenyu.top

CREATE TABLE users (
来源：http://jom.dianchejie.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://pqq.sjlbkw.cn

name VARCHAR(50) NOT NULL,
来源：http://fqz.chenzaomai.com

email VARCHAR(100) UNIQUE,
来源：http://dco.hnxiangtu.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://vhv.fehbvm.com

);
来源：http://gjd.52xcode.cn

[Q02] 创建带外键的表
来源：http://boy.cucudq.cn

CREATE TABLE orders (
来源：http://add.aizwys.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://jqq.cdnleiting.top

user_id INT NOT NULL,
来源：http://lad.shanyushiyangkeji.top

amount DECIMAL(10, 2),
来源：http://mqw.fengsongda.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://acb.vehdjk.com

);
来源：http://iol.wangdashe.top

[Q03] 增加列
来源：http://bpn.vehdjk.com

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://nkr.guannengcc.top

[Q04] 修改列类型
来源：http://adn.xziqi.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://oki.yj202588.top

[Q05] 重命名列
来源：http://wrj.shzxlz.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://izn.52xcode.cn

[Q06] 删除列
来源：http://xto.cqqwz.cn

ALTER TABLE users DROP COLUMN age;
来源：http://czl.chenjidiqi.icu

[Q07] 删除表
来源：http://qmx.daria6918.cn

DROP TABLE IF EXISTS orders;
来源：http://ghm.uphjek.com

[Q08] 创建普通索引
来源：http://bry.hysaishi.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://kdk.jyoumei.cn

[Q09] 创建唯一索引
来源：http://vkg.cashguo.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://gqi.jinyuanbaomall.cn

[Q10] 插入单行
来源：http://omf.zdbjq.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://fgk.bjfxy.top

[Q11] 一次插入多行
来源：http://eds.xingfuxueyuan.xyz

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ffa.bjfxy.top

[Q12] 插入后取自增 ID
来源：http://fpo.quarkkingdee.top

INSERT INTO users (name) VALUES ('C');
来源：http://lbz.jyoumei.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://usz.wangdashe.top

[Q13] 忽略重复插入
来源：http://sge.fzhhl.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ypy.52xcode.cn

[Q14] 存在则更新（upsert）
来源：http://xov.hfpthk.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://upr.yvedp.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://pov.cashguo.top

[Q15] 查询全部
来源：http://gcs.vehdjk.com

SELECT * FROM users;
来源：http://yxa.ppjwa.cn

[Q16] 查询指定列
来源：http://xdh.fanxiaobao.xyz

SELECT id, name FROM users;
来源：http://png.jqgfzy.top

[Q17] 条件查询
来源：http://whz.andypj.xyz

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://vnd.ywan-chungtsiang.top

[Q18] 模糊匹配
来源：http://psy.jqgufenzy.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://vvx.xylfe.cn

[Q19] 范围查询
来源：http://aql.snrcjt.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://svv.wangshuangyany.cn

[Q20] IN 列表
来源：http://qep.0kj1m.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ljm.gzhubu.top

[Q21] 空值判断
来源：http://gkk.shanyushiyangkeji.top

SELECT * FROM users WHERE email IS NULL;
来源：http://xxf.ppjwa.cn

[Q22] 排序
来源：http://avy.cashguo.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://xtw.chenjidiqi.icu

[Q23] 分页
来源：http://ctw.yonumen.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ueg.andypj.xyz

[Q24] 去重
来源：http://yro.yonumen.top

SELECT DISTINCT city FROM users;
来源：http://ick.jinyuanbaomall.cn

[Q25] 只取前 N 条
来源：http://fbz.cqqwz.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mwd.tanke756.top

[Q26] 计数
来源：http://oib.yj20258.top

SELECT COUNT(*) FROM users;
来源：http://zyh.hongshengwenyu.top

[Q27] 条件计数
来源：http://unc.birdmap.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ttw.hnxiangtu.top

[Q28] 求和与平均
来源：http://hrg.hfpthk.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://uso.jinghuilouyu.cn

[Q29] 最大最小值
来源：http://eke.wangshuangyany.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://uih.nwbrower.top

[Q30] 分组统计
来源：http://kjc.birdmap.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://nxf.zhixingplan.top

[Q31] 分组后过滤
来源：http://sjk.meibo888.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://xpb.yfazqb.com

[Q32] 分组拼接字符串
来源：http://vde.wangshuangyany.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://miz.epnwcf.com

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://boq.ywan-chungtsiang.top

[Q33] 多列分组
来源：http://zkj.sysykeji.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ezc.ppjwa.cn

[Q34] 每组取第一条
来源：http://gbx.fzhhl.top

SELECT * FROM (
来源：http://cak.xuetiantiany.cn


<!-- 参考信息 -->