代发 wailian999

Java: new Thread(() -> f()).start()
来源：http://qla.pycfn.com

Go:   go f()
来源：http://gdg.tanke756.top

Ruby: Thread.new { f }
来源：http://vnk.shuidangran.top

C#:   Task.Run(() => F());
来源：http://nbm.xuetiantiany.cn

[O02] 使用线程池
来源：http://vez.meibo888.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://tix.ywan-chungtsiang.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wns.xylfe.cn

JS:   // worker_threads 线程池
来源：http://cyi.hcnkem.com

TS:   // worker_threads 线程池
来源：http://byz.jinqigufen.top

Java: Executors.newFixedThreadPool(4)
来源：http://pqn.ydzc1.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://std.ybcxt.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://osx.xingfuxueyuan.xyz

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ami.ydzc1.top

[O03] 加锁保护共享数据
来源：http://wge.smart0.xyz

Py:   with lock: shared += 1
来源：http://wzn.ydjk.org.cn

PHP:  // 用 flock() 做文件锁
来源：http://ixw.tarul.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ggw.hongshengwenyu.top

TS:   // 同 JS
来源：http://jwx.cdnleiting.top

Java: synchronized (this) { shared++; }
来源：http://qqu.jinyuanbaomall.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://vmq.zhengqikj.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://ibe.birdmap.top

C#:   lock (gate) { shared++; }
来源：http://suo.aibaodan.cn

[O04] 定义异步函数并等待
来源：http://piq.gzhubu.top

Py:   async def f():⏎    await g()
来源：http://cew.uphjek.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://yie.hongshengwenyu.top

JS:   async function f() { await g(); }
来源：http://jbw.chenjidiqi.icu

TS:   async function f(): Promise<void> { await g(); }
来源：http://bxt.tian-w.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://bkt.316326.xyz

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ojj.zhengqikj.top

Ruby: # 用 Fiber 或 async gem
来源：http://cqk.zycfv.cn

C#:   async Task F() { await G(); }
来源：http://wrw.zycfv.cn

[O05] 并发执行并等待全部完成
来源：http://ell.gotoacloud.top

Py:   asyncio.gather(*tasks)
来源：http://atg.svipenyu.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ilg.xingfuxueyuan.xyz

JS:   await Promise.all(tasks)
来源：http://got.yangfankeji.com

TS:   await Promise.all(tasks)
来源：http://geg.zhongyouzk.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://dks.ydjk.org.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://aac.zhijiandao.cn

Ruby: threads.map(&:join)
来源：http://jev.zdqjudy.top

C#:   await Task.WhenAll(t1, t2)
来源：http://ecd.guowangkeji.top

[O06] 使用进程池
来源：http://owy.jqgfzy.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://quj.chenlongwang.top

PHP:  // pcntl_fork 或多进程队列
来源：http://itx.sweek.top

JS:   // child_process / cluster 模块
来源：http://ngk.gaohongyu789.top

TS:   // child_process / cluster 模块
来源：http://bnz.jyoumei.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://qfj.vqdsnc.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://zbu.yangfankeji.com

Ruby: // fork 块
来源：http://ywy.chenzaomai.com

C#:   Parallel.For
来源：http://yrj.fzhhl.top

================================================================================
来源：http://mxd.zycfv.cn

P. 常用工具函数
来源：http://bfc.yonumen.top

================================================================================
来源：http://feq.zhijiandao.cn

[P01] 生成 UUID
来源：http://gbi.gaohongyu789.top

Py:   str(uuid.uuid4())
来源：http://ubs.smart0.xyz

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://jvr.xuetiantiany.cn

JS:   crypto.randomUUID()
来源：http://plt.vehdjk.com

TS:   crypto.randomUUID()
来源：http://gnm.wangshuangyany.cn

Java: UUID.randomUUID().toString()
来源：http://yjj.hnqzz.top

Go:   // 用 github.com/google/uuid
来源：http://qxo.gaohongyu789.top

Ruby: SecureRandom.uuid
来源：http://iug.tarul.cn

C#:   Guid.NewGuid().ToString()
来源：http://prn.vqdsnc.cn

[P02] MD5 / SHA256 摘要
来源：http://wqc.hcnkem.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mnd.sxryk.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://mcy.wangshuangyany.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://gvv.bjfxy.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://qcc.ctjpmb.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://idb.ehwqpu.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://xdt.hnxiangtu.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://diz.pengpengdd.cyou

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://kvz.chenlongwang.top

[P03] 生成短随机字符串
来源：http://dkf.yfazqb.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://gkq.aizwys.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://cta.gzhubu.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jsm.andypj.xyz

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://msv.havefunace.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://tgy.xinyue.icu

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://doy.uphjek.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://hwa.ybcxt.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ytq.daria6918.cn

[P04] 求长度
来源：http://tbk.cheryme.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://nct.meibo888.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://uns.fktsv.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://oid.52xcode.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xdd.yangfankeji.com

Java: list.size();  map.size();  s.length()
来源：http://aiy.chenzaomai.com

Go:   len(arr);  len(m)
来源：http://psc.xuetiantiany.cn

Ruby: x.length;  x.size
来源：http://ugc.shanyushiyangtech.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://pss.zhiwuduotai.top

[P05] 判断两个对象内容是否相等
来源：http://dbc.uphjek.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://pxr.jianghu66.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://fvz.iojbl.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://squ.pycfn.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://dbc.chenlongwang.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://nba.jinyuanbaomall.cn

Go:   reflect.DeepEqual(a, b)
来源：http://fzd.sjlbkw.cn

Ruby: a == b
来源：http://dtn.hesvh.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://zjm.yfazqb.com

[P06] 综合判空（null / 空串 / 空集合）
来源：http://qbv.c1oappe.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://tug.chenlongwang.top

PHP:  if (empty($x)) {}
来源：http://vow.chenjidiqi.icu

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ond.xuetiantiany.cn

TS:   if (x == null) {}
来源：http://wyi.cashguo.top

Java: if (x == null || x.isEmpty()) {}
来源：http://yrr.dashuyun.cn

Go:   if x == nil {}
来源：http://sjh.nanxuanxn.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://dyp.xingfuxueyuan.xyz

C#:   if (x is null) {}
来源：http://msk.yuanzhike.top

[P07] 防抖与节流
来源：http://qcv.guowangkeji.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://cvd.fktsv.cn

PHP:  // 手写时间戳比较
来源：http://aka.zdqjudy.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xsk.xuanzx.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://giu.316326.xyz

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://vuf.xuetiantiany.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ljy.gogol.net.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://qhi.tarul.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://pim.cdnleiting.top

[P08] 处理浮点精度问题
来源：http://val.smart0.xyz

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://bcc.gzhubu.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://lka.cqqwz.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://pvc.pengpengdd.cyou

TS:   (0.1 + 0.2).toFixed(2)
来源：http://iel.jqgufenzy.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://qld.zdqjudy.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://jaz.c1oappe.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://pzm.hesvh.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://tws.jqgufenzy.top

================================================================================
来源：http://wft.havefunace.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://nml.xylfe.cn

================================================================================
来源：http://fxq.dashuyun.cn

[Q01] 创建表
来源：http://egg.dianchejie.cn

CREATE TABLE users (
来源：http://vuy.sxryk.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://bwp.aizwys.cn

name VARCHAR(50) NOT NULL,
来源：http://sft.yangfankeji.com

email VARCHAR(100) UNIQUE,
来源：http://hyu.jinyuanbaomall.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://bso.kuanghao11.cn

);
来源：http://mbg.zhijiandao.cn

[Q02] 创建带外键的表
来源：http://geu.sweek.top

CREATE TABLE orders (
来源：http://gsb.yonumen.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://sno.yongpay.top

user_id INT NOT NULL,
来源：http://eeb.vehdjk.com

amount DECIMAL(10, 2),
来源：http://zdb.yvedp.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://irq.cashguo.top

);
来源：http://svt.dianchejie.cn

[Q03] 增加列
来源：http://ifs.yanxiufei.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://vzf.9152youxi.cn

[Q04] 修改列类型
来源：http://qnt.jinghuilouyu.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://pzg.shangyingyoupin.top

[Q05] 重命名列
来源：http://mqx.yj20258.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://qpl.fanxiaobao.xyz

[Q06] 删除列
来源：http://fyw.shanyushiyangtech.top

ALTER TABLE users DROP COLUMN age;
来源：http://pam.yonumen.top

[Q07] 删除表
来源：http://jjx.zdqjudy.top

DROP TABLE IF EXISTS orders;
来源：http://egj.yuanzhike.top

[Q08] 创建普通索引
来源：http://djj.hnxiangtu.top

CREATE INDEX idx_users_email ON users(email);
来源：http://gfm.feifeiyinyue.top

[Q09] 创建唯一索引
来源：http://ssn.jinqigufen.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hzl.bjfxy.top

[Q10] 插入单行
来源：http://cbg.shangyingyoupin.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://kdl.ehwqpu.com

[Q11] 一次插入多行
来源：http://zdt.chenzaomai.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://abo.jyoumei.cn

[Q12] 插入后取自增 ID
来源：http://crs.pengpengdd.cyou

INSERT INTO users (name) VALUES ('C');
来源：http://ohj.yongpay.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://yci.ctjpmb.com

[Q13] 忽略重复插入
来源：http://oxx.zhoulong.xyz

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ruc.yueranfly.top

[Q14] 存在则更新（upsert）
来源：http://poe.yonumen.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://oju.fehbvm.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://bvb.iojbl.cn

[Q15] 查询全部
来源：http://bso.yanxiufei.cn

SELECT * FROM users;
来源：http://abb.vehdjk.com

[Q16] 查询指定列
来源：http://mrt.jqgfzy.top

SELECT id, name FROM users;
来源：http://kvd.hcnkem.com

[Q17] 条件查询
来源：http://lsn.0kj1m.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://asv.cheryme.top

[Q18] 模糊匹配
来源：http://tij.xuetiantiany.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://jxm.yueranfly.top

[Q19] 范围查询
来源：http://wap.jyoumei.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://jiq.fzhhl.top

[Q20] IN 列表
来源：http://wug.sufxvd.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://gik.snrcjt.cn

[Q21] 空值判断
来源：http://ggx.ydjk.org.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://tru.shanyushiyangkeji.top

[Q22] 排序
来源：http://dvz.0kj1m.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hks.haohaochexian.top

[Q23] 分页
来源：http://qpf.jinghuilouyu.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://xsh.tanke756.top

[Q24] 去重
来源：http://dmt.sxryk.cn

SELECT DISTINCT city FROM users;
来源：http://twa.xylfe.cn

[Q25] 只取前 N 条
来源：http://dwo.guowangkeji.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://lec.jinghuilouyu.cn

[Q26] 计数
来源：http://jbg.yangfankeji.com

SELECT COUNT(*) FROM users;
来源：http://sie.fktsv.cn

[Q27] 条件计数
来源：http://jpu.gzhubu.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://xzy.nanxinkj.top

[Q28] 求和与平均
来源：http://lhb.hnqzz.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ibe.dianchejie.cn

[Q29] 最大最小值
来源：http://dln.hysaishi.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://why.316326.xyz

[Q30] 分组统计
来源：http://fpt.haohaochexian.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://szw.ywan-chungtsiang.top

[Q31] 分组后过滤
来源：http://dzo.jinqigfzy.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://njw.chenjidiqi.icu

[Q32] 分组拼接字符串
来源：http://nba.guannengcc.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://trt.svipenyu.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://lno.fehbvm.com

[Q33] 多列分组
来源：http://mrb.sxryk.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://lqd.fanxiaobao.xyz

[Q34] 每组取第一条
来源：http://upn.zhengqikj.top

SELECT * FROM (
来源：http://zqx.xuanzx.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ukq.shanyushiyangtech.top

) t WHERE rn = 1;
来源：http://enx.jianghu66.top

[Q35] 内连接
来源：http://rnz.hnxiangtu.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://zkt.cqqwz.cn

[Q36] 左连接
来源：http://yuk.hnxiangtu.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://oam.meibo888.top

[Q37] 右连接
来源：http://rcr.xuetiantiany.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://jtg.feifeiyinyue.top

[Q38] 全外连接（PostgreSQL）
来源：http://lqw.jlsjyb.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://nxy.pycfn.com

[Q39] 自连接（查上下级）
来源：http://efn.gzhubu.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://ppn.0kj1m.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://izz.xylfe.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://cly.zhoulong.xyz

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ucp.daxiang520.top

[Q41] 多表连接
来源：http://xgr.yuanzhike.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://wld.feifeiyinyue.top

JOIN users u ON u.id = o.user_id
来源：http://nnv.ppjwa.cn

JOIN products p ON p.id = o.product_id;
来源：http://hdv.hysaishi.cn

[Q42] 连接条件附加过滤
来源：http://bky.cheryme.top

SELECT u.name, o.amount FROM users u
来源：http://jau.jianghu66.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://nwu.zhijiandao.cn

[Q43] 标量子查询
来源：http://bij.shangyingyoupin.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://asl.daxiang520.top

[Q44] IN 子查询
来源：http://lvr.ydjk.org.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://voq.fengsongda.top

[Q45] EXISTS 判断存在
来源：http://dfo.jqgufenzy.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://skt.ywan-chungtsiang.top

[Q46] NOT EXISTS 判断不存在
来源：http://dbt.daria6918.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ieh.hysaishi.cn

[Q47] 与平均值比较
来源：http://psc.zdbjq.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wik.cucudq.cn

[Q48] CTE 公用表表达式
来源：http://ifg.jqgfzy.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://nwb.sxryk.cn

SELECT * FROM t WHERE c > 5;
来源：http://mmo.bjfxy.top

[Q49] 更新单行
来源：http://xfm.hcnkem.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://kec.zhongyouzk.top

[Q50] 批量更新
来源：http://eet.fzhhl.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://bsf.dianchejie.cn

[Q51] 用子查询更新
来源：http://iyk.zhengqikj.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://pkl.cashguo.top

[Q52] 删除指定行
来源：http://pwn.jqgfzy.top

DELETE FROM users WHERE id = 10;
来源：http://jmx.yangfankeji.com

[Q53] 按条件删除
来源：http://ndy.hnxiangtu.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://kho.fehbvm.com

[Q54] 清空表
来源：http://hmd.shangyingyoupin.top

TRUNCATE TABLE logs;
来源：http://xyg.xuetiantiany.cn

[Q55] 排名（并列占位）
来源：http://xdm.zhaomingkeji.xyz

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ozn.tianlin.xyz

[Q56] 密集排名（并列不占位）
来源：http://hlm.uphjek.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://uhr.jiagoushi.top

[Q57] 行号
来源：http://ivc.yuxming.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://eck.cheryme.top

[Q58] 累计求和
来源：http://lgd.hfpthk.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://huk.xuetiantiany.cn

[Q59] 分组内累计
来源：http://yle.wangdashe.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ktj.jyoumei.cn

[Q60] 取上一行 / 下一行
来源：http://fdz.316326.xyz

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://nxc.yvedp.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://zmq.yvedp.cn

[Q61] 移动平均
来源：http://cgr.dianchejie.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://njf.zhixingplan.top

[Q62] 分组占比
来源：http://vhl.sjlbkw.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ovk.dashuyun.cn

[Q63] 开启事务
来源：http://qja.hnqzz.top

START TRANSACTION;                -- 或 BEGIN
来源：http://xta.guowangkeji.top

[Q64] 提交事务
来源：http://sdt.shzxlz.cn

COMMIT;
来源：http://sjs.xuetiantiany.cn

[Q65] 回滚事务
来源：http://ysq.xuanzx.com

ROLLBACK;
来源：http://vvl.aibaodan.cn

[Q66] 行锁查询
来源：http://pdb.jinghuilouyu.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://zum.yonumen.top

[Q67] 设置隔离级别
来源：http://qwv.shzxlz.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://stn.zhongyouzk.top

[Q68] 保存点
来源：http://rnk.hongshengwenyu.top

SAVEPOINT sp1;
来源：http://cwy.tian-w.cn

ROLLBACK TO sp1;
来源：http://twb.xinyue.icu

[Q69] 查看执行计划
来源：http://lpi.wangdashe.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://gvh.uphjek.com

[Q70] 更新统计信息
来源：http://zog.gotoacloud.top

ANALYZE TABLE users;
来源：http://fcl.hfpthk.cn

[Q71] 查看建表语句
来源：http://mln.shzxlz.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ytt.sysykeji.top

[Q72] 查看索引
来源：http://syf.ppjwa.cn

SHOW INDEX FROM users;
来源：http://rfz.havefunace.top

[Q73] 查看表状态
来源：http://mqy.chenjidiqi.icu

SHOW TABLE STATUS LIKE 'users';
来源：http://ghy.hysaishi.cn

[Q74] 强制使用索引
来源：http://wvl.jqgfzy.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hdj.fanxiaobao.xyz

[Q75] 日期格式化
来源：http://smr.chenjidiqi.icu

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://xxm.nanxinkj.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ute.chenzaomai.com


<!-- 参考信息 -->