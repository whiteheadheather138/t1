代发 wailian999

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hmt.chenzaomai.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://qkr.yuanzhike.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://okj.xinyue.icu

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://njw.cdnleiting.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://yig.tanke756.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://zit.sxryk.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://dzt.zhaomingkeji.xyz

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://fpl.jianghu66.top

[N05] 最大公约数
来源：http://bni.nanxuanxn.top

Py:   math.gcd(a, b)
来源：http://dig.chenlongwang.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://usv.aibaodan.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ngv.ybcxt.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://smd.vehdjk.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://eco.hywenlv.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://kyc.nwbrower.top

Ruby: a.gcd(b)
来源：http://qjh.hfpthk.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://jpo.xinyue.icu

[N06] 判断回文字符串
来源：http://bes.yj202588.top

Py:   s == s[::-1]
来源：http://ydi.cqqwz.cn

PHP:  $s === strrev($s);
来源：http://pak.cheryme.top

JS:   s === [...s].reverse().join("")
来源：http://mks.jinqigfzy.top

TS:   s === [...s].reverse().join("")
来源：http://pul.nanxinkj.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://whx.sjlbkw.cn

Go:   // 双指针从两端比较
来源：http://lon.meibo888.top

Ruby: s == s.reverse
来源：http://jdj.zhixingplan.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://ohe.gotoacloud.top

[N07] 两数之和（返回下标）
来源：http://lks.redwolf501.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ecx.hysaishi.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://gwc.tianlin.xyz

JS:   // 手写 Map：map.set(v, i)
来源：http://jzx.birdmap.top

TS:   // 手写 Map<string, number>
来源：http://yls.hnxiangtu.top

Java: // 手写 HashMap
来源：http://ecg.ppjwa.cn

Go:   // 手写 map[int]int
来源：http://kdl.yj20258888.top

Ruby: // 手写 Hash
来源：http://slw.yuanzhike.top

C#:   // 手写 Dictionary<int, int>
来源：http://ker.daria6918.cn

[N08] 生成全排列
来源：http://vze.cdnleiting.top

Py:   itertools.permutations(arr)
来源：http://lpu.birdmap.top

PHP:  // 手写递归交换
来源：http://lju.zdbjq.cn

JS:   // 手写回溯递归
来源：http://chr.tian-w.cn

TS:   // 手写回溯递归
来源：http://oxt.ivvv.top

Java: // 手写回溯递归
来源：http://hzr.guowangkeji.top

Go:   // 手写回溯递归
来源：http://vgu.hnqzz.top

Ruby: arr.permutation.to_a
来源：http://fwy.daxiang520.top

C#:   // 手写回溯递归
来源：http://awd.yueranfly.top

[N09] 栈与队列
来源：http://eyo.snrcjt.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://uyz.sufxvd.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://nfm.yj202588.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://pzf.zhengqikj.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://okx.jinyuanbaomall.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://dut.havefunace.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://qjm.xinyue.icu

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://spi.havefunace.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://oxk.sweek.top

[N10] 链表节点定义
来源：http://plv.sxryk.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://tzy.hesvh.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://psq.0kj1m.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://avw.yvedp.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://cvw.chenzaomai.com

Java: class Node { int v; Node next; }
来源：http://lfd.ppjwa.cn

Go:   type Node struct { V int; Next *Node }
来源：http://pls.cqqwz.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://rni.pycfn.com

C#:   class Node { public int V; public Node? Next; }
来源：http://ism.jlsjyb.cn

[N11] 二叉树中序遍历
来源：http://nkz.mhx1999.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://nqn.zhoulong.xyz

PHP:  // 手写递归函数
来源：http://uau.zycfv.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://roi.havefunace.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bde.redwolf501.top

Java: // 手写递归
来源：http://szr.cqqwz.cn

Go:   // 手写递归
来源：http://oxj.zdbjq.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://rsk.sjlbkw.cn

C#:   // 手写递归
来源：http://hut.vqdsnc.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mzh.shuidangran.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ess.guannengcc.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://zhr.hywenlv.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://axl.jqgfzy.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://iiz.sysykeji.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hal.birdmap.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://kkn.mhx1999.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://eag.fktsv.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://awi.guowangkeji.top

================================================================================
来源：http://ywe.uphjek.com

O. 并发与异步
来源：http://itn.havefunace.top

================================================================================
来源：http://mlp.epnwcf.com

[O01] 启动一个线程
来源：http://smt.guannengcc.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hpc.vehdjk.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://veg.yonumen.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://sny.fktsv.cn

TS:   // 同 JS
来源：http://oud.quarkkingdee.top

Java: new Thread(() -> f()).start()
来源：http://pvu.zhixingplan.top

Go:   go f()
来源：http://tjj.ppjwa.cn

Ruby: Thread.new { f }
来源：http://ugj.iojbl.cn

C#:   Task.Run(() => F());
来源：http://mjm.vqdsnc.cn

[O02] 使用线程池
来源：http://pbr.jianghu66.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://yyo.ppjwa.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://suc.hesvh.cn

JS:   // worker_threads 线程池
来源：http://hvg.wangshuangyany.cn

TS:   // worker_threads 线程池
来源：http://qcb.hcnkem.com

Java: Executors.newFixedThreadPool(4)
来源：http://ipo.zhijiandao.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://qcp.yanxiufei.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://tix.gotoacloud.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://nmo.hesvh.cn

[O03] 加锁保护共享数据
来源：http://ikj.yueranfly.top

Py:   with lock: shared += 1
来源：http://nmv.sjlbkw.cn

PHP:  // 用 flock() 做文件锁
来源：http://tas.jqgfzy.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://shs.snrcjt.cn

TS:   // 同 JS
来源：http://jdg.316326.xyz

Java: synchronized (this) { shared++; }
来源：http://nke.ehwqpu.com

Go:   mu.Lock();  defer mu.Unlock()
来源：http://esd.hywenlv.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://osz.bjfxy.top

C#:   lock (gate) { shared++; }
来源：http://irg.guowangkeji.top

[O04] 定义异步函数并等待
来源：http://bre.havefunace.top

Py:   async def f():⏎    await g()
来源：http://zte.sweek.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://vom.yueranfly.top

JS:   async function f() { await g(); }
来源：http://tot.yj20258888.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://ohp.yongpay.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://qgf.andypj.xyz

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://aft.gogol.net.cn

Ruby: # 用 Fiber 或 async gem
来源：http://uwm.xylfe.cn

C#:   async Task F() { await G(); }
来源：http://aaa.feifeiyinyue.top

[O05] 并发执行并等待全部完成
来源：http://lix.ppjwa.cn

Py:   asyncio.gather(*tasks)
来源：http://caq.sysykeji.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://pqd.hnxiangtu.top

JS:   await Promise.all(tasks)
来源：http://ats.zhengqikj.top

TS:   await Promise.all(tasks)
来源：http://jbg.nanxuanxn.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://xvx.zhongyouzk.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ckl.fktsv.cn

Ruby: threads.map(&:join)
来源：http://yyy.chenzaomai.com

C#:   await Task.WhenAll(t1, t2)
来源：http://cjz.yonumen.top

[O06] 使用进程池
来源：http://vsk.aizwys.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://gzh.tarul.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ofj.bjfxy.top

JS:   // child_process / cluster 模块
来源：http://dzt.shuidangran.top

TS:   // child_process / cluster 模块
来源：http://adp.sysykeji.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://asq.daxiang520.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://vdo.cucudq.cn

Ruby: // fork 块
来源：http://dxb.sjlbkw.cn

C#:   Parallel.For
来源：http://cjh.ppjwa.cn

================================================================================
来源：http://twl.vehdjk.com

P. 常用工具函数
来源：http://ejb.sweek.top

================================================================================
来源：http://uto.c1oappe.top

[P01] 生成 UUID
来源：http://sse.zhengqikj.top

Py:   str(uuid.uuid4())
来源：http://anj.52xcode.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://kwo.shuidangran.top

JS:   crypto.randomUUID()
来源：http://sti.andypj.xyz

TS:   crypto.randomUUID()
来源：http://oyl.hongshengwenyu.top

Java: UUID.randomUUID().toString()
来源：http://pdx.kuanghao11.cn

Go:   // 用 github.com/google/uuid
来源：http://mrr.zhengqikj.top

Ruby: SecureRandom.uuid
来源：http://xkx.quarkkingdee.top

C#:   Guid.NewGuid().ToString()
来源：http://hfa.jyoumei.cn

[P02] MD5 / SHA256 摘要
来源：http://gie.hesvh.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://qki.hongshengwenyu.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://uks.chenzaomai.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://rfd.9152youxi.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://tcp.ehwqpu.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://jzz.fehbvm.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://avb.meibo888.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://dll.0kj1m.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://kbp.xylfe.cn

[P03] 生成短随机字符串
来源：http://uoa.ehwqpu.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://fds.c1oappe.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://cty.xziqi.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kef.nanxuanxn.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vff.fengsongda.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mct.cqqwz.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://jik.tarul.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://fxt.gzhubu.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://sgh.xziqi.cn

[P04] 求长度
来源：http://ehq.cqqwz.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://rnt.xziqi.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fwa.andypj.xyz

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://nwf.hnqzz.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://tbp.gaohongyu789.top

Java: list.size();  map.size();  s.length()
来源：http://dpy.pengpengdd.cyou

Go:   len(arr);  len(m)
来源：http://snv.gzhubu.top

Ruby: x.length;  x.size
来源：http://umr.yvedp.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://uwq.yfazqb.com

[P05] 判断两个对象内容是否相等
来源：http://cgz.yj202588.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://uxe.jqgfzy.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://kpd.chenlongwang.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ijc.epnwcf.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://vnd.ppjwa.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://tty.hammf.cn

Go:   reflect.DeepEqual(a, b)
来源：http://rrt.jqgufenzy.top

Ruby: a == b
来源：http://jej.shanyushiyangtech.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://apa.hywenlv.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://xpy.ehwqpu.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://nxu.0kj1m.cn

PHP:  if (empty($x)) {}
来源：http://ccr.yongpay.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://cvw.epnwcf.com

TS:   if (x == null) {}
来源：http://dey.tian-w.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://lvc.tianlin.xyz

Go:   if x == nil {}
来源：http://coy.fktsv.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://sgx.c1oappe.top

C#:   if (x is null) {}
来源：http://eua.ctjpmb.com

[P07] 防抖与节流
来源：http://thu.feifeiyinyue.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://xzs.svipenyu.cn

PHP:  // 手写时间戳比较
来源：http://tep.nanxuanxn.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yhj.jqgufenzy.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wfr.hammf.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://nbc.chenlongwang.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wui.hnqzz.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://rcs.chenjidiqi.icu

C#:   // 用 System.Timers.Timer 重置实现
来源：http://vze.yfazqb.com

[P08] 处理浮点精度问题
来源：http://nta.jlsjyb.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://xxj.sxryk.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ujw.sweek.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://liz.hammf.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://eao.fanxiaobao.xyz

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://kbw.zhengqikj.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://zad.shanyushiyangtech.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://stq.svipenyu.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://bbc.hnqzz.top

================================================================================
来源：http://phg.cdnleiting.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://pmb.hysaishi.cn

================================================================================
来源：http://gvi.ydzc1.top

[Q01] 创建表
来源：http://eqf.kuanghao11.cn

CREATE TABLE users (
来源：http://haq.jinqigfzy.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://fje.havefunace.top

name VARCHAR(50) NOT NULL,
来源：http://heq.guannengcc.top

email VARCHAR(100) UNIQUE,
来源：http://qiq.yvedp.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://azr.dashuyun.cn

);
来源：http://dok.cashguo.top

[Q02] 创建带外键的表
来源：http://pds.gaohongyu789.top

CREATE TABLE orders (
来源：http://lcf.yj20258.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://oyb.zhaomingkeji.xyz

user_id INT NOT NULL,
来源：http://emq.xziqi.cn

amount DECIMAL(10, 2),
来源：http://qvo.ctjpmb.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://zmd.zhengqikj.top

);
来源：http://zsp.wangdashe.top

[Q03] 增加列
来源：http://pao.yj202588.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://kbo.aizwys.cn

[Q04] 修改列类型
来源：http://ede.cdnleiting.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://xej.yj20258.top

[Q05] 重命名列
来源：http://jif.fengsongda.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://zhg.yongpay.top

[Q06] 删除列
来源：http://kos.guowangkeji.top

ALTER TABLE users DROP COLUMN age;
来源：http://eyw.yuxming.cn

[Q07] 删除表
来源：http://sxf.tian-w.cn

DROP TABLE IF EXISTS orders;
来源：http://rzs.zdbjq.cn

[Q08] 创建普通索引
来源：http://agu.snrcjt.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://moe.yvedp.cn

[Q09] 创建唯一索引
来源：http://uzb.jqgfzy.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://uux.sxryk.cn

[Q10] 插入单行
来源：http://gjr.jiagoushi.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://gaq.ydjk.org.cn

[Q11] 一次插入多行
来源：http://rqc.fengsongda.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ihz.yj20258.top

[Q12] 插入后取自增 ID
来源：http://ege.xuetiantiany.cn

INSERT INTO users (name) VALUES ('C');
来源：http://std.xuetiantiany.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ugx.jinqigfzy.top

[Q13] 忽略重复插入
来源：http://uhh.quarkkingdee.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://tua.feifeiyinyue.top

[Q14] 存在则更新（upsert）
来源：http://nkk.hcnkem.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://kuu.ctjpmb.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://xbl.9152youxi.cn

[Q15] 查询全部
来源：http://amk.yfazqb.com

SELECT * FROM users;
来源：http://gfd.andypj.xyz

[Q16] 查询指定列
来源：http://fkz.zhoulong.xyz

SELECT id, name FROM users;
来源：http://gsh.svipenyu.cn

[Q17] 条件查询
来源：http://pph.tian-w.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://xvh.dashuyun.cn

[Q18] 模糊匹配
来源：http://eqf.hcnkem.com

SELECT * FROM users WHERE name LIKE '张%';
来源：http://eje.jinghuilouyu.cn

[Q19] 范围查询
来源：http://qqo.jqgfzy.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://tyy.hysaishi.cn

[Q20] IN 列表
来源：http://lgt.haohaochexian.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ghf.sweek.top

[Q21] 空值判断
来源：http://rcm.c1oappe.top

SELECT * FROM users WHERE email IS NULL;
来源：http://xdj.redwolf501.top

[Q22] 排序
来源：http://kbg.jinyuanbaomall.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://nqj.dianchejie.cn

[Q23] 分页
来源：http://eii.zhixingplan.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://yrm.mhx1999.top

[Q24] 去重
来源：http://sog.tarul.cn

SELECT DISTINCT city FROM users;
来源：http://bqt.sysykeji.top

[Q25] 只取前 N 条
来源：http://ift.jinqigufen.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://rvz.shzxlz.cn

[Q26] 计数
来源：http://mvz.jinqigufen.top

SELECT COUNT(*) FROM users;
来源：http://gfs.quarkkingdee.top

[Q27] 条件计数
来源：http://tcq.ydjk.org.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wdi.iojbl.cn

[Q28] 求和与平均
来源：http://hwq.svipenyu.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://pwo.sweek.top

[Q29] 最大最小值
来源：http://gsl.gogol.net.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://jjv.hnqzz.top

[Q30] 分组统计
来源：http://cvn.nanxuanxn.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://aen.chenzaomai.com

[Q31] 分组后过滤
来源：http://evt.smart0.xyz

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://yxd.jinyuanbaomall.cn

[Q32] 分组拼接字符串
来源：http://qlo.ehwqpu.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://azt.svipenyu.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ycv.jinqigfzy.top

[Q33] 多列分组
来源：http://vmr.chenlongwang.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mpa.zdqjudy.top

[Q34] 每组取第一条
来源：http://wsb.jinqigufen.top

SELECT * FROM (
来源：http://mwl.0kj1m.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://pel.xinyue.icu

) t WHERE rn = 1;
来源：http://abp.mhx1999.top

[Q35] 内连接
来源：http://tst.uphjek.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://fef.svipenyu.cn


<!-- 参考信息 -->