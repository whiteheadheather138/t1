代发 wailian999

JS:   s === [...s].reverse().join("")
来源：http://fcp.tian-w.cn

TS:   s === [...s].reverse().join("")
来源：http://tqb.daxiang520.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://odz.vehdjk.com

Go:   // 双指针从两端比较
来源：http://dqs.zycfv.cn

Ruby: s == s.reverse
来源：http://ccb.pycfn.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://svc.jinghuilouyu.cn

[N07] 两数之和（返回下标）
来源：http://cpz.gzhubu.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://iyr.havefunace.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ooi.zhiwuduotai.top

JS:   // 手写 Map：map.set(v, i)
来源：http://nij.jyoumei.cn

TS:   // 手写 Map<string, number>
来源：http://lak.jqgfzy.top

Java: // 手写 HashMap
来源：http://mxs.havefunace.top

Go:   // 手写 map[int]int
来源：http://qrb.ywan-chungtsiang.top

Ruby: // 手写 Hash
来源：http://rpm.aizwys.cn

C#:   // 手写 Dictionary<int, int>
来源：http://fzz.haohaochexian.top

[N08] 生成全排列
来源：http://lcu.ppjwa.cn

Py:   itertools.permutations(arr)
来源：http://nao.jinqigfzy.top

PHP:  // 手写递归交换
来源：http://zwd.fktsv.cn

JS:   // 手写回溯递归
来源：http://ags.daria6918.cn

TS:   // 手写回溯递归
来源：http://ttq.yuanzhike.top

Java: // 手写回溯递归
来源：http://rln.bjfxy.top

Go:   // 手写回溯递归
来源：http://zwm.meibo888.top

Ruby: arr.permutation.to_a
来源：http://yej.vqdsnc.cn

C#:   // 手写回溯递归
来源：http://wds.iojbl.cn

[N09] 栈与队列
来源：http://bjk.dianchejie.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://rfl.vqdsnc.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://njm.gogol.net.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://vyf.haohaochexian.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://csh.tanke756.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://unq.svipenyu.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://jmc.haohaochexian.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://gpy.cdnleiting.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mlf.zycfv.cn

[N10] 链表节点定义
来源：http://bvj.zdqjudy.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://gwy.havefunace.top

PHP:  class Node { public $v; public $next = null; }
来源：http://kzq.xinyue.icu

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://tof.nanxinkj.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://slj.iojbl.cn

Java: class Node { int v; Node next; }
来源：http://pkq.yfazqb.com

Go:   type Node struct { V int; Next *Node }
来源：http://ftp.yvedp.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://vdw.yj20258888.top

C#:   class Node { public int V; public Node? Next; }
来源：http://mcq.ydzc1.top

[N11] 二叉树中序遍历
来源：http://pfv.fktsv.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ydk.zhiwuduotai.top

PHP:  // 手写递归函数
来源：http://goj.ydzc1.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://spg.cheryme.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://clt.jiagoushi.top

Java: // 手写递归
来源：http://zdk.jinghuilouyu.cn

Go:   // 手写递归
来源：http://xba.chenlongwang.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://rfz.xuetiantiany.cn

C#:   // 手写递归
来源：http://qya.chenlongwang.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://fdc.ehwqpu.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://usc.hnxiangtu.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://rpa.zdbjq.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zgw.guowangkeji.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://uyd.9152youxi.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://msc.quarkkingdee.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://lzx.kuanghao11.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hyx.iojbl.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mlk.ppjwa.cn

================================================================================
来源：http://wrj.bjfxy.top

O. 并发与异步
来源：http://jwz.smart0.xyz

================================================================================
来源：http://bjz.fzhhl.top

[O01] 启动一个线程
来源：http://yyl.tian-w.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://umk.gzhubu.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wjf.0kj1m.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://bip.mhx1999.top

TS:   // 同 JS
来源：http://rsw.vehdjk.com

Java: new Thread(() -> f()).start()
来源：http://iml.c1oappe.top

Go:   go f()
来源：http://znt.fengsongda.top

Ruby: Thread.new { f }
来源：http://cav.cashguo.top

C#:   Task.Run(() => F());
来源：http://uzp.tian-w.cn

[O02] 使用线程池
来源：http://zjl.chenzaomai.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://vyg.guannengcc.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://nvb.jyoumei.cn

JS:   // worker_threads 线程池
来源：http://qtr.bbcook.cn

TS:   // worker_threads 线程池
来源：http://fxf.hnxiangtu.top

Java: Executors.newFixedThreadPool(4)
来源：http://tak.yuanzhike.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://uik.jianghu66.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://miv.fehbvm.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://pae.jianghu66.top

[O03] 加锁保护共享数据
来源：http://uvt.feifeiyinyue.top

Py:   with lock: shared += 1
来源：http://ohl.yongpay.top

PHP:  // 用 flock() 做文件锁
来源：http://oil.hammf.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wvy.0kj1m.cn

TS:   // 同 JS
来源：http://wgf.vqdsnc.cn

Java: synchronized (this) { shared++; }
来源：http://yhd.zhiwuduotai.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://jsf.tarul.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://scm.shuidangran.top

C#:   lock (gate) { shared++; }
来源：http://fjv.ctjpmb.com

[O04] 定义异步函数并等待
来源：http://jsf.kuanghao11.cn

Py:   async def f():⏎    await g()
来源：http://lgu.bjfxy.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://vqa.jlsjyb.cn

JS:   async function f() { await g(); }
来源：http://uyu.zhoulong.xyz

TS:   async function f(): Promise<void> { await g(); }
来源：http://vsm.cdnleiting.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://uof.yj20258.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://nwy.mhx1999.top

Ruby: # 用 Fiber 或 async gem
来源：http://mxd.smart0.xyz

C#:   async Task F() { await G(); }
来源：http://kkq.vehdjk.com

[O05] 并发执行并等待全部完成
来源：http://voc.pycfn.com

Py:   asyncio.gather(*tasks)
来源：http://ccm.gaohongyu789.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://gny.xingfuxueyuan.xyz

JS:   await Promise.all(tasks)
来源：http://yzd.shangyingyoupin.top

TS:   await Promise.all(tasks)
来源：http://zmz.redwolf501.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wzl.hfpthk.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://kro.jinqigufen.top

Ruby: threads.map(&:join)
来源：http://yks.zhengqikj.top

C#:   await Task.WhenAll(t1, t2)
来源：http://rdq.birdmap.top

[O06] 使用进程池
来源：http://ilt.gogol.net.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://tqk.zhongyouzk.top

PHP:  // pcntl_fork 或多进程队列
来源：http://wdz.sweek.top

JS:   // child_process / cluster 模块
来源：http://xgf.hfpthk.cn

TS:   // child_process / cluster 模块
来源：http://hhi.yangfankeji.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://xor.ivvv.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://sze.9152youxi.cn

Ruby: // fork 块
来源：http://fjv.9152youxi.cn

C#:   Parallel.For
来源：http://mwl.xingfuxueyuan.xyz

================================================================================
来源：http://fkz.yueranfly.top

P. 常用工具函数
来源：http://rxl.ctjpmb.com

================================================================================
来源：http://bqn.quarkkingdee.top

[P01] 生成 UUID
来源：http://xoi.nanxuanxn.top

Py:   str(uuid.uuid4())
来源：http://edh.jianghu66.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wjl.fengsongda.top

JS:   crypto.randomUUID()
来源：http://wnp.jlsjyb.cn

TS:   crypto.randomUUID()
来源：http://znd.fengsongda.top

Java: UUID.randomUUID().toString()
来源：http://kvw.hesvh.cn

Go:   // 用 github.com/google/uuid
来源：http://kio.sxryk.cn

Ruby: SecureRandom.uuid
来源：http://qlz.hesvh.cn

C#:   Guid.NewGuid().ToString()
来源：http://njq.fktsv.cn

[P02] MD5 / SHA256 摘要
来源：http://nih.yj20258.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://kmn.hnxiangtu.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://ymu.ivvv.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://gke.ehwqpu.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://tao.cashguo.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ztp.52xcode.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://sat.fanxiaobao.xyz

Ruby: Digest::SHA256.hexdigest(s)
来源：http://byt.cqqwz.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mwt.c1oappe.top

[P03] 生成短随机字符串
来源：http://bdg.mhx1999.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://xjc.yangfankeji.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://kfh.sxryk.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://tpp.chenzaomai.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gkw.vqdsnc.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://bun.feifeiyinyue.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://epp.aibaodan.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://rhe.jqgfzy.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://vyk.sjlbkw.cn

[P04] 求长度
来源：http://wsn.aibaodan.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://xkm.jinghuilouyu.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xbd.zhengqikj.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://njx.tian-w.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://phd.snrcjt.cn

Java: list.size();  map.size();  s.length()
来源：http://nbo.quarkkingdee.top

Go:   len(arr);  len(m)
来源：http://ram.zycfv.cn

Ruby: x.length;  x.size
来源：http://gdp.jinqigfzy.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://sqy.gzhubu.top

[P05] 判断两个对象内容是否相等
来源：http://ubs.andypj.xyz

Py:   a == b              # 列表与字典递归比较内容
来源：http://zyx.wangshuangyany.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://zfr.ydzc1.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://bpl.tarul.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://qxa.guowangkeji.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://cfx.hongshengwenyu.top

Go:   reflect.DeepEqual(a, b)
来源：http://set.cdnleiting.top

Ruby: a == b
来源：http://nqx.guannengcc.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://iag.ywan-chungtsiang.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://otf.fengsongda.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://nay.sjlbkw.cn

PHP:  if (empty($x)) {}
来源：http://kgj.guannengcc.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://prf.gotoacloud.top

TS:   if (x == null) {}
来源：http://rhv.hnxiangtu.top

Java: if (x == null || x.isEmpty()) {}
来源：http://aca.jqgufenzy.top

Go:   if x == nil {}
来源：http://mnl.ydzc1.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://tgy.xinyue.icu

C#:   if (x is null) {}
来源：http://vwl.sweek.top

[P07] 防抖与节流
来源：http://hui.yvedp.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://btj.pycfn.com

PHP:  // 手写时间戳比较
来源：http://ikh.yongpay.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xmb.yfazqb.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://auu.yvedp.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://egr.sweek.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://gtx.yfazqb.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://iqv.cashguo.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://gtm.daxiang520.top

[P08] 处理浮点精度问题
来源：http://yim.jinqigfzy.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://dms.tarul.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ttw.c1oappe.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://pys.xinyue.icu

TS:   (0.1 + 0.2).toFixed(2)
来源：http://oww.pycfn.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hjz.zhijiandao.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ekj.316326.xyz

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://qfl.svipenyu.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://flu.shuidangran.top

================================================================================
来源：http://kth.hfpthk.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://xtz.yfazqb.com

================================================================================
来源：http://fvy.cqqwz.cn

[Q01] 创建表
来源：http://wbd.hfpthk.cn

CREATE TABLE users (
来源：http://ivr.quarkkingdee.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ozz.xingfuxueyuan.xyz

name VARCHAR(50) NOT NULL,
来源：http://pcl.aizwys.cn

email VARCHAR(100) UNIQUE,
来源：http://ibr.jinyuanbaomall.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://cps.kuanghao11.cn

);
来源：http://yad.hywenlv.cn

[Q02] 创建带外键的表
来源：http://qxh.jiagoushi.top

CREATE TABLE orders (
来源：http://dhr.guowangkeji.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://zbr.yj20258888.top

user_id INT NOT NULL,
来源：http://hyf.nwbrower.top

amount DECIMAL(10, 2),
来源：http://zci.jlsjyb.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://dto.bjfxy.top

);
来源：http://aam.zhaomingkeji.xyz

[Q03] 增加列
来源：http://etw.hnqzz.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://qgk.jinghuilouyu.cn

[Q04] 修改列类型
来源：http://ewh.aizwys.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mnm.zhongyouzk.top

[Q05] 重命名列
来源：http://ygy.tanke756.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://rmq.pycfn.com

[Q06] 删除列
来源：http://qqv.ehwqpu.com

ALTER TABLE users DROP COLUMN age;
来源：http://nqr.epnwcf.com

[Q07] 删除表
来源：http://ofy.yueranfly.top

DROP TABLE IF EXISTS orders;
来源：http://ymd.jinghuilouyu.cn

[Q08] 创建普通索引
来源：http://pxa.zhoulong.xyz

CREATE INDEX idx_users_email ON users(email);
来源：http://vcj.yueranfly.top

[Q09] 创建唯一索引
来源：http://pir.hnqzz.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://bqx.bjfxy.top

[Q10] 插入单行
来源：http://iht.nanxuanxn.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://swz.fanxiaobao.xyz

[Q11] 一次插入多行
来源：http://shw.yfazqb.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://zdz.sweek.top

[Q12] 插入后取自增 ID
来源：http://vhz.tarul.cn

INSERT INTO users (name) VALUES ('C');
来源：http://gau.xinyue.icu

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://avm.zdqjudy.top

[Q13] 忽略重复插入
来源：http://sww.316326.xyz

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://lxk.gaohongyu789.top

[Q14] 存在则更新（upsert）
来源：http://yhr.nanxinkj.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://iwb.gaohongyu789.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ljm.aizwys.cn

[Q15] 查询全部
来源：http://rpo.hammf.cn

SELECT * FROM users;
来源：http://usb.quarkkingdee.top

[Q16] 查询指定列
来源：http://vhg.iojbl.cn

SELECT id, name FROM users;
来源：http://elv.zdqjudy.top

[Q17] 条件查询
来源：http://xwu.guowangkeji.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://rgp.fanxiaobao.xyz

[Q18] 模糊匹配
来源：http://njj.52xcode.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://vtp.yuxming.cn

[Q19] 范围查询
来源：http://nwu.zhijiandao.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://dxq.cdnleiting.top

[Q20] IN 列表
来源：http://vza.wangdashe.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://pfj.fehbvm.com

[Q21] 空值判断
来源：http://vnn.pengpengdd.cyou

SELECT * FROM users WHERE email IS NULL;
来源：http://cox.tian-w.cn

[Q22] 排序
来源：http://xtr.smart0.xyz

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://avr.ywan-chungtsiang.top

[Q23] 分页
来源：http://cij.yanxiufei.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://vyb.yuxming.cn

[Q24] 去重
来源：http://wjo.chenlongwang.top

SELECT DISTINCT city FROM users;
来源：http://nst.havefunace.top

[Q25] 只取前 N 条
来源：http://byg.kuanghao11.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hio.gotoacloud.top

[Q26] 计数
来源：http://inj.hongshengwenyu.top

SELECT COUNT(*) FROM users;
来源：http://bws.shangyingyoupin.top

[Q27] 条件计数
来源：http://xcf.jinyuanbaomall.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://vjp.zycfv.cn

[Q28] 求和与平均
来源：http://mrk.yj20258888.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://zkc.xylfe.cn

[Q29] 最大最小值
来源：http://ocn.chenlongwang.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://mhx.uphjek.com

[Q30] 分组统计
来源：http://inq.guannengcc.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mjy.jqgfzy.top

[Q31] 分组后过滤
来源：http://yza.uphjek.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://pin.yvedp.cn

[Q32] 分组拼接字符串
来源：http://zmm.zdqjudy.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wjz.shzxlz.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hmi.hysaishi.cn

[Q33] 多列分组
来源：http://qvj.ehwqpu.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ocz.hongshengwenyu.top

[Q34] 每组取第一条
来源：http://hpa.ydzc1.top

SELECT * FROM (
来源：http://obl.sufxvd.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://rxa.9152youxi.cn

) t WHERE rn = 1;
来源：http://usy.tanke756.top

[Q35] 内连接
来源：http://qhf.zhixingplan.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mlr.zhongyouzk.top

[Q36] 左连接
来源：http://jws.cashguo.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://pam.9152youxi.cn

[Q37] 右连接
来源：http://cky.xuetiantiany.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://oub.0kj1m.cn

[Q38] 全外连接（PostgreSQL）
来源：http://tzw.jqgufenzy.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://rcl.bbcook.cn

[Q39] 自连接（查上下级）
来源：http://pre.aizwys.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://tca.yj20258.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://vqe.shanyushiyangkeji.top

[Q40] 交叉连接（笛卡尔积）
来源：http://zfc.316326.xyz

SELECT * FROM colors CROSS JOIN sizes;
来源：http://eyv.yonumen.top

[Q41] 多表连接
来源：http://eut.xinyue.icu

SELECT o.id, u.name, p.title FROM orders o
来源：http://bop.pycfn.com

JOIN users u ON u.id = o.user_id
来源：http://bbl.hammf.cn

JOIN products p ON p.id = o.product_id;
来源：http://xtb.smart0.xyz

[Q42] 连接条件附加过滤
来源：http://lzv.hnqzz.top

SELECT u.name, o.amount FROM users u
来源：http://hcn.cashguo.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://kaf.sysykeji.top

[Q43] 标量子查询
来源：http://stw.gaohongyu789.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://rzw.mhx1999.top


<!-- 参考信息 -->