代发 wailian999

PHP:  // 递归实现，或用 usort
来源：http://xqg.jinghuilouyu.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bgw.yj202588.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zcq.316326.xyz

Java: // 手写递归，或直接用 Arrays.sort
来源：http://pgw.jianghu66.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://cuw.shangyingyoupin.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://tuc.epnwcf.com

C#:   // 手写递归，或 Array.Sort
来源：http://fjc.tanke756.top

[N04] 斐波那契数列
来源：http://qzy.yj20258888.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://zup.yj20258888.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://get.c1oappe.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://evm.fzhhl.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rps.yuanzhike.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mmx.zycfv.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wde.zhixingplan.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ifk.hfpthk.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://sye.gogol.net.cn

[N05] 最大公约数
来源：http://svr.yuxming.cn

Py:   math.gcd(a, b)
来源：http://lak.ppjwa.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hmb.ctjpmb.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://syg.sysykeji.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xbd.kuanghao11.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://weg.yj20258888.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://gxa.guannengcc.top

Ruby: a.gcd(b)
来源：http://mka.tarul.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wkr.yueranfly.top

[N06] 判断回文字符串
来源：http://bxk.yj20258.top

Py:   s == s[::-1]
来源：http://acb.cheryme.top

PHP:  $s === strrev($s);
来源：http://puq.birdmap.top

JS:   s === [...s].reverse().join("")
来源：http://ook.fehbvm.com

TS:   s === [...s].reverse().join("")
来源：http://wwe.0kj1m.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://uqd.gzhubu.top

Go:   // 双指针从两端比较
来源：http://sir.hongshengwenyu.top

Ruby: s == s.reverse
来源：http://kni.bbcook.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://uew.hysaishi.cn

[N07] 两数之和（返回下标）
来源：http://wyg.nwbrower.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://zpk.guannengcc.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://zgm.cucudq.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://jxq.yfazqb.com

TS:   // 手写 Map<string, number>
来源：http://rgg.yj202588.top

Java: // 手写 HashMap
来源：http://ekj.hysaishi.cn

Go:   // 手写 map[int]int
来源：http://dqf.ctjpmb.com

Ruby: // 手写 Hash
来源：http://oxw.meibo888.top

C#:   // 手写 Dictionary<int, int>
来源：http://iyy.yj202588.top

[N08] 生成全排列
来源：http://sje.xinyue.icu

Py:   itertools.permutations(arr)
来源：http://rmt.xuetiantiany.cn

PHP:  // 手写递归交换
来源：http://swb.ybcxt.top

JS:   // 手写回溯递归
来源：http://iwm.cucudq.cn

TS:   // 手写回溯递归
来源：http://ale.snrcjt.cn

Java: // 手写回溯递归
来源：http://dew.zycfv.cn

Go:   // 手写回溯递归
来源：http://lqx.haohaochexian.top

Ruby: arr.permutation.to_a
来源：http://vml.yonumen.top

C#:   // 手写回溯递归
来源：http://oiu.jyoumei.cn

[N09] 栈与队列
来源：http://jnv.hfpthk.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://bxe.daxiang520.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://xtv.hesvh.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://tqo.hesvh.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://prf.daria6918.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://jis.pycfn.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mqf.aibaodan.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://gqp.gaohongyu789.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ppv.jiagoushi.top

[N10] 链表节点定义
来源：http://mhg.havefunace.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://npo.nanxinkj.top

PHP:  class Node { public $v; public $next = null; }
来源：http://xlr.fanxiaobao.xyz

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://iux.ivvv.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://rah.zdqjudy.top

Java: class Node { int v; Node next; }
来源：http://gaf.xylfe.cn

Go:   type Node struct { V int; Next *Node }
来源：http://boj.bjfxy.top

Ruby: Node = Struct.new(:v, :next)
来源：http://bvd.zhengqikj.top

C#:   class Node { public int V; public Node? Next; }
来源：http://qej.svipenyu.cn

[N11] 二叉树中序遍历
来源：http://cgm.ydjk.org.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ubi.sxryk.cn

PHP:  // 手写递归函数
来源：http://xex.jqgfzy.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rzu.zycfv.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yfv.svipenyu.cn

Java: // 手写递归
来源：http://lyl.yj202588.top

Go:   // 手写递归
来源：http://jlt.gaohongyu789.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://sdn.cucudq.cn

C#:   // 手写递归
来源：http://iud.dianchejie.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://yoo.wangdashe.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://raw.yonumen.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://oav.yangfankeji.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yxe.redwolf501.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ocy.gaohongyu789.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://bob.gotoacloud.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://dop.cdnleiting.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://auf.kuanghao11.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://orq.redwolf501.top

================================================================================
来源：http://vyx.chenjidiqi.icu

O. 并发与异步
来源：http://afn.yonumen.top

================================================================================
来源：http://lqj.tarul.cn

[O01] 启动一个线程
来源：http://cmj.sysykeji.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://vcq.xingfuxueyuan.xyz

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ien.ivvv.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://xit.cashguo.top

TS:   // 同 JS
来源：http://yqc.guannengcc.top

Java: new Thread(() -> f()).start()
来源：http://okx.gogol.net.cn

Go:   go f()
来源：http://xud.vqdsnc.cn

Ruby: Thread.new { f }
来源：http://rwh.zdbjq.cn

C#:   Task.Run(() => F());
来源：http://plw.shangyingyoupin.top

[O02] 使用线程池
来源：http://pks.jinyuanbaomall.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://qks.zhijiandao.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://tsc.ehwqpu.com

JS:   // worker_threads 线程池
来源：http://liy.shanyushiyangtech.top

TS:   // worker_threads 线程池
来源：http://zig.hysaishi.cn

Java: Executors.newFixedThreadPool(4)
来源：http://qeb.ctjpmb.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://tbe.uphjek.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://lfw.epnwcf.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://epz.0kj1m.cn

[O03] 加锁保护共享数据
来源：http://sej.haohaochexian.top

Py:   with lock: shared += 1
来源：http://elp.nwbrower.top

PHP:  // 用 flock() 做文件锁
来源：http://ctf.birdmap.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://lde.bjfxy.top

TS:   // 同 JS
来源：http://qgt.fehbvm.com

Java: synchronized (this) { shared++; }
来源：http://ydn.vqdsnc.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://qky.hywenlv.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ywg.xuanzx.com

C#:   lock (gate) { shared++; }
来源：http://frb.ivvv.top

[O04] 定义异步函数并等待
来源：http://hsa.xingfuxueyuan.xyz

Py:   async def f():⏎    await g()
来源：http://veq.cucudq.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://yjh.hnqzz.top

JS:   async function f() { await g(); }
来源：http://xwr.zhongyouzk.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://rad.tarul.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://vge.vehdjk.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://eti.jinqigfzy.top

Ruby: # 用 Fiber 或 async gem
来源：http://ogj.ivvv.top

C#:   async Task F() { await G(); }
来源：http://pkx.ydzc1.top

[O05] 并发执行并等待全部完成
来源：http://tra.hcnkem.com

Py:   asyncio.gather(*tasks)
来源：http://zxu.daxiang520.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://phs.hnqzz.top

JS:   await Promise.all(tasks)
来源：http://yom.ivvv.top

TS:   await Promise.all(tasks)
来源：http://wwy.hnxiangtu.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mmy.epnwcf.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hqr.meibo888.top

Ruby: threads.map(&:join)
来源：http://bxm.hcnkem.com

C#:   await Task.WhenAll(t1, t2)
来源：http://aua.yuanzhike.top

[O06] 使用进程池
来源：http://qac.sweek.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ylp.zhaomingkeji.xyz

PHP:  // pcntl_fork 或多进程队列
来源：http://kjg.wangshuangyany.cn

JS:   // child_process / cluster 模块
来源：http://lxu.hongshengwenyu.top

TS:   // child_process / cluster 模块
来源：http://inw.jinyuanbaomall.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://evj.birdmap.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://zlb.zhixingplan.top

Ruby: // fork 块
来源：http://vpj.gzhubu.top

C#:   Parallel.For
来源：http://iba.pengpengdd.cyou

================================================================================
来源：http://rpp.sufxvd.cn

P. 常用工具函数
来源：http://boq.cqqwz.cn

================================================================================
来源：http://fbg.havefunace.top

[P01] 生成 UUID
来源：http://jyc.yangfankeji.com

Py:   str(uuid.uuid4())
来源：http://xig.zdbjq.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://nmc.316326.xyz

JS:   crypto.randomUUID()
来源：http://ozy.ybcxt.top

TS:   crypto.randomUUID()
来源：http://ehb.aizwys.cn

Java: UUID.randomUUID().toString()
来源：http://pxk.jqgufenzy.top

Go:   // 用 github.com/google/uuid
来源：http://fso.hnqzz.top

Ruby: SecureRandom.uuid
来源：http://yrd.hysaishi.cn

C#:   Guid.NewGuid().ToString()
来源：http://kyq.yanxiufei.cn

[P02] MD5 / SHA256 摘要
来源：http://xdp.yueranfly.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ubq.smart0.xyz

PHP:  hash("sha256", $s);  md5($s);
来源：http://eif.yuanzhike.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://irf.svipenyu.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ylu.cucudq.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hds.jlsjyb.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wvh.xinyue.icu

Ruby: Digest::SHA256.hexdigest(s)
来源：http://bow.0kj1m.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://khz.jinghuilouyu.cn

[P03] 生成短随机字符串
来源：http://gpw.chenjidiqi.icu

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hje.zhixingplan.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://qtk.nwbrower.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://oqi.xuanzx.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://itg.cheryme.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://pml.feifeiyinyue.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://whv.ydzc1.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://jzf.meibo888.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ixl.yanxiufei.cn

[P04] 求长度
来源：http://enx.pycfn.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://kzv.9152youxi.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vnd.zhongyouzk.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mvy.ctjpmb.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ojy.xinyue.icu

Java: list.size();  map.size();  s.length()
来源：http://lwm.epnwcf.com

Go:   len(arr);  len(m)
来源：http://ozu.snrcjt.cn

Ruby: x.length;  x.size
来源：http://mkj.ydzc1.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://zmi.gotoacloud.top

[P05] 判断两个对象内容是否相等
来源：http://ukl.yuanzhike.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://izc.hywenlv.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://fts.tianlin.xyz

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://nua.jinqigfzy.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://qvs.chenzaomai.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://xbr.havefunace.top

Go:   reflect.DeepEqual(a, b)
来源：http://hvo.jianghu66.top

Ruby: a == b
来源：http://pmh.ywan-chungtsiang.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ffa.uphjek.com

[P06] 综合判空（null / 空串 / 空集合）
来源：http://tdc.fzhhl.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ubd.9152youxi.cn

PHP:  if (empty($x)) {}
来源：http://rgl.cqqwz.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ivu.yj202588.top

TS:   if (x == null) {}
来源：http://rjn.xinyue.icu

Java: if (x == null || x.isEmpty()) {}
来源：http://uym.snrcjt.cn

Go:   if x == nil {}
来源：http://qih.chenzaomai.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wrb.quarkkingdee.top

C#:   if (x is null) {}
来源：http://iqg.sufxvd.cn

[P07] 防抖与节流
来源：http://urp.c1oappe.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hps.daxiang520.top

PHP:  // 手写时间戳比较
来源：http://eby.redwolf501.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lqi.zhiwuduotai.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rry.nanxinkj.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://bkt.haohaochexian.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ada.jqgfzy.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://ilx.xuetiantiany.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://keh.wangshuangyany.cn

[P08] 处理浮点精度问题
来源：http://mxe.ppjwa.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://cek.wangdashe.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://vrc.yuxming.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://sfd.yvedp.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hjx.hywenlv.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://quw.jqgfzy.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://lnk.zdqjudy.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ppo.sufxvd.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://omw.xuetiantiany.cn

================================================================================
来源：http://myu.nanxinkj.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://rmn.yfazqb.com

================================================================================
来源：http://srs.tian-w.cn

[Q01] 创建表
来源：http://icn.xziqi.cn

CREATE TABLE users (
来源：http://liq.svipenyu.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://jdz.redwolf501.top

name VARCHAR(50) NOT NULL,
来源：http://lhe.epnwcf.com

email VARCHAR(100) UNIQUE,
来源：http://nae.sjlbkw.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://kkv.zhaomingkeji.xyz

);
来源：http://fzv.birdmap.top

[Q02] 创建带外键的表
来源：http://iyg.316326.xyz

CREATE TABLE orders (
来源：http://blb.gzhubu.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://odg.haohaochexian.top

user_id INT NOT NULL,
来源：http://axu.dianchejie.cn

amount DECIMAL(10, 2),
来源：http://vlc.yvedp.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://dji.zhiwuduotai.top

);
来源：http://ddh.zhongyouzk.top

[Q03] 增加列
来源：http://agv.gogol.net.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://tsg.snrcjt.cn

[Q04] 修改列类型
来源：http://hga.aizwys.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wlw.aibaodan.cn

[Q05] 重命名列
来源：http://imt.ydjk.org.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://rjr.dianchejie.cn

[Q06] 删除列
来源：http://tgc.zhiwuduotai.top

ALTER TABLE users DROP COLUMN age;
来源：http://iyp.jianghu66.top

[Q07] 删除表
来源：http://ehg.mhx1999.top

DROP TABLE IF EXISTS orders;
来源：http://vfl.yonumen.top

[Q08] 创建普通索引
来源：http://vlb.yj20258888.top

CREATE INDEX idx_users_email ON users(email);
来源：http://xbb.tianlin.xyz

[Q09] 创建唯一索引
来源：http://zmd.ydjk.org.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://shp.guannengcc.top

[Q10] 插入单行
来源：http://vmy.ehwqpu.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hxs.fengsongda.top

[Q11] 一次插入多行
来源：http://htq.xinyue.icu

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://pzq.nanxuanxn.top

[Q12] 插入后取自增 ID
来源：http://opy.fktsv.cn

INSERT INTO users (name) VALUES ('C');
来源：http://bub.cdnleiting.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://qng.ehwqpu.com

[Q13] 忽略重复插入
来源：http://tqd.jiagoushi.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://yxw.cucudq.cn

[Q14] 存在则更新（upsert）
来源：http://mpq.yonumen.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://krb.sweek.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://xpe.jqgufenzy.top

[Q15] 查询全部
来源：http://uzp.fanxiaobao.xyz

SELECT * FROM users;
来源：http://gaw.tarul.cn

[Q16] 查询指定列
来源：http://ray.shuidangran.top

SELECT id, name FROM users;
来源：http://dnp.hfpthk.cn

[Q17] 条件查询
来源：http://zga.zhengqikj.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://bft.fanxiaobao.xyz

[Q18] 模糊匹配
来源：http://ygn.hysaishi.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://nno.yuanzhike.top

[Q19] 范围查询
来源：http://mml.ctjpmb.com

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ecv.zhoulong.xyz

[Q20] IN 列表
来源：http://ytj.birdmap.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ksw.yueranfly.top

[Q21] 空值判断
来源：http://xno.sysykeji.top

SELECT * FROM users WHERE email IS NULL;
来源：http://nsm.uphjek.com

[Q22] 排序
来源：http://cdh.jlsjyb.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mfs.guowangkeji.top

[Q23] 分页
来源：http://erk.birdmap.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://fjo.nanxinkj.top

[Q24] 去重
来源：http://onr.hnxiangtu.top

SELECT DISTINCT city FROM users;
来源：http://xub.guannengcc.top

[Q25] 只取前 N 条
来源：http://thx.ppjwa.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://vhq.tarul.cn

[Q26] 计数
来源：http://rpq.chenzaomai.com

SELECT COUNT(*) FROM users;
来源：http://deh.hywenlv.cn

[Q27] 条件计数
来源：http://zkh.epnwcf.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://lcs.hongshengwenyu.top

[Q28] 求和与平均
来源：http://hyf.yfazqb.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://jgi.xuanzx.com

[Q29] 最大最小值
来源：http://lpu.ydjk.org.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://afu.havefunace.top

[Q30] 分组统计
来源：http://gvo.hysaishi.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hzg.shanyushiyangkeji.top

[Q31] 分组后过滤
来源：http://bxn.feifeiyinyue.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://xru.yuanzhike.top

[Q32] 分组拼接字符串
来源：http://sqb.ctjpmb.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://drx.uphjek.com

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://gry.hnxiangtu.top


<!-- 参考信息 -->