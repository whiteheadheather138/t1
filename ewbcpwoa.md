代发 wailian999

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hjq.smart0.xyz

[N10] 链表节点定义
来源：http://plv.kuanghao11.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://tki.cqqwz.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://khj.ivvv.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://kit.sxryk.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://iwl.yj20258.top

Java: class Node { int v; Node next; }
来源：http://ltt.pycfn.com

Go:   type Node struct { V int; Next *Node }
来源：http://hru.9152youxi.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://lio.fzhhl.top

C#:   class Node { public int V; public Node? Next; }
来源：http://oyv.meibo888.top

[N11] 二叉树中序遍历
来源：http://vxb.yj20258888.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://vpi.cdnleiting.top

PHP:  // 手写递归函数
来源：http://dbr.jinyuanbaomall.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yhn.ydjk.org.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yvs.cheryme.top

Java: // 手写递归
来源：http://sgi.nanxinkj.top

Go:   // 手写递归
来源：http://nff.jqgfzy.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://cbr.tian-w.cn

C#:   // 手写递归
来源：http://fqe.vqdsnc.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://qoa.uphjek.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://lcy.ppjwa.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://tli.andypj.xyz

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gqo.sxryk.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nvv.snrcjt.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://prk.shanyushiyangtech.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://psf.yj20258.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://yqz.nanxinkj.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://vme.sufxvd.cn

================================================================================
来源：http://loe.chenzaomai.com

O. 并发与异步
来源：http://vax.tarul.cn

================================================================================
来源：http://sys.zhijiandao.cn

[O01] 启动一个线程
来源：http://jyx.yueranfly.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://qxe.jqgufenzy.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://yxk.feifeiyinyue.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://fut.mhx1999.top

TS:   // 同 JS
来源：http://zha.snrcjt.cn

Java: new Thread(() -> f()).start()
来源：http://hsu.ybcxt.top

Go:   go f()
来源：http://nax.tianlin.xyz

Ruby: Thread.new { f }
来源：http://ght.wangdashe.top

C#:   Task.Run(() => F());
来源：http://xsp.guowangkeji.top

[O02] 使用线程池
来源：http://muk.pycfn.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://kye.chenlongwang.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ltv.ywan-chungtsiang.top

JS:   // worker_threads 线程池
来源：http://vct.xinyue.icu

TS:   // worker_threads 线程池
来源：http://ieb.guannengcc.top

Java: Executors.newFixedThreadPool(4)
来源：http://usl.hnxiangtu.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ifs.vehdjk.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://esg.cucudq.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://dfv.epnwcf.com

[O03] 加锁保护共享数据
来源：http://abe.yuxming.cn

Py:   with lock: shared += 1
来源：http://uol.guowangkeji.top

PHP:  // 用 flock() 做文件锁
来源：http://gqi.vehdjk.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mos.zhengqikj.top

TS:   // 同 JS
来源：http://tfm.cheryme.top

Java: synchronized (this) { shared++; }
来源：http://ibh.uphjek.com

Go:   mu.Lock();  defer mu.Unlock()
来源：http://xnf.nwbrower.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://tli.zhengqikj.top

C#:   lock (gate) { shared++; }
来源：http://ear.gotoacloud.top

[O04] 定义异步函数并等待
来源：http://dgw.zdqjudy.top

Py:   async def f():⏎    await g()
来源：http://zxk.cdnleiting.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://oer.xuanzx.com

JS:   async function f() { await g(); }
来源：http://niv.chenjidiqi.icu

TS:   async function f(): Promise<void> { await g(); }
来源：http://vgm.ctjpmb.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wgj.sysykeji.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://zsm.cdnleiting.top

Ruby: # 用 Fiber 或 async gem
来源：http://ylz.havefunace.top

C#:   async Task F() { await G(); }
来源：http://byw.feifeiyinyue.top

[O05] 并发执行并等待全部完成
来源：http://wfk.zhiwuduotai.top

Py:   asyncio.gather(*tasks)
来源：http://txm.zdqjudy.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://oxk.yanxiufei.cn

JS:   await Promise.all(tasks)
来源：http://xjn.gaohongyu789.top

TS:   await Promise.all(tasks)
来源：http://whd.yj202588.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://uln.jinqigfzy.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://kik.pengpengdd.cyou

Ruby: threads.map(&:join)
来源：http://sjp.xziqi.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ujc.chenlongwang.top

[O06] 使用进程池
来源：http://blh.tianlin.xyz

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ugn.ivvv.top

PHP:  // pcntl_fork 或多进程队列
来源：http://pkf.sweek.top

JS:   // child_process / cluster 模块
来源：http://tdw.yvedp.cn

TS:   // child_process / cluster 模块
来源：http://pxo.uphjek.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hdz.jiagoushi.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://qod.aibaodan.cn

Ruby: // fork 块
来源：http://oio.zhoulong.xyz

C#:   Parallel.For
来源：http://ewb.jyoumei.cn

================================================================================
来源：http://ssx.gaohongyu789.top

P. 常用工具函数
来源：http://ybt.yfazqb.com

================================================================================
来源：http://xzt.tian-w.cn

[P01] 生成 UUID
来源：http://giu.0kj1m.cn

Py:   str(uuid.uuid4())
来源：http://smq.yanxiufei.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://pcd.yongpay.top

JS:   crypto.randomUUID()
来源：http://avm.shuidangran.top

TS:   crypto.randomUUID()
来源：http://ibf.jinyuanbaomall.cn

Java: UUID.randomUUID().toString()
来源：http://miu.jqgfzy.top

Go:   // 用 github.com/google/uuid
来源：http://kni.hysaishi.cn

Ruby: SecureRandom.uuid
来源：http://ugf.smart0.xyz

C#:   Guid.NewGuid().ToString()
来源：http://qac.xuetiantiany.cn

[P02] MD5 / SHA256 摘要
来源：http://dsy.kuanghao11.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wdy.ydzc1.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://zcg.shanyushiyangkeji.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://dyy.hongshengwenyu.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://whh.mhx1999.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://cdb.fengsongda.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hfz.yj202588.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://pva.vqdsnc.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://yte.meibo888.top

[P03] 生成短随机字符串
来源：http://twf.fanxiaobao.xyz

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ozt.52xcode.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://qha.bbcook.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ntz.fengsongda.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ogi.sufxvd.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://akk.birdmap.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ppe.nanxinkj.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://ikj.zhiwuduotai.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mlh.smart0.xyz

[P04] 求长度
来源：http://qyf.zhixingplan.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://qgp.hammf.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://chw.aizwys.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://owl.shzxlz.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://pgt.ctjpmb.com

Java: list.size();  map.size();  s.length()
来源：http://zsl.fehbvm.com

Go:   len(arr);  len(m)
来源：http://chk.cheryme.top

Ruby: x.length;  x.size
来源：http://fzn.bjfxy.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://zrt.wangshuangyany.cn

[P05] 判断两个对象内容是否相等
来源：http://dqp.hcnkem.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://ucc.jinqigufen.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://gut.nanxinkj.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://vnb.cashguo.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://tlx.jinghuilouyu.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://atb.chenjidiqi.icu

Go:   reflect.DeepEqual(a, b)
来源：http://zzb.ywan-chungtsiang.top

Ruby: a == b
来源：http://ehu.pycfn.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://agw.fehbvm.com

[P06] 综合判空（null / 空串 / 空集合）
来源：http://lqa.jqgfzy.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://dfz.ydjk.org.cn

PHP:  if (empty($x)) {}
来源：http://bnx.guowangkeji.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://pbw.jlsjyb.cn

TS:   if (x == null) {}
来源：http://vtm.0kj1m.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ixi.hammf.cn

Go:   if x == nil {}
来源：http://zek.xziqi.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wsl.ywan-chungtsiang.top

C#:   if (x is null) {}
来源：http://gyc.fanxiaobao.xyz

[P07] 防抖与节流
来源：http://opn.gogol.net.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://vqm.meibo888.top

PHP:  // 手写时间戳比较
来源：http://sbc.nanxinkj.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://afj.jiagoushi.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://chw.havefunace.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://phd.yonumen.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://bhh.hesvh.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ini.xylfe.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://jqa.svipenyu.cn

[P08] 处理浮点精度问题
来源：http://mvg.jinyuanbaomall.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ptc.mhx1999.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://nxd.xziqi.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://iny.xingfuxueyuan.xyz

TS:   (0.1 + 0.2).toFixed(2)
来源：http://cwj.snrcjt.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://zdv.svipenyu.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ijc.vqdsnc.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://lyn.cdnleiting.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://tao.meibo888.top

================================================================================
来源：http://qsj.zycfv.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://uxf.gotoacloud.top

================================================================================
来源：http://isz.zdbjq.cn

[Q01] 创建表
来源：http://qhc.9152youxi.cn

CREATE TABLE users (
来源：http://tau.andypj.xyz

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://gml.9152youxi.cn

name VARCHAR(50) NOT NULL,
来源：http://hzx.wangdashe.top

email VARCHAR(100) UNIQUE,
来源：http://zhw.zhixingplan.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ups.jlsjyb.cn

);
来源：http://lie.cdnleiting.top

[Q02] 创建带外键的表
来源：http://aft.tanke756.top

CREATE TABLE orders (
来源：http://uml.tanke756.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://rzb.zycfv.cn

user_id INT NOT NULL,
来源：http://zyw.zdbjq.cn

amount DECIMAL(10, 2),
来源：http://neo.fanxiaobao.xyz

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://loo.0kj1m.cn

);
来源：http://iof.hnqzz.top

[Q03] 增加列
来源：http://qsr.9152youxi.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://xno.feifeiyinyue.top

[Q04] 修改列类型
来源：http://zic.zhixingplan.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://buo.cqqwz.cn

[Q05] 重命名列
来源：http://ujs.nwbrower.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://akp.shangyingyoupin.top

[Q06] 删除列
来源：http://czb.hnqzz.top

ALTER TABLE users DROP COLUMN age;
来源：http://jip.yonumen.top

[Q07] 删除表
来源：http://tjp.fehbvm.com

DROP TABLE IF EXISTS orders;
来源：http://xgk.zhaomingkeji.xyz

[Q08] 创建普通索引
来源：http://jtz.52xcode.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://jld.fktsv.cn

[Q09] 创建唯一索引
来源：http://jah.shuidangran.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ucd.tianlin.xyz

[Q10] 插入单行
来源：http://ymk.ydjk.org.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://qly.tarul.cn

[Q11] 一次插入多行
来源：http://crd.yanxiufei.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://pjt.andypj.xyz

[Q12] 插入后取自增 ID
来源：http://wfb.ivvv.top

INSERT INTO users (name) VALUES ('C');
来源：http://ivz.zhaomingkeji.xyz

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ogf.zdbjq.cn

[Q13] 忽略重复插入
来源：http://dbl.smart0.xyz

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://xbd.yuanzhike.top

[Q14] 存在则更新（upsert）
来源：http://wsk.zhengqikj.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://dix.vqdsnc.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://otp.guannengcc.top

[Q15] 查询全部
来源：http://mbx.chenjidiqi.icu

SELECT * FROM users;
来源：http://uso.aizwys.cn

[Q16] 查询指定列
来源：http://qit.chenjidiqi.icu

SELECT id, name FROM users;
来源：http://pdm.zhijiandao.cn

[Q17] 条件查询
来源：http://gtd.jinqigufen.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://iys.svipenyu.cn

[Q18] 模糊匹配
来源：http://pqu.zhongyouzk.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://thh.shanyushiyangkeji.top

[Q19] 范围查询
来源：http://exs.shuidangran.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://olv.fzhhl.top

[Q20] IN 列表
来源：http://pqj.cdnleiting.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wnx.jyoumei.cn

[Q21] 空值判断
来源：http://gah.ywan-chungtsiang.top

SELECT * FROM users WHERE email IS NULL;
来源：http://ooe.pycfn.com

[Q22] 排序
来源：http://sst.9152youxi.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://fkf.daxiang520.top

[Q23] 分页
来源：http://rwh.yj20258888.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hfl.hammf.cn

[Q24] 去重
来源：http://djq.zhoulong.xyz

SELECT DISTINCT city FROM users;
来源：http://zyx.wangdashe.top

[Q25] 只取前 N 条
来源：http://inc.jiagoushi.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://zyg.hywenlv.cn

[Q26] 计数
来源：http://afy.aibaodan.cn

SELECT COUNT(*) FROM users;
来源：http://arx.vqdsnc.cn

[Q27] 条件计数
来源：http://vsz.svipenyu.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://rsg.snrcjt.cn

[Q28] 求和与平均
来源：http://zaa.hnqzz.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hte.birdmap.top

[Q29] 最大最小值
来源：http://kjn.yanxiufei.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://gzc.yueranfly.top

[Q30] 分组统计
来源：http://llh.hywenlv.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://lla.fktsv.cn

[Q31] 分组后过滤
来源：http://oiz.shanyushiyangtech.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hux.aizwys.cn

[Q32] 分组拼接字符串
来源：http://ppq.tarul.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://jfo.jinyuanbaomall.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://zhr.yj202588.top

[Q33] 多列分组
来源：http://chm.yangfankeji.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://qce.ehwqpu.com

[Q34] 每组取第一条
来源：http://fju.hysaishi.cn

SELECT * FROM (
来源：http://lou.ydjk.org.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://cqg.andypj.xyz

) t WHERE rn = 1;
来源：http://tzw.yuanzhike.top

[Q35] 内连接
来源：http://ehy.yuanzhike.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://jip.jianghu66.top

[Q36] 左连接
来源：http://lda.daxiang520.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://gbj.dashuyun.cn

[Q37] 右连接
来源：http://sdv.jqgufenzy.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://shz.snrcjt.cn

[Q38] 全外连接（PostgreSQL）
来源：http://anb.yj20258.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://yjh.quarkkingdee.top

[Q39] 自连接（查上下级）
来源：http://dpa.bbcook.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://psi.shzxlz.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://nka.chenzaomai.com

[Q40] 交叉连接（笛卡尔积）
来源：http://eoy.fengsongda.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ewn.cdnleiting.top

[Q41] 多表连接
来源：http://uyt.nwbrower.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://pvd.pengpengdd.cyou

JOIN users u ON u.id = o.user_id
来源：http://uud.xuanzx.com

JOIN products p ON p.id = o.product_id;
来源：http://nub.yj202588.top

[Q42] 连接条件附加过滤
来源：http://wyb.quarkkingdee.top

SELECT u.name, o.amount FROM users u
来源：http://ejz.wangdashe.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://lkr.pycfn.com

[Q43] 标量子查询
来源：http://ako.52xcode.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://svz.hcnkem.com

[Q44] IN 子查询
来源：http://lhc.hammf.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://eof.havefunace.top

[Q45] EXISTS 判断存在
来源：http://igd.9152youxi.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://yvm.ctjpmb.com

[Q46] NOT EXISTS 判断不存在
来源：http://iyh.yj20258888.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://glj.ywan-chungtsiang.top

[Q47] 与平均值比较
来源：http://hvu.xuanzx.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://omd.zhijiandao.cn

[Q48] CTE 公用表表达式
来源：http://uyj.chenzaomai.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ram.cdnleiting.top

SELECT * FROM t WHERE c > 5;
来源：http://qir.jqgfzy.top

[Q49] 更新单行
来源：http://atl.tianlin.xyz

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ugz.svipenyu.cn

[Q50] 批量更新
来源：http://osk.ivvv.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://zxe.fengsongda.top

[Q51] 用子查询更新
来源：http://mbv.xuanzx.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ach.pengpengdd.cyou

[Q52] 删除指定行
来源：http://qnj.daria6918.cn

DELETE FROM users WHERE id = 10;
来源：http://lvn.sxryk.cn

[Q53] 按条件删除
来源：http://mke.jinqigfzy.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://cos.hesvh.cn

[Q54] 清空表
来源：http://eud.yonumen.top

TRUNCATE TABLE logs;
来源：http://noc.hcnkem.com

[Q55] 排名（并列占位）
来源：http://noo.nanxuanxn.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://pbf.ydjk.org.cn

[Q56] 密集排名（并列不占位）
来源：http://wct.smart0.xyz

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://jwv.jinghuilouyu.cn

[Q57] 行号
来源：http://fqz.jyoumei.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://vnn.dashuyun.cn

[Q58] 累计求和
来源：http://zdw.yvedp.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://tlz.gaohongyu789.top

[Q59] 分组内累计
来源：http://vbj.sjlbkw.cn


<!-- 参考信息 -->