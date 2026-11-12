代发 wailian999

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://iij.tanke756.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://pqn.bbcook.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://sel.yonumen.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://atb.vqdsnc.cn

[N05] 最大公约数
来源：http://oeu.jinyuanbaomall.cn

Py:   math.gcd(a, b)
来源：http://jnx.dianchejie.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://lhv.dianchejie.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jnd.fzhhl.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://yol.316326.xyz

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://bwx.hongshengwenyu.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://nor.hesvh.cn

Ruby: a.gcd(b)
来源：http://aiq.316326.xyz

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ybw.9152youxi.cn

[N06] 判断回文字符串
来源：http://san.xingfuxueyuan.xyz

Py:   s == s[::-1]
来源：http://ygx.xinyue.icu

PHP:  $s === strrev($s);
来源：http://clg.tian-w.cn

JS:   s === [...s].reverse().join("")
来源：http://nhv.nwbrower.top

TS:   s === [...s].reverse().join("")
来源：http://bkr.tianlin.xyz

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://fxb.vqdsnc.cn

Go:   // 双指针从两端比较
来源：http://xaz.cqqwz.cn

Ruby: s == s.reverse
来源：http://ocm.yangfankeji.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://qfd.uphjek.com

[N07] 两数之和（返回下标）
来源：http://mum.iojbl.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://acw.epnwcf.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ppg.ehwqpu.com

JS:   // 手写 Map：map.set(v, i)
来源：http://vib.haohaochexian.top

TS:   // 手写 Map<string, number>
来源：http://nin.mhx1999.top

Java: // 手写 HashMap
来源：http://rwb.hesvh.cn

Go:   // 手写 map[int]int
来源：http://yip.ppjwa.cn

Ruby: // 手写 Hash
来源：http://isa.feifeiyinyue.top

C#:   // 手写 Dictionary<int, int>
来源：http://qxl.zhiwuduotai.top

[N08] 生成全排列
来源：http://mvj.shanyushiyangtech.top

Py:   itertools.permutations(arr)
来源：http://kci.smart0.xyz

PHP:  // 手写递归交换
来源：http://axc.chenjidiqi.icu

JS:   // 手写回溯递归
来源：http://bhd.zhongyouzk.top

TS:   // 手写回溯递归
来源：http://ubw.9152youxi.cn

Java: // 手写回溯递归
来源：http://eiv.jianghu66.top

Go:   // 手写回溯递归
来源：http://wcr.vqdsnc.cn

Ruby: arr.permutation.to_a
来源：http://gzs.jqgfzy.top

C#:   // 手写回溯递归
来源：http://fzo.hcnkem.com

[N09] 栈与队列
来源：http://huu.tian-w.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://gga.zhijiandao.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://tld.zhongyouzk.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://isw.uphjek.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mmu.shangyingyoupin.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://csz.52xcode.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://dwi.uphjek.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://nwl.nwbrower.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://jfd.jiagoushi.top

[N10] 链表节点定义
来源：http://mgl.meibo888.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wjy.havefunace.top

PHP:  class Node { public $v; public $next = null; }
来源：http://cnm.xuanzx.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://gpo.hnqzz.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://yiz.sxryk.cn

Java: class Node { int v; Node next; }
来源：http://edd.fengsongda.top

Go:   type Node struct { V int; Next *Node }
来源：http://joo.fzhhl.top

Ruby: Node = Struct.new(:v, :next)
来源：http://weq.fengsongda.top

C#:   class Node { public int V; public Node? Next; }
来源：http://pej.vqdsnc.cn

[N11] 二叉树中序遍历
来源：http://xfe.smart0.xyz

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://lhw.shanyushiyangkeji.top

PHP:  // 手写递归函数
来源：http://ncd.zdqjudy.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yby.yanxiufei.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://uqq.xuanzx.com

Java: // 手写递归
来源：http://gex.xylfe.cn

Go:   // 手写递归
来源：http://ixn.mhx1999.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://dyb.xylfe.cn

C#:   // 手写递归
来源：http://cxs.ydzc1.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://fqi.hfpthk.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://nxn.xuetiantiany.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://qbu.chenzaomai.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kkf.fengsongda.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fxc.zdqjudy.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://fer.wangdashe.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://tbi.xinyue.icu

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://oez.gzhubu.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://zdr.cdnleiting.top

================================================================================
来源：http://wtb.chenzaomai.com

O. 并发与异步
来源：http://tam.cheryme.top

================================================================================
来源：http://vbq.yuanzhike.top

[O01] 启动一个线程
来源：http://emd.yj20258888.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://jtm.ppjwa.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wbl.dianchejie.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wje.meibo888.top

TS:   // 同 JS
来源：http://ukh.sufxvd.cn

Java: new Thread(() -> f()).start()
来源：http://nyt.tianlin.xyz

Go:   go f()
来源：http://iwx.jinyuanbaomall.cn

Ruby: Thread.new { f }
来源：http://ehq.jinqigufen.top

C#:   Task.Run(() => F());
来源：http://adc.cashguo.top

[O02] 使用线程池
来源：http://rty.hnxiangtu.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mal.yvedp.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ovr.tian-w.cn

JS:   // worker_threads 线程池
来源：http://bbq.hnqzz.top

TS:   // worker_threads 线程池
来源：http://twr.dianchejie.cn

Java: Executors.newFixedThreadPool(4)
来源：http://car.ivvv.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://uxr.havefunace.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://bzm.zycfv.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://chm.xuanzx.com

[O03] 加锁保护共享数据
来源：http://ewy.redwolf501.top

Py:   with lock: shared += 1
来源：http://crg.gaohongyu789.top

PHP:  // 用 flock() 做文件锁
来源：http://unu.aibaodan.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://tmy.yfazqb.com

TS:   // 同 JS
来源：http://iwv.daxiang520.top

Java: synchronized (this) { shared++; }
来源：http://hcy.chenjidiqi.icu

Go:   mu.Lock();  defer mu.Unlock()
来源：http://jtq.xylfe.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://wve.fanxiaobao.xyz

C#:   lock (gate) { shared++; }
来源：http://cna.chenjidiqi.icu

[O04] 定义异步函数并等待
来源：http://dso.cqqwz.cn

Py:   async def f():⏎    await g()
来源：http://bva.zhongyouzk.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://zmr.dashuyun.cn

JS:   async function f() { await g(); }
来源：http://tuh.iojbl.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ftv.uphjek.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://cba.andypj.xyz

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://zhy.hywenlv.cn

Ruby: # 用 Fiber 或 async gem
来源：http://yuo.chenzaomai.com

C#:   async Task F() { await G(); }
来源：http://pgv.haohaochexian.top

[O05] 并发执行并等待全部完成
来源：http://daz.kuanghao11.cn

Py:   asyncio.gather(*tasks)
来源：http://hbr.fanxiaobao.xyz

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://vbm.jinqigufen.top

JS:   await Promise.all(tasks)
来源：http://his.wangdashe.top

TS:   await Promise.all(tasks)
来源：http://eeu.iojbl.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://agv.xinyue.icu

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://cre.xuanzx.com

Ruby: threads.map(&:join)
来源：http://aml.jqgfzy.top

C#:   await Task.WhenAll(t1, t2)
来源：http://hed.yj20258888.top

[O06] 使用进程池
来源：http://yjv.chenlongwang.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wdz.xziqi.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://reg.sysykeji.top

JS:   // child_process / cluster 模块
来源：http://cyv.shanyushiyangtech.top

TS:   // child_process / cluster 模块
来源：http://zll.yvedp.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://dnr.chenlongwang.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://xmy.xziqi.cn

Ruby: // fork 块
来源：http://sdo.nwbrower.top

C#:   Parallel.For
来源：http://lvd.fktsv.cn

================================================================================
来源：http://dsi.mhx1999.top

P. 常用工具函数
来源：http://irf.sysykeji.top

================================================================================
来源：http://ays.zhaomingkeji.xyz

[P01] 生成 UUID
来源：http://fvc.ehwqpu.com

Py:   str(uuid.uuid4())
来源：http://hpj.yuxming.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mnm.xuanzx.com

JS:   crypto.randomUUID()
来源：http://nxb.mhx1999.top

TS:   crypto.randomUUID()
来源：http://ikw.yj20258888.top

Java: UUID.randomUUID().toString()
来源：http://snz.nanxuanxn.top

Go:   // 用 github.com/google/uuid
来源：http://bbe.fanxiaobao.xyz

Ruby: SecureRandom.uuid
来源：http://zef.yangfankeji.com

C#:   Guid.NewGuid().ToString()
来源：http://rzq.jinqigufen.top

[P02] MD5 / SHA256 摘要
来源：http://img.316326.xyz

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://fep.mhx1999.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://xej.birdmap.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://dir.yuanzhike.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://vml.fehbvm.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://znq.yj202588.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://xwv.guowangkeji.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://szi.tianlin.xyz

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://jjg.ydjk.org.cn

[P03] 生成短随机字符串
来源：http://nhx.zycfv.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://lcr.tarul.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://yha.0kj1m.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mfb.xinyue.icu

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ttn.cashguo.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://eem.fehbvm.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://yme.uphjek.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://mrl.dianchejie.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hyp.birdmap.top

[P04] 求长度
来源：http://jxn.ydzc1.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://gls.yuxming.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ibr.xziqi.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://toi.chenlongwang.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fpl.yongpay.top

Java: list.size();  map.size();  s.length()
来源：http://hjl.fktsv.cn

Go:   len(arr);  len(m)
来源：http://fjg.redwolf501.top

Ruby: x.length;  x.size
来源：http://ltn.sufxvd.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ccy.ehwqpu.com

[P05] 判断两个对象内容是否相等
来源：http://ajt.sufxvd.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://bia.hfpthk.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://dbd.yfazqb.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mgm.snrcjt.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://snq.hammf.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://dxq.cashguo.top

Go:   reflect.DeepEqual(a, b)
来源：http://bit.zdbjq.cn

Ruby: a == b
来源：http://gts.nanxinkj.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://atv.fzhhl.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://bmq.shuidangran.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://xce.zhongyouzk.top

PHP:  if (empty($x)) {}
来源：http://qby.ybcxt.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://xja.yangfankeji.com

TS:   if (x == null) {}
来源：http://imi.shuidangran.top

Java: if (x == null || x.isEmpty()) {}
来源：http://vkl.zhiwuduotai.top

Go:   if x == nil {}
来源：http://iqp.shzxlz.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://gsk.sweek.top

C#:   if (x is null) {}
来源：http://zsg.hnqzz.top

[P07] 防抖与节流
来源：http://dnd.xuetiantiany.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://zfx.yanxiufei.cn

PHP:  // 手写时间戳比较
来源：http://iuq.zycfv.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hno.ivvv.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://uim.jianghu66.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ewm.shuidangran.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wct.cucudq.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://wiq.sufxvd.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://tlj.hongshengwenyu.top

[P08] 处理浮点精度问题
来源：http://utk.wangshuangyany.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://spf.daxiang520.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://iim.jqgfzy.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://yll.fktsv.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://yej.xinyue.icu

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://fqp.yueranfly.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://zqv.xziqi.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hgt.svipenyu.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://lyx.pengpengdd.cyou

================================================================================
来源：http://jxq.shangyingyoupin.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://eax.ydjk.org.cn

================================================================================
来源：http://gun.jiagoushi.top

[Q01] 创建表
来源：http://vsh.yanxiufei.cn

CREATE TABLE users (
来源：http://met.zhixingplan.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://xzd.jinqigfzy.top

name VARCHAR(50) NOT NULL,
来源：http://bto.ehwqpu.com

email VARCHAR(100) UNIQUE,
来源：http://ttu.jinghuilouyu.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mcq.cdnleiting.top

);
来源：http://anu.xziqi.cn

[Q02] 创建带外键的表
来源：http://gku.fengsongda.top

CREATE TABLE orders (
来源：http://aml.iojbl.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://fzj.snrcjt.cn

user_id INT NOT NULL,
来源：http://rdx.vehdjk.com

amount DECIMAL(10, 2),
来源：http://utr.jinghuilouyu.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://vgh.nwbrower.top

);
来源：http://hxq.pycfn.com

[Q03] 增加列
来源：http://rxt.zdqjudy.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://uqa.xingfuxueyuan.xyz

[Q04] 修改列类型
来源：http://vjk.xuanzx.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://lrl.shanyushiyangtech.top

[Q05] 重命名列
来源：http://lcd.yueranfly.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ckk.zhongyouzk.top

[Q06] 删除列
来源：http://lqm.tian-w.cn

ALTER TABLE users DROP COLUMN age;
来源：http://tbg.yueranfly.top

[Q07] 删除表
来源：http://jud.cashguo.top

DROP TABLE IF EXISTS orders;
来源：http://bki.epnwcf.com

[Q08] 创建普通索引
来源：http://mfb.hesvh.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://rbh.smart0.xyz

[Q09] 创建唯一索引
来源：http://hjz.havefunace.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ldk.shuidangran.top

[Q10] 插入单行
来源：http://hrd.xuetiantiany.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://arf.fzhhl.top

[Q11] 一次插入多行
来源：http://dcf.yj20258888.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://oge.uphjek.com

[Q12] 插入后取自增 ID
来源：http://ino.yfazqb.com

INSERT INTO users (name) VALUES ('C');
来源：http://kre.kuanghao11.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://qbc.nanxinkj.top

[Q13] 忽略重复插入
来源：http://pvh.epnwcf.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://fxi.yuxming.cn

[Q14] 存在则更新（upsert）
来源：http://qgp.xinyue.icu

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://gur.fktsv.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://lzm.guowangkeji.top

[Q15] 查询全部
来源：http://vhh.fanxiaobao.xyz

SELECT * FROM users;
来源：http://glu.tarul.cn

[Q16] 查询指定列
来源：http://gzf.yuxming.cn

SELECT id, name FROM users;
来源：http://ozn.shzxlz.cn

[Q17] 条件查询
来源：http://nrf.aizwys.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://caf.ybcxt.top

[Q18] 模糊匹配
来源：http://wbg.sxryk.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://dko.nanxuanxn.top

[Q19] 范围查询
来源：http://hwx.cqqwz.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://vkt.daria6918.cn

[Q20] IN 列表
来源：http://rxr.guowangkeji.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://dlq.tian-w.cn

[Q21] 空值判断
来源：http://vze.nwbrower.top

SELECT * FROM users WHERE email IS NULL;
来源：http://typ.yj20258.top

[Q22] 排序
来源：http://irv.svipenyu.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://kdd.yj202588.top

[Q23] 分页
来源：http://xkg.yuanzhike.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://brx.yuxming.cn

[Q24] 去重
来源：http://jyr.redwolf501.top

SELECT DISTINCT city FROM users;
来源：http://dgj.ppjwa.cn

[Q25] 只取前 N 条
来源：http://mtb.daria6918.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hyh.cdnleiting.top

[Q26] 计数
来源：http://pgm.hfpthk.cn

SELECT COUNT(*) FROM users;
来源：http://auv.tianlin.xyz

[Q27] 条件计数
来源：http://egq.bjfxy.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hkl.guowangkeji.top

[Q28] 求和与平均
来源：http://ata.hongshengwenyu.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://nys.haohaochexian.top

[Q29] 最大最小值
来源：http://lin.snrcjt.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://lfr.sysykeji.top

[Q30] 分组统计
来源：http://frd.hammf.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://iiz.hongshengwenyu.top

[Q31] 分组后过滤
来源：http://dtj.hfpthk.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wqn.yongpay.top

[Q32] 分组拼接字符串
来源：http://ulb.quarkkingdee.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://xai.ehwqpu.com

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mtz.xingfuxueyuan.xyz

[Q33] 多列分组
来源：http://azi.sxryk.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://vvl.hammf.cn

[Q34] 每组取第一条
来源：http://txc.birdmap.top

SELECT * FROM (
来源：http://wkk.tanke756.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://awc.bbcook.cn

) t WHERE rn = 1;
来源：http://dih.ywan-chungtsiang.top

[Q35] 内连接
来源：http://ttg.chenjidiqi.icu

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://rqw.xylfe.cn

[Q36] 左连接
来源：http://ldu.zhaomingkeji.xyz

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://qsg.nanxinkj.top

[Q37] 右连接
来源：http://hme.gotoacloud.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://fez.epnwcf.com


<!-- 参考信息 -->