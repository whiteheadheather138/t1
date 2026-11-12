代发 wailian999

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://rcl.zdqjudy.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://deb.chenzaomai.com

Ruby: threads.map(&:join)
来源：http://igb.cashguo.top

C#:   await Task.WhenAll(t1, t2)
来源：http://sip.zycfv.cn

[O06] 使用进程池
来源：http://lhk.chenzaomai.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://rbd.hywenlv.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://gel.jinqigfzy.top

JS:   // child_process / cluster 模块
来源：http://dtp.bjfxy.top

TS:   // child_process / cluster 模块
来源：http://oig.gotoacloud.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://adn.shanyushiyangkeji.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://eet.hammf.cn

Ruby: // fork 块
来源：http://tzi.chenjidiqi.icu

C#:   Parallel.For
来源：http://yzu.xuetiantiany.cn

================================================================================
来源：http://yje.hammf.cn

P. 常用工具函数
来源：http://ywa.iojbl.cn

================================================================================
来源：http://gbq.jianghu66.top

[P01] 生成 UUID
来源：http://lkl.hysaishi.cn

Py:   str(uuid.uuid4())
来源：http://bmx.yongpay.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://yvi.ybcxt.top

JS:   crypto.randomUUID()
来源：http://oen.cashguo.top

TS:   crypto.randomUUID()
来源：http://jnw.jyoumei.cn

Java: UUID.randomUUID().toString()
来源：http://arg.ydzc1.top

Go:   // 用 github.com/google/uuid
来源：http://fnf.nanxinkj.top

Ruby: SecureRandom.uuid
来源：http://iiu.hcnkem.com

C#:   Guid.NewGuid().ToString()
来源：http://ftt.meibo888.top

[P02] MD5 / SHA256 摘要
来源：http://hxi.zycfv.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://yvu.52xcode.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://rab.yj20258888.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://njk.fktsv.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://nle.hfpthk.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://tjc.zhengqikj.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://doz.0kj1m.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://iyd.svipenyu.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://fbl.hnxiangtu.top

[P03] 生成短随机字符串
来源：http://rzn.cashguo.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://tfc.nanxinkj.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://yra.hammf.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xei.chenlongwang.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jmh.svipenyu.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://rlg.aibaodan.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://zuq.nanxuanxn.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://rji.cucudq.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ldd.hcnkem.com

[P04] 求长度
来源：http://cxs.iojbl.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://jey.fktsv.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fvd.dianchejie.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ndu.yonumen.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://udd.svipenyu.cn

Java: list.size();  map.size();  s.length()
来源：http://rfq.xuetiantiany.cn

Go:   len(arr);  len(m)
来源：http://omx.vehdjk.com

Ruby: x.length;  x.size
来源：http://auz.ivvv.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://off.ydjk.org.cn

[P05] 判断两个对象内容是否相等
来源：http://ulh.hesvh.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://mvm.fanxiaobao.xyz

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://cdp.tian-w.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://nps.xuetiantiany.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://xjz.mhx1999.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://dyh.hammf.cn

Go:   reflect.DeepEqual(a, b)
来源：http://qdr.tian-w.cn

Ruby: a == b
来源：http://ehd.tian-w.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://cgq.ydzc1.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://dvg.jinyuanbaomall.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://gen.fktsv.cn

PHP:  if (empty($x)) {}
来源：http://kwe.nanxuanxn.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ahn.jiagoushi.top

TS:   if (x == null) {}
来源：http://tzl.jinyuanbaomall.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://aln.yonumen.top

Go:   if x == nil {}
来源：http://uvt.sysykeji.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://uqy.gotoacloud.top

C#:   if (x is null) {}
来源：http://xiv.sufxvd.cn

[P07] 防抖与节流
来源：http://hdt.sweek.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://qhz.cqqwz.cn

PHP:  // 手写时间戳比较
来源：http://mbk.yvedp.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gij.zhiwuduotai.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dqa.gaohongyu789.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://sih.feifeiyinyue.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://vuy.jiagoushi.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://jup.yuanzhike.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://abv.chenjidiqi.icu

[P08] 处理浮点精度问题
来源：http://icc.mhx1999.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://aul.zycfv.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ker.pycfn.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://may.jinqigufen.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hxu.snrcjt.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://afk.snrcjt.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://sqo.daria6918.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://czz.jinghuilouyu.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hco.yj20258.top

================================================================================
来源：http://vkw.fanxiaobao.xyz

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blc.daria6918.cn

================================================================================
来源：http://lcq.ydjk.org.cn

[Q01] 创建表
来源：http://giu.tian-w.cn

CREATE TABLE users (
来源：http://maj.jiagoushi.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hox.yj20258.top

name VARCHAR(50) NOT NULL,
来源：http://rzi.hnxiangtu.top

email VARCHAR(100) UNIQUE,
来源：http://fbt.ydzc1.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://vif.hnxiangtu.top

);
来源：http://buf.kuanghao11.cn

[Q02] 创建带外键的表
来源：http://zhr.yangfankeji.com

CREATE TABLE orders (
来源：http://zvb.shanyushiyangtech.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://nsa.xziqi.cn

user_id INT NOT NULL,
来源：http://ysw.yueranfly.top

amount DECIMAL(10, 2),
来源：http://qxw.redwolf501.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://qsn.ydzc1.top

);
来源：http://xno.guannengcc.top

[Q03] 增加列
来源：http://cse.yonumen.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://toj.cucudq.cn

[Q04] 修改列类型
来源：http://nzt.svipenyu.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://yjn.yangfankeji.com

[Q05] 重命名列
来源：http://jwt.jinqigfzy.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://gqd.vehdjk.com

[Q06] 删除列
来源：http://bbj.mhx1999.top

ALTER TABLE users DROP COLUMN age;
来源：http://bcn.zycfv.cn

[Q07] 删除表
来源：http://bkh.hysaishi.cn

DROP TABLE IF EXISTS orders;
来源：http://aks.cdnleiting.top

[Q08] 创建普通索引
来源：http://ycy.andypj.xyz

CREATE INDEX idx_users_email ON users(email);
来源：http://whl.chenzaomai.com

[Q09] 创建唯一索引
来源：http://uhm.9152youxi.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mqy.feifeiyinyue.top

[Q10] 插入单行
来源：http://zil.gogol.net.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://zhn.zhaomingkeji.xyz

[Q11] 一次插入多行
来源：http://tqt.epnwcf.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://dgc.ybcxt.top

[Q12] 插入后取自增 ID
来源：http://gfq.quarkkingdee.top

INSERT INTO users (name) VALUES ('C');
来源：http://yxv.hysaishi.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://vem.feifeiyinyue.top

[Q13] 忽略重复插入
来源：http://zxt.cdnleiting.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://snw.jiagoushi.top

[Q14] 存在则更新（upsert）
来源：http://vsw.nanxinkj.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mgj.xuanzx.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://sls.zhaomingkeji.xyz

[Q15] 查询全部
来源：http://doq.jinyuanbaomall.cn

SELECT * FROM users;
来源：http://alb.316326.xyz

[Q16] 查询指定列
来源：http://qkz.iojbl.cn

SELECT id, name FROM users;
来源：http://egy.jinqigufen.top

[Q17] 条件查询
来源：http://wnb.hywenlv.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://epk.sxryk.cn

[Q18] 模糊匹配
来源：http://vwp.zdbjq.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://zbq.jqgfzy.top

[Q19] 范围查询
来源：http://ffq.xuetiantiany.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://las.zycfv.cn

[Q20] IN 列表
来源：http://iaq.fktsv.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mgz.jiagoushi.top

[Q21] 空值判断
来源：http://ens.zhengqikj.top

SELECT * FROM users WHERE email IS NULL;
来源：http://ics.316326.xyz

[Q22] 排序
来源：http://qxd.yfazqb.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://whw.hcnkem.com

[Q23] 分页
来源：http://lyx.cashguo.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://lio.jianghu66.top

[Q24] 去重
来源：http://paw.svipenyu.cn

SELECT DISTINCT city FROM users;
来源：http://wko.vehdjk.com

[Q25] 只取前 N 条
来源：http://hwt.316326.xyz

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ytq.dianchejie.cn

[Q26] 计数
来源：http://zvk.guannengcc.top

SELECT COUNT(*) FROM users;
来源：http://dim.svipenyu.cn

[Q27] 条件计数
来源：http://mpq.fehbvm.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://asw.ywan-chungtsiang.top

[Q28] 求和与平均
来源：http://dpl.sysykeji.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://uyv.sxryk.cn

[Q29] 最大最小值
来源：http://tbm.yj20258888.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://wdz.sufxvd.cn

[Q30] 分组统计
来源：http://bgl.havefunace.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://thq.shanyushiyangtech.top

[Q31] 分组后过滤
来源：http://omh.dianchejie.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://kka.wangshuangyany.cn

[Q32] 分组拼接字符串
来源：http://bic.yueranfly.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://jgz.hywenlv.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hri.shanyushiyangkeji.top

[Q33] 多列分组
来源：http://dxk.yongpay.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://vam.ivvv.top

[Q34] 每组取第一条
来源：http://aoq.hywenlv.cn

SELECT * FROM (
来源：http://xme.gaohongyu789.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://rgq.tian-w.cn

) t WHERE rn = 1;
来源：http://gjz.sysykeji.top

[Q35] 内连接
来源：http://ils.xuanzx.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://gye.hysaishi.cn

[Q36] 左连接
来源：http://pwl.fanxiaobao.xyz

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://pnw.jiagoushi.top

[Q37] 右连接
来源：http://qdv.yj202588.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://agb.havefunace.top

[Q38] 全外连接（PostgreSQL）
来源：http://tib.xinyue.icu

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ckg.hcnkem.com

[Q39] 自连接（查上下级）
来源：http://ktm.zhengqikj.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://obb.yueranfly.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://drr.jinqigfzy.top

[Q40] 交叉连接（笛卡尔积）
来源：http://dwm.daria6918.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://aeh.jianghu66.top

[Q41] 多表连接
来源：http://wmu.316326.xyz

SELECT o.id, u.name, p.title FROM orders o
来源：http://tig.quarkkingdee.top

JOIN users u ON u.id = o.user_id
来源：http://yuw.aibaodan.cn

JOIN products p ON p.id = o.product_id;
来源：http://mnw.haohaochexian.top

[Q42] 连接条件附加过滤
来源：http://lsl.dianchejie.cn

SELECT u.name, o.amount FROM users u
来源：http://zhr.mhx1999.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://jdz.hnxiangtu.top

[Q43] 标量子查询
来源：http://mmj.zycfv.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ttx.yuxming.cn

[Q44] IN 子查询
来源：http://tjv.ppjwa.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://uiw.hysaishi.cn

[Q45] EXISTS 判断存在
来源：http://zzd.shuidangran.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://dnj.daria6918.cn

[Q46] NOT EXISTS 判断不存在
来源：http://aky.hcnkem.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jna.yonumen.top

[Q47] 与平均值比较
来源：http://utx.jinqigufen.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://out.daria6918.cn

[Q48] CTE 公用表表达式
来源：http://blh.zhongyouzk.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://eel.hywenlv.cn

SELECT * FROM t WHERE c > 5;
来源：http://kkv.zhiwuduotai.top

[Q49] 更新单行
来源：http://lte.c1oappe.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://sbx.jiagoushi.top

[Q50] 批量更新
来源：http://adr.haohaochexian.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://onl.dashuyun.cn

[Q51] 用子查询更新
来源：http://jkb.xingfuxueyuan.xyz

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://juw.iojbl.cn

[Q52] 删除指定行
来源：http://bij.hongshengwenyu.top

DELETE FROM users WHERE id = 10;
来源：http://xyh.xziqi.cn

[Q53] 按条件删除
来源：http://fjj.jiagoushi.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ygt.uphjek.com

[Q54] 清空表
来源：http://zvp.vehdjk.com

TRUNCATE TABLE logs;
来源：http://fpz.mhx1999.top

[Q55] 排名（并列占位）
来源：http://hhh.jianghu66.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://tnd.316326.xyz

[Q56] 密集排名（并列不占位）
来源：http://nim.chenjidiqi.icu

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://cbg.zhongyouzk.top

[Q57] 行号
来源：http://gqk.havefunace.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://byp.dashuyun.cn

[Q58] 累计求和
来源：http://ray.ybcxt.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wlo.tarul.cn

[Q59] 分组内累计
来源：http://ipw.zhongyouzk.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ruv.jqgfzy.top

[Q60] 取上一行 / 下一行
来源：http://dse.sxryk.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hjy.zdqjudy.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://nbf.quarkkingdee.top

[Q61] 移动平均
来源：http://cmg.yuxming.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://csq.zhixingplan.top

[Q62] 分组占比
来源：http://klr.yueranfly.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://dpg.ywan-chungtsiang.top

[Q63] 开启事务
来源：http://rqa.fktsv.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://dfz.jqgufenzy.top

[Q64] 提交事务
来源：http://gyx.zhiwuduotai.top

COMMIT;
来源：http://xuc.sjlbkw.cn

[Q65] 回滚事务
来源：http://ufe.epnwcf.com

ROLLBACK;
来源：http://hyk.shangyingyoupin.top

[Q66] 行锁查询
来源：http://yvw.redwolf501.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://rnb.xinyue.icu

[Q67] 设置隔离级别
来源：http://bkm.fktsv.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://sep.meibo888.top

[Q68] 保存点
来源：http://gob.daria6918.cn

SAVEPOINT sp1;
来源：http://zbf.nanxinkj.top

ROLLBACK TO sp1;
来源：http://hiq.mhx1999.top

[Q69] 查看执行计划
来源：http://ayg.yj20258888.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://oqk.shuidangran.top

[Q70] 更新统计信息
来源：http://kzv.gzhubu.top

ANALYZE TABLE users;
来源：http://sgn.yj202588.top

[Q71] 查看建表语句
来源：http://mby.fktsv.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://jkb.zhijiandao.cn

[Q72] 查看索引
来源：http://zvt.ctjpmb.com

SHOW INDEX FROM users;
来源：http://tvg.shangyingyoupin.top

[Q73] 查看表状态
来源：http://edm.vqdsnc.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://xto.wangshuangyany.cn

[Q74] 强制使用索引
来源：http://otg.jinghuilouyu.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.fengsongda.top

[Q75] 日期格式化
来源：http://kxz.ppjwa.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://qjn.snrcjt.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mvt.birdmap.top

[Q76] 按天统计
来源：http://wip.vqdsnc.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ixm.epnwcf.com

[Q77] 时间加减
来源：http://jfd.yj202588.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://klb.zhoulong.xyz

[Q78] 当前时间
来源：http://zyx.yuanzhike.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://anp.jinghuilouyu.cn

[Q79] 字符串拼接
来源：http://oky.9152youxi.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://kvm.chenzaomai.com

[Q80] 字符串截取
来源：http://wju.9152youxi.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wnw.zdqjudy.top

[Q81] 字符串替换
来源：http://cxx.shuidangran.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://cnx.jqgufenzy.top

[Q82] 字符长度与字节长度
来源：http://ykg.mhx1999.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://gst.pycfn.com

[Q83] 大小写转换
来源：http://ycb.ybcxt.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ndh.smart0.xyz

[Q84] 去除首尾空格
来源：http://qyj.fzhhl.top

SELECT TRIM(name) FROM users;
来源：http://uqe.fengsongda.top

[Q85] 数值取整
来源：http://hnx.ywan-chungtsiang.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://uzl.fengsongda.top

[Q86] 读取 JSON 字段
来源：http://rvi.havefunace.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ltl.aibaodan.cn

[Q87] JSON 字段做条件
来源：http://dhe.tianlin.xyz

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://cte.sufxvd.cn

[Q88] 行转列（条件聚合）
来源：http://kxe.jyoumei.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://fgf.fktsv.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://lou.ehwqpu.com

[Q89] 判断表是否存在
来源：http://ryx.guowangkeji.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://rcr.yongpay.top

[Q90] 生成序号列
来源：http://adu.dianchejie.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://exd.ydjk.org.cn

================================================================================
来源：http://pvj.fehbvm.com

R. Bash 专题
来源：http://kfs.sxryk.cn

================================================================================
来源：http://gpq.hesvh.cn

[R01] shebang 与严格模式
来源：http://zix.svipenyu.cn

#!/usr/bin/env bash
来源：http://koa.cashguo.top


<!-- 参考信息 -->