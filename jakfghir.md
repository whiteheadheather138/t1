代发 wailian999

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://psu.cqqwz.cn

JS:   async function f() { await g(); }
来源：http://sjl.chenzaomai.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://pph.yj20258.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://cqc.ydjk.org.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://pov.ctjpmb.com

Ruby: # 用 Fiber 或 async gem
来源：http://cqo.ybcxt.top

C#:   async Task F() { await G(); }
来源：http://hdq.9152youxi.cn

[O05] 并发执行并等待全部完成
来源：http://vtk.ppjwa.cn

Py:   asyncio.gather(*tasks)
来源：http://ukr.fengsongda.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://iol.daria6918.cn

JS:   await Promise.all(tasks)
来源：http://vnd.shanyushiyangtech.top

TS:   await Promise.all(tasks)
来源：http://akg.hammf.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wlc.gogol.net.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://asw.daxiang520.top

Ruby: threads.map(&:join)
来源：http://qqj.yuxming.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://caa.shuidangran.top

[O06] 使用进程池
来源：http://mba.shangyingyoupin.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://xxz.tanke756.top

PHP:  // pcntl_fork 或多进程队列
来源：http://cuu.fanxiaobao.xyz

JS:   // child_process / cluster 模块
来源：http://unx.zhengqikj.top

TS:   // child_process / cluster 模块
来源：http://ihv.zhengqikj.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mww.zhaomingkeji.xyz

Go:   // goroutine 已占用多核，直接并发即可
来源：http://rfd.yuxming.cn

Ruby: // fork 块
来源：http://uui.yangfankeji.com

C#:   Parallel.For
来源：http://vcn.wangdashe.top

================================================================================
来源：http://beh.hfpthk.cn

P. 常用工具函数
来源：http://epj.hnxiangtu.top

================================================================================
来源：http://kdr.chenjidiqi.icu

[P01] 生成 UUID
来源：http://dtr.jqgfzy.top

Py:   str(uuid.uuid4())
来源：http://irb.hongshengwenyu.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ota.shuidangran.top

JS:   crypto.randomUUID()
来源：http://ong.zhengqikj.top

TS:   crypto.randomUUID()
来源：http://tol.kuanghao11.cn

Java: UUID.randomUUID().toString()
来源：http://vzr.bjfxy.top

Go:   // 用 github.com/google/uuid
来源：http://azz.pengpengdd.cyou

Ruby: SecureRandom.uuid
来源：http://mhl.epnwcf.com

C#:   Guid.NewGuid().ToString()
来源：http://xpa.fanxiaobao.xyz

[P02] MD5 / SHA256 摘要
来源：http://djr.cashguo.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://dya.sxryk.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://icw.316326.xyz

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://iah.ppjwa.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://pne.hysaishi.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://edm.quarkkingdee.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://jge.jqgufenzy.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://owu.0kj1m.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://gpd.52xcode.cn

[P03] 生成短随机字符串
来源：http://bkd.ehwqpu.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://peq.cheryme.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://kdr.0kj1m.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://caj.chenzaomai.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ahw.yfazqb.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://azx.haohaochexian.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://xac.hnxiangtu.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://tcv.yuxming.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ygr.c1oappe.top

[P04] 求长度
来源：http://kmh.yueranfly.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mua.daria6918.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://inw.pengpengdd.cyou

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qoi.uphjek.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://oij.gzhubu.top

Java: list.size();  map.size();  s.length()
来源：http://mbl.jinyuanbaomall.cn

Go:   len(arr);  len(m)
来源：http://zfo.birdmap.top

Ruby: x.length;  x.size
来源：http://xho.snrcjt.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://oil.hnqzz.top

[P05] 判断两个对象内容是否相等
来源：http://qec.ywan-chungtsiang.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://sje.9152youxi.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://gkb.xylfe.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mlh.cashguo.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://dla.chenzaomai.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://xar.gaohongyu789.top

Go:   reflect.DeepEqual(a, b)
来源：http://tyh.aizwys.cn

Ruby: a == b
来源：http://lnh.sufxvd.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://kkm.jyoumei.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://xno.ybcxt.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://xjx.tian-w.cn

PHP:  if (empty($x)) {}
来源：http://rvm.ydjk.org.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://zmy.zdqjudy.top

TS:   if (x == null) {}
来源：http://hzn.nwbrower.top

Java: if (x == null || x.isEmpty()) {}
来源：http://mmo.jianghu66.top

Go:   if x == nil {}
来源：http://kfg.zhijiandao.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://dwb.zhiwuduotai.top

C#:   if (x is null) {}
来源：http://kko.xuanzx.com

[P07] 防抖与节流
来源：http://igv.yuxming.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://zvj.shzxlz.cn

PHP:  // 手写时间戳比较
来源：http://gsu.fengsongda.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://iei.svipenyu.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kbr.xylfe.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mtp.shangyingyoupin.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://uri.wangdashe.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://uyc.ctjpmb.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://lxx.jinghuilouyu.cn

[P08] 处理浮点精度问题
来源：http://psh.pycfn.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://kyi.wangshuangyany.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://cgy.xuetiantiany.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://cug.yonumen.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://dgk.ivvv.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://beo.xingfuxueyuan.xyz

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wug.zhijiandao.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://vqe.bbcook.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://vtk.cheryme.top

================================================================================
来源：http://inw.tianlin.xyz

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://uqp.dianchejie.cn

================================================================================
来源：http://sdy.jinqigufen.top

[Q01] 创建表
来源：http://kth.sjlbkw.cn

CREATE TABLE users (
来源：http://ezq.iojbl.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hyc.gaohongyu789.top

name VARCHAR(50) NOT NULL,
来源：http://nhf.aizwys.cn

email VARCHAR(100) UNIQUE,
来源：http://vrh.ydzc1.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://rwa.yfazqb.com

);
来源：http://jue.ydjk.org.cn

[Q02] 创建带外键的表
来源：http://vaq.tianlin.xyz

CREATE TABLE orders (
来源：http://rou.iojbl.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://xqm.yuanzhike.top

user_id INT NOT NULL,
来源：http://rfn.0kj1m.cn

amount DECIMAL(10, 2),
来源：http://eow.cashguo.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ksk.tianlin.xyz

);
来源：http://gzu.xinyue.icu

[Q03] 增加列
来源：http://wmu.andypj.xyz

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ssa.yonumen.top

[Q04] 修改列类型
来源：http://rvq.zhiwuduotai.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://sjp.cashguo.top

[Q05] 重命名列
来源：http://fxe.xuetiantiany.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ktw.sjlbkw.cn

[Q06] 删除列
来源：http://ahq.shanyushiyangtech.top

ALTER TABLE users DROP COLUMN age;
来源：http://trs.sxryk.cn

[Q07] 删除表
来源：http://ifd.316326.xyz

DROP TABLE IF EXISTS orders;
来源：http://tjl.jqgfzy.top

[Q08] 创建普通索引
来源：http://qvh.yueranfly.top

CREATE INDEX idx_users_email ON users(email);
来源：http://wxq.shzxlz.cn

[Q09] 创建唯一索引
来源：http://vsw.xziqi.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://bax.yj20258888.top

[Q10] 插入单行
来源：http://anw.svipenyu.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://tuc.316326.xyz

[Q11] 一次插入多行
来源：http://ilx.dashuyun.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://css.fengsongda.top

[Q12] 插入后取自增 ID
来源：http://kxk.shanyushiyangkeji.top

INSERT INTO users (name) VALUES ('C');
来源：http://akh.fehbvm.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://aul.xuetiantiany.cn

[Q13] 忽略重复插入
来源：http://pzs.pengpengdd.cyou

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://vgt.0kj1m.cn

[Q14] 存在则更新（upsert）
来源：http://qav.nanxinkj.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ioq.cdnleiting.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ktv.redwolf501.top

[Q15] 查询全部
来源：http://dun.wangdashe.top

SELECT * FROM users;
来源：http://gue.hywenlv.cn

[Q16] 查询指定列
来源：http://rpt.havefunace.top

SELECT id, name FROM users;
来源：http://rok.yangfankeji.com

[Q17] 条件查询
来源：http://wvx.yj20258888.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://yhz.zhixingplan.top

[Q18] 模糊匹配
来源：http://uev.epnwcf.com

SELECT * FROM users WHERE name LIKE '张%';
来源：http://bmm.ydzc1.top

[Q19] 范围查询
来源：http://zxy.gotoacloud.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://foi.jlsjyb.cn

[Q20] IN 列表
来源：http://mto.chenjidiqi.icu

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://fes.daria6918.cn

[Q21] 空值判断
来源：http://gdm.sysykeji.top

SELECT * FROM users WHERE email IS NULL;
来源：http://vts.jqgufenzy.top

[Q22] 排序
来源：http://jgn.xziqi.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://tyn.chenjidiqi.icu

[Q23] 分页
来源：http://tsq.birdmap.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://fsz.shuidangran.top

[Q24] 去重
来源：http://hyy.jinyuanbaomall.cn

SELECT DISTINCT city FROM users;
来源：http://rfp.cashguo.top

[Q25] 只取前 N 条
来源：http://him.zhengqikj.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hev.hesvh.cn

[Q26] 计数
来源：http://sgy.meibo888.top

SELECT COUNT(*) FROM users;
来源：http://xpw.9152youxi.cn

[Q27] 条件计数
来源：http://xoi.ybcxt.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hel.52xcode.cn

[Q28] 求和与平均
来源：http://oie.ybcxt.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://xax.wangdashe.top

[Q29] 最大最小值
来源：http://aai.gogol.net.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://pgx.zycfv.cn

[Q30] 分组统计
来源：http://luv.kuanghao11.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://rro.jinyuanbaomall.cn

[Q31] 分组后过滤
来源：http://yin.wangshuangyany.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mpe.xingfuxueyuan.xyz

[Q32] 分组拼接字符串
来源：http://chc.xylfe.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://kfv.cdnleiting.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://huu.9152youxi.cn

[Q33] 多列分组
来源：http://blt.fanxiaobao.xyz

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://pim.zhixingplan.top

[Q34] 每组取第一条
来源：http://qly.epnwcf.com

SELECT * FROM (
来源：http://ijj.xylfe.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ajl.shanyushiyangkeji.top

) t WHERE rn = 1;
来源：http://zbw.cdnleiting.top

[Q35] 内连接
来源：http://dbx.birdmap.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://sxj.hcnkem.com

[Q36] 左连接
来源：http://uwl.zdqjudy.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://cie.vehdjk.com

[Q37] 右连接
来源：http://wvb.cucudq.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://qvj.zdbjq.cn

[Q38] 全外连接（PostgreSQL）
来源：http://lqd.sxryk.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://iff.tianlin.xyz

[Q39] 自连接（查上下级）
来源：http://fow.tian-w.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://qkt.shanyushiyangtech.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://eck.xinyue.icu

[Q40] 交叉连接（笛卡尔积）
来源：http://qbf.ivvv.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://djf.zhixingplan.top

[Q41] 多表连接
来源：http://pkr.chenlongwang.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://dnd.fktsv.cn

JOIN users u ON u.id = o.user_id
来源：http://fci.hfpthk.cn

JOIN products p ON p.id = o.product_id;
来源：http://dxw.shanyushiyangkeji.top

[Q42] 连接条件附加过滤
来源：http://urd.zhaomingkeji.xyz

SELECT u.name, o.amount FROM users u
来源：http://pfo.tian-w.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://yxp.xingfuxueyuan.xyz

[Q43] 标量子查询
来源：http://bru.hongshengwenyu.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://kdx.haohaochexian.top

[Q44] IN 子查询
来源：http://dtn.andypj.xyz

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://cwu.ehwqpu.com

[Q45] EXISTS 判断存在
来源：http://vbt.yongpay.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://lso.zhongyouzk.top

[Q46] NOT EXISTS 判断不存在
来源：http://smw.hongshengwenyu.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://yvv.tanke756.top

[Q47] 与平均值比较
来源：http://zri.sjlbkw.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://pjg.vehdjk.com

[Q48] CTE 公用表表达式
来源：http://icb.vehdjk.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ahe.epnwcf.com

SELECT * FROM t WHERE c > 5;
来源：http://evo.tian-w.cn

[Q49] 更新单行
来源：http://scx.guannengcc.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://cmm.zhongyouzk.top

[Q50] 批量更新
来源：http://dqx.xingfuxueyuan.xyz

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://nyj.fzhhl.top

[Q51] 用子查询更新
来源：http://vcw.hnqzz.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://tud.jinyuanbaomall.cn

[Q52] 删除指定行
来源：http://dhy.ctjpmb.com

DELETE FROM users WHERE id = 10;
来源：http://ctn.hammf.cn

[Q53] 按条件删除
来源：http://uou.daxiang520.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ybc.shzxlz.cn

[Q54] 清空表
来源：http://des.fengsongda.top

TRUNCATE TABLE logs;
来源：http://ife.birdmap.top

[Q55] 排名（并列占位）
来源：http://rhf.pycfn.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://yxm.hcnkem.com

[Q56] 密集排名（并列不占位）
来源：http://ypw.guowangkeji.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://djl.0kj1m.cn

[Q57] 行号
来源：http://eqd.iojbl.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://dfo.jiagoushi.top

[Q58] 累计求和
来源：http://uex.andypj.xyz

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ybi.yongpay.top

[Q59] 分组内累计
来源：http://qqb.fktsv.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://fdm.yj20258888.top

[Q60] 取上一行 / 下一行
来源：http://tqe.dashuyun.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://fui.birdmap.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://xtp.c1oappe.top

[Q61] 移动平均
来源：http://djx.cheryme.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://rwy.xingfuxueyuan.xyz

[Q62] 分组占比
来源：http://bmz.52xcode.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://xmw.sweek.top

[Q63] 开启事务
来源：http://qci.fehbvm.com

START TRANSACTION;                -- 或 BEGIN
来源：http://rdo.yuxming.cn

[Q64] 提交事务
来源：http://xuz.zhiwuduotai.top

COMMIT;
来源：http://iga.sxryk.cn

[Q65] 回滚事务
来源：http://rje.zdqjudy.top

ROLLBACK;
来源：http://xia.yanxiufei.cn

[Q66] 行锁查询
来源：http://pks.52xcode.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://zwr.jianghu66.top

[Q67] 设置隔离级别
来源：http://tuk.cdnleiting.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://iwq.jqgufenzy.top

[Q68] 保存点
来源：http://sjv.nanxinkj.top

SAVEPOINT sp1;
来源：http://jwt.hysaishi.cn

ROLLBACK TO sp1;
来源：http://pqf.xylfe.cn

[Q69] 查看执行计划
来源：http://czk.sysykeji.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://zuw.zdbjq.cn

[Q70] 更新统计信息
来源：http://saz.shanyushiyangtech.top

ANALYZE TABLE users;
来源：http://xeb.redwolf501.top

[Q71] 查看建表语句
来源：http://nqo.tarul.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://axt.xinyue.icu

[Q72] 查看索引
来源：http://mfs.chenzaomai.com

SHOW INDEX FROM users;
来源：http://xsh.jqgfzy.top

[Q73] 查看表状态
来源：http://bor.zhijiandao.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://mza.ivvv.top

[Q74] 强制使用索引
来源：http://yjj.jqgfzy.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://toj.fengsongda.top

[Q75] 日期格式化
来源：http://pen.xinyue.icu

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://xrl.chenjidiqi.icu

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://vlu.yfazqb.com

[Q76] 按天统计
来源：http://sqz.daxiang520.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://pva.iojbl.cn

[Q77] 时间加减
来源：http://dnb.snrcjt.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://riw.zhengqikj.top

[Q78] 当前时间
来源：http://tim.yj202588.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://xuz.52xcode.cn

[Q79] 字符串拼接
来源：http://jhb.quarkkingdee.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://suw.ctjpmb.com

[Q80] 字符串截取
来源：http://oqz.yj202588.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://uqh.zhaomingkeji.xyz

[Q81] 字符串替换
来源：http://tih.hnqzz.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://azd.zdqjudy.top

[Q82] 字符长度与字节长度
来源：http://ymy.9152youxi.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://zjk.zycfv.cn

[Q83] 大小写转换
来源：http://dhm.cdnleiting.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://jpb.0kj1m.cn

[Q84] 去除首尾空格
来源：http://qim.birdmap.top

SELECT TRIM(name) FROM users;
来源：http://evo.meibo888.top

[Q85] 数值取整
来源：http://xiv.xylfe.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://fah.hcnkem.com

[Q86] 读取 JSON 字段
来源：http://suz.jyoumei.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://kvt.mhx1999.top

[Q87] JSON 字段做条件
来源：http://ysp.gzhubu.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://rtk.hfpthk.cn


<!-- 参考信息 -->