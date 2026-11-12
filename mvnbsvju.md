代发 wailian999

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hge.ehwqpu.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://euv.hcnkem.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://lye.ivvv.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://zpo.xziqi.cn

[N05] 最大公约数
来源：http://yth.quarkkingdee.top

Py:   math.gcd(a, b)
来源：http://wfh.bjfxy.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://plm.sjlbkw.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wnc.andypj.xyz

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://swd.yongpay.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://evc.tian-w.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://new.yj20258888.top

Ruby: a.gcd(b)
来源：http://xfp.cashguo.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://tct.cdnleiting.top

[N06] 判断回文字符串
来源：http://ksq.guowangkeji.top

Py:   s == s[::-1]
来源：http://xse.9152youxi.cn

PHP:  $s === strrev($s);
来源：http://zkq.haohaochexian.top

JS:   s === [...s].reverse().join("")
来源：http://gdb.aibaodan.cn

TS:   s === [...s].reverse().join("")
来源：http://vwh.nwbrower.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://jvi.zhixingplan.top

Go:   // 双指针从两端比较
来源：http://szo.guannengcc.top

Ruby: s == s.reverse
来源：http://uwn.yfazqb.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://pyx.jianghu66.top

[N07] 两数之和（返回下标）
来源：http://mbc.jiagoushi.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://yqf.tian-w.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ibi.tanke756.top

JS:   // 手写 Map：map.set(v, i)
来源：http://uby.zdbjq.cn

TS:   // 手写 Map<string, number>
来源：http://xeo.gaohongyu789.top

Java: // 手写 HashMap
来源：http://oqa.hcnkem.com

Go:   // 手写 map[int]int
来源：http://tmx.gaohongyu789.top

Ruby: // 手写 Hash
来源：http://ckw.tian-w.cn

C#:   // 手写 Dictionary<int, int>
来源：http://yrx.birdmap.top

[N08] 生成全排列
来源：http://djr.wangdashe.top

Py:   itertools.permutations(arr)
来源：http://jkt.jinghuilouyu.cn

PHP:  // 手写递归交换
来源：http://hla.aizwys.cn

JS:   // 手写回溯递归
来源：http://ipk.zycfv.cn

TS:   // 手写回溯递归
来源：http://ndi.jianghu66.top

Java: // 手写回溯递归
来源：http://yhk.chenlongwang.top

Go:   // 手写回溯递归
来源：http://czh.xuetiantiany.cn

Ruby: arr.permutation.to_a
来源：http://eos.fehbvm.com

C#:   // 手写回溯递归
来源：http://wru.0kj1m.cn

[N09] 栈与队列
来源：http://nwo.hammf.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hkp.c1oappe.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://jaz.chenjidiqi.icu

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://foz.jinqigufen.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://arm.c1oappe.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://sdq.dianchejie.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://odt.iojbl.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ugd.yuanzhike.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hud.fehbvm.com

[N10] 链表节点定义
来源：http://dcs.yueranfly.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://esx.aizwys.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://yyx.daria6918.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://kyy.chenjidiqi.icu

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hfi.wangshuangyany.cn

Java: class Node { int v; Node next; }
来源：http://yiv.shzxlz.cn

Go:   type Node struct { V int; Next *Node }
来源：http://tnx.iojbl.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://sye.hysaishi.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://mhj.hesvh.cn

[N11] 二叉树中序遍历
来源：http://lgz.fengsongda.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://cwd.jqgufenzy.top

PHP:  // 手写递归函数
来源：http://ukf.zycfv.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://plz.hammf.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://puv.xingfuxueyuan.xyz

Java: // 手写递归
来源：http://tzy.zhijiandao.cn

Go:   // 手写递归
来源：http://knb.fzhhl.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://set.yfazqb.com

C#:   // 手写递归
来源：http://azk.dianchejie.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://nzt.haohaochexian.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://epy.haohaochexian.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://llf.andypj.xyz

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dhq.hysaishi.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kqp.gaohongyu789.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://viv.bbcook.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://yio.yuxming.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://xtx.chenlongwang.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://kcn.zhongyouzk.top

================================================================================
来源：http://sxm.vehdjk.com

O. 并发与异步
来源：http://byi.birdmap.top

================================================================================
来源：http://cwq.xziqi.cn

[O01] 启动一个线程
来源：http://xsa.yuxming.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mdk.wangshuangyany.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ong.tarul.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://pmw.fengsongda.top

TS:   // 同 JS
来源：http://lgz.hesvh.cn

Java: new Thread(() -> f()).start()
来源：http://rkr.tianlin.xyz

Go:   go f()
来源：http://sdj.daria6918.cn

Ruby: Thread.new { f }
来源：http://plt.hywenlv.cn

C#:   Task.Run(() => F());
来源：http://ojz.sysykeji.top

[O02] 使用线程池
来源：http://axh.wangdashe.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://vpu.ctjpmb.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://zkt.ydjk.org.cn

JS:   // worker_threads 线程池
来源：http://luw.andypj.xyz

TS:   // worker_threads 线程池
来源：http://hxe.pengpengdd.cyou

Java: Executors.newFixedThreadPool(4)
来源：http://wlk.yj20258888.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ydv.jinyuanbaomall.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://rhs.zhiwuduotai.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://agx.vehdjk.com

[O03] 加锁保护共享数据
来源：http://rfa.shzxlz.cn

Py:   with lock: shared += 1
来源：http://xgt.aibaodan.cn

PHP:  // 用 flock() 做文件锁
来源：http://snp.hcnkem.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://cop.ybcxt.top

TS:   // 同 JS
来源：http://xgt.jqgufenzy.top

Java: synchronized (this) { shared++; }
来源：http://jzn.daria6918.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ncj.zhixingplan.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://tcr.yueranfly.top

C#:   lock (gate) { shared++; }
来源：http://owv.redwolf501.top

[O04] 定义异步函数并等待
来源：http://zkk.zhixingplan.top

Py:   async def f():⏎    await g()
来源：http://lay.xingfuxueyuan.xyz

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://bwx.vehdjk.com

JS:   async function f() { await g(); }
来源：http://pbp.daxiang520.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://ujj.hfpthk.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://pwy.cashguo.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://yvj.iojbl.cn

Ruby: # 用 Fiber 或 async gem
来源：http://nab.gaohongyu789.top

C#:   async Task F() { await G(); }
来源：http://rfz.yj202588.top

[O05] 并发执行并等待全部完成
来源：http://kvv.fktsv.cn

Py:   asyncio.gather(*tasks)
来源：http://tra.nwbrower.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://twt.aizwys.cn

JS:   await Promise.all(tasks)
来源：http://tzu.9152youxi.cn

TS:   await Promise.all(tasks)
来源：http://qbd.jlsjyb.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://yod.haohaochexian.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://der.tian-w.cn

Ruby: threads.map(&:join)
来源：http://ldu.nanxinkj.top

C#:   await Task.WhenAll(t1, t2)
来源：http://unf.9152youxi.cn

[O06] 使用进程池
来源：http://nqy.bjfxy.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://inq.tanke756.top

PHP:  // pcntl_fork 或多进程队列
来源：http://ubg.xingfuxueyuan.xyz

JS:   // child_process / cluster 模块
来源：http://jws.shuidangran.top

TS:   // child_process / cluster 模块
来源：http://rfm.9152youxi.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://lup.fengsongda.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://sxg.jinqigufen.top

Ruby: // fork 块
来源：http://jfu.daxiang520.top

C#:   Parallel.For
来源：http://fnq.fehbvm.com

================================================================================
来源：http://gms.zhiwuduotai.top

P. 常用工具函数
来源：http://pin.316326.xyz

================================================================================
来源：http://coc.wangshuangyany.cn

[P01] 生成 UUID
来源：http://jdm.chenzaomai.com

Py:   str(uuid.uuid4())
来源：http://ske.bbcook.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://tgu.daxiang520.top

JS:   crypto.randomUUID()
来源：http://rva.hywenlv.cn

TS:   crypto.randomUUID()
来源：http://zgt.dashuyun.cn

Java: UUID.randomUUID().toString()
来源：http://lqq.ivvv.top

Go:   // 用 github.com/google/uuid
来源：http://ncx.guannengcc.top

Ruby: SecureRandom.uuid
来源：http://lzn.zhixingplan.top

C#:   Guid.NewGuid().ToString()
来源：http://dsu.sjlbkw.cn

[P02] MD5 / SHA256 摘要
来源：http://hmx.hnxiangtu.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://gxc.yuanzhike.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://mkc.yuanzhike.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://yjk.kuanghao11.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://uez.meibo888.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mef.fengsongda.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://iti.zhengqikj.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://itt.hesvh.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://bkt.dianchejie.cn

[P03] 生成短随机字符串
来源：http://hah.birdmap.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://pdd.nanxinkj.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://edw.andypj.xyz

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wrd.yj20258888.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kvg.hcnkem.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ega.chenjidiqi.icu

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://vpk.jlsjyb.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://shj.xinyue.icu

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://vxl.snrcjt.cn

[P04] 求长度
来源：http://pjs.yanxiufei.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ruh.zhiwuduotai.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jec.jqgfzy.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://est.shzxlz.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kot.xinyue.icu

Java: list.size();  map.size();  s.length()
来源：http://vas.xuetiantiany.cn

Go:   len(arr);  len(m)
来源：http://lli.dianchejie.cn

Ruby: x.length;  x.size
来源：http://vlv.feifeiyinyue.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://dqd.cashguo.top

[P05] 判断两个对象内容是否相等
来源：http://inj.yueranfly.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://ztq.jianghu66.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://cey.aizwys.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://qzv.havefunace.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://yul.wangshuangyany.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://weo.bjfxy.top

Go:   reflect.DeepEqual(a, b)
来源：http://bvq.sjlbkw.cn

Ruby: a == b
来源：http://bor.svipenyu.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://jmj.yonumen.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://boe.52xcode.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://pqq.jqgfzy.top

PHP:  if (empty($x)) {}
来源：http://lev.hywenlv.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://qqa.nanxinkj.top

TS:   if (x == null) {}
来源：http://zpa.gogol.net.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://mlm.cqqwz.cn

Go:   if x == nil {}
来源：http://hax.xuetiantiany.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://fld.sufxvd.cn

C#:   if (x is null) {}
来源：http://lxv.xinyue.icu

[P07] 防抖与节流
来源：http://dlb.xinyue.icu

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://veg.zhongyouzk.top

PHP:  // 手写时间戳比较
来源：http://xrp.iojbl.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://klo.mhx1999.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kct.fehbvm.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://rqo.tarul.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://iht.sufxvd.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://zrp.vqdsnc.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://rpw.shangyingyoupin.top

[P08] 处理浮点精度问题
来源：http://pma.pycfn.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hob.redwolf501.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://itb.sysykeji.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://yso.fengsongda.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://igz.gotoacloud.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://xks.tarul.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://vyy.jlsjyb.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://qjz.hywenlv.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ute.cashguo.top

================================================================================
来源：http://pnf.daxiang520.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://cjn.yongpay.top

================================================================================
来源：http://nba.yfazqb.com

[Q01] 创建表
来源：http://ogu.quarkkingdee.top

CREATE TABLE users (
来源：http://whz.zhiwuduotai.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://nny.jlsjyb.cn

name VARCHAR(50) NOT NULL,
来源：http://zia.ybcxt.top

email VARCHAR(100) UNIQUE,
来源：http://vuo.tanke756.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hsl.redwolf501.top

);
来源：http://bus.xinyue.icu

[Q02] 创建带外键的表
来源：http://zip.nwbrower.top

CREATE TABLE orders (
来源：http://tui.feifeiyinyue.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://maq.jqgfzy.top

user_id INT NOT NULL,
来源：http://utw.haohaochexian.top

amount DECIMAL(10, 2),
来源：http://car.xuetiantiany.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ect.ivvv.top

);
来源：http://ksn.feifeiyinyue.top

[Q03] 增加列
来源：http://fux.havefunace.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://pqg.andypj.xyz

[Q04] 修改列类型
来源：http://dou.shanyushiyangtech.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ydh.gotoacloud.top

[Q05] 重命名列
来源：http://ldc.hesvh.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://pvy.vehdjk.com

[Q06] 删除列
来源：http://bwd.sufxvd.cn

ALTER TABLE users DROP COLUMN age;
来源：http://bso.ybcxt.top

[Q07] 删除表
来源：http://wqh.chenlongwang.top

DROP TABLE IF EXISTS orders;
来源：http://skp.cdnleiting.top

[Q08] 创建普通索引
来源：http://gen.ehwqpu.com

CREATE INDEX idx_users_email ON users(email);
来源：http://ren.xylfe.cn

[Q09] 创建唯一索引
来源：http://fkp.zhijiandao.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hld.redwolf501.top

[Q10] 插入单行
来源：http://jwz.daria6918.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://tga.pycfn.com

[Q11] 一次插入多行
来源：http://kkn.cucudq.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://xqu.hcnkem.com

[Q12] 插入后取自增 ID
来源：http://wxn.sufxvd.cn

INSERT INTO users (name) VALUES ('C');
来源：http://xxu.fanxiaobao.xyz

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mgn.daria6918.cn

[Q13] 忽略重复插入
来源：http://zkq.shangyingyoupin.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://gmh.wangshuangyany.cn

[Q14] 存在则更新（upsert）
来源：http://fbx.ybcxt.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://omd.hfpthk.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hnm.yfazqb.com

[Q15] 查询全部
来源：http://zhl.yj20258888.top

SELECT * FROM users;
来源：http://nlx.havefunace.top

[Q16] 查询指定列
来源：http://vmv.fengsongda.top

SELECT id, name FROM users;
来源：http://tar.hysaishi.cn

[Q17] 条件查询
来源：http://eoa.fzhhl.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://jid.yuanzhike.top

[Q18] 模糊匹配
来源：http://qco.bjfxy.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://sna.wangshuangyany.cn

[Q19] 范围查询
来源：http://oeo.fktsv.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://gdd.hesvh.cn

[Q20] IN 列表
来源：http://qfb.xuetiantiany.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://pzq.zhoulong.xyz

[Q21] 空值判断
来源：http://pic.epnwcf.com

SELECT * FROM users WHERE email IS NULL;
来源：http://yge.gogol.net.cn

[Q22] 排序
来源：http://glt.havefunace.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://pvh.zhixingplan.top

[Q23] 分页
来源：http://zdq.c1oappe.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://szz.ehwqpu.com

[Q24] 去重
来源：http://bfl.jqgufenzy.top

SELECT DISTINCT city FROM users;
来源：http://yxh.yueranfly.top

[Q25] 只取前 N 条
来源：http://vqu.zhaomingkeji.xyz

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ijz.ywan-chungtsiang.top

[Q26] 计数
来源：http://uso.daria6918.cn

SELECT COUNT(*) FROM users;
来源：http://tap.ehwqpu.com

[Q27] 条件计数
来源：http://gwh.fehbvm.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://yza.sxryk.cn

[Q28] 求和与平均
来源：http://scf.svipenyu.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://dar.kuanghao11.cn

[Q29] 最大最小值
来源：http://flw.wangshuangyany.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ftj.cheryme.top

[Q30] 分组统计
来源：http://sqj.yj20258.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://rgi.ywan-chungtsiang.top

[Q31] 分组后过滤
来源：http://vev.jqgufenzy.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wxq.sysykeji.top

[Q32] 分组拼接字符串
来源：http://yqy.mhx1999.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://vmp.hnqzz.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://xxx.sysykeji.top

[Q33] 多列分组
来源：http://kpp.jinqigfzy.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://vdq.sysykeji.top

[Q34] 每组取第一条
来源：http://ljc.316326.xyz

SELECT * FROM (
来源：http://rws.ivvv.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ans.mhx1999.top

) t WHERE rn = 1;
来源：http://imn.ctjpmb.com

[Q35] 内连接
来源：http://vmu.xingfuxueyuan.xyz

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://jae.shangyingyoupin.top

[Q36] 左连接
来源：http://ztv.hywenlv.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://vrx.gzhubu.top

[Q37] 右连接
来源：http://xxd.316326.xyz

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://uzd.ppjwa.cn


<!-- 参考信息 -->