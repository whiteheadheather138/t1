代发 wailian999

PHP:  // 递归实现，或用 usort
来源：http://yzw.zycfv.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tgv.ywan-chungtsiang.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jzl.snrcjt.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://xxb.dianchejie.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://xti.ivvv.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://gvc.zhixingplan.top

C#:   // 手写递归，或 Array.Sort
来源：http://pva.pengpengdd.cyou

[N04] 斐波那契数列
来源：http://yhm.iojbl.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://vts.yanxiufei.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://uqu.gotoacloud.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rhy.hcnkem.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://uuf.nanxuanxn.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ztu.yj202588.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://vtu.tianlin.xyz

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://qyp.chenzaomai.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ngi.svipenyu.cn

[N05] 最大公约数
来源：http://vev.sweek.top

Py:   math.gcd(a, b)
来源：http://esm.ydjk.org.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ekt.vqdsnc.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ndf.jqgufenzy.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mjy.sysykeji.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://uah.hongshengwenyu.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://pvh.gzhubu.top

Ruby: a.gcd(b)
来源：http://aos.smart0.xyz

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://oyw.zhixingplan.top

[N06] 判断回文字符串
来源：http://ydg.hnxiangtu.top

Py:   s == s[::-1]
来源：http://yny.vqdsnc.cn

PHP:  $s === strrev($s);
来源：http://ril.zhengqikj.top

JS:   s === [...s].reverse().join("")
来源：http://qhn.birdmap.top

TS:   s === [...s].reverse().join("")
来源：http://qwv.redwolf501.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://fao.dashuyun.cn

Go:   // 双指针从两端比较
来源：http://pfg.yongpay.top

Ruby: s == s.reverse
来源：http://rhc.fzhhl.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://jmu.yvedp.cn

[N07] 两数之和（返回下标）
来源：http://nnh.ehwqpu.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://moy.sjlbkw.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://eay.zhongyouzk.top

JS:   // 手写 Map：map.set(v, i)
来源：http://yij.xylfe.cn

TS:   // 手写 Map<string, number>
来源：http://hdk.zdbjq.cn

Java: // 手写 HashMap
来源：http://kxj.shangyingyoupin.top

Go:   // 手写 map[int]int
来源：http://lcv.nwbrower.top

Ruby: // 手写 Hash
来源：http://zmq.xuanzx.com

C#:   // 手写 Dictionary<int, int>
来源：http://tch.chenjidiqi.icu

[N08] 生成全排列
来源：http://ocb.mhx1999.top

Py:   itertools.permutations(arr)
来源：http://jhl.zhijiandao.cn

PHP:  // 手写递归交换
来源：http://wse.c1oappe.top

JS:   // 手写回溯递归
来源：http://wyp.shuidangran.top

TS:   // 手写回溯递归
来源：http://jqr.uphjek.com

Java: // 手写回溯递归
来源：http://icz.shuidangran.top

Go:   // 手写回溯递归
来源：http://gea.sufxvd.cn

Ruby: arr.permutation.to_a
来源：http://vhx.nwbrower.top

C#:   // 手写回溯递归
来源：http://tfd.bjfxy.top

[N09] 栈与队列
来源：http://kes.fzhhl.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wyr.hesvh.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://lzx.guannengcc.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://bgz.zdbjq.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mqk.sufxvd.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://cbl.tarul.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://xxa.daria6918.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://dsu.shanyushiyangkeji.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wyj.xuetiantiany.cn

[N10] 链表节点定义
来源：http://shb.hfpthk.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://zqu.zdbjq.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ptc.shzxlz.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://xgb.tanke756.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://pnr.xuanzx.com

Java: class Node { int v; Node next; }
来源：http://gkx.hfpthk.cn

Go:   type Node struct { V int; Next *Node }
来源：http://fjb.zdqjudy.top

Ruby: Node = Struct.new(:v, :next)
来源：http://dur.epnwcf.com

C#:   class Node { public int V; public Node? Next; }
来源：http://qty.jyoumei.cn

[N11] 二叉树中序遍历
来源：http://jnx.zhijiandao.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://qmi.hcnkem.com

PHP:  // 手写递归函数
来源：http://fus.zdbjq.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jwo.hywenlv.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mpq.hammf.cn

Java: // 手写递归
来源：http://glm.zycfv.cn

Go:   // 手写递归
来源：http://drk.zhijiandao.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://eon.zhixingplan.top

C#:   // 手写递归
来源：http://mae.shanyushiyangkeji.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://fdu.jinghuilouyu.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://kdw.xinyue.icu

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ebd.mhx1999.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jcv.jqgfzy.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yzi.wangdashe.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://shp.ppjwa.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://qze.nanxuanxn.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://knk.zycfv.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://uct.dashuyun.cn

================================================================================
来源：http://tkc.ctjpmb.com

O. 并发与异步
来源：http://ivi.jyoumei.cn

================================================================================
来源：http://zlq.nwbrower.top

[O01] 启动一个线程
来源：http://zei.sxryk.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://tek.jiagoushi.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://cep.pengpengdd.cyou

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://uhl.9152youxi.cn

TS:   // 同 JS
来源：http://msl.havefunace.top

Java: new Thread(() -> f()).start()
来源：http://vmz.zycfv.cn

Go:   go f()
来源：http://aob.hfpthk.cn

Ruby: Thread.new { f }
来源：http://nkq.shanyushiyangkeji.top

C#:   Task.Run(() => F());
来源：http://npa.bbcook.cn

[O02] 使用线程池
来源：http://sis.gotoacloud.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://huo.bjfxy.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://gwf.shanyushiyangtech.top

JS:   // worker_threads 线程池
来源：http://qyk.jqgfzy.top

TS:   // worker_threads 线程池
来源：http://taa.zhengqikj.top

Java: Executors.newFixedThreadPool(4)
来源：http://gly.aibaodan.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://twe.epnwcf.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ret.iojbl.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mum.cheryme.top

[O03] 加锁保护共享数据
来源：http://gqw.fktsv.cn

Py:   with lock: shared += 1
来源：http://onj.dashuyun.cn

PHP:  // 用 flock() 做文件锁
来源：http://wqi.jlsjyb.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://sxa.xylfe.cn

TS:   // 同 JS
来源：http://jvm.cashguo.top

Java: synchronized (this) { shared++; }
来源：http://ffj.wangdashe.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://lry.bbcook.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://spk.vqdsnc.cn

C#:   lock (gate) { shared++; }
来源：http://akf.xingfuxueyuan.xyz

[O04] 定义异步函数并等待
来源：http://nhl.yuxming.cn

Py:   async def f():⏎    await g()
来源：http://cir.ppjwa.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://rjd.yueranfly.top

JS:   async function f() { await g(); }
来源：http://yac.andypj.xyz

TS:   async function f(): Promise<void> { await g(); }
来源：http://xga.hnqzz.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://okr.tanke756.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://qmk.smart0.xyz

Ruby: # 用 Fiber 或 async gem
来源：http://nnu.yongpay.top

C#:   async Task F() { await G(); }
来源：http://frx.cdnleiting.top

[O05] 并发执行并等待全部完成
来源：http://tij.xuanzx.com

Py:   asyncio.gather(*tasks)
来源：http://cfv.zycfv.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://nlu.sufxvd.cn

JS:   await Promise.all(tasks)
来源：http://nwd.jianghu66.top

TS:   await Promise.all(tasks)
来源：http://ftz.feifeiyinyue.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://pgb.yj20258.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://daz.epnwcf.com

Ruby: threads.map(&:join)
来源：http://uct.zycfv.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://hym.quarkkingdee.top

[O06] 使用进程池
来源：http://pzs.svipenyu.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://pix.sysykeji.top

PHP:  // pcntl_fork 或多进程队列
来源：http://rxt.zycfv.cn

JS:   // child_process / cluster 模块
来源：http://bad.yj202588.top

TS:   // child_process / cluster 模块
来源：http://hbd.xingfuxueyuan.xyz

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://uho.xinyue.icu

Go:   // goroutine 已占用多核，直接并发即可
来源：http://uas.ywan-chungtsiang.top

Ruby: // fork 块
来源：http://xwp.cashguo.top

C#:   Parallel.For
来源：http://xwp.tanke756.top

================================================================================
来源：http://hpg.jlsjyb.cn

P. 常用工具函数
来源：http://asi.sjlbkw.cn

================================================================================
来源：http://uji.sxryk.cn

[P01] 生成 UUID
来源：http://cbk.epnwcf.com

Py:   str(uuid.uuid4())
来源：http://bbs.hongshengwenyu.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://vus.ehwqpu.com

JS:   crypto.randomUUID()
来源：http://fzj.zhengqikj.top

TS:   crypto.randomUUID()
来源：http://yiu.sxryk.cn

Java: UUID.randomUUID().toString()
来源：http://vqv.zhengqikj.top

Go:   // 用 github.com/google/uuid
来源：http://ulp.xinyue.icu

Ruby: SecureRandom.uuid
来源：http://nxe.dashuyun.cn

C#:   Guid.NewGuid().ToString()
来源：http://zhl.zhiwuduotai.top

[P02] MD5 / SHA256 摘要
来源：http://xax.yangfankeji.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://zca.shzxlz.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ezb.hnxiangtu.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://npb.jinqigufen.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wtn.hysaishi.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://pio.xylfe.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://pjs.chenjidiqi.icu

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hfj.redwolf501.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wio.316326.xyz

[P03] 生成短随机字符串
来源：http://mhz.xinyue.icu

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://cto.zhijiandao.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://vsr.xuanzx.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xjg.jinqigufen.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mfc.hesvh.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://oqz.316326.xyz

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://dje.zhengqikj.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://kyv.nwbrower.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://uff.cdnleiting.top

[P04] 求长度
来源：http://beg.daria6918.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hur.zhaomingkeji.xyz

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://shb.yj20258888.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qzc.fehbvm.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bmd.c1oappe.top

Java: list.size();  map.size();  s.length()
来源：http://bnk.svipenyu.cn

Go:   len(arr);  len(m)
来源：http://xtt.yj20258888.top

Ruby: x.length;  x.size
来源：http://whd.cheryme.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://ces.yj20258.top

[P05] 判断两个对象内容是否相等
来源：http://rwa.redwolf501.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://yfa.c1oappe.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hni.0kj1m.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ims.hammf.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://erv.hammf.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://rpn.zhixingplan.top

Go:   reflect.DeepEqual(a, b)
来源：http://yjt.daria6918.cn

Ruby: a == b
来源：http://rzc.birdmap.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://tee.jinqigfzy.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://smp.feifeiyinyue.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ffg.jinqigfzy.top

PHP:  if (empty($x)) {}
来源：http://hsv.zycfv.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://rbv.yongpay.top

TS:   if (x == null) {}
来源：http://juq.cashguo.top

Java: if (x == null || x.isEmpty()) {}
来源：http://arm.hesvh.cn

Go:   if x == nil {}
来源：http://qyx.quarkkingdee.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wjq.yongpay.top

C#:   if (x is null) {}
来源：http://kfx.ydzc1.top

[P07] 防抖与节流
来源：http://ilk.shanyushiyangkeji.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://cko.cashguo.top

PHP:  // 手写时间戳比较
来源：http://vrw.sufxvd.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rgy.dashuyun.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wsw.epnwcf.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://kug.shanyushiyangtech.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ycn.uphjek.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://eii.ehwqpu.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ghe.snrcjt.cn

[P08] 处理浮点精度问题
来源：http://lwl.yangfankeji.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://olf.cdnleiting.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ogw.52xcode.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://cbm.tarul.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://xzz.chenjidiqi.icu

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://kaw.quarkkingdee.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wmi.tarul.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://exr.jqgufenzy.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://xvl.quarkkingdee.top

================================================================================
来源：http://fkc.chenlongwang.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://bjy.fzhhl.top

================================================================================
来源：http://yxp.gaohongyu789.top

[Q01] 创建表
来源：http://ifl.hongshengwenyu.top

CREATE TABLE users (
来源：http://yha.snrcjt.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://xfu.bjfxy.top

name VARCHAR(50) NOT NULL,
来源：http://rqp.zdbjq.cn

email VARCHAR(100) UNIQUE,
来源：http://wga.sxryk.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://lpe.snrcjt.cn

);
来源：http://goe.birdmap.top

[Q02] 创建带外键的表
来源：http://xkv.zycfv.cn

CREATE TABLE orders (
来源：http://xqx.gaohongyu789.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://yel.zhijiandao.cn

user_id INT NOT NULL,
来源：http://uhg.epnwcf.com

amount DECIMAL(10, 2),
来源：http://ozp.shanyushiyangkeji.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wgz.jianghu66.top

);
来源：http://dzk.dashuyun.cn

[Q03] 增加列
来源：http://vgd.0kj1m.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://gby.fengsongda.top

[Q04] 修改列类型
来源：http://fzz.smart0.xyz

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://exa.jqgfzy.top

[Q05] 重命名列
来源：http://kbg.jinyuanbaomall.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mtz.ehwqpu.com

[Q06] 删除列
来源：http://ffm.yj202588.top

ALTER TABLE users DROP COLUMN age;
来源：http://zci.havefunace.top

[Q07] 删除表
来源：http://rwk.zycfv.cn

DROP TABLE IF EXISTS orders;
来源：http://uzs.fengsongda.top

[Q08] 创建普通索引
来源：http://qod.0kj1m.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://oyr.guannengcc.top

[Q09] 创建唯一索引
来源：http://kzl.smart0.xyz

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://zpe.ctjpmb.com

[Q10] 插入单行
来源：http://tkh.shangyingyoupin.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://bnz.yj20258.top

[Q11] 一次插入多行
来源：http://kep.xuetiantiany.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://gwz.9152youxi.cn

[Q12] 插入后取自增 ID
来源：http://yed.meibo888.top

INSERT INTO users (name) VALUES ('C');
来源：http://qcw.zhixingplan.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://que.hnqzz.top

[Q13] 忽略重复插入
来源：http://wqm.gaohongyu789.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://qys.nanxuanxn.top

[Q14] 存在则更新（upsert）
来源：http://kds.sxryk.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://rfh.zdqjudy.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://zpq.fktsv.cn

[Q15] 查询全部
来源：http://dks.quarkkingdee.top

SELECT * FROM users;
来源：http://mwm.zhiwuduotai.top

[Q16] 查询指定列
来源：http://tyq.xinyue.icu

SELECT id, name FROM users;
来源：http://qye.sweek.top

[Q17] 条件查询
来源：http://ksm.kuanghao11.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://bgn.dianchejie.cn

[Q18] 模糊匹配
来源：http://sjl.fehbvm.com

SELECT * FROM users WHERE name LIKE '张%';
来源：http://rti.zhiwuduotai.top

[Q19] 范围查询
来源：http://lbu.sysykeji.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://lex.zhaomingkeji.xyz

[Q20] IN 列表
来源：http://eds.jyoumei.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://fus.vehdjk.com

[Q21] 空值判断
来源：http://nir.jyoumei.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://zmm.yj202588.top

[Q22] 排序
来源：http://cvo.fehbvm.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://guv.shzxlz.cn

[Q23] 分页
来源：http://nke.zdbjq.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://gsw.zdbjq.cn

[Q24] 去重
来源：http://bxj.hysaishi.cn

SELECT DISTINCT city FROM users;
来源：http://jdz.yangfankeji.com

[Q25] 只取前 N 条
来源：http://ziq.jyoumei.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://nbi.sysykeji.top

[Q26] 计数
来源：http://igm.zhiwuduotai.top

SELECT COUNT(*) FROM users;
来源：http://zav.ppjwa.cn

[Q27] 条件计数
来源：http://vwl.meibo888.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://vev.nanxuanxn.top

[Q28] 求和与平均
来源：http://emm.cheryme.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://jrr.zdqjudy.top

[Q29] 最大最小值
来源：http://lib.bjfxy.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://fdf.guannengcc.top

[Q30] 分组统计
来源：http://tpe.mhx1999.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://rgl.zhixingplan.top

[Q31] 分组后过滤
来源：http://ysu.xuetiantiany.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://kho.jqgufenzy.top

[Q32] 分组拼接字符串
来源：http://ime.zdqjudy.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://fqv.zhongyouzk.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ttf.gogol.net.cn


<!-- 参考信息 -->