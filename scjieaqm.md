代发 wailian999

Go:   // 手写递归
来源：http://bwv.iojbl.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://por.hesvh.cn

C#:   // 手写递归
来源：http://tqq.sjlbkw.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://zce.yuanzhike.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ulv.wangshuangyany.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wkz.jqgfzy.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wat.yj202588.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mnx.guannengcc.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://pvo.redwolf501.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://psb.andypj.xyz

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://asl.fktsv.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://qzd.tanke756.top

================================================================================
来源：http://lgz.sysykeji.top

O. 并发与异步
来源：http://pej.yuanzhike.top

================================================================================
来源：http://aav.zhoulong.xyz

[O01] 启动一个线程
来源：http://dga.shuidangran.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://sod.hysaishi.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wsc.feifeiyinyue.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://zcw.quarkkingdee.top

TS:   // 同 JS
来源：http://dlg.havefunace.top

Java: new Thread(() -> f()).start()
来源：http://dji.hammf.cn

Go:   go f()
来源：http://hoc.yueranfly.top

Ruby: Thread.new { f }
来源：http://ziv.sweek.top

C#:   Task.Run(() => F());
来源：http://dco.aizwys.cn

[O02] 使用线程池
来源：http://umj.hnxiangtu.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://uqc.nanxuanxn.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://nxs.yfazqb.com

JS:   // worker_threads 线程池
来源：http://foi.wangdashe.top

TS:   // worker_threads 线程池
来源：http://rir.xziqi.cn

Java: Executors.newFixedThreadPool(4)
来源：http://fnh.meibo888.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://xcw.hfpthk.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://kzh.xuanzx.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://bvt.chenjidiqi.icu

[O03] 加锁保护共享数据
来源：http://jtk.0kj1m.cn

Py:   with lock: shared += 1
来源：http://ecz.yj20258888.top

PHP:  // 用 flock() 做文件锁
来源：http://mdf.zhaomingkeji.xyz

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://vjv.ivvv.top

TS:   // 同 JS
来源：http://hdl.chenlongwang.top

Java: synchronized (this) { shared++; }
来源：http://vzl.yj20258.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://kda.hnxiangtu.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://xxf.kuanghao11.cn

C#:   lock (gate) { shared++; }
来源：http://koy.guowangkeji.top

[O04] 定义异步函数并等待
来源：http://owh.fktsv.cn

Py:   async def f():⏎    await g()
来源：http://gjq.vqdsnc.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://vpc.smart0.xyz

JS:   async function f() { await g(); }
来源：http://hur.yangfankeji.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://ozx.havefunace.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://qtw.epnwcf.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://zay.epnwcf.com

Ruby: # 用 Fiber 或 async gem
来源：http://tnq.ybcxt.top

C#:   async Task F() { await G(); }
来源：http://qyt.dianchejie.cn

[O05] 并发执行并等待全部完成
来源：http://bkk.daxiang520.top

Py:   asyncio.gather(*tasks)
来源：http://fqb.jyoumei.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://cjr.fehbvm.com

JS:   await Promise.all(tasks)
来源：http://gwa.gotoacloud.top

TS:   await Promise.all(tasks)
来源：http://cqh.tianlin.xyz

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://rly.xinyue.icu

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://icy.ehwqpu.com

Ruby: threads.map(&:join)
来源：http://oux.cashguo.top

C#:   await Task.WhenAll(t1, t2)
来源：http://zwz.hysaishi.cn

[O06] 使用进程池
来源：http://mtc.vehdjk.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://nuy.chenjidiqi.icu

PHP:  // pcntl_fork 或多进程队列
来源：http://nvh.ehwqpu.com

JS:   // child_process / cluster 模块
来源：http://yan.zhijiandao.cn

TS:   // child_process / cluster 模块
来源：http://upm.chenzaomai.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://lzu.jinyuanbaomall.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://dzz.hongshengwenyu.top

Ruby: // fork 块
来源：http://tlf.ywan-chungtsiang.top

C#:   Parallel.For
来源：http://nkn.jianghu66.top

================================================================================
来源：http://zgp.shzxlz.cn

P. 常用工具函数
来源：http://rfl.hnxiangtu.top

================================================================================
来源：http://plk.daria6918.cn

[P01] 生成 UUID
来源：http://ezy.ivvv.top

Py:   str(uuid.uuid4())
来源：http://rxp.zdbjq.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wfw.zhijiandao.cn

JS:   crypto.randomUUID()
来源：http://hyt.0kj1m.cn

TS:   crypto.randomUUID()
来源：http://gtf.zdqjudy.top

Java: UUID.randomUUID().toString()
来源：http://ymx.zdbjq.cn

Go:   // 用 github.com/google/uuid
来源：http://syr.yj20258.top

Ruby: SecureRandom.uuid
来源：http://opx.ivvv.top

C#:   Guid.NewGuid().ToString()
来源：http://xwh.yanxiufei.cn

[P02] MD5 / SHA256 摘要
来源：http://rkk.fehbvm.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://jiz.wangdashe.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://emm.shanyushiyangtech.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://udv.redwolf501.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://bsh.chenzaomai.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ohe.jinqigfzy.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ayh.ehwqpu.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://pqe.chenlongwang.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://vrk.shanyushiyangtech.top

[P03] 生成短随机字符串
来源：http://vyu.sufxvd.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://tnx.hywenlv.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://yxv.hammf.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://dbf.pycfn.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xuh.gogol.net.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://zao.yj20258888.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://pcx.c1oappe.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://tjl.0kj1m.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://bsr.hammf.cn

[P04] 求长度
来源：http://mko.dianchejie.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ajp.tianlin.xyz

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://cty.havefunace.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dyu.feifeiyinyue.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://sis.shzxlz.cn

Java: list.size();  map.size();  s.length()
来源：http://mhg.aizwys.cn

Go:   len(arr);  len(m)
来源：http://cxj.zhaomingkeji.xyz

Ruby: x.length;  x.size
来源：http://eye.shanyushiyangtech.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://pby.sufxvd.cn

[P05] 判断两个对象内容是否相等
来源：http://eeq.fanxiaobao.xyz

Py:   a == b              # 列表与字典递归比较内容
来源：http://pkk.yonumen.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://idw.birdmap.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ngw.hammf.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ojo.ehwqpu.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://djj.shangyingyoupin.top

Go:   reflect.DeepEqual(a, b)
来源：http://lof.jinqigfzy.top

Ruby: a == b
来源：http://reb.zdbjq.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ccb.zhaomingkeji.xyz

[P06] 综合判空（null / 空串 / 空集合）
来源：http://rgs.iojbl.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://bdo.jyoumei.cn

PHP:  if (empty($x)) {}
来源：http://ciq.bbcook.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hhj.vehdjk.com

TS:   if (x == null) {}
来源：http://uvk.jqgufenzy.top

Java: if (x == null || x.isEmpty()) {}
来源：http://iop.smart0.xyz

Go:   if x == nil {}
来源：http://wle.redwolf501.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mdy.cdnleiting.top

C#:   if (x is null) {}
来源：http://tvs.meibo888.top

[P07] 防抖与节流
来源：http://wst.xuetiantiany.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://rse.daxiang520.top

PHP:  // 手写时间戳比较
来源：http://sdu.shangyingyoupin.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zjf.vehdjk.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ekh.ctjpmb.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ugs.havefunace.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ewl.tarul.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://gbn.hysaishi.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://efy.yfazqb.com

[P08] 处理浮点精度问题
来源：http://tug.pycfn.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://bpg.jqgfzy.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://cov.shanyushiyangkeji.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://dlg.nwbrower.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://lrw.hammf.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://yab.fzhhl.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://diy.shanyushiyangtech.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://uod.tian-w.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://alq.shanyushiyangtech.top

================================================================================
来源：http://fzd.fzhhl.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://kjc.epnwcf.com

================================================================================
来源：http://wqd.zhiwuduotai.top

[Q01] 创建表
来源：http://upf.nanxuanxn.top

CREATE TABLE users (
来源：http://mun.meibo888.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://vim.cqqwz.cn

name VARCHAR(50) NOT NULL,
来源：http://wuu.zdqjudy.top

email VARCHAR(100) UNIQUE,
来源：http://kqn.fzhhl.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wry.pycfn.com

);
来源：http://llh.zdbjq.cn

[Q02] 创建带外键的表
来源：http://xdz.aizwys.cn

CREATE TABLE orders (
来源：http://oiw.yuxming.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://nsj.shangyingyoupin.top

user_id INT NOT NULL,
来源：http://pkd.dianchejie.cn

amount DECIMAL(10, 2),
来源：http://tbj.xinyue.icu

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ihj.9152youxi.cn

);
来源：http://mve.jianghu66.top

[Q03] 增加列
来源：http://jad.ivvv.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mwx.hesvh.cn

[Q04] 修改列类型
来源：http://ocl.nanxuanxn.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://dmr.yfazqb.com

[Q05] 重命名列
来源：http://tfk.meibo888.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://yqk.vqdsnc.cn

[Q06] 删除列
来源：http://ian.kuanghao11.cn

ALTER TABLE users DROP COLUMN age;
来源：http://mus.shzxlz.cn

[Q07] 删除表
来源：http://nqx.jqgfzy.top

DROP TABLE IF EXISTS orders;
来源：http://kpp.yongpay.top

[Q08] 创建普通索引
来源：http://eli.0kj1m.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://zsy.hywenlv.cn

[Q09] 创建唯一索引
来源：http://yrl.fanxiaobao.xyz

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://fnq.zhijiandao.cn

[Q10] 插入单行
来源：http://syc.bbcook.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://yck.ppjwa.cn

[Q11] 一次插入多行
来源：http://gfr.zhongyouzk.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://gjy.jiagoushi.top

[Q12] 插入后取自增 ID
来源：http://odq.aibaodan.cn

INSERT INTO users (name) VALUES ('C');
来源：http://hqg.fengsongda.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hiy.meibo888.top

[Q13] 忽略重复插入
来源：http://nub.zhixingplan.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://xvv.aizwys.cn

[Q14] 存在则更新（upsert）
来源：http://pke.fanxiaobao.xyz

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://nua.0kj1m.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://bbx.dashuyun.cn

[Q15] 查询全部
来源：http://rgi.jinghuilouyu.cn

SELECT * FROM users;
来源：http://aym.yvedp.cn

[Q16] 查询指定列
来源：http://rxa.guowangkeji.top

SELECT id, name FROM users;
来源：http://omg.fehbvm.com

[Q17] 条件查询
来源：http://mrb.yueranfly.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ouv.cqqwz.cn

[Q18] 模糊匹配
来源：http://dpo.gotoacloud.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mrb.yangfankeji.com

[Q19] 范围查询
来源：http://srn.tanke756.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ixs.ctjpmb.com

[Q20] IN 列表
来源：http://lms.sjlbkw.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://jjx.sxryk.cn

[Q21] 空值判断
来源：http://dsz.xziqi.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://kjl.ydjk.org.cn

[Q22] 排序
来源：http://jwe.9152youxi.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://tgy.yangfankeji.com

[Q23] 分页
来源：http://yfs.cheryme.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://abe.zycfv.cn

[Q24] 去重
来源：http://rio.yanxiufei.cn

SELECT DISTINCT city FROM users;
来源：http://kwu.sjlbkw.cn

[Q25] 只取前 N 条
来源：http://fsd.epnwcf.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://qzj.ydjk.org.cn

[Q26] 计数
来源：http://gfb.zhijiandao.cn

SELECT COUNT(*) FROM users;
来源：http://wtp.chenjidiqi.icu

[Q27] 条件计数
来源：http://aqx.tianlin.xyz

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://nre.zhijiandao.cn

[Q28] 求和与平均
来源：http://xva.chenjidiqi.icu

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://yxt.hfpthk.cn

[Q29] 最大最小值
来源：http://mph.sjlbkw.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://gau.tianlin.xyz

[Q30] 分组统计
来源：http://zie.xuanzx.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://bbw.dashuyun.cn

[Q31] 分组后过滤
来源：http://ulb.aizwys.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://jgp.vehdjk.com

[Q32] 分组拼接字符串
来源：http://zkn.hnxiangtu.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ajr.pycfn.com

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://inz.svipenyu.cn

[Q33] 多列分组
来源：http://thw.pycfn.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://xok.ctjpmb.com

[Q34] 每组取第一条
来源：http://aon.shanyushiyangkeji.top

SELECT * FROM (
来源：http://mkz.yfazqb.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://bhz.tian-w.cn

) t WHERE rn = 1;
来源：http://sqy.fanxiaobao.xyz

[Q35] 内连接
来源：http://oju.jinghuilouyu.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://fos.ydzc1.top

[Q36] 左连接
来源：http://wnc.xingfuxueyuan.xyz

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://nja.fanxiaobao.xyz

[Q37] 右连接
来源：http://byn.fzhhl.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hfw.zhiwuduotai.top

[Q38] 全外连接（PostgreSQL）
来源：http://vse.pycfn.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://bvo.epnwcf.com

[Q39] 自连接（查上下级）
来源：http://zqu.cdnleiting.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://pvg.snrcjt.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://nhd.52xcode.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://rvv.snrcjt.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ume.xingfuxueyuan.xyz

[Q41] 多表连接
来源：http://rxw.cucudq.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://fsa.fengsongda.top

JOIN users u ON u.id = o.user_id
来源：http://jbp.nwbrower.top

JOIN products p ON p.id = o.product_id;
来源：http://fdk.jlsjyb.cn

[Q42] 连接条件附加过滤
来源：http://etf.guowangkeji.top

SELECT u.name, o.amount FROM users u
来源：http://smt.cheryme.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://arn.aizwys.cn

[Q43] 标量子查询
来源：http://cqn.shangyingyoupin.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ogz.birdmap.top

[Q44] IN 子查询
来源：http://bvd.shuidangran.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://asl.epnwcf.com

[Q45] EXISTS 判断存在
来源：http://pwd.hnxiangtu.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://teb.cheryme.top

[Q46] NOT EXISTS 判断不存在
来源：http://rwq.quarkkingdee.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ggu.mhx1999.top

[Q47] 与平均值比较
来源：http://wuz.birdmap.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://vqh.tarul.cn

[Q48] CTE 公用表表达式
来源：http://lwi.jinyuanbaomall.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wzy.tanke756.top

SELECT * FROM t WHERE c > 5;
来源：http://sgs.yj20258888.top

[Q49] 更新单行
来源：http://qqw.feifeiyinyue.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://lyi.ppjwa.cn

[Q50] 批量更新
来源：http://jro.yangfankeji.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://vwo.tarul.cn

[Q51] 用子查询更新
来源：http://afe.cucudq.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hhe.xuetiantiany.cn

[Q52] 删除指定行
来源：http://dhi.0kj1m.cn

DELETE FROM users WHERE id = 10;
来源：http://jel.jinqigufen.top

[Q53] 按条件删除
来源：http://hga.ywan-chungtsiang.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://fsz.tarul.cn

[Q54] 清空表
来源：http://nmu.ctjpmb.com

TRUNCATE TABLE logs;
来源：http://rvu.uphjek.com

[Q55] 排名（并列占位）
来源：http://kam.zhixingplan.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ooi.chenlongwang.top

[Q56] 密集排名（并列不占位）
来源：http://lka.zycfv.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://gqh.gzhubu.top

[Q57] 行号
来源：http://kov.redwolf501.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://xkb.mhx1999.top

[Q58] 累计求和
来源：http://yoc.yanxiufei.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://nah.cheryme.top

[Q59] 分组内累计
来源：http://lmh.jianghu66.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://vjl.hfpthk.cn

[Q60] 取上一行 / 下一行
来源：http://caf.pengpengdd.cyou

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ktw.yj20258.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://xdy.dianchejie.cn

[Q61] 移动平均
来源：http://dwc.cqqwz.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ucq.nanxinkj.top

[Q62] 分组占比
来源：http://pjm.redwolf501.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wly.chenjidiqi.icu

[Q63] 开启事务
来源：http://asw.mhx1999.top

START TRANSACTION;                -- 或 BEGIN
来源：http://xnz.tian-w.cn

[Q64] 提交事务
来源：http://wrs.xylfe.cn

COMMIT;
来源：http://nmi.hongshengwenyu.top

[Q65] 回滚事务
来源：http://xhn.sxryk.cn

ROLLBACK;
来源：http://zjm.yueranfly.top

[Q66] 行锁查询
来源：http://dla.sysykeji.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://fdx.fanxiaobao.xyz


<!-- 参考信息 -->