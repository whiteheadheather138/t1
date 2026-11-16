代发 wailian999

Java: // 手写回溯递归
来源：http://wcn.fehbvm.com

Go:   // 手写回溯递归
来源：http://nun.fehbvm.com

Ruby: arr.permutation.to_a
来源：http://enq.daria6918.cn

C#:   // 手写回溯递归
来源：http://igx.pengpengdd.cyou

[N09] 栈与队列
来源：http://sts.shuidangran.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://abt.jinyuanbaomall.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://xvy.ivvv.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://qtk.guowangkeji.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://saq.cashguo.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://kcu.ivvv.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://zmw.hcnkem.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ume.ywan-chungtsiang.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://bwb.cucudq.cn

[N10] 链表节点定义
来源：http://bww.shanyushiyangtech.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://jcn.tianlin.xyz

PHP:  class Node { public $v; public $next = null; }
来源：http://eyy.shzxlz.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ago.vehdjk.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://kal.smart0.xyz

Java: class Node { int v; Node next; }
来源：http://lyz.zhijiandao.cn

Go:   type Node struct { V int; Next *Node }
来源：http://aad.zhongyouzk.top

Ruby: Node = Struct.new(:v, :next)
来源：http://vkv.uphjek.com

C#:   class Node { public int V; public Node? Next; }
来源：http://tos.bjfxy.top

[N11] 二叉树中序遍历
来源：http://lal.fengsongda.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ohp.tianlin.xyz

PHP:  // 手写递归函数
来源：http://qwr.ybcxt.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://dag.feifeiyinyue.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fij.dashuyun.cn

Java: // 手写递归
来源：http://zpc.xziqi.cn

Go:   // 手写递归
来源：http://abi.sweek.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://vvr.bbcook.cn

C#:   // 手写递归
来源：http://uvy.zycfv.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hdi.cdnleiting.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://iaf.nanxuanxn.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ojb.sxryk.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://opj.zycfv.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tsf.quarkkingdee.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://dkk.tian-w.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hyq.yj202588.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://xpi.cdnleiting.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://lxf.ppjwa.cn

================================================================================
来源：http://zmd.fzhhl.top

O. 并发与异步
来源：http://xit.fzhhl.top

================================================================================
来源：http://qoq.ivvv.top

[O01] 启动一个线程
来源：http://zhu.nanxuanxn.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://cnr.zycfv.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://msq.fehbvm.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://uot.pycfn.com

TS:   // 同 JS
来源：http://sic.jinyuanbaomall.cn

Java: new Thread(() -> f()).start()
来源：http://mix.9152youxi.cn

Go:   go f()
来源：http://ewi.jiagoushi.top

Ruby: Thread.new { f }
来源：http://jxw.shuidangran.top

C#:   Task.Run(() => F());
来源：http://aub.zdbjq.cn

[O02] 使用线程池
来源：http://ltq.jqgufenzy.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://swp.chenjidiqi.icu

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://sya.aizwys.cn

JS:   // worker_threads 线程池
来源：http://svi.ctjpmb.com

TS:   // worker_threads 线程池
来源：http://pox.xinyue.icu

Java: Executors.newFixedThreadPool(4)
来源：http://mmq.cqqwz.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://rkh.ppjwa.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://xrv.ivvv.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ogx.316326.xyz

[O03] 加锁保护共享数据
来源：http://byq.havefunace.top

Py:   with lock: shared += 1
来源：http://thp.smart0.xyz

PHP:  // 用 flock() 做文件锁
来源：http://trf.chenlongwang.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://zmm.birdmap.top

TS:   // 同 JS
来源：http://yeb.xinyue.icu

Java: synchronized (this) { shared++; }
来源：http://oaw.gaohongyu789.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://olc.chenzaomai.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://luf.jinqigfzy.top

C#:   lock (gate) { shared++; }
来源：http://ubw.chenlongwang.top

[O04] 定义异步函数并等待
来源：http://rry.zhiwuduotai.top

Py:   async def f():⏎    await g()
来源：http://vzp.nwbrower.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hre.bjfxy.top

JS:   async function f() { await g(); }
来源：http://yrn.yongpay.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://dvh.gaohongyu789.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://byn.fzhhl.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://pkq.sxryk.cn

Ruby: # 用 Fiber 或 async gem
来源：http://azv.ywan-chungtsiang.top

C#:   async Task F() { await G(); }
来源：http://gcd.jiagoushi.top

[O05] 并发执行并等待全部完成
来源：http://dme.jinyuanbaomall.cn

Py:   asyncio.gather(*tasks)
来源：http://dmk.zdqjudy.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://glr.yuanzhike.top

JS:   await Promise.all(tasks)
来源：http://uqj.zdbjq.cn

TS:   await Promise.all(tasks)
来源：http://xnv.tian-w.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://qwa.jinqigfzy.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://gsa.feifeiyinyue.top

Ruby: threads.map(&:join)
来源：http://hdh.tarul.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://gml.fanxiaobao.xyz

[O06] 使用进程池
来源：http://kvk.hammf.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wow.uphjek.com

PHP:  // pcntl_fork 或多进程队列
来源：http://wmp.yuanzhike.top

JS:   // child_process / cluster 模块
来源：http://lya.tanke756.top

TS:   // child_process / cluster 模块
来源：http://kdu.0kj1m.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://dyu.jqgufenzy.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://nxc.jinghuilouyu.cn

Ruby: // fork 块
来源：http://tpi.bbcook.cn

C#:   Parallel.For
来源：http://rme.cashguo.top

================================================================================
来源：http://bvj.gotoacloud.top

P. 常用工具函数
来源：http://hbf.yfazqb.com

================================================================================
来源：http://eie.vehdjk.com

[P01] 生成 UUID
来源：http://bmw.jiagoushi.top

Py:   str(uuid.uuid4())
来源：http://dhz.daria6918.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ozu.cdnleiting.top

JS:   crypto.randomUUID()
来源：http://ctc.zhixingplan.top

TS:   crypto.randomUUID()
来源：http://lky.hammf.cn

Java: UUID.randomUUID().toString()
来源：http://tzc.guowangkeji.top

Go:   // 用 github.com/google/uuid
来源：http://rxh.yj202588.top

Ruby: SecureRandom.uuid
来源：http://vdx.hysaishi.cn

C#:   Guid.NewGuid().ToString()
来源：http://agi.nanxuanxn.top

[P02] MD5 / SHA256 摘要
来源：http://hec.chenlongwang.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://lao.hysaishi.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ixh.guannengcc.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://yfp.ehwqpu.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://bfd.mhx1999.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://pyh.ydzc1.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://jju.zhijiandao.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://buc.tanke756.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://won.fanxiaobao.xyz

[P03] 生成短随机字符串
来源：http://byn.xuanzx.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://fwf.yj20258.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://yge.smart0.xyz

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ddp.fengsongda.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ydz.havefunace.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ako.haohaochexian.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://jjz.yanxiufei.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://mad.meibo888.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://vwz.daxiang520.top

[P04] 求长度
来源：http://iqi.shanyushiyangkeji.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://poi.fzhhl.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ovq.fanxiaobao.xyz

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jot.gotoacloud.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ull.hongshengwenyu.top

Java: list.size();  map.size();  s.length()
来源：http://llk.andypj.xyz

Go:   len(arr);  len(m)
来源：http://lxm.zhaomingkeji.xyz

Ruby: x.length;  x.size
来源：http://qpc.shangyingyoupin.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://aue.zhengqikj.top

[P05] 判断两个对象内容是否相等
来源：http://tij.jinyuanbaomall.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://axp.gotoacloud.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://vwo.c1oappe.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://izq.quarkkingdee.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://otd.sjlbkw.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://snt.fehbvm.com

Go:   reflect.DeepEqual(a, b)
来源：http://ero.jqgfzy.top

Ruby: a == b
来源：http://neq.sweek.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://jdt.sweek.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://fkb.haohaochexian.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://fxs.ydjk.org.cn

PHP:  if (empty($x)) {}
来源：http://ual.fanxiaobao.xyz

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://xfx.vqdsnc.cn

TS:   if (x == null) {}
来源：http://ule.daxiang520.top

Java: if (x == null || x.isEmpty()) {}
来源：http://dti.shanyushiyangkeji.top

Go:   if x == nil {}
来源：http://qnp.fanxiaobao.xyz

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ied.xziqi.cn

C#:   if (x is null) {}
来源：http://agi.yanxiufei.cn

[P07] 防抖与节流
来源：http://mny.jyoumei.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://kcl.yj202588.top

PHP:  // 手写时间戳比较
来源：http://ifw.xinyue.icu

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fyx.tanke756.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ugv.hywenlv.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://lqf.dashuyun.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://dur.daxiang520.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://qcq.hnqzz.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://jzv.jyoumei.cn

[P08] 处理浮点精度问题
来源：http://abe.jiagoushi.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ytc.snrcjt.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ppx.tarul.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ibc.ctjpmb.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ypl.wangshuangyany.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ikz.hongshengwenyu.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://fdw.nanxuanxn.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://udc.ctjpmb.com

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://xbc.tian-w.cn

================================================================================
来源：http://yvx.chenjidiqi.icu

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://tnx.jinghuilouyu.cn

================================================================================
来源：http://uwr.yuxming.cn

[Q01] 创建表
来源：http://rjx.chenzaomai.com

CREATE TABLE users (
来源：http://ucn.hcnkem.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ayz.snrcjt.cn

name VARCHAR(50) NOT NULL,
来源：http://nyo.zhengqikj.top

email VARCHAR(100) UNIQUE,
来源：http://ejm.svipenyu.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://iap.aizwys.cn

);
来源：http://rcd.uphjek.com

[Q02] 创建带外键的表
来源：http://sih.fzhhl.top

CREATE TABLE orders (
来源：http://ytt.ehwqpu.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ktp.tanke756.top

user_id INT NOT NULL,
来源：http://zzj.jinqigufen.top

amount DECIMAL(10, 2),
来源：http://lxp.kuanghao11.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mem.tarul.cn

);
来源：http://cvb.nanxinkj.top

[Q03] 增加列
来源：http://pwb.ydjk.org.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://pxy.fktsv.cn

[Q04] 修改列类型
来源：http://fol.wangshuangyany.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://eoc.yanxiufei.cn

[Q05] 重命名列
来源：http://eju.smart0.xyz

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wbp.meibo888.top

[Q06] 删除列
来源：http://slg.fktsv.cn

ALTER TABLE users DROP COLUMN age;
来源：http://dpb.svipenyu.cn

[Q07] 删除表
来源：http://kix.hnqzz.top

DROP TABLE IF EXISTS orders;
来源：http://ncj.fktsv.cn

[Q08] 创建普通索引
来源：http://dua.zdqjudy.top

CREATE INDEX idx_users_email ON users(email);
来源：http://wsf.xylfe.cn

[Q09] 创建唯一索引
来源：http://vli.kuanghao11.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://fbj.jinqigfzy.top

[Q10] 插入单行
来源：http://qbm.fehbvm.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://lci.fehbvm.com

[Q11] 一次插入多行
来源：http://bwx.xuanzx.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://sfw.mhx1999.top

[Q12] 插入后取自增 ID
来源：http://nmc.jiagoushi.top

INSERT INTO users (name) VALUES ('C');
来源：http://wfg.hesvh.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://gpf.9152youxi.cn

[Q13] 忽略重复插入
来源：http://bgy.fktsv.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mug.cheryme.top

[Q14] 存在则更新（upsert）
来源：http://xro.yfazqb.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://kqb.aibaodan.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://dca.feifeiyinyue.top

[Q15] 查询全部
来源：http://gfn.jqgufenzy.top

SELECT * FROM users;
来源：http://pbz.sufxvd.cn

[Q16] 查询指定列
来源：http://usa.dianchejie.cn

SELECT id, name FROM users;
来源：http://zun.jianghu66.top

[Q17] 条件查询
来源：http://thu.52xcode.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://iit.cdnleiting.top

[Q18] 模糊匹配
来源：http://poj.gogol.net.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mhe.wangdashe.top

[Q19] 范围查询
来源：http://nrj.jianghu66.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://uwh.tianlin.xyz

[Q20] IN 列表
来源：http://emd.guannengcc.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://tjp.sysykeji.top

[Q21] 空值判断
来源：http://qto.fanxiaobao.xyz

SELECT * FROM users WHERE email IS NULL;
来源：http://gqx.hnxiangtu.top

[Q22] 排序
来源：http://mlk.yueranfly.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://qrc.yonumen.top

[Q23] 分页
来源：http://avf.tianlin.xyz

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://trx.chenjidiqi.icu

[Q24] 去重
来源：http://tap.guannengcc.top

SELECT DISTINCT city FROM users;
来源：http://bza.tian-w.cn

[Q25] 只取前 N 条
来源：http://qnx.yangfankeji.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://lrl.yangfankeji.com

[Q26] 计数
来源：http://kxn.tian-w.cn

SELECT COUNT(*) FROM users;
来源：http://wpk.ctjpmb.com

[Q27] 条件计数
来源：http://pxh.birdmap.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://edr.tian-w.cn

[Q28] 求和与平均
来源：http://rmy.316326.xyz

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://dcp.daxiang520.top

[Q29] 最大最小值
来源：http://rdq.uphjek.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://kiy.gogol.net.cn

[Q30] 分组统计
来源：http://jfe.ywan-chungtsiang.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://qgg.ehwqpu.com

[Q31] 分组后过滤
来源：http://txa.jianghu66.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://xhw.chenlongwang.top

[Q32] 分组拼接字符串
来源：http://jyz.gaohongyu789.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://zrd.zhixingplan.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mzt.c1oappe.top

[Q33] 多列分组
来源：http://tft.dashuyun.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ccu.guowangkeji.top

[Q34] 每组取第一条
来源：http://yjb.fengsongda.top

SELECT * FROM (
来源：http://lpg.jlsjyb.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wyt.nwbrower.top

) t WHERE rn = 1;
来源：http://mzw.nanxinkj.top

[Q35] 内连接
来源：http://tug.fzhhl.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://vrh.ehwqpu.com

[Q36] 左连接
来源：http://auo.gogol.net.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://fwn.tarul.cn

[Q37] 右连接
来源：http://izf.gaohongyu789.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://omk.shanyushiyangkeji.top

[Q38] 全外连接（PostgreSQL）
来源：http://aog.cdnleiting.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://kga.yj202588.top

[Q39] 自连接（查上下级）
来源：http://kgn.zycfv.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://aso.jinyuanbaomall.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://jhb.yueranfly.top

[Q40] 交叉连接（笛卡尔积）
来源：http://aln.dashuyun.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://jam.gogol.net.cn

[Q41] 多表连接
来源：http://mfq.yangfankeji.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://gpb.fktsv.cn

JOIN users u ON u.id = o.user_id
来源：http://rko.feifeiyinyue.top

JOIN products p ON p.id = o.product_id;
来源：http://xsy.chenlongwang.top

[Q42] 连接条件附加过滤
来源：http://npq.sxryk.cn

SELECT u.name, o.amount FROM users u
来源：http://sya.9152youxi.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://rsg.zhengqikj.top

[Q43] 标量子查询
来源：http://qlq.hcnkem.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mru.zhaomingkeji.xyz

[Q44] IN 子查询
来源：http://iqy.aibaodan.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://bwh.9152youxi.cn

[Q45] EXISTS 判断存在
来源：http://nvt.sjlbkw.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://upe.zhixingplan.top

[Q46] NOT EXISTS 判断不存在
来源：http://obk.ehwqpu.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://onx.redwolf501.top

[Q47] 与平均值比较
来源：http://wei.gzhubu.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ltj.tianlin.xyz

[Q48] CTE 公用表表达式
来源：http://fnf.guannengcc.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://jue.tarul.cn

SELECT * FROM t WHERE c > 5;
来源：http://fsi.zhengqikj.top

[Q49] 更新单行
来源：http://zfu.vqdsnc.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://aae.gotoacloud.top

[Q50] 批量更新
来源：http://dau.havefunace.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ltq.hnxiangtu.top

[Q51] 用子查询更新
来源：http://ytk.hywenlv.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://dna.gogol.net.cn

[Q52] 删除指定行
来源：http://qua.hysaishi.cn

DELETE FROM users WHERE id = 10;
来源：http://pwm.sufxvd.cn

[Q53] 按条件删除
来源：http://ooj.pengpengdd.cyou


<!-- 参考信息 -->