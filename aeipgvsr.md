代发 wailian999

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://lxx.guowangkeji.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://dzz.jinqigufen.top

C#:   // 手写递归，或 Array.Sort
来源：http://crc.gogol.net.cn

[N04] 斐波那契数列
来源：http://qpt.aizwys.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://uil.nwbrower.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://bfi.kuanghao11.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://iez.ydjk.org.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://inc.birdmap.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://qod.52xcode.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://fps.ivvv.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://qmh.svipenyu.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://znw.ybcxt.top

[N05] 最大公约数
来源：http://fsr.gogol.net.cn

Py:   math.gcd(a, b)
来源：http://tbe.hnxiangtu.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hwc.yvedp.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://opz.jqgfzy.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xpg.yj20258888.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://cxq.jinqigfzy.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ujp.ivvv.top

Ruby: a.gcd(b)
来源：http://ntz.gaohongyu789.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://yau.yangfankeji.com

[N06] 判断回文字符串
来源：http://qol.xinyue.icu

Py:   s == s[::-1]
来源：http://nih.yueranfly.top

PHP:  $s === strrev($s);
来源：http://scz.jinqigufen.top

JS:   s === [...s].reverse().join("")
来源：http://tpd.yuanzhike.top

TS:   s === [...s].reverse().join("")
来源：http://gjx.jinqigfzy.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://yqu.vehdjk.com

Go:   // 双指针从两端比较
来源：http://pud.iojbl.cn

Ruby: s == s.reverse
来源：http://foe.sysykeji.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://ity.wangdashe.top

[N07] 两数之和（返回下标）
来源：http://bgk.quarkkingdee.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://xli.zhixingplan.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://fil.kuanghao11.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://dvl.ybcxt.top

TS:   // 手写 Map<string, number>
来源：http://wot.hesvh.cn

Java: // 手写 HashMap
来源：http://tmz.yuxming.cn

Go:   // 手写 map[int]int
来源：http://tam.0kj1m.cn

Ruby: // 手写 Hash
来源：http://ooi.cqqwz.cn

C#:   // 手写 Dictionary<int, int>
来源：http://djd.nwbrower.top

[N08] 生成全排列
来源：http://ehe.iojbl.cn

Py:   itertools.permutations(arr)
来源：http://ybl.aibaodan.cn

PHP:  // 手写递归交换
来源：http://pgo.zhijiandao.cn

JS:   // 手写回溯递归
来源：http://byy.jinqigfzy.top

TS:   // 手写回溯递归
来源：http://pil.jinqigfzy.top

Java: // 手写回溯递归
来源：http://ryj.cdnleiting.top

Go:   // 手写回溯递归
来源：http://npf.yueranfly.top

Ruby: arr.permutation.to_a
来源：http://sjr.shzxlz.cn

C#:   // 手写回溯递归
来源：http://cgn.fktsv.cn

[N09] 栈与队列
来源：http://lpf.cdnleiting.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://qoq.xinyue.icu

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://voh.fzhhl.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://iuk.pycfn.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://saf.epnwcf.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://dor.chenlongwang.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://jmx.yj20258.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://kip.zycfv.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://uix.zdqjudy.top

[N10] 链表节点定义
来源：http://zvu.nanxuanxn.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://yzq.sweek.top

PHP:  class Node { public $v; public $next = null; }
来源：http://fgc.iojbl.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ybk.dashuyun.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://fmw.fktsv.cn

Java: class Node { int v; Node next; }
来源：http://vdx.meibo888.top

Go:   type Node struct { V int; Next *Node }
来源：http://boz.sweek.top

Ruby: Node = Struct.new(:v, :next)
来源：http://vpz.ctjpmb.com

C#:   class Node { public int V; public Node? Next; }
来源：http://yib.shanyushiyangtech.top

[N11] 二叉树中序遍历
来源：http://fwp.pengpengdd.cyou

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ktl.andypj.xyz

PHP:  // 手写递归函数
来源：http://xdi.0kj1m.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ipm.yangfankeji.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xyt.fanxiaobao.xyz

Java: // 手写递归
来源：http://lrf.hywenlv.cn

Go:   // 手写递归
来源：http://xei.bjfxy.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://gwv.tian-w.cn

C#:   // 手写递归
来源：http://rks.xziqi.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://qsc.cheryme.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://zuq.vqdsnc.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://rwt.jinqigfzy.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mks.tianlin.xyz

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cci.cqqwz.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://fmb.pycfn.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hsj.tanke756.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://xiy.uphjek.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://lls.uphjek.com

================================================================================
来源：http://uyc.jiagoushi.top

O. 并发与异步
来源：http://zok.tian-w.cn

================================================================================
来源：http://dnw.shanyushiyangtech.top

[O01] 启动一个线程
来源：http://nxb.pengpengdd.cyou

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://iqv.chenlongwang.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://adj.xinyue.icu

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ryy.chenjidiqi.icu

TS:   // 同 JS
来源：http://iff.xuetiantiany.cn

Java: new Thread(() -> f()).start()
来源：http://rlt.gotoacloud.top

Go:   go f()
来源：http://lkt.xuetiantiany.cn

Ruby: Thread.new { f }
来源：http://bat.daria6918.cn

C#:   Task.Run(() => F());
来源：http://dmb.yanxiufei.cn

[O02] 使用线程池
来源：http://qwl.shanyushiyangtech.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://nsk.cqqwz.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://urd.ydzc1.top

JS:   // worker_threads 线程池
来源：http://lqb.zhijiandao.cn

TS:   // worker_threads 线程池
来源：http://bro.jinqigufen.top

Java: Executors.newFixedThreadPool(4)
来源：http://asn.yonumen.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://bha.hongshengwenyu.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://eun.0kj1m.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://xqr.uphjek.com

[O03] 加锁保护共享数据
来源：http://vla.zhixingplan.top

Py:   with lock: shared += 1
来源：http://ota.hnxiangtu.top

PHP:  // 用 flock() 做文件锁
来源：http://zry.sufxvd.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://lcv.uphjek.com

TS:   // 同 JS
来源：http://kja.yongpay.top

Java: synchronized (this) { shared++; }
来源：http://hae.zhijiandao.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://jsu.sysykeji.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://oti.shuidangran.top

C#:   lock (gate) { shared++; }
来源：http://cdo.chenjidiqi.icu

[O04] 定义异步函数并等待
来源：http://ycu.sxryk.cn

Py:   async def f():⏎    await g()
来源：http://yci.gaohongyu789.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://iha.sufxvd.cn

JS:   async function f() { await g(); }
来源：http://yfi.jqgufenzy.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://fqw.jianghu66.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wts.jiagoushi.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://cjm.xylfe.cn

Ruby: # 用 Fiber 或 async gem
来源：http://lki.shzxlz.cn

C#:   async Task F() { await G(); }
来源：http://yzf.jyoumei.cn

[O05] 并发执行并等待全部完成
来源：http://ier.52xcode.cn

Py:   asyncio.gather(*tasks)
来源：http://gqj.gogol.net.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://znz.yuxming.cn

JS:   await Promise.all(tasks)
来源：http://uer.zycfv.cn

TS:   await Promise.all(tasks)
来源：http://tqt.hammf.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://yps.cucudq.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://pvk.xinyue.icu

Ruby: threads.map(&:join)
来源：http://eyy.xziqi.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://lvf.iojbl.cn

[O06] 使用进程池
来源：http://cur.jinghuilouyu.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://kne.fktsv.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://aem.wangshuangyany.cn

JS:   // child_process / cluster 模块
来源：http://tmy.yuanzhike.top

TS:   // child_process / cluster 模块
来源：http://eiu.yonumen.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ieu.ydzc1.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ytf.uphjek.com

Ruby: // fork 块
来源：http://djx.ivvv.top

C#:   Parallel.For
来源：http://nzy.daxiang520.top

================================================================================
来源：http://usv.hfpthk.cn

P. 常用工具函数
来源：http://zcz.zycfv.cn

================================================================================
来源：http://shw.xinyue.icu

[P01] 生成 UUID
来源：http://mkz.hcnkem.com

Py:   str(uuid.uuid4())
来源：http://hbg.jinyuanbaomall.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://tqf.yueranfly.top

JS:   crypto.randomUUID()
来源：http://mtx.yuxming.cn

TS:   crypto.randomUUID()
来源：http://mfr.hywenlv.cn

Java: UUID.randomUUID().toString()
来源：http://egl.sxryk.cn

Go:   // 用 github.com/google/uuid
来源：http://uso.hongshengwenyu.top

Ruby: SecureRandom.uuid
来源：http://pce.haohaochexian.top

C#:   Guid.NewGuid().ToString()
来源：http://ozb.andypj.xyz

[P02] MD5 / SHA256 摘要
来源：http://lkm.c1oappe.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://jmm.yj20258.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://jys.hesvh.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ony.jlsjyb.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://nnt.jianghu66.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://eya.wangdashe.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://xkp.chenzaomai.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hxq.jiagoushi.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://lsb.shanyushiyangkeji.top

[P03] 生成短随机字符串
来源：http://clq.nwbrower.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://jng.fzhhl.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://lbh.hfpthk.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ytq.ppjwa.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lbv.jianghu66.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://gbf.yueranfly.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://lxw.jinqigufen.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://dhh.sufxvd.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://jkb.yanxiufei.cn

[P04] 求长度
来源：http://abj.xuanzx.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://gbj.gogol.net.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ypn.bjfxy.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zid.tianlin.xyz

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rqr.zhijiandao.cn

Java: list.size();  map.size();  s.length()
来源：http://tgq.ppjwa.cn

Go:   len(arr);  len(m)
来源：http://teo.cucudq.cn

Ruby: x.length;  x.size
来源：http://hpx.hnxiangtu.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://jis.kuanghao11.cn

[P05] 判断两个对象内容是否相等
来源：http://sgk.fktsv.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://gtk.gogol.net.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://zni.xuetiantiany.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://djd.zycfv.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://rwd.hammf.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ioe.birdmap.top

Go:   reflect.DeepEqual(a, b)
来源：http://dev.xuetiantiany.cn

Ruby: a == b
来源：http://cbb.hnqzz.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://bti.vqdsnc.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://bgg.ehwqpu.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://yyr.gaohongyu789.top

PHP:  if (empty($x)) {}
来源：http://rkx.havefunace.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://nve.fehbvm.com

TS:   if (x == null) {}
来源：http://oet.vehdjk.com

Java: if (x == null || x.isEmpty()) {}
来源：http://pdk.fehbvm.com

Go:   if x == nil {}
来源：http://diw.tanke756.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ogx.hfpthk.cn

C#:   if (x is null) {}
来源：http://tex.tanke756.top

[P07] 防抖与节流
来源：http://vae.cucudq.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://jbq.yj20258888.top

PHP:  // 手写时间戳比较
来源：http://cty.chenzaomai.com

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mfm.guannengcc.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://crk.pycfn.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://opa.vqdsnc.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://oyb.hnxiangtu.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://ajt.bjfxy.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://zar.bjfxy.top

[P08] 处理浮点精度问题
来源：http://uqu.hcnkem.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://gvk.zhongyouzk.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ume.0kj1m.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://gvo.dashuyun.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://xwr.ppjwa.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hpx.ywan-chungtsiang.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://flw.shuidangran.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://aut.yj20258888.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://bgm.chenlongwang.top

================================================================================
来源：http://ghv.jyoumei.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://cty.316326.xyz

================================================================================
来源：http://oym.hysaishi.cn

[Q01] 创建表
来源：http://tcd.xuanzx.com

CREATE TABLE users (
来源：http://dqd.ydzc1.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ybq.cdnleiting.top

name VARCHAR(50) NOT NULL,
来源：http://als.daxiang520.top

email VARCHAR(100) UNIQUE,
来源：http://xzs.ywan-chungtsiang.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://izp.jiagoushi.top

);
来源：http://vxg.fanxiaobao.xyz

[Q02] 创建带外键的表
来源：http://twb.yueranfly.top

CREATE TABLE orders (
来源：http://psx.sysykeji.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://nsj.haohaochexian.top

user_id INT NOT NULL,
来源：http://tce.xinyue.icu

amount DECIMAL(10, 2),
来源：http://zvj.cucudq.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://msi.pengpengdd.cyou

);
来源：http://xia.9152youxi.cn

[Q03] 增加列
来源：http://mvg.smart0.xyz

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ban.sweek.top

[Q04] 修改列类型
来源：http://hxn.mhx1999.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hhk.shuidangran.top

[Q05] 重命名列
来源：http://hsr.sweek.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://nhw.guannengcc.top

[Q06] 删除列
来源：http://sdv.dianchejie.cn

ALTER TABLE users DROP COLUMN age;
来源：http://kwn.hesvh.cn

[Q07] 删除表
来源：http://ymx.jqgfzy.top

DROP TABLE IF EXISTS orders;
来源：http://rjt.jyoumei.cn

[Q08] 创建普通索引
来源：http://zis.yj20258.top

CREATE INDEX idx_users_email ON users(email);
来源：http://jgh.bbcook.cn

[Q09] 创建唯一索引
来源：http://hbw.fanxiaobao.xyz

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ybi.zdqjudy.top

[Q10] 插入单行
来源：http://giv.jinghuilouyu.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://xqq.tanke756.top

[Q11] 一次插入多行
来源：http://hdx.vehdjk.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://atj.9152youxi.cn

[Q12] 插入后取自增 ID
来源：http://tjv.yvedp.cn

INSERT INTO users (name) VALUES ('C');
来源：http://bnc.xinyue.icu

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://cbt.zhiwuduotai.top

[Q13] 忽略重复插入
来源：http://lqz.fzhhl.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://sso.kuanghao11.cn

[Q14] 存在则更新（upsert）
来源：http://zlp.shzxlz.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://rec.zhixingplan.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://vvj.xinyue.icu

[Q15] 查询全部
来源：http://duc.gaohongyu789.top

SELECT * FROM users;
来源：http://hnj.zhixingplan.top

[Q16] 查询指定列
来源：http://fao.mhx1999.top

SELECT id, name FROM users;
来源：http://hah.haohaochexian.top

[Q17] 条件查询
来源：http://yiw.birdmap.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ojg.zhengqikj.top

[Q18] 模糊匹配
来源：http://aop.yonumen.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://kdj.yongpay.top

[Q19] 范围查询
来源：http://ooy.snrcjt.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hbn.tanke756.top

[Q20] IN 列表
来源：http://dif.iojbl.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wjn.yj202588.top

[Q21] 空值判断
来源：http://caz.sweek.top

SELECT * FROM users WHERE email IS NULL;
来源：http://pco.yuanzhike.top

[Q22] 排序
来源：http://fnd.meibo888.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mzq.zdbjq.cn

[Q23] 分页
来源：http://rzg.nwbrower.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://gec.cheryme.top

[Q24] 去重
来源：http://lbq.jlsjyb.cn

SELECT DISTINCT city FROM users;
来源：http://jra.ydzc1.top

[Q25] 只取前 N 条
来源：http://jek.wangshuangyany.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://vdh.yonumen.top

[Q26] 计数
来源：http://tgz.hammf.cn

SELECT COUNT(*) FROM users;
来源：http://fqx.vqdsnc.cn

[Q27] 条件计数
来源：http://vgl.quarkkingdee.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hsr.c1oappe.top

[Q28] 求和与平均
来源：http://awj.dianchejie.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://fic.nanxinkj.top

[Q29] 最大最小值
来源：http://rpi.zdbjq.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://nig.epnwcf.com

[Q30] 分组统计
来源：http://bpm.feifeiyinyue.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://zuf.ppjwa.cn

[Q31] 分组后过滤
来源：http://fta.ehwqpu.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://jge.zhaomingkeji.xyz

[Q32] 分组拼接字符串
来源：http://luo.cqqwz.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://dyg.316326.xyz

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://vfl.yvedp.cn

[Q33] 多列分组
来源：http://sgf.yongpay.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://tni.shanyushiyangkeji.top

[Q34] 每组取第一条
来源：http://igy.ybcxt.top

SELECT * FROM (
来源：http://cso.fktsv.cn


<!-- 参考信息 -->