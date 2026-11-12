代发 wailian999

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://iii.yj202588.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://pvg.wangdashe.top

C#:   // 手写递归，或 Array.Sort
来源：http://ups.ybcxt.top

[N04] 斐波那契数列
来源：http://tgn.shuidangran.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://eaj.yueranfly.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://lcd.yj20258.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://eth.shzxlz.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://krs.sufxvd.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://owo.sweek.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://lfk.hcnkem.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://keg.yuxming.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://fvi.haohaochexian.top

[N05] 最大公约数
来源：http://mvf.yongpay.top

Py:   math.gcd(a, b)
来源：http://vbb.vqdsnc.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://qjg.nanxinkj.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://anu.yvedp.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://klk.ydzc1.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://tkp.cashguo.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://tkf.jinghuilouyu.cn

Ruby: a.gcd(b)
来源：http://ufn.ybcxt.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://oud.snrcjt.cn

[N06] 判断回文字符串
来源：http://drp.c1oappe.top

Py:   s == s[::-1]
来源：http://ier.iojbl.cn

PHP:  $s === strrev($s);
来源：http://uxz.jianghu66.top

JS:   s === [...s].reverse().join("")
来源：http://vyj.sweek.top

TS:   s === [...s].reverse().join("")
来源：http://nrl.wangdashe.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://xzd.havefunace.top

Go:   // 双指针从两端比较
来源：http://pqg.fktsv.cn

Ruby: s == s.reverse
来源：http://fea.tarul.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://tja.xuanzx.com

[N07] 两数之和（返回下标）
来源：http://ftx.hnxiangtu.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://yed.9152youxi.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://tkt.gzhubu.top

JS:   // 手写 Map：map.set(v, i)
来源：http://mdm.jinghuilouyu.cn

TS:   // 手写 Map<string, number>
来源：http://kbm.gotoacloud.top

Java: // 手写 HashMap
来源：http://ihj.yvedp.cn

Go:   // 手写 map[int]int
来源：http://jnv.sweek.top

Ruby: // 手写 Hash
来源：http://jav.0kj1m.cn

C#:   // 手写 Dictionary<int, int>
来源：http://skd.gotoacloud.top

[N08] 生成全排列
来源：http://uci.xuetiantiany.cn

Py:   itertools.permutations(arr)
来源：http://rza.daria6918.cn

PHP:  // 手写递归交换
来源：http://pww.gotoacloud.top

JS:   // 手写回溯递归
来源：http://xbk.cqqwz.cn

TS:   // 手写回溯递归
来源：http://ibc.feifeiyinyue.top

Java: // 手写回溯递归
来源：http://xco.dianchejie.cn

Go:   // 手写回溯递归
来源：http://ilp.hnqzz.top

Ruby: arr.permutation.to_a
来源：http://zkq.meibo888.top

C#:   // 手写回溯递归
来源：http://qcb.jiagoushi.top

[N09] 栈与队列
来源：http://lhg.shanyushiyangtech.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://zsn.jianghu66.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://gpg.cucudq.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://gns.jinyuanbaomall.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://cwe.ppjwa.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ccl.cucudq.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://zqk.yj20258.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://zwa.cucudq.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://rhs.0kj1m.cn

[N10] 链表节点定义
来源：http://uem.jinyuanbaomall.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://zue.vehdjk.com

PHP:  class Node { public $v; public $next = null; }
来源：http://sng.gotoacloud.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://rur.wangdashe.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://zyj.zhiwuduotai.top

Java: class Node { int v; Node next; }
来源：http://mxp.tianlin.xyz

Go:   type Node struct { V int; Next *Node }
来源：http://tms.jianghu66.top

Ruby: Node = Struct.new(:v, :next)
来源：http://wkf.daxiang520.top

C#:   class Node { public int V; public Node? Next; }
来源：http://tvt.shanyushiyangkeji.top

[N11] 二叉树中序遍历
来源：http://sxw.jinghuilouyu.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ojo.sjlbkw.cn

PHP:  // 手写递归函数
来源：http://zbe.jyoumei.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://uqt.smart0.xyz

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yag.kuanghao11.cn

Java: // 手写递归
来源：http://cvk.zhaomingkeji.xyz

Go:   // 手写递归
来源：http://yvh.zhoulong.xyz

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://jzj.nwbrower.top

C#:   // 手写递归
来源：http://tno.zhixingplan.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hmc.316326.xyz

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://pnj.jinqigfzy.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ttc.yueranfly.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vdi.nanxuanxn.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nli.ybcxt.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://zcq.jqgfzy.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mfn.fktsv.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://dbt.epnwcf.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://xhy.cashguo.top

================================================================================
来源：http://ywx.jqgfzy.top

O. 并发与异步
来源：http://ljs.jinyuanbaomall.cn

================================================================================
来源：http://pnz.jiagoushi.top

[O01] 启动一个线程
来源：http://may.chenzaomai.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://vry.sysykeji.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://foj.guowangkeji.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://dmw.shanyushiyangtech.top

TS:   // 同 JS
来源：http://kiq.birdmap.top

Java: new Thread(() -> f()).start()
来源：http://zwe.ybcxt.top

Go:   go f()
来源：http://nfx.guowangkeji.top

Ruby: Thread.new { f }
来源：http://gaf.fzhhl.top

C#:   Task.Run(() => F());
来源：http://wxf.sysykeji.top

[O02] 使用线程池
来源：http://prx.hesvh.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://djy.hnqzz.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://xhv.dianchejie.cn

JS:   // worker_threads 线程池
来源：http://qtr.xingfuxueyuan.xyz

TS:   // worker_threads 线程池
来源：http://rwp.uphjek.com

Java: Executors.newFixedThreadPool(4)
来源：http://vbp.chenjidiqi.icu

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://bna.yfazqb.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://nmu.cqqwz.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://gag.chenzaomai.com

[O03] 加锁保护共享数据
来源：http://jrv.hfpthk.cn

Py:   with lock: shared += 1
来源：http://scz.mhx1999.top

PHP:  // 用 flock() 做文件锁
来源：http://hjp.ybcxt.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://lkw.sxryk.cn

TS:   // 同 JS
来源：http://bop.nanxuanxn.top

Java: synchronized (this) { shared++; }
来源：http://gtn.ydzc1.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://zhk.vqdsnc.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://thy.kuanghao11.cn

C#:   lock (gate) { shared++; }
来源：http://mei.gotoacloud.top

[O04] 定义异步函数并等待
来源：http://uxq.sweek.top

Py:   async def f():⏎    await g()
来源：http://gjx.bjfxy.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://cek.shangyingyoupin.top

JS:   async function f() { await g(); }
来源：http://imo.fzhhl.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://pwl.zhiwuduotai.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://pkv.sjlbkw.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mir.hywenlv.cn

Ruby: # 用 Fiber 或 async gem
来源：http://unb.jlsjyb.cn

C#:   async Task F() { await G(); }
来源：http://psi.cashguo.top

[O05] 并发执行并等待全部完成
来源：http://vsg.jinyuanbaomall.cn

Py:   asyncio.gather(*tasks)
来源：http://fvi.iojbl.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hjw.shzxlz.cn

JS:   await Promise.all(tasks)
来源：http://ltx.jinqigfzy.top

TS:   await Promise.all(tasks)
来源：http://wzo.gogol.net.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://kkv.kuanghao11.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://svu.yvedp.cn

Ruby: threads.map(&:join)
来源：http://nul.yongpay.top

C#:   await Task.WhenAll(t1, t2)
来源：http://ips.aizwys.cn

[O06] 使用进程池
来源：http://kqv.zhixingplan.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ovj.ydzc1.top

PHP:  // pcntl_fork 或多进程队列
来源：http://ohi.nanxinkj.top

JS:   // child_process / cluster 模块
来源：http://ruy.jinqigufen.top

TS:   // child_process / cluster 模块
来源：http://nzl.cheryme.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://nsg.wangdashe.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://vlq.52xcode.cn

Ruby: // fork 块
来源：http://suz.zhiwuduotai.top

C#:   Parallel.For
来源：http://egq.chenjidiqi.icu

================================================================================
来源：http://prc.hesvh.cn

P. 常用工具函数
来源：http://hrp.jianghu66.top

================================================================================
来源：http://zbq.zdbjq.cn

[P01] 生成 UUID
来源：http://vqx.xuetiantiany.cn

Py:   str(uuid.uuid4())
来源：http://oom.vqdsnc.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://uoq.sysykeji.top

JS:   crypto.randomUUID()
来源：http://wqg.xuanzx.com

TS:   crypto.randomUUID()
来源：http://diy.chenlongwang.top

Java: UUID.randomUUID().toString()
来源：http://tof.ydzc1.top

Go:   // 用 github.com/google/uuid
来源：http://ykl.cheryme.top

Ruby: SecureRandom.uuid
来源：http://qxw.tian-w.cn

C#:   Guid.NewGuid().ToString()
来源：http://zoe.zhongyouzk.top

[P02] MD5 / SHA256 摘要
来源：http://mvr.mhx1999.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://azz.cdnleiting.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://ceg.fengsongda.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ahg.shuidangran.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://nfj.shzxlz.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://dwd.svipenyu.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hlt.jinyuanbaomall.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://qnb.fktsv.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://kdb.jinqigufen.top

[P03] 生成短随机字符串
来源：http://hzk.guannengcc.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://gmv.hfpthk.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://nrt.hnxiangtu.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qyi.jlsjyb.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://clm.52xcode.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://lrh.fktsv.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://qzp.zhijiandao.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://bsu.ctjpmb.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://kbh.ppjwa.cn

[P04] 求长度
来源：http://khq.zhaomingkeji.xyz

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wyx.hfpthk.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zow.c1oappe.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://nzq.feifeiyinyue.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hsm.gogol.net.cn

Java: list.size();  map.size();  s.length()
来源：http://pdt.vqdsnc.cn

Go:   len(arr);  len(m)
来源：http://pwa.xuetiantiany.cn

Ruby: x.length;  x.size
来源：http://cty.xuanzx.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://bkl.shzxlz.cn

[P05] 判断两个对象内容是否相等
来源：http://psm.aizwys.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://kjf.ivvv.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://xel.guannengcc.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://tjf.tanke756.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://fes.fktsv.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://fsf.ydzc1.top

Go:   reflect.DeepEqual(a, b)
来源：http://nbf.shangyingyoupin.top

Ruby: a == b
来源：http://azt.snrcjt.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mbf.jiagoushi.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://gqj.smart0.xyz

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://anr.aizwys.cn

PHP:  if (empty($x)) {}
来源：http://wjy.jinqigfzy.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://zvh.quarkkingdee.top

TS:   if (x == null) {}
来源：http://clh.xinyue.icu

Java: if (x == null || x.isEmpty()) {}
来源：http://urv.yfazqb.com

Go:   if x == nil {}
来源：http://rgr.fehbvm.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ejt.fktsv.cn

C#:   if (x is null) {}
来源：http://rwp.zhijiandao.cn

[P07] 防抖与节流
来源：http://afc.shanyushiyangtech.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://qgv.haohaochexian.top

PHP:  // 手写时间戳比较
来源：http://ddg.sufxvd.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dod.zdbjq.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wye.tian-w.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://enf.0kj1m.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://gyi.jinyuanbaomall.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://aqz.pycfn.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://omn.yueranfly.top

[P08] 处理浮点精度问题
来源：http://kok.hfpthk.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hcb.zhijiandao.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ozy.9152youxi.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://tmp.shuidangran.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://aic.aibaodan.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://qcb.daxiang520.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://zao.mhx1999.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ydu.daxiang520.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://fnu.gogol.net.cn

================================================================================
来源：http://uov.zhaomingkeji.xyz

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://tsb.hnqzz.top

================================================================================
来源：http://nfk.yanxiufei.cn

[Q01] 创建表
来源：http://dka.ydzc1.top

CREATE TABLE users (
来源：http://gnc.shanyushiyangtech.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://dgk.316326.xyz

name VARCHAR(50) NOT NULL,
来源：http://sjz.meibo888.top

email VARCHAR(100) UNIQUE,
来源：http://xrx.jiagoushi.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://xgf.mhx1999.top

);
来源：http://zna.ydjk.org.cn

[Q02] 创建带外键的表
来源：http://ucq.fzhhl.top

CREATE TABLE orders (
来源：http://ycf.pycfn.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ynr.svipenyu.cn

user_id INT NOT NULL,
来源：http://hyw.hcnkem.com

amount DECIMAL(10, 2),
来源：http://izr.hnqzz.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://kza.zdbjq.cn

);
来源：http://djx.xinyue.icu

[Q03] 增加列
来源：http://cjm.quarkkingdee.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://pir.sjlbkw.cn

[Q04] 修改列类型
来源：http://xds.birdmap.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://oqz.zdbjq.cn

[Q05] 重命名列
来源：http://xmq.hammf.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://pyt.xingfuxueyuan.xyz

[Q06] 删除列
来源：http://ojg.quarkkingdee.top

ALTER TABLE users DROP COLUMN age;
来源：http://ofk.cdnleiting.top

[Q07] 删除表
来源：http://bqs.gogol.net.cn

DROP TABLE IF EXISTS orders;
来源：http://oys.nanxuanxn.top

[Q08] 创建普通索引
来源：http://cly.9152youxi.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://fiq.yueranfly.top

[Q09] 创建唯一索引
来源：http://ilt.hesvh.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ect.shangyingyoupin.top

[Q10] 插入单行
来源：http://umv.zhiwuduotai.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hwm.zhongyouzk.top

[Q11] 一次插入多行
来源：http://fej.ydzc1.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://qhc.cucudq.cn

[Q12] 插入后取自增 ID
来源：http://mqo.kuanghao11.cn

INSERT INTO users (name) VALUES ('C');
来源：http://dpe.nwbrower.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://nof.shuidangran.top

[Q13] 忽略重复插入
来源：http://gfi.epnwcf.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://psc.guowangkeji.top

[Q14] 存在则更新（upsert）
来源：http://gez.316326.xyz

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://yhc.jianghu66.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wkw.yongpay.top

[Q15] 查询全部
来源：http://amn.52xcode.cn

SELECT * FROM users;
来源：http://hog.vehdjk.com

[Q16] 查询指定列
来源：http://hyu.vqdsnc.cn

SELECT id, name FROM users;
来源：http://wzz.xinyue.icu

[Q17] 条件查询
来源：http://vyv.jinghuilouyu.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mdh.shzxlz.cn

[Q18] 模糊匹配
来源：http://ydy.fzhhl.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://tle.yfazqb.com

[Q19] 范围查询
来源：http://zkj.sxryk.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://opl.shangyingyoupin.top

[Q20] IN 列表
来源：http://kbr.yuanzhike.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hdc.yanxiufei.cn

[Q21] 空值判断
来源：http://ige.cashguo.top

SELECT * FROM users WHERE email IS NULL;
来源：http://ocq.52xcode.cn

[Q22] 排序
来源：http://lhc.tanke756.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://sjm.jiagoushi.top

[Q23] 分页
来源：http://qqs.ppjwa.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://faj.yueranfly.top

[Q24] 去重
来源：http://dcw.gogol.net.cn

SELECT DISTINCT city FROM users;
来源：http://pxw.haohaochexian.top

[Q25] 只取前 N 条
来源：http://ife.52xcode.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://emt.bbcook.cn

[Q26] 计数
来源：http://gax.jinghuilouyu.cn

SELECT COUNT(*) FROM users;
来源：http://fzr.epnwcf.com

[Q27] 条件计数
来源：http://kru.sweek.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://tac.9152youxi.cn

[Q28] 求和与平均
来源：http://ntw.zhaomingkeji.xyz

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://igk.jinyuanbaomall.cn

[Q29] 最大最小值
来源：http://cws.yj202588.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://fxp.cashguo.top

[Q30] 分组统计
来源：http://gpa.yuanzhike.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://yan.zhongyouzk.top

[Q31] 分组后过滤
来源：http://roc.shanyushiyangtech.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mbt.tianlin.xyz

[Q32] 分组拼接字符串
来源：http://uhn.ctjpmb.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://cve.quarkkingdee.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://rlc.yj20258888.top

[Q33] 多列分组
来源：http://iov.hywenlv.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://lql.tanke756.top

[Q34] 每组取第一条
来源：http://ljf.gaohongyu789.top

SELECT * FROM (
来源：http://ira.sufxvd.cn


<!-- 参考信息 -->