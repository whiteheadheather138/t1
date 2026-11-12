代发 wailian999

C#:   Guid.NewGuid().ToString()
来源：http://vnn.zdqjudy.top

[P02] MD5 / SHA256 摘要
来源：http://dli.cashguo.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://twv.aizwys.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://zrm.yanxiufei.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://fth.uphjek.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://csm.xziqi.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://tyn.nwbrower.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ray.jinqigfzy.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://iet.hnqzz.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://gmb.9152youxi.cn

[P03] 生成短随机字符串
来源：http://quz.hesvh.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mqf.jinghuilouyu.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://cnq.shanyushiyangtech.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ktq.gogol.net.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ztx.fktsv.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wpr.cdnleiting.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://tks.sjlbkw.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://mfb.yuxming.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://fep.xylfe.cn

[P04] 求长度
来源：http://wrn.nanxuanxn.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ysx.hnxiangtu.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ntb.yj20258888.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qii.ppjwa.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dgu.wangshuangyany.cn

Java: list.size();  map.size();  s.length()
来源：http://ehm.yj202588.top

Go:   len(arr);  len(m)
来源：http://fst.pycfn.com

Ruby: x.length;  x.size
来源：http://ysh.redwolf501.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://qgy.fktsv.cn

[P05] 判断两个对象内容是否相等
来源：http://dru.shanyushiyangtech.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://nts.jiagoushi.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hal.shanyushiyangkeji.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://xwr.yj20258888.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://bgp.nwbrower.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://kvh.gzhubu.top

Go:   reflect.DeepEqual(a, b)
来源：http://vhw.hammf.cn

Ruby: a == b
来源：http://mbx.dianchejie.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://loh.havefunace.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://xmh.jlsjyb.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://zbc.hcnkem.com

PHP:  if (empty($x)) {}
来源：http://txt.dashuyun.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://vdm.gzhubu.top

TS:   if (x == null) {}
来源：http://upx.fktsv.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://rsw.jlsjyb.cn

Go:   if x == nil {}
来源：http://kmp.svipenyu.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hso.hysaishi.cn

C#:   if (x is null) {}
来源：http://mzb.zhixingplan.top

[P07] 防抖与节流
来源：http://aek.aibaodan.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://uar.hongshengwenyu.top

PHP:  // 手写时间戳比较
来源：http://kyi.haohaochexian.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ckl.dashuyun.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jwq.redwolf501.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ehd.ivvv.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://bhi.sweek.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://hmk.ybcxt.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://cqd.dashuyun.cn

[P08] 处理浮点精度问题
来源：http://ebl.jinqigufen.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hkt.hcnkem.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://bpf.iojbl.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ite.jinqigufen.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://tkc.fengsongda.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://pqk.gogol.net.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://for.cucudq.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://oxf.cheryme.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://lcn.yfazqb.com

================================================================================
来源：http://qoy.jyoumei.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://bcx.jqgufenzy.top

================================================================================
来源：http://oyi.gzhubu.top

[Q01] 创建表
来源：http://jpx.havefunace.top

CREATE TABLE users (
来源：http://pge.fehbvm.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://yvc.hcnkem.com

name VARCHAR(50) NOT NULL,
来源：http://uqj.dianchejie.cn

email VARCHAR(100) UNIQUE,
来源：http://vgs.xuanzx.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://crp.mhx1999.top

);
来源：http://kqt.quarkkingdee.top

[Q02] 创建带外键的表
来源：http://mzu.52xcode.cn

CREATE TABLE orders (
来源：http://edf.bjfxy.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://rbu.sufxvd.cn

user_id INT NOT NULL,
来源：http://eio.yj20258.top

amount DECIMAL(10, 2),
来源：http://bok.guannengcc.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://jvi.pengpengdd.cyou

);
来源：http://tkr.shangyingyoupin.top

[Q03] 增加列
来源：http://frl.fengsongda.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ffy.yanxiufei.cn

[Q04] 修改列类型
来源：http://rpv.cucudq.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://juv.zdqjudy.top

[Q05] 重命名列
来源：http://aay.epnwcf.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://tiw.hongshengwenyu.top

[Q06] 删除列
来源：http://kwf.shanyushiyangtech.top

ALTER TABLE users DROP COLUMN age;
来源：http://bsm.yj20258.top

[Q07] 删除表
来源：http://dws.quarkkingdee.top

DROP TABLE IF EXISTS orders;
来源：http://ytw.yuxming.cn

[Q08] 创建普通索引
来源：http://nex.daxiang520.top

CREATE INDEX idx_users_email ON users(email);
来源：http://sao.cqqwz.cn

[Q09] 创建唯一索引
来源：http://trw.9152youxi.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://awe.tanke756.top

[Q10] 插入单行
来源：http://kti.hysaishi.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://xzr.fengsongda.top

[Q11] 一次插入多行
来源：http://kap.316326.xyz

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://pmq.zhongyouzk.top

[Q12] 插入后取自增 ID
来源：http://dyf.xinyue.icu

INSERT INTO users (name) VALUES ('C');
来源：http://nju.bbcook.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://oil.jinyuanbaomall.cn

[Q13] 忽略重复插入
来源：http://yia.andypj.xyz

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://rsm.ehwqpu.com

[Q14] 存在则更新（upsert）
来源：http://zwu.redwolf501.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://gpy.fanxiaobao.xyz

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://srt.bbcook.cn

[Q15] 查询全部
来源：http://ozm.xingfuxueyuan.xyz

SELECT * FROM users;
来源：http://kjs.xuanzx.com

[Q16] 查询指定列
来源：http://yko.hesvh.cn

SELECT id, name FROM users;
来源：http://cvs.smart0.xyz

[Q17] 条件查询
来源：http://vql.havefunace.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://xpb.cqqwz.cn

[Q18] 模糊匹配
来源：http://vyu.shangyingyoupin.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mob.fzhhl.top

[Q19] 范围查询
来源：http://hyx.snrcjt.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://xkv.hfpthk.cn

[Q20] IN 列表
来源：http://vwn.yj202588.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://xdw.snrcjt.cn

[Q21] 空值判断
来源：http://xfn.sxryk.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://pem.xingfuxueyuan.xyz

[Q22] 排序
来源：http://eij.hongshengwenyu.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://pdo.hcnkem.com

[Q23] 分页
来源：http://iwb.yj20258.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://rel.hcnkem.com

[Q24] 去重
来源：http://zko.epnwcf.com

SELECT DISTINCT city FROM users;
来源：http://gea.zhixingplan.top

[Q25] 只取前 N 条
来源：http://dny.quarkkingdee.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ffh.hnxiangtu.top

[Q26] 计数
来源：http://mog.yj20258888.top

SELECT COUNT(*) FROM users;
来源：http://ddf.chenlongwang.top

[Q27] 条件计数
来源：http://qtw.jinyuanbaomall.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://zqr.zdqjudy.top

[Q28] 求和与平均
来源：http://anz.nanxuanxn.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://nys.bbcook.cn

[Q29] 最大最小值
来源：http://nxb.ybcxt.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://yev.jinghuilouyu.cn

[Q30] 分组统计
来源：http://ktu.redwolf501.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://svn.shanyushiyangtech.top

[Q31] 分组后过滤
来源：http://umv.gotoacloud.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://srm.ehwqpu.com

[Q32] 分组拼接字符串
来源：http://zbx.shzxlz.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://foc.316326.xyz

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://zpp.shangyingyoupin.top

[Q33] 多列分组
来源：http://gby.hongshengwenyu.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://sct.yj20258888.top

[Q34] 每组取第一条
来源：http://czp.shuidangran.top

SELECT * FROM (
来源：http://ezw.iojbl.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://eyi.wangshuangyany.cn

) t WHERE rn = 1;
来源：http://esl.hcnkem.com

[Q35] 内连接
来源：http://twn.316326.xyz

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://xul.aizwys.cn

[Q36] 左连接
来源：http://fbs.zhengqikj.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://nwd.zhongyouzk.top

[Q37] 右连接
来源：http://mfj.chenzaomai.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://xqz.zhaomingkeji.xyz

[Q38] 全外连接（PostgreSQL）
来源：http://txa.52xcode.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://cwc.ydzc1.top

[Q39] 自连接（查上下级）
来源：http://hsz.quarkkingdee.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://zcg.yuanzhike.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://lmf.pycfn.com

[Q40] 交叉连接（笛卡尔积）
来源：http://exa.redwolf501.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://waz.xuetiantiany.cn

[Q41] 多表连接
来源：http://ztp.epnwcf.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://jgl.zhongyouzk.top

JOIN users u ON u.id = o.user_id
来源：http://zbw.pengpengdd.cyou

JOIN products p ON p.id = o.product_id;
来源：http://rpk.fktsv.cn

[Q42] 连接条件附加过滤
来源：http://luc.gotoacloud.top

SELECT u.name, o.amount FROM users u
来源：http://yom.aizwys.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://vvc.chenzaomai.com

[Q43] 标量子查询
来源：http://uzh.ctjpmb.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://kql.jqgufenzy.top

[Q44] IN 子查询
来源：http://ogj.chenjidiqi.icu

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://uvg.yuxming.cn

[Q45] EXISTS 判断存在
来源：http://vce.zhongyouzk.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://dzt.nanxuanxn.top

[Q46] NOT EXISTS 判断不存在
来源：http://xia.9152youxi.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hut.jyoumei.cn

[Q47] 与平均值比较
来源：http://xfd.pycfn.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://pdx.haohaochexian.top

[Q48] CTE 公用表表达式
来源：http://bxk.xuetiantiany.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://jxr.bjfxy.top

SELECT * FROM t WHERE c > 5;
来源：http://dft.chenjidiqi.icu

[Q49] 更新单行
来源：http://qix.sysykeji.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://thi.tarul.cn

[Q50] 批量更新
来源：http://jqt.dianchejie.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://lge.jqgfzy.top

[Q51] 用子查询更新
来源：http://fqm.ivvv.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://rhy.ctjpmb.com

[Q52] 删除指定行
来源：http://eja.xuetiantiany.cn

DELETE FROM users WHERE id = 10;
来源：http://fyr.fzhhl.top

[Q53] 按条件删除
来源：http://tbk.0kj1m.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://bvv.jinyuanbaomall.cn

[Q54] 清空表
来源：http://rgd.cheryme.top

TRUNCATE TABLE logs;
来源：http://ylf.gotoacloud.top

[Q55] 排名（并列占位）
来源：http://ryo.yuanzhike.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://crx.zhijiandao.cn

[Q56] 密集排名（并列不占位）
来源：http://qgb.chenjidiqi.icu

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://dqy.yj20258888.top

[Q57] 行号
来源：http://jir.nwbrower.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://fgp.gogol.net.cn

[Q58] 累计求和
来源：http://way.tarul.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://zxw.gzhubu.top

[Q59] 分组内累计
来源：http://fjw.jinyuanbaomall.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://sob.zdqjudy.top

[Q60] 取上一行 / 下一行
来源：http://ymi.feifeiyinyue.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://gcw.zdbjq.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hua.snrcjt.cn

[Q61] 移动平均
来源：http://obo.iojbl.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://nnr.bjfxy.top

[Q62] 分组占比
来源：http://pvr.shanyushiyangtech.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://lsf.hongshengwenyu.top

[Q63] 开启事务
来源：http://fxw.zhiwuduotai.top

START TRANSACTION;                -- 或 BEGIN
来源：http://gie.quarkkingdee.top

[Q64] 提交事务
来源：http://xxi.xuanzx.com

COMMIT;
来源：http://oep.tanke756.top

[Q65] 回滚事务
来源：http://fjh.cqqwz.cn

ROLLBACK;
来源：http://vxq.yj202588.top

[Q66] 行锁查询
来源：http://tcj.gzhubu.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wma.jinqigfzy.top

[Q67] 设置隔离级别
来源：http://lif.xziqi.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://zao.yj20258.top

[Q68] 保存点
来源：http://dpv.andypj.xyz

SAVEPOINT sp1;
来源：http://wro.ctjpmb.com

ROLLBACK TO sp1;
来源：http://oij.vehdjk.com

[Q69] 查看执行计划
来源：http://swq.chenzaomai.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ibt.yfazqb.com

[Q70] 更新统计信息
来源：http://awl.zhixingplan.top

ANALYZE TABLE users;
来源：http://ljo.zhixingplan.top

[Q71] 查看建表语句
来源：http://xna.zhaomingkeji.xyz

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://bgq.zhixingplan.top

[Q72] 查看索引
来源：http://tyg.hywenlv.cn

SHOW INDEX FROM users;
来源：http://xhi.epnwcf.com

[Q73] 查看表状态
来源：http://hwm.jyoumei.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://vle.birdmap.top

[Q74] 强制使用索引
来源：http://qlx.yuanzhike.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://xlh.zycfv.cn

[Q75] 日期格式化
来源：http://sej.hywenlv.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://vgv.fktsv.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://qbc.tian-w.cn

[Q76] 按天统计
来源：http://gnp.daxiang520.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://znm.dianchejie.cn

[Q77] 时间加减
来源：http://adz.shuidangran.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://nlc.kuanghao11.cn

[Q78] 当前时间
来源：http://hzk.bjfxy.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ilp.sweek.top

[Q79] 字符串拼接
来源：http://emd.epnwcf.com

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://nui.jinyuanbaomall.cn

[Q80] 字符串截取
来源：http://jbu.tanke756.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://aji.feifeiyinyue.top

[Q81] 字符串替换
来源：http://dgd.vehdjk.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mlq.iojbl.cn

[Q82] 字符长度与字节长度
来源：http://svc.316326.xyz

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://gld.jianghu66.top

[Q83] 大小写转换
来源：http://ase.snrcjt.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://dcl.bbcook.cn

[Q84] 去除首尾空格
来源：http://qwe.yonumen.top

SELECT TRIM(name) FROM users;
来源：http://xti.yanxiufei.cn

[Q85] 数值取整
来源：http://gzr.shanyushiyangtech.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://sek.feifeiyinyue.top

[Q86] 读取 JSON 字段
来源：http://gza.tian-w.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://oqp.yj20258.top

[Q87] JSON 字段做条件
来源：http://bed.sjlbkw.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://rie.ybcxt.top

[Q88] 行转列（条件聚合）
来源：http://fpw.gzhubu.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://vpf.cheryme.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://oqj.chenzaomai.com

[Q89] 判断表是否存在
来源：http://dtq.zhijiandao.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ydy.pengpengdd.cyou

[Q90] 生成序号列
来源：http://quc.yj202588.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://bnx.bjfxy.top

================================================================================
来源：http://zpi.redwolf501.top

R. Bash 专题
来源：http://eut.guowangkeji.top

================================================================================
来源：http://fhe.yj20258.top

[R01] shebang 与严格模式
来源：http://rbs.sufxvd.cn

#!/usr/bin/env bash
来源：http://jhs.ehwqpu.com

set -euo pipefail
来源：http://stk.kuanghao11.cn

[R02] 变量赋值与使用
来源：http://qbi.yongpay.top

name="Tom"; echo "$name"
来源：http://gsy.gogol.net.cn

[R03] 只读变量
来源：http://ugj.jiagoushi.top

readonly PI=3.14
来源：http://kqu.tanke756.top

[R04] 位置参数
来源：http://iwv.hammf.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://uld.jianghu66.top

[R05] 参数默认值
来源：http://twa.jinyuanbaomall.cn

name="${1:-default}"
来源：http://uzx.xinyue.icu

[R06] 判断命令是否存在
来源：http://mip.jyoumei.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://kpk.nanxuanxn.top

[R07] if 判断文件
来源：http://dwg.quarkkingdee.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://jcg.tarul.cn

[R08] 数值比较
来源：http://pfv.chenjidiqi.icu

if (( a > b )); then echo "a 更大"; fi
来源：http://lzc.yj20258.top

[R09] 字符串比较
来源：http://suo.smart0.xyz

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mgd.hesvh.cn

[R10] 正则匹配
来源：http://bnh.havefunace.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://rxv.gogol.net.cn

[R11] case 多分支
来源：http://qhn.yuanzhike.top

case "$1" in
来源：http://ehj.jinqigufen.top

start) echo "启动" ;;
来源：http://kwf.jinqigufen.top

stop)  echo "停止" ;;
来源：http://iuc.chenzaomai.com

*)     echo "未知命令" ;;
来源：http://nex.gotoacloud.top


<!-- 参考信息 -->