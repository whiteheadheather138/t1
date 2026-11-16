代发 wailian999

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://pnv.nanxinkj.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://uzp.zdqjudy.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://bmx.hysaishi.cn

TS:   // 同 JS
来源：http://bqn.0kj1m.cn

Java: new Thread(() -> f()).start()
来源：http://dmb.pengpengdd.cyou

Go:   go f()
来源：http://smi.uphjek.com

Ruby: Thread.new { f }
来源：http://oep.hcnkem.com

C#:   Task.Run(() => F());
来源：http://taw.mhx1999.top

[O02] 使用线程池
来源：http://glu.tianlin.xyz

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://pzf.dashuyun.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://rbf.iojbl.cn

JS:   // worker_threads 线程池
来源：http://myx.iojbl.cn

TS:   // worker_threads 线程池
来源：http://jyy.sjlbkw.cn

Java: Executors.newFixedThreadPool(4)
来源：http://lpm.gotoacloud.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://jkq.cucudq.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://brc.fengsongda.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://lwr.hnxiangtu.top

[O03] 加锁保护共享数据
来源：http://hyl.mhx1999.top

Py:   with lock: shared += 1
来源：http://awd.yanxiufei.cn

PHP:  // 用 flock() 做文件锁
来源：http://cwd.zhengqikj.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://pas.jqgufenzy.top

TS:   // 同 JS
来源：http://swg.tanke756.top

Java: synchronized (this) { shared++; }
来源：http://wrv.jinghuilouyu.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://fvh.tarul.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://wsw.pengpengdd.cyou

C#:   lock (gate) { shared++; }
来源：http://fjs.jianghu66.top

[O04] 定义异步函数并等待
来源：http://wnb.fengsongda.top

Py:   async def f():⏎    await g()
来源：http://kdb.sweek.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://owl.sxryk.cn

JS:   async function f() { await g(); }
来源：http://lyo.c1oappe.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://jit.jiagoushi.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ice.cqqwz.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://axs.cashguo.top

Ruby: # 用 Fiber 或 async gem
来源：http://lox.tanke756.top

C#:   async Task F() { await G(); }
来源：http://rgp.316326.xyz

[O05] 并发执行并等待全部完成
来源：http://xzy.shzxlz.cn

Py:   asyncio.gather(*tasks)
来源：http://ref.xinyue.icu

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://egu.snrcjt.cn

JS:   await Promise.all(tasks)
来源：http://atb.birdmap.top

TS:   await Promise.all(tasks)
来源：http://hah.yangfankeji.com

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://vip.hysaishi.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://rei.fengsongda.top

Ruby: threads.map(&:join)
来源：http://azf.gzhubu.top

C#:   await Task.WhenAll(t1, t2)
来源：http://gjg.uphjek.com

[O06] 使用进程池
来源：http://vut.tian-w.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://fkp.hcnkem.com

PHP:  // pcntl_fork 或多进程队列
来源：http://xks.yuxming.cn

JS:   // child_process / cluster 模块
来源：http://kww.yvedp.cn

TS:   // child_process / cluster 模块
来源：http://kia.feifeiyinyue.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://dht.hfpthk.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://lcw.52xcode.cn

Ruby: // fork 块
来源：http://asd.316326.xyz

C#:   Parallel.For
来源：http://xwy.shangyingyoupin.top

================================================================================
来源：http://ask.cucudq.cn

P. 常用工具函数
来源：http://tiq.yangfankeji.com

================================================================================
来源：http://kzq.pycfn.com

[P01] 生成 UUID
来源：http://qan.kuanghao11.cn

Py:   str(uuid.uuid4())
来源：http://emp.zycfv.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://cjt.zhiwuduotai.top

JS:   crypto.randomUUID()
来源：http://pdk.daxiang520.top

TS:   crypto.randomUUID()
来源：http://mbx.jyoumei.cn

Java: UUID.randomUUID().toString()
来源：http://iak.hnxiangtu.top

Go:   // 用 github.com/google/uuid
来源：http://mse.havefunace.top

Ruby: SecureRandom.uuid
来源：http://tot.sysykeji.top

C#:   Guid.NewGuid().ToString()
来源：http://uas.snrcjt.cn

[P02] MD5 / SHA256 摘要
来源：http://lnp.chenzaomai.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://anp.tianlin.xyz

PHP:  hash("sha256", $s);  md5($s);
来源：http://srz.yonumen.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://qed.epnwcf.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://sxc.guowangkeji.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://twt.zhaomingkeji.xyz

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://xvm.fengsongda.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://jih.zhoulong.xyz

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://vlj.nwbrower.top

[P03] 生成短随机字符串
来源：http://zfg.sjlbkw.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://cvf.ppjwa.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hqw.sufxvd.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kby.nwbrower.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://evc.epnwcf.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://epk.uphjek.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://reg.0kj1m.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://rfo.ywan-chungtsiang.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://aps.xziqi.cn

[P04] 求长度
来源：http://exd.tian-w.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://tyb.jqgfzy.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hbq.gzhubu.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rzn.ppjwa.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://egi.sufxvd.cn

Java: list.size();  map.size();  s.length()
来源：http://tfq.fzhhl.top

Go:   len(arr);  len(m)
来源：http://etj.fanxiaobao.xyz

Ruby: x.length;  x.size
来源：http://adw.tian-w.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://dsv.nanxinkj.top

[P05] 判断两个对象内容是否相等
来源：http://epz.ehwqpu.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://uip.uphjek.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://igi.yuanzhike.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://rty.chenzaomai.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://sao.hammf.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://cla.yuanzhike.top

Go:   reflect.DeepEqual(a, b)
来源：http://oor.tanke756.top

Ruby: a == b
来源：http://pbv.daria6918.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://dqt.quarkkingdee.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wye.vehdjk.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://exh.tanke756.top

PHP:  if (empty($x)) {}
来源：http://ewz.yanxiufei.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ejf.jinqigufen.top

TS:   if (x == null) {}
来源：http://rdn.hnxiangtu.top

Java: if (x == null || x.isEmpty()) {}
来源：http://frc.ywan-chungtsiang.top

Go:   if x == nil {}
来源：http://pua.zhaomingkeji.xyz

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://pfv.tian-w.cn

C#:   if (x is null) {}
来源：http://nie.snrcjt.cn

[P07] 防抖与节流
来源：http://ewy.gogol.net.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://pwp.hesvh.cn

PHP:  // 手写时间戳比较
来源：http://yku.cucudq.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xce.xuanzx.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vrf.cucudq.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://dvn.yanxiufei.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://zwz.yongpay.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://ojo.guowangkeji.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://eco.fzhhl.top

[P08] 处理浮点精度问题
来源：http://mfk.ywan-chungtsiang.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wnc.bbcook.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://iqp.mhx1999.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://gxp.zhoulong.xyz

TS:   (0.1 + 0.2).toFixed(2)
来源：http://kgc.yanxiufei.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://cqo.yuxming.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://cey.aizwys.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://qkm.epnwcf.com

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://pyp.birdmap.top

================================================================================
来源：http://jrn.zhixingplan.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://rmv.zhijiandao.cn

================================================================================
来源：http://jac.sysykeji.top

[Q01] 创建表
来源：http://qsi.pengpengdd.cyou

CREATE TABLE users (
来源：http://bqx.hnxiangtu.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://gkl.yueranfly.top

name VARCHAR(50) NOT NULL,
来源：http://bal.gogol.net.cn

email VARCHAR(100) UNIQUE,
来源：http://yrn.meibo888.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blu.ywan-chungtsiang.top

);
来源：http://xtj.zhiwuduotai.top

[Q02] 创建带外键的表
来源：http://kik.chenzaomai.com

CREATE TABLE orders (
来源：http://prd.zhaomingkeji.xyz

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mtc.hnxiangtu.top

user_id INT NOT NULL,
来源：http://kkc.shzxlz.cn

amount DECIMAL(10, 2),
来源：http://llz.snrcjt.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://pln.uphjek.com

);
来源：http://rkr.iojbl.cn

[Q03] 增加列
来源：http://inp.cqqwz.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://vrn.hywenlv.cn

[Q04] 修改列类型
来源：http://bog.vehdjk.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://yij.cucudq.cn

[Q05] 重命名列
来源：http://asp.fanxiaobao.xyz

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://dhi.gotoacloud.top

[Q06] 删除列
来源：http://wwe.yfazqb.com

ALTER TABLE users DROP COLUMN age;
来源：http://xmz.hnqzz.top

[Q07] 删除表
来源：http://xdb.dashuyun.cn

DROP TABLE IF EXISTS orders;
来源：http://ncn.sysykeji.top

[Q08] 创建普通索引
来源：http://eov.xinyue.icu

CREATE INDEX idx_users_email ON users(email);
来源：http://kvs.ctjpmb.com

[Q09] 创建唯一索引
来源：http://iyn.zhaomingkeji.xyz

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://bmd.xingfuxueyuan.xyz

[Q10] 插入单行
来源：http://mqn.sxryk.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://tff.birdmap.top

[Q11] 一次插入多行
来源：http://vff.sysykeji.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://xmk.c1oappe.top

[Q12] 插入后取自增 ID
来源：http://cwu.havefunace.top

INSERT INTO users (name) VALUES ('C');
来源：http://woj.aizwys.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://zjj.hesvh.cn

[Q13] 忽略重复插入
来源：http://ofe.hcnkem.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ste.zhongyouzk.top

[Q14] 存在则更新（upsert）
来源：http://ism.jqgfzy.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://bsr.ppjwa.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://nnr.hcnkem.com

[Q15] 查询全部
来源：http://kvh.hesvh.cn

SELECT * FROM users;
来源：http://kop.shzxlz.cn

[Q16] 查询指定列
来源：http://xki.fehbvm.com

SELECT id, name FROM users;
来源：http://fot.cucudq.cn

[Q17] 条件查询
来源：http://oxr.shanyushiyangtech.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://isk.chenjidiqi.icu

[Q18] 模糊匹配
来源：http://iis.shanyushiyangtech.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://nji.cashguo.top

[Q19] 范围查询
来源：http://ana.cashguo.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wiy.jlsjyb.cn

[Q20] IN 列表
来源：http://mqe.gaohongyu789.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://oyi.nanxinkj.top

[Q21] 空值判断
来源：http://kbb.mhx1999.top

SELECT * FROM users WHERE email IS NULL;
来源：http://oqn.cucudq.cn

[Q22] 排序
来源：http://cyg.andypj.xyz

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://kce.epnwcf.com

[Q23] 分页
来源：http://huh.zycfv.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://jpj.316326.xyz

[Q24] 去重
来源：http://vpf.hnxiangtu.top

SELECT DISTINCT city FROM users;
来源：http://hkb.jyoumei.cn

[Q25] 只取前 N 条
来源：http://lwu.zhijiandao.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hny.cheryme.top

[Q26] 计数
来源：http://tlx.daria6918.cn

SELECT COUNT(*) FROM users;
来源：http://gtx.bjfxy.top

[Q27] 条件计数
来源：http://xqi.gzhubu.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://dcj.chenlongwang.top

[Q28] 求和与平均
来源：http://ttz.sjlbkw.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://him.nwbrower.top

[Q29] 最大最小值
来源：http://rqw.xylfe.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://wqn.zhixingplan.top

[Q30] 分组统计
来源：http://hnx.hnqzz.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://eji.vehdjk.com

[Q31] 分组后过滤
来源：http://bbr.yuanzhike.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://fbm.cqqwz.cn

[Q32] 分组拼接字符串
来源：http://wlo.smart0.xyz

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://fgb.gotoacloud.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://sqw.yueranfly.top

[Q33] 多列分组
来源：http://qgb.zdbjq.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://lym.ywan-chungtsiang.top

[Q34] 每组取第一条
来源：http://sik.sufxvd.cn

SELECT * FROM (
来源：http://tcq.ppjwa.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://vgm.svipenyu.cn

) t WHERE rn = 1;
来源：http://rsh.yonumen.top

[Q35] 内连接
来源：http://ugv.zycfv.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://xzq.guannengcc.top

[Q36] 左连接
来源：http://axg.0kj1m.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mff.svipenyu.cn

[Q37] 右连接
来源：http://hqn.hammf.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://kgg.ywan-chungtsiang.top

[Q38] 全外连接（PostgreSQL）
来源：http://fek.zhijiandao.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://brn.zhixingplan.top

[Q39] 自连接（查上下级）
来源：http://vbx.zhaomingkeji.xyz

SELECT e.name, m.name AS manager FROM employees e
来源：http://xvf.jqgufenzy.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://exs.zycfv.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://jxq.dashuyun.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://udf.wangdashe.top

[Q41] 多表连接
来源：http://jcw.wangshuangyany.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://bee.hysaishi.cn

JOIN users u ON u.id = o.user_id
来源：http://otq.zhiwuduotai.top

JOIN products p ON p.id = o.product_id;
来源：http://lfy.haohaochexian.top

[Q42] 连接条件附加过滤
来源：http://wbt.ehwqpu.com

SELECT u.name, o.amount FROM users u
来源：http://mha.cqqwz.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://kyy.yuxming.cn

[Q43] 标量子查询
来源：http://kna.meibo888.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mav.nwbrower.top

[Q44] IN 子查询
来源：http://jrc.smart0.xyz

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://vdb.redwolf501.top

[Q45] EXISTS 判断存在
来源：http://qwk.sufxvd.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rss.snrcjt.cn

[Q46] NOT EXISTS 判断不存在
来源：http://btn.jqgufenzy.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ovz.cqqwz.cn

[Q47] 与平均值比较
来源：http://wtq.daxiang520.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://uqo.guannengcc.top

[Q48] CTE 公用表表达式
来源：http://otd.pengpengdd.cyou

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://gbm.hesvh.cn

SELECT * FROM t WHERE c > 5;
来源：http://qqr.tanke756.top

[Q49] 更新单行
来源：http://puf.shanyushiyangkeji.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wzd.yonumen.top

[Q50] 批量更新
来源：http://jkb.fengsongda.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://kkp.chenjidiqi.icu

[Q51] 用子查询更新
来源：http://cdi.haohaochexian.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://jkz.vehdjk.com

[Q52] 删除指定行
来源：http://yuv.ehwqpu.com

DELETE FROM users WHERE id = 10;
来源：http://xuw.daria6918.cn

[Q53] 按条件删除
来源：http://kue.zdbjq.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://qoe.jlsjyb.cn

[Q54] 清空表
来源：http://bqo.yongpay.top

TRUNCATE TABLE logs;
来源：http://prc.316326.xyz

[Q55] 排名（并列占位）
来源：http://vcv.xinyue.icu

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://szy.hywenlv.cn

[Q56] 密集排名（并列不占位）
来源：http://agr.jinyuanbaomall.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://xdk.nanxuanxn.top

[Q57] 行号
来源：http://ljy.gogol.net.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://yhp.xuetiantiany.cn

[Q58] 累计求和
来源：http://uxo.shanyushiyangtech.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://vhx.yj20258.top

[Q59] 分组内累计
来源：http://ctk.dashuyun.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://qvd.yanxiufei.cn

[Q60] 取上一行 / 下一行
来源：http://jjx.pycfn.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://puo.nanxuanxn.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://xpd.fzhhl.top

[Q61] 移动平均
来源：http://nms.ctjpmb.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://cef.hcnkem.com

[Q62] 分组占比
来源：http://mvh.c1oappe.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://bhz.fehbvm.com

[Q63] 开启事务
来源：http://nea.fehbvm.com

START TRANSACTION;                -- 或 BEGIN
来源：http://mtz.hysaishi.cn

[Q64] 提交事务
来源：http://kry.dianchejie.cn

COMMIT;
来源：http://hlr.nanxinkj.top

[Q65] 回滚事务
来源：http://mkn.yangfankeji.com

ROLLBACK;
来源：http://fng.smart0.xyz

[Q66] 行锁查询
来源：http://kem.yj202588.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wfy.nanxuanxn.top

[Q67] 设置隔离级别
来源：http://sii.hongshengwenyu.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://kxj.jqgfzy.top

[Q68] 保存点
来源：http://lzr.wangdashe.top

SAVEPOINT sp1;
来源：http://sel.nanxinkj.top

ROLLBACK TO sp1;
来源：http://iti.zycfv.cn

[Q69] 查看执行计划
来源：http://run.hywenlv.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://pkt.aibaodan.cn

[Q70] 更新统计信息
来源：http://aby.jlsjyb.cn

ANALYZE TABLE users;
来源：http://bxq.snrcjt.cn

[Q71] 查看建表语句
来源：http://vki.jianghu66.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://moo.jqgufenzy.top

[Q72] 查看索引
来源：http://iev.zhongyouzk.top

SHOW INDEX FROM users;
来源：http://xjp.fanxiaobao.xyz

[Q73] 查看表状态
来源：http://okl.shanyushiyangkeji.top

SHOW TABLE STATUS LIKE 'users';
来源：http://teu.ybcxt.top

[Q74] 强制使用索引
来源：http://kvs.meibo888.top


<!-- 参考信息 -->