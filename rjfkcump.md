代发 wailian999

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://lue.kuanghao11.cn

[N10] 链表节点定义
来源：http://awj.vehdjk.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://fom.sweek.top

PHP:  class Node { public $v; public $next = null; }
来源：http://zwk.quarkkingdee.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://avr.hysaishi.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://gnj.svipenyu.cn

Java: class Node { int v; Node next; }
来源：http://scy.meibo888.top

Go:   type Node struct { V int; Next *Node }
来源：http://els.hcnkem.com

Ruby: Node = Struct.new(:v, :next)
来源：http://ank.aibaodan.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ith.yueranfly.top

[N11] 二叉树中序遍历
来源：http://eye.yuxming.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://tsi.xingfuxueyuan.xyz

PHP:  // 手写递归函数
来源：http://umj.xingfuxueyuan.xyz

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://brm.smart0.xyz

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bwx.aizwys.cn

Java: // 手写递归
来源：http://ohq.zhiwuduotai.top

Go:   // 手写递归
来源：http://swy.tarul.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ndu.ctjpmb.com

C#:   // 手写递归
来源：http://ett.dashuyun.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://gfa.dianchejie.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://uip.xinyue.icu

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://lrc.pengpengdd.cyou

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://byn.sysykeji.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://onk.yonumen.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://dzn.jqgufenzy.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://qet.316326.xyz

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://zux.wangshuangyany.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wqb.havefunace.top

================================================================================
来源：http://ost.yj202588.top

O. 并发与异步
来源：http://znq.zhiwuduotai.top

================================================================================
来源：http://tcy.nwbrower.top

[O01] 启动一个线程
来源：http://nor.chenjidiqi.icu

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ckn.epnwcf.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://tkq.dianchejie.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ufq.ppjwa.cn

TS:   // 同 JS
来源：http://iuq.ivvv.top

Java: new Thread(() -> f()).start()
来源：http://tcs.jyoumei.cn

Go:   go f()
来源：http://rcj.zhiwuduotai.top

Ruby: Thread.new { f }
来源：http://kdj.jinqigfzy.top

C#:   Task.Run(() => F());
来源：http://xtb.xuanzx.com

[O02] 使用线程池
来源：http://nhl.jlsjyb.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://pxo.zhengqikj.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://jrh.gaohongyu789.top

JS:   // worker_threads 线程池
来源：http://tba.sjlbkw.cn

TS:   // worker_threads 线程池
来源：http://qrd.ywan-chungtsiang.top

Java: Executors.newFixedThreadPool(4)
来源：http://zcn.iojbl.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://oce.tarul.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://qxw.ctjpmb.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://zbs.epnwcf.com

[O03] 加锁保护共享数据
来源：http://ppp.jinqigufen.top

Py:   with lock: shared += 1
来源：http://qyz.yanxiufei.cn

PHP:  // 用 flock() 做文件锁
来源：http://rsj.xuanzx.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://xcn.wangshuangyany.cn

TS:   // 同 JS
来源：http://pqw.0kj1m.cn

Java: synchronized (this) { shared++; }
来源：http://dqk.guowangkeji.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://zyy.daxiang520.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://auv.tanke756.top

C#:   lock (gate) { shared++; }
来源：http://sgp.yongpay.top

[O04] 定义异步函数并等待
来源：http://gwp.xuetiantiany.cn

Py:   async def f():⏎    await g()
来源：http://amq.cucudq.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://pez.ywan-chungtsiang.top

JS:   async function f() { await g(); }
来源：http://iqk.kuanghao11.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://jnv.jinqigufen.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mej.jinqigfzy.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hbx.ywan-chungtsiang.top

Ruby: # 用 Fiber 或 async gem
来源：http://qdo.pycfn.com

C#:   async Task F() { await G(); }
来源：http://giu.ybcxt.top

[O05] 并发执行并等待全部完成
来源：http://rmu.guowangkeji.top

Py:   asyncio.gather(*tasks)
来源：http://nyk.dashuyun.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://omm.xingfuxueyuan.xyz

JS:   await Promise.all(tasks)
来源：http://ero.xingfuxueyuan.xyz

TS:   await Promise.all(tasks)
来源：http://dvb.ppjwa.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://xbp.ctjpmb.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://nnz.yfazqb.com

Ruby: threads.map(&:join)
来源：http://vai.ydzc1.top

C#:   await Task.WhenAll(t1, t2)
来源：http://cbq.chenjidiqi.icu

[O06] 使用进程池
来源：http://wdy.ppjwa.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://rha.316326.xyz

PHP:  // pcntl_fork 或多进程队列
来源：http://rce.feifeiyinyue.top

JS:   // child_process / cluster 模块
来源：http://jha.yj20258.top

TS:   // child_process / cluster 模块
来源：http://noq.aizwys.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://jje.havefunace.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wwt.gzhubu.top

Ruby: // fork 块
来源：http://qcq.epnwcf.com

C#:   Parallel.For
来源：http://nnz.gaohongyu789.top

================================================================================
来源：http://hcd.haohaochexian.top

P. 常用工具函数
来源：http://trl.xuetiantiany.cn

================================================================================
来源：http://gpy.cqqwz.cn

[P01] 生成 UUID
来源：http://oxq.xingfuxueyuan.xyz

Py:   str(uuid.uuid4())
来源：http://xfy.zdqjudy.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://lue.uphjek.com

JS:   crypto.randomUUID()
来源：http://mud.kuanghao11.cn

TS:   crypto.randomUUID()
来源：http://jte.aizwys.cn

Java: UUID.randomUUID().toString()
来源：http://vjq.ivvv.top

Go:   // 用 github.com/google/uuid
来源：http://rdu.cashguo.top

Ruby: SecureRandom.uuid
来源：http://qev.bjfxy.top

C#:   Guid.NewGuid().ToString()
来源：http://xhk.pengpengdd.cyou

[P02] MD5 / SHA256 摘要
来源：http://zev.pengpengdd.cyou

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://bce.zhongyouzk.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://cqg.yuanzhike.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://qyt.ppjwa.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://lge.jyoumei.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wml.shzxlz.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://yuf.daxiang520.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ocd.shanyushiyangkeji.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hoq.yuxming.cn

[P03] 生成短随机字符串
来源：http://rpr.xingfuxueyuan.xyz

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://yza.xingfuxueyuan.xyz

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mks.tarul.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://uda.ivvv.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://plj.nanxinkj.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://fqx.jianghu66.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://jyd.yongpay.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://uwk.jiagoushi.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://fgi.ydzc1.top

[P04] 求长度
来源：http://rge.fzhhl.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://uxo.feifeiyinyue.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rlk.hammf.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qqg.sufxvd.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://pdu.xuetiantiany.cn

Java: list.size();  map.size();  s.length()
来源：http://amy.ywan-chungtsiang.top

Go:   len(arr);  len(m)
来源：http://iqt.pycfn.com

Ruby: x.length;  x.size
来源：http://cur.yj20258.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://csj.hammf.cn

[P05] 判断两个对象内容是否相等
来源：http://apf.zhengqikj.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://kpp.ydzc1.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wgw.yj20258888.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://bih.cqqwz.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://qye.chenlongwang.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mal.yfazqb.com

Go:   reflect.DeepEqual(a, b)
来源：http://vck.hcnkem.com

Ruby: a == b
来源：http://gpq.xziqi.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://znx.0kj1m.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://eaj.zhaomingkeji.xyz

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://sfz.xuanzx.com

PHP:  if (empty($x)) {}
来源：http://qmx.jinqigfzy.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://cie.xinyue.icu

TS:   if (x == null) {}
来源：http://mlh.mhx1999.top

Java: if (x == null || x.isEmpty()) {}
来源：http://laq.andypj.xyz

Go:   if x == nil {}
来源：http://zjw.jianghu66.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://vwg.jinqigfzy.top

C#:   if (x is null) {}
来源：http://lgc.yuxming.cn

[P07] 防抖与节流
来源：http://nyf.zhengqikj.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://xjj.sweek.top

PHP:  // 手写时间戳比较
来源：http://vsw.xinyue.icu

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://opt.daxiang520.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nbl.ppjwa.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://rdz.shangyingyoupin.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://uvk.nwbrower.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://ehj.hcnkem.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://zuf.bjfxy.top

[P08] 处理浮点精度问题
来源：http://iqw.uphjek.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ecw.dianchejie.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://qwf.fanxiaobao.xyz

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://gwx.yvedp.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mvi.nanxuanxn.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://eyi.bjfxy.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://vlv.yuxming.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://uqb.c1oappe.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://qvo.sweek.top

================================================================================
来源：http://dyd.svipenyu.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://dxl.ydjk.org.cn

================================================================================
来源：http://hir.bbcook.cn

[Q01] 创建表
来源：http://prw.yj20258888.top

CREATE TABLE users (
来源：http://btk.aibaodan.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://yjs.snrcjt.cn

name VARCHAR(50) NOT NULL,
来源：http://uwk.jinqigfzy.top

email VARCHAR(100) UNIQUE,
来源：http://tla.ywan-chungtsiang.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://cji.jqgfzy.top

);
来源：http://iwy.ybcxt.top

[Q02] 创建带外键的表
来源：http://ryn.zhiwuduotai.top

CREATE TABLE orders (
来源：http://qzr.feifeiyinyue.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://xyp.aibaodan.cn

user_id INT NOT NULL,
来源：http://ugq.yangfankeji.com

amount DECIMAL(10, 2),
来源：http://jgv.yj202588.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://idb.tian-w.cn

);
来源：http://esk.dianchejie.cn

[Q03] 增加列
来源：http://zim.andypj.xyz

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://xbv.zhengqikj.top

[Q04] 修改列类型
来源：http://bca.yuxming.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://jfk.sweek.top

[Q05] 重命名列
来源：http://pem.cashguo.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://fxq.c1oappe.top

[Q06] 删除列
来源：http://fat.dashuyun.cn

ALTER TABLE users DROP COLUMN age;
来源：http://cub.chenjidiqi.icu

[Q07] 删除表
来源：http://ffw.shanyushiyangkeji.top

DROP TABLE IF EXISTS orders;
来源：http://exu.fzhhl.top

[Q08] 创建普通索引
来源：http://yqi.ybcxt.top

CREATE INDEX idx_users_email ON users(email);
来源：http://fpz.shuidangran.top

[Q09] 创建唯一索引
来源：http://xsx.xziqi.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://sca.cucudq.cn

[Q10] 插入单行
来源：http://luo.uphjek.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://pvy.iojbl.cn

[Q11] 一次插入多行
来源：http://npn.chenjidiqi.icu

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ssk.zhaomingkeji.xyz

[Q12] 插入后取自增 ID
来源：http://rvf.kuanghao11.cn

INSERT INTO users (name) VALUES ('C');
来源：http://hzi.shanyushiyangtech.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://amd.yfazqb.com

[Q13] 忽略重复插入
来源：http://crv.hnqzz.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://dpr.ehwqpu.com

[Q14] 存在则更新（upsert）
来源：http://xnt.zhixingplan.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://pqt.hcnkem.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://uoc.mhx1999.top

[Q15] 查询全部
来源：http://rvg.daria6918.cn

SELECT * FROM users;
来源：http://ssa.ydjk.org.cn

[Q16] 查询指定列
来源：http://pgc.jinghuilouyu.cn

SELECT id, name FROM users;
来源：http://qnp.xziqi.cn

[Q17] 条件查询
来源：http://amx.tianlin.xyz

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://iph.hnqzz.top

[Q18] 模糊匹配
来源：http://tal.ivvv.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://tli.haohaochexian.top

[Q19] 范围查询
来源：http://evi.jinqigfzy.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://evl.xuanzx.com

[Q20] IN 列表
来源：http://yst.hammf.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://cvr.zdbjq.cn

[Q21] 空值判断
来源：http://cni.dianchejie.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://qce.zdbjq.cn

[Q22] 排序
来源：http://hrg.ivvv.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mix.redwolf501.top

[Q23] 分页
来源：http://koa.cheryme.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://yho.jlsjyb.cn

[Q24] 去重
来源：http://xtg.zycfv.cn

SELECT DISTINCT city FROM users;
来源：http://mdx.vehdjk.com

[Q25] 只取前 N 条
来源：http://rdb.ivvv.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ish.0kj1m.cn

[Q26] 计数
来源：http://doa.zhoulong.xyz

SELECT COUNT(*) FROM users;
来源：http://oyd.cashguo.top

[Q27] 条件计数
来源：http://rey.xingfuxueyuan.xyz

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://sfk.jqgfzy.top

[Q28] 求和与平均
来源：http://hln.nwbrower.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wpm.hesvh.cn

[Q29] 最大最小值
来源：http://dzc.jqgfzy.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://txr.hnxiangtu.top

[Q30] 分组统计
来源：http://zuk.shanyushiyangtech.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wtv.pengpengdd.cyou

[Q31] 分组后过滤
来源：http://tms.quarkkingdee.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://izi.fanxiaobao.xyz

[Q32] 分组拼接字符串
来源：http://woh.epnwcf.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://axd.pengpengdd.cyou

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ugs.epnwcf.com

[Q33] 多列分组
来源：http://xco.guannengcc.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://rfq.xylfe.cn

[Q34] 每组取第一条
来源：http://mys.cheryme.top

SELECT * FROM (
来源：http://rzk.xuanzx.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://rap.nanxuanxn.top

) t WHERE rn = 1;
来源：http://evi.sweek.top

[Q35] 内连接
来源：http://jel.vqdsnc.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://jzk.gogol.net.cn

[Q36] 左连接
来源：http://dnc.tarul.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://bqi.cqqwz.cn

[Q37] 右连接
来源：http://ukx.yj20258.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ela.shuidangran.top

[Q38] 全外连接（PostgreSQL）
来源：http://akt.zhongyouzk.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://snt.yangfankeji.com

[Q39] 自连接（查上下级）
来源：http://yds.yj20258888.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://knm.yj20258.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://efo.xuetiantiany.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://fmf.cqqwz.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ron.hammf.cn

[Q41] 多表连接
来源：http://kut.52xcode.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://rpe.ybcxt.top

JOIN users u ON u.id = o.user_id
来源：http://ihs.shangyingyoupin.top

JOIN products p ON p.id = o.product_id;
来源：http://ids.iojbl.cn

[Q42] 连接条件附加过滤
来源：http://coq.meibo888.top

SELECT u.name, o.amount FROM users u
来源：http://qkf.meibo888.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ohq.zhoulong.xyz

[Q43] 标量子查询
来源：http://hwi.zhiwuduotai.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://tfy.shanyushiyangtech.top

[Q44] IN 子查询
来源：http://bkg.zhiwuduotai.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mwy.ydjk.org.cn

[Q45] EXISTS 判断存在
来源：http://aaw.mhx1999.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vsr.quarkkingdee.top

[Q46] NOT EXISTS 判断不存在
来源：http://fnw.jinqigfzy.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kwd.aizwys.cn

[Q47] 与平均值比较
来源：http://qty.9152youxi.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wtd.yuxming.cn

[Q48] CTE 公用表表达式
来源：http://cul.shanyushiyangtech.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://aji.zhiwuduotai.top

SELECT * FROM t WHERE c > 5;
来源：http://jmp.gaohongyu789.top

[Q49] 更新单行
来源：http://txo.fktsv.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://kyj.fehbvm.com

[Q50] 批量更新
来源：http://cec.yonumen.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://rnh.yj20258888.top

[Q51] 用子查询更新
来源：http://tgz.havefunace.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://sib.dianchejie.cn

[Q52] 删除指定行
来源：http://spm.zhijiandao.cn

DELETE FROM users WHERE id = 10;
来源：http://pvd.jlsjyb.cn

[Q53] 按条件删除
来源：http://kwt.fktsv.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ptd.cdnleiting.top

[Q54] 清空表
来源：http://ttn.0kj1m.cn

TRUNCATE TABLE logs;
来源：http://jlp.yuanzhike.top

[Q55] 排名（并列占位）
来源：http://qkh.fengsongda.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://uld.iojbl.cn

[Q56] 密集排名（并列不占位）
来源：http://ztp.cheryme.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://gfw.sufxvd.cn

[Q57] 行号
来源：http://lwa.c1oappe.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://dib.cdnleiting.top

[Q58] 累计求和
来源：http://qje.shanyushiyangkeji.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://tkt.9152youxi.cn

[Q59] 分组内累计
来源：http://mtj.shuidangran.top


<!-- 参考信息 -->