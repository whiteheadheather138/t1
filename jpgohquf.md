代发 wailian999

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://nwn.hcnkem.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mbk.jinyuanbaomall.cn

C#:   // 手写递归，或 Array.Sort
来源：http://jst.zhijiandao.cn

[N04] 斐波那契数列
来源：http://szv.vqdsnc.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://jhd.sjlbkw.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wxn.sxryk.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://aca.yanxiufei.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hkx.fktsv.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://jdm.fzhhl.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ino.haohaochexian.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://rcx.yuanzhike.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wij.vqdsnc.cn

[N05] 最大公约数
来源：http://tcq.shzxlz.cn

Py:   math.gcd(a, b)
来源：http://fcp.c1oappe.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://lmn.gzhubu.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ftf.birdmap.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vpy.aizwys.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://dno.jianghu66.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://nmk.xingfuxueyuan.xyz

Ruby: a.gcd(b)
来源：http://psh.chenlongwang.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mkn.haohaochexian.top

[N06] 判断回文字符串
来源：http://lex.yfazqb.com

Py:   s == s[::-1]
来源：http://pye.xuanzx.com

PHP:  $s === strrev($s);
来源：http://yvq.shzxlz.cn

JS:   s === [...s].reverse().join("")
来源：http://dcn.yuxming.cn

TS:   s === [...s].reverse().join("")
来源：http://pzq.ivvv.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ibc.c1oappe.top

Go:   // 双指针从两端比较
来源：http://otf.tian-w.cn

Ruby: s == s.reverse
来源：http://vlf.jyoumei.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://jec.guannengcc.top

[N07] 两数之和（返回下标）
来源：http://rif.zhiwuduotai.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://kvv.cdnleiting.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mwu.uphjek.com

JS:   // 手写 Map：map.set(v, i)
来源：http://eia.svipenyu.cn

TS:   // 手写 Map<string, number>
来源：http://vsb.xinyue.icu

Java: // 手写 HashMap
来源：http://fkp.jqgufenzy.top

Go:   // 手写 map[int]int
来源：http://swk.daria6918.cn

Ruby: // 手写 Hash
来源：http://amd.sxryk.cn

C#:   // 手写 Dictionary<int, int>
来源：http://yoa.yuanzhike.top

[N08] 生成全排列
来源：http://fvk.vehdjk.com

Py:   itertools.permutations(arr)
来源：http://kdi.hnxiangtu.top

PHP:  // 手写递归交换
来源：http://gci.birdmap.top

JS:   // 手写回溯递归
来源：http://tha.birdmap.top

TS:   // 手写回溯递归
来源：http://iut.ywan-chungtsiang.top

Java: // 手写回溯递归
来源：http://tjd.yongpay.top

Go:   // 手写回溯递归
来源：http://soz.zhongyouzk.top

Ruby: arr.permutation.to_a
来源：http://kho.jianghu66.top

C#:   // 手写回溯递归
来源：http://tpc.jqgufenzy.top

[N09] 栈与队列
来源：http://ojn.fzhhl.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://pnm.hnqzz.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ljr.chenjidiqi.icu

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://rtu.yonumen.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://euw.cheryme.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://vyi.ydjk.org.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://fvm.gzhubu.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://occ.guowangkeji.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://iii.snrcjt.cn

[N10] 链表节点定义
来源：http://ugj.tarul.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://fsy.birdmap.top

PHP:  class Node { public $v; public $next = null; }
来源：http://gph.feifeiyinyue.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ozz.feifeiyinyue.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://gdt.hnxiangtu.top

Java: class Node { int v; Node next; }
来源：http://ape.sysykeji.top

Go:   type Node struct { V int; Next *Node }
来源：http://szh.smart0.xyz

Ruby: Node = Struct.new(:v, :next)
来源：http://ybh.fanxiaobao.xyz

C#:   class Node { public int V; public Node? Next; }
来源：http://vlk.ppjwa.cn

[N11] 二叉树中序遍历
来源：http://eop.yanxiufei.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://lpr.jinqigfzy.top

PHP:  // 手写递归函数
来源：http://efw.yueranfly.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qxh.zhoulong.xyz

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fnn.jqgufenzy.top

Java: // 手写递归
来源：http://ska.shuidangran.top

Go:   // 手写递归
来源：http://ntr.dashuyun.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ygr.andypj.xyz

C#:   // 手写递归
来源：http://xvz.bjfxy.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://xgu.jyoumei.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ccb.yangfankeji.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://cru.yj20258888.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ttu.tarul.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qpb.snrcjt.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://kvt.shangyingyoupin.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://vte.52xcode.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://kyt.ivvv.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://sva.feifeiyinyue.top

================================================================================
来源：http://xiq.dianchejie.cn

O. 并发与异步
来源：http://yfq.pycfn.com

================================================================================
来源：http://lkn.zdqjudy.top

[O01] 启动一个线程
来源：http://kun.bjfxy.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://sns.vehdjk.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://lya.yj20258888.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://jqn.zhoulong.xyz

TS:   // 同 JS
来源：http://afb.jyoumei.cn

Java: new Thread(() -> f()).start()
来源：http://kfi.bbcook.cn

Go:   go f()
来源：http://ino.xuanzx.com

Ruby: Thread.new { f }
来源：http://mkm.jyoumei.cn

C#:   Task.Run(() => F());
来源：http://txv.jinyuanbaomall.cn

[O02] 使用线程池
来源：http://anu.tian-w.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://drw.hywenlv.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://lwd.zhiwuduotai.top

JS:   // worker_threads 线程池
来源：http://ohi.hesvh.cn

TS:   // worker_threads 线程池
来源：http://rce.yj20258.top

Java: Executors.newFixedThreadPool(4)
来源：http://izb.0kj1m.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://vwr.fanxiaobao.xyz

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://gzn.hfpthk.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://cla.bbcook.cn

[O03] 加锁保护共享数据
来源：http://ziy.9152youxi.cn

Py:   with lock: shared += 1
来源：http://nmm.yueranfly.top

PHP:  // 用 flock() 做文件锁
来源：http://aen.tarul.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://plt.chenjidiqi.icu

TS:   // 同 JS
来源：http://smu.52xcode.cn

Java: synchronized (this) { shared++; }
来源：http://xoz.ivvv.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://xsd.epnwcf.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://wrx.hcnkem.com

C#:   lock (gate) { shared++; }
来源：http://vhy.smart0.xyz

[O04] 定义异步函数并等待
来源：http://fym.zhijiandao.cn

Py:   async def f():⏎    await g()
来源：http://ovs.jinghuilouyu.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://pwh.fehbvm.com

JS:   async function f() { await g(); }
来源：http://wqo.fehbvm.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://cuf.tanke756.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://bzv.yueranfly.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://bnq.aibaodan.cn

Ruby: # 用 Fiber 或 async gem
来源：http://fse.gzhubu.top

C#:   async Task F() { await G(); }
来源：http://rbs.316326.xyz

[O05] 并发执行并等待全部完成
来源：http://jux.pengpengdd.cyou

Py:   asyncio.gather(*tasks)
来源：http://hxw.tarul.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://fay.nwbrower.top

JS:   await Promise.all(tasks)
来源：http://jjc.jiagoushi.top

TS:   await Promise.all(tasks)
来源：http://ahg.chenjidiqi.icu

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://thn.guannengcc.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://znn.zhongyouzk.top

Ruby: threads.map(&:join)
来源：http://vbl.cucudq.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://zkl.fzhhl.top

[O06] 使用进程池
来源：http://llp.tanke756.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hjl.jlsjyb.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ayk.hesvh.cn

JS:   // child_process / cluster 模块
来源：http://rdi.316326.xyz

TS:   // child_process / cluster 模块
来源：http://nkd.dianchejie.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://rkr.fanxiaobao.xyz

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mul.ybcxt.top

Ruby: // fork 块
来源：http://qll.ywan-chungtsiang.top

C#:   Parallel.For
来源：http://bnm.hnxiangtu.top

================================================================================
来源：http://zkt.nwbrower.top

P. 常用工具函数
来源：http://sbu.aizwys.cn

================================================================================
来源：http://cdx.ehwqpu.com

[P01] 生成 UUID
来源：http://ayu.gzhubu.top

Py:   str(uuid.uuid4())
来源：http://hcl.wangshuangyany.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://glc.jiagoushi.top

JS:   crypto.randomUUID()
来源：http://zcq.ydjk.org.cn

TS:   crypto.randomUUID()
来源：http://iey.ydzc1.top

Java: UUID.randomUUID().toString()
来源：http://xan.jyoumei.cn

Go:   // 用 github.com/google/uuid
来源：http://zos.hysaishi.cn

Ruby: SecureRandom.uuid
来源：http://zch.yj202588.top

C#:   Guid.NewGuid().ToString()
来源：http://rtf.redwolf501.top

[P02] MD5 / SHA256 摘要
来源：http://vuu.hammf.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://xbv.sweek.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://qjx.cheryme.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://xiq.gaohongyu789.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://otk.ybcxt.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://zab.fktsv.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://fpk.zhaomingkeji.xyz

Ruby: Digest::SHA256.hexdigest(s)
来源：http://rpd.zdbjq.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://qhg.pengpengdd.cyou

[P03] 生成短随机字符串
来源：http://noh.tian-w.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://erz.tian-w.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://vjv.daria6918.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://awn.hesvh.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://cbm.wangshuangyany.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://pyg.andypj.xyz

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://nrg.feifeiyinyue.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://zbu.nanxinkj.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ioj.yj20258.top

[P04] 求长度
来源：http://fsx.cheryme.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://nfz.yj202588.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ego.tian-w.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://txj.wangshuangyany.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rnz.chenjidiqi.icu

Java: list.size();  map.size();  s.length()
来源：http://rtw.jqgufenzy.top

Go:   len(arr);  len(m)
来源：http://nbg.nanxuanxn.top

Ruby: x.length;  x.size
来源：http://iua.yuxming.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://awe.yfazqb.com

[P05] 判断两个对象内容是否相等
来源：http://vks.shzxlz.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://feu.nanxinkj.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://lhi.hnqzz.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wkm.guowangkeji.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://kgk.nwbrower.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hks.52xcode.cn

Go:   reflect.DeepEqual(a, b)
来源：http://sgm.jlsjyb.cn

Ruby: a == b
来源：http://ght.gzhubu.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://kzt.sysykeji.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://plu.daria6918.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://bqe.jinghuilouyu.cn

PHP:  if (empty($x)) {}
来源：http://wfo.tianlin.xyz

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hrv.yueranfly.top

TS:   if (x == null) {}
来源：http://fed.jiagoushi.top

Java: if (x == null || x.isEmpty()) {}
来源：http://kez.jqgufenzy.top

Go:   if x == nil {}
来源：http://ydg.316326.xyz

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://gqa.shangyingyoupin.top

C#:   if (x is null) {}
来源：http://lkw.kuanghao11.cn

[P07] 防抖与节流
来源：http://jsd.quarkkingdee.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://gfu.cucudq.cn

PHP:  // 手写时间戳比较
来源：http://vsy.hnqzz.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://syq.feifeiyinyue.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jce.hysaishi.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://gwx.yuxming.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://xrp.epnwcf.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://izs.xingfuxueyuan.xyz

C#:   // 用 System.Timers.Timer 重置实现
来源：http://skc.fengsongda.top

[P08] 处理浮点精度问题
来源：http://hyg.xinyue.icu

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://sjw.cdnleiting.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://xzb.zhixingplan.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://adt.bbcook.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://qnf.bbcook.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://qmo.feifeiyinyue.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://eoo.ywan-chungtsiang.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://yts.wangdashe.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://gup.aizwys.cn

================================================================================
来源：http://tzn.feifeiyinyue.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://yvv.chenjidiqi.icu

================================================================================
来源：http://ndw.c1oappe.top

[Q01] 创建表
来源：http://vyu.xinyue.icu

CREATE TABLE users (
来源：http://qqa.shangyingyoupin.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wri.ywan-chungtsiang.top

name VARCHAR(50) NOT NULL,
来源：http://ozf.aizwys.cn

email VARCHAR(100) UNIQUE,
来源：http://vus.yangfankeji.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://rmu.wangdashe.top

);
来源：http://kig.yuanzhike.top

[Q02] 创建带外键的表
来源：http://hik.meibo888.top

CREATE TABLE orders (
来源：http://mbw.zhengqikj.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://yvg.guowangkeji.top

user_id INT NOT NULL,
来源：http://dhp.52xcode.cn

amount DECIMAL(10, 2),
来源：http://xlv.cqqwz.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://fva.yangfankeji.com

);
来源：http://onn.hfpthk.cn

[Q03] 增加列
来源：http://itx.nanxuanxn.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://qca.pycfn.com

[Q04] 修改列类型
来源：http://auv.hnqzz.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://oac.jinyuanbaomall.cn

[Q05] 重命名列
来源：http://hoi.xingfuxueyuan.xyz

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://dnv.haohaochexian.top

[Q06] 删除列
来源：http://rja.ybcxt.top

ALTER TABLE users DROP COLUMN age;
来源：http://ybk.sjlbkw.cn

[Q07] 删除表
来源：http://fff.ehwqpu.com

DROP TABLE IF EXISTS orders;
来源：http://hbg.ppjwa.cn

[Q08] 创建普通索引
来源：http://mtu.birdmap.top

CREATE INDEX idx_users_email ON users(email);
来源：http://lrc.shuidangran.top

[Q09] 创建唯一索引
来源：http://blj.jinqigfzy.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mmv.zhijiandao.cn

[Q10] 插入单行
来源：http://iym.iojbl.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://isy.zdqjudy.top

[Q11] 一次插入多行
来源：http://qdf.ppjwa.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://csg.fehbvm.com

[Q12] 插入后取自增 ID
来源：http://tdh.bbcook.cn

INSERT INTO users (name) VALUES ('C');
来源：http://fnj.xziqi.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://qqd.redwolf501.top

[Q13] 忽略重复插入
来源：http://jff.jqgufenzy.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://nnh.cucudq.cn

[Q14] 存在则更新（upsert）
来源：http://czq.zhiwuduotai.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mcm.zycfv.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://gtx.cucudq.cn

[Q15] 查询全部
来源：http://rqi.gaohongyu789.top

SELECT * FROM users;
来源：http://vvu.dianchejie.cn

[Q16] 查询指定列
来源：http://bvf.zhixingplan.top

SELECT id, name FROM users;
来源：http://glo.xingfuxueyuan.xyz

[Q17] 条件查询
来源：http://nga.yueranfly.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://apd.zycfv.cn

[Q18] 模糊匹配
来源：http://xzg.wangdashe.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://nqb.haohaochexian.top

[Q19] 范围查询
来源：http://mxb.jianghu66.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://bsr.yj20258.top

[Q20] IN 列表
来源：http://fey.tian-w.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://uie.ybcxt.top

[Q21] 空值判断
来源：http://ghu.guannengcc.top

SELECT * FROM users WHERE email IS NULL;
来源：http://bor.hcnkem.com

[Q22] 排序
来源：http://gry.daxiang520.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://uip.shanyushiyangkeji.top

[Q23] 分页
来源：http://mmi.birdmap.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://btp.jinghuilouyu.cn

[Q24] 去重
来源：http://ohf.wangdashe.top

SELECT DISTINCT city FROM users;
来源：http://swc.yvedp.cn

[Q25] 只取前 N 条
来源：http://jui.jinqigfzy.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ydv.yfazqb.com

[Q26] 计数
来源：http://fxz.chenlongwang.top

SELECT COUNT(*) FROM users;
来源：http://yeo.redwolf501.top

[Q27] 条件计数
来源：http://rfu.xinyue.icu

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hwq.0kj1m.cn

[Q28] 求和与平均
来源：http://xmf.zhengqikj.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://otg.yj20258.top

[Q29] 最大最小值
来源：http://zoe.xziqi.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://xgg.gaohongyu789.top

[Q30] 分组统计
来源：http://rnq.yuxming.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://saf.jianghu66.top

[Q31] 分组后过滤
来源：http://wgy.fktsv.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://yll.yonumen.top

[Q32] 分组拼接字符串
来源：http://iap.xuanzx.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://dyv.ehwqpu.com

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://bce.gotoacloud.top

[Q33] 多列分组
来源：http://rds.yongpay.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://toa.zycfv.cn

[Q34] 每组取第一条
来源：http://dxw.vehdjk.com

SELECT * FROM (
来源：http://pks.52xcode.cn


<!-- 参考信息 -->