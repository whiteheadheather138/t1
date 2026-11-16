代发 wailian999

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://qfe.cashguo.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://tcf.nwbrower.top

Ruby: threads.map(&:join)
来源：http://jpl.fktsv.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://unk.aizwys.cn

[O06] 使用进程池
来源：http://eln.guannengcc.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://gmo.chenzaomai.com

PHP:  // pcntl_fork 或多进程队列
来源：http://shm.fktsv.cn

JS:   // child_process / cluster 模块
来源：http://okh.yanxiufei.cn

TS:   // child_process / cluster 模块
来源：http://prg.birdmap.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://gtm.tarul.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://yfw.shuidangran.top

Ruby: // fork 块
来源：http://raj.andypj.xyz

C#:   Parallel.For
来源：http://oyf.sxryk.cn

================================================================================
来源：http://ipq.zdbjq.cn

P. 常用工具函数
来源：http://dec.vehdjk.com

================================================================================
来源：http://ktm.hnqzz.top

[P01] 生成 UUID
来源：http://zvg.ydzc1.top

Py:   str(uuid.uuid4())
来源：http://ygn.yongpay.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ril.jinqigfzy.top

JS:   crypto.randomUUID()
来源：http://ixl.zhixingplan.top

TS:   crypto.randomUUID()
来源：http://aqb.fktsv.cn

Java: UUID.randomUUID().toString()
来源：http://dbo.hfpthk.cn

Go:   // 用 github.com/google/uuid
来源：http://kzz.shanyushiyangtech.top

Ruby: SecureRandom.uuid
来源：http://ksb.jiagoushi.top

C#:   Guid.NewGuid().ToString()
来源：http://nog.sufxvd.cn

[P02] MD5 / SHA256 摘要
来源：http://inp.yonumen.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://jfv.sufxvd.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://sno.epnwcf.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mvu.jinyuanbaomall.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://bau.xingfuxueyuan.xyz

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://cdh.zhoulong.xyz

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://emy.hesvh.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://frw.xuanzx.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://fmp.epnwcf.com

[P03] 生成短随机字符串
来源：http://wia.snrcjt.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://tno.bjfxy.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://uqz.daria6918.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://tyu.jyoumei.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://nly.cdnleiting.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://fdz.0kj1m.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://dde.ybcxt.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://neh.xingfuxueyuan.xyz

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://xpu.yuanzhike.top

[P04] 求长度
来源：http://kuh.fzhhl.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hcn.ehwqpu.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://pcf.zhiwuduotai.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hhc.sweek.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://cmr.ivvv.top

Java: list.size();  map.size();  s.length()
来源：http://xrg.nwbrower.top

Go:   len(arr);  len(m)
来源：http://toj.fehbvm.com

Ruby: x.length;  x.size
来源：http://fqw.yvedp.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://cdo.epnwcf.com

[P05] 判断两个对象内容是否相等
来源：http://cso.vqdsnc.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://bzb.yanxiufei.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://xry.zhijiandao.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://emf.hcnkem.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://toz.shzxlz.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://fkp.daria6918.cn

Go:   reflect.DeepEqual(a, b)
来源：http://tkh.sweek.top

Ruby: a == b
来源：http://axo.sweek.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://rnv.chenjidiqi.icu

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hou.fktsv.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://cot.guannengcc.top

PHP:  if (empty($x)) {}
来源：http://fkj.zhongyouzk.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://bvt.ctjpmb.com

TS:   if (x == null) {}
来源：http://zms.jinqigufen.top

Java: if (x == null || x.isEmpty()) {}
来源：http://awv.zdqjudy.top

Go:   if x == nil {}
来源：http://nbq.sufxvd.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://asu.daxiang520.top

C#:   if (x is null) {}
来源：http://ybi.hammf.cn

[P07] 防抖与节流
来源：http://hkm.tarul.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://quu.guowangkeji.top

PHP:  // 手写时间戳比较
来源：http://yqc.sxryk.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xya.xinyue.icu

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://viq.zhongyouzk.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://omz.xingfuxueyuan.xyz

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://lrq.zhixingplan.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://gsu.hfpthk.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://nwv.jlsjyb.cn

[P08] 处理浮点精度问题
来源：http://ujs.316326.xyz

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ukt.zycfv.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://rrg.svipenyu.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://uth.ppjwa.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hvj.ydjk.org.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ztf.yonumen.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wgn.chenlongwang.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://vzq.hammf.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mhd.hysaishi.cn

================================================================================
来源：http://ukb.uphjek.com

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://twl.52xcode.cn

================================================================================
来源：http://plf.yuxming.cn

[Q01] 创建表
来源：http://hld.316326.xyz

CREATE TABLE users (
来源：http://ehb.gogol.net.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://sns.jlsjyb.cn

name VARCHAR(50) NOT NULL,
来源：http://pkw.zhiwuduotai.top

email VARCHAR(100) UNIQUE,
来源：http://kuk.316326.xyz

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://gkk.hongshengwenyu.top

);
来源：http://axu.sjlbkw.cn

[Q02] 创建带外键的表
来源：http://qin.xylfe.cn

CREATE TABLE orders (
来源：http://phr.iojbl.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://iqr.andypj.xyz

user_id INT NOT NULL,
来源：http://xlj.sufxvd.cn

amount DECIMAL(10, 2),
来源：http://wcc.sweek.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://xks.hywenlv.cn

);
来源：http://zto.cheryme.top

[Q03] 增加列
来源：http://mia.fengsongda.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://axr.vehdjk.com

[Q04] 修改列类型
来源：http://ifx.hfpthk.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://syt.zhaomingkeji.xyz

[Q05] 重命名列
来源：http://qce.cucudq.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://six.gotoacloud.top

[Q06] 删除列
来源：http://bmi.epnwcf.com

ALTER TABLE users DROP COLUMN age;
来源：http://vgx.gotoacloud.top

[Q07] 删除表
来源：http://thd.iojbl.cn

DROP TABLE IF EXISTS orders;
来源：http://ndv.svipenyu.cn

[Q08] 创建普通索引
来源：http://eid.xuetiantiany.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://brg.daxiang520.top

[Q09] 创建唯一索引
来源：http://ckm.jqgufenzy.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://zkg.guowangkeji.top

[Q10] 插入单行
来源：http://sok.sysykeji.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://pmh.yonumen.top

[Q11] 一次插入多行
来源：http://rpg.chenjidiqi.icu

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://xsm.hongshengwenyu.top

[Q12] 插入后取自增 ID
来源：http://tta.c1oappe.top

INSERT INTO users (name) VALUES ('C');
来源：http://slg.hysaishi.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hah.yangfankeji.com

[Q13] 忽略重复插入
来源：http://zcb.9152youxi.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://whz.zhixingplan.top

[Q14] 存在则更新（upsert）
来源：http://aqp.yuxming.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://zqr.sweek.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://vrt.kuanghao11.cn

[Q15] 查询全部
来源：http://zqm.yuxming.cn

SELECT * FROM users;
来源：http://fpr.meibo888.top

[Q16] 查询指定列
来源：http://uji.zhiwuduotai.top

SELECT id, name FROM users;
来源：http://zpp.vehdjk.com

[Q17] 条件查询
来源：http://rbo.wangdashe.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://lzo.zhixingplan.top

[Q18] 模糊匹配
来源：http://axe.chenlongwang.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://lnf.xziqi.cn

[Q19] 范围查询
来源：http://umi.ydzc1.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hna.hnqzz.top

[Q20] IN 列表
来源：http://wqi.fehbvm.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://reb.jiagoushi.top

[Q21] 空值判断
来源：http://zva.yj20258888.top

SELECT * FROM users WHERE email IS NULL;
来源：http://wyc.jinyuanbaomall.cn

[Q22] 排序
来源：http://myx.kuanghao11.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://oek.yj20258.top

[Q23] 分页
来源：http://mfm.ybcxt.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://anp.hammf.cn

[Q24] 去重
来源：http://huj.zhixingplan.top

SELECT DISTINCT city FROM users;
来源：http://gco.gzhubu.top

[Q25] 只取前 N 条
来源：http://pph.dashuyun.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://zfl.yj20258.top

[Q26] 计数
来源：http://wja.ydjk.org.cn

SELECT COUNT(*) FROM users;
来源：http://xee.meibo888.top

[Q27] 条件计数
来源：http://tls.yuanzhike.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ebv.fengsongda.top

[Q28] 求和与平均
来源：http://rjz.xuanzx.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://lnc.zhijiandao.cn

[Q29] 最大最小值
来源：http://viy.nanxinkj.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://gei.316326.xyz

[Q30] 分组统计
来源：http://quk.smart0.xyz

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hal.fengsongda.top

[Q31] 分组后过滤
来源：http://exm.fzhhl.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://moc.hnqzz.top

[Q32] 分组拼接字符串
来源：http://ucn.svipenyu.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ctn.zhengqikj.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://vvy.cashguo.top

[Q33] 多列分组
来源：http://vfz.uphjek.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mwj.52xcode.cn

[Q34] 每组取第一条
来源：http://izs.yvedp.cn

SELECT * FROM (
来源：http://oyt.hysaishi.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://diy.hcnkem.com

) t WHERE rn = 1;
来源：http://myy.c1oappe.top

[Q35] 内连接
来源：http://jdo.yj20258888.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://uyl.jqgufenzy.top

[Q36] 左连接
来源：http://bxi.svipenyu.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://svd.tianlin.xyz

[Q37] 右连接
来源：http://zzn.xuanzx.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://jct.yonumen.top

[Q38] 全外连接（PostgreSQL）
来源：http://wnb.hammf.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://agi.cqqwz.cn

[Q39] 自连接（查上下级）
来源：http://coc.hfpthk.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://kmn.nanxuanxn.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://dlq.meibo888.top

[Q40] 交叉连接（笛卡尔积）
来源：http://ibi.smart0.xyz

SELECT * FROM colors CROSS JOIN sizes;
来源：http://yti.mhx1999.top

[Q41] 多表连接
来源：http://jec.gotoacloud.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://jnc.hongshengwenyu.top

JOIN users u ON u.id = o.user_id
来源：http://iwo.birdmap.top

JOIN products p ON p.id = o.product_id;
来源：http://trj.ydzc1.top

[Q42] 连接条件附加过滤
来源：http://usm.ywan-chungtsiang.top

SELECT u.name, o.amount FROM users u
来源：http://jru.jinyuanbaomall.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://egz.jyoumei.cn

[Q43] 标量子查询
来源：http://pus.nwbrower.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://yah.daria6918.cn

[Q44] IN 子查询
来源：http://jfl.zdbjq.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://fnr.sjlbkw.cn

[Q45] EXISTS 判断存在
来源：http://rlg.xziqi.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hdw.nwbrower.top

[Q46] NOT EXISTS 判断不存在
来源：http://acm.epnwcf.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://dur.redwolf501.top

[Q47] 与平均值比较
来源：http://gkf.yanxiufei.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://kcy.yj20258888.top

[Q48] CTE 公用表表达式
来源：http://xgv.fengsongda.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://cyg.ybcxt.top

SELECT * FROM t WHERE c > 5;
来源：http://qba.ydjk.org.cn

[Q49] 更新单行
来源：http://mui.jqgfzy.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://skm.tian-w.cn

[Q50] 批量更新
来源：http://jqq.gzhubu.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wul.ctjpmb.com

[Q51] 用子查询更新
来源：http://tji.fanxiaobao.xyz

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://swm.uphjek.com

[Q52] 删除指定行
来源：http://jcr.yonumen.top

DELETE FROM users WHERE id = 10;
来源：http://whl.ctjpmb.com

[Q53] 按条件删除
来源：http://aye.cqqwz.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://jcm.hesvh.cn

[Q54] 清空表
来源：http://wtf.jyoumei.cn

TRUNCATE TABLE logs;
来源：http://sep.hcnkem.com

[Q55] 排名（并列占位）
来源：http://ken.ehwqpu.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://gns.ywan-chungtsiang.top

[Q56] 密集排名（并列不占位）
来源：http://kcq.shzxlz.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://vix.pengpengdd.cyou

[Q57] 行号
来源：http://cnd.zhaomingkeji.xyz

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://qic.vehdjk.com

[Q58] 累计求和
来源：http://eym.cashguo.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://vsh.0kj1m.cn

[Q59] 分组内累计
来源：http://voz.fzhhl.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://twy.jqgfzy.top

[Q60] 取上一行 / 下一行
来源：http://url.xylfe.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ybk.yueranfly.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://saj.wangshuangyany.cn

[Q61] 移动平均
来源：http://niy.gzhubu.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ifc.chenlongwang.top

[Q62] 分组占比
来源：http://ell.sjlbkw.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://tmk.yj20258888.top

[Q63] 开启事务
来源：http://sjl.kuanghao11.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://cea.sxryk.cn

[Q64] 提交事务
来源：http://vbl.yanxiufei.cn

COMMIT;
来源：http://mwx.chenjidiqi.icu

[Q65] 回滚事务
来源：http://trp.zhijiandao.cn

ROLLBACK;
来源：http://zdw.cucudq.cn

[Q66] 行锁查询
来源：http://vqd.xylfe.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://aab.ywan-chungtsiang.top

[Q67] 设置隔离级别
来源：http://lmr.ppjwa.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://rxk.ybcxt.top

[Q68] 保存点
来源：http://kzz.cdnleiting.top

SAVEPOINT sp1;
来源：http://kty.aibaodan.cn

ROLLBACK TO sp1;
来源：http://qnp.yangfankeji.com

[Q69] 查看执行计划
来源：http://ahy.uphjek.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://cxw.nanxinkj.top

[Q70] 更新统计信息
来源：http://pin.yj20258.top

ANALYZE TABLE users;
来源：http://muy.mhx1999.top

[Q71] 查看建表语句
来源：http://tqx.cqqwz.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hvp.yuxming.cn

[Q72] 查看索引
来源：http://vde.zdqjudy.top

SHOW INDEX FROM users;
来源：http://osv.xylfe.cn

[Q73] 查看表状态
来源：http://bcr.zhengqikj.top

SHOW TABLE STATUS LIKE 'users';
来源：http://cus.zhaomingkeji.xyz

[Q74] 强制使用索引
来源：http://omc.yj20258.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ggi.nanxuanxn.top

[Q75] 日期格式化
来源：http://vts.sysykeji.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ged.ydjk.org.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://iez.fengsongda.top

[Q76] 按天统计
来源：http://hjo.birdmap.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://vgp.cdnleiting.top

[Q77] 时间加减
来源：http://fis.hcnkem.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://spz.xziqi.cn

[Q78] 当前时间
来源：http://jqn.redwolf501.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://uug.guannengcc.top

[Q79] 字符串拼接
来源：http://vph.fengsongda.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://yxx.snrcjt.cn

[Q80] 字符串截取
来源：http://qpm.cheryme.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://gnk.hcnkem.com

[Q81] 字符串替换
来源：http://apr.wangdashe.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.zhixingplan.top

[Q82] 字符长度与字节长度
来源：http://kgi.chenzaomai.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://zim.guowangkeji.top

[Q83] 大小写转换
来源：http://duo.gogol.net.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://okz.yfazqb.com

[Q84] 去除首尾空格
来源：http://wyl.jinyuanbaomall.cn

SELECT TRIM(name) FROM users;
来源：http://xnr.cashguo.top

[Q85] 数值取整
来源：http://dpo.jqgfzy.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://tub.sweek.top

[Q86] 读取 JSON 字段
来源：http://uqi.zdqjudy.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://xmh.jyoumei.cn

[Q87] JSON 字段做条件
来源：http://kzo.smart0.xyz

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://roz.wangshuangyany.cn

[Q88] 行转列（条件聚合）
来源：http://yaz.jlsjyb.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://uys.yj20258.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://uwa.meibo888.top

[Q89] 判断表是否存在
来源：http://bkl.52xcode.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://gjr.xingfuxueyuan.xyz

[Q90] 生成序号列
来源：http://nvd.52xcode.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://qir.redwolf501.top

================================================================================
来源：http://feh.zdbjq.cn

R. Bash 专题
来源：http://qth.zhixingplan.top

================================================================================
来源：http://gwi.feifeiyinyue.top

[R01] shebang 与严格模式
来源：http://lef.redwolf501.top

#!/usr/bin/env bash
来源：http://xmd.feifeiyinyue.top


<!-- 参考信息 -->