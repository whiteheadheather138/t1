代发 wailian999

Ruby: Digest::SHA256.hexdigest(s)
来源：http://yog.gzhubu.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://cbf.fengsongda.top

[P03] 生成短随机字符串
来源：http://lak.yj202588.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://qmb.chenlongwang.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://zqs.xuanzx.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.epnwcf.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://otg.ydzc1.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://aaj.c1oappe.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://drj.nanxuanxn.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://nii.vqdsnc.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://uad.yueranfly.top

[P04] 求长度
来源：http://roi.hcnkem.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ehr.jinqigufen.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://anq.yj202588.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://uov.yvedp.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://uxv.hfpthk.cn

Java: list.size();  map.size();  s.length()
来源：http://fsa.fanxiaobao.xyz

Go:   len(arr);  len(m)
来源：http://gvl.fktsv.cn

Ruby: x.length;  x.size
来源：http://vkr.bbcook.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://mcz.fengsongda.top

[P05] 判断两个对象内容是否相等
来源：http://kfj.fanxiaobao.xyz

Py:   a == b              # 列表与字典递归比较内容
来源：http://eeg.aizwys.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://dax.316326.xyz

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ber.gogol.net.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ttd.nwbrower.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://pqz.wangdashe.top

Go:   reflect.DeepEqual(a, b)
来源：http://snf.zhixingplan.top

Ruby: a == b
来源：http://rsz.316326.xyz

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://bna.zhongyouzk.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://vhw.xziqi.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://leh.meibo888.top

PHP:  if (empty($x)) {}
来源：http://xld.ywan-chungtsiang.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://pod.smart0.xyz

TS:   if (x == null) {}
来源：http://xrl.yj202588.top

Java: if (x == null || x.isEmpty()) {}
来源：http://qfg.mhx1999.top

Go:   if x == nil {}
来源：http://ujz.havefunace.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://fik.aibaodan.cn

C#:   if (x is null) {}
来源：http://rvu.ivvv.top

[P07] 防抖与节流
来源：http://nzb.ivvv.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://fzr.gotoacloud.top

PHP:  // 手写时间戳比较
来源：http://dwo.fktsv.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vis.zycfv.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dwm.yueranfly.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wwd.shangyingyoupin.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://qji.nanxinkj.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://rll.yj202588.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://guo.yfazqb.com

[P08] 处理浮点精度问题
来源：http://rch.shangyingyoupin.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://kso.sweek.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://rry.nanxuanxn.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://tzc.haohaochexian.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://vpw.c1oappe.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://txq.jyoumei.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ekn.52xcode.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hrb.9152youxi.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ynv.aizwys.cn

================================================================================
来源：http://rge.0kj1m.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ens.epnwcf.com

================================================================================
来源：http://luf.redwolf501.top

[Q01] 创建表
来源：http://yme.jinyuanbaomall.cn

CREATE TABLE users (
来源：http://iuj.zdbjq.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://lgx.hammf.cn

name VARCHAR(50) NOT NULL,
来源：http://mce.zhoulong.xyz

email VARCHAR(100) UNIQUE,
来源：http://yba.svipenyu.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hfu.0kj1m.cn

);
来源：http://iyw.cdnleiting.top

[Q02] 创建带外键的表
来源：http://rsn.snrcjt.cn

CREATE TABLE orders (
来源：http://tqw.jianghu66.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://nok.yfazqb.com

user_id INT NOT NULL,
来源：http://bhe.xinyue.icu

amount DECIMAL(10, 2),
来源：http://wbc.andypj.xyz

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ntg.cqqwz.cn

);
来源：http://caq.yfazqb.com

[Q03] 增加列
来源：http://ozk.pycfn.com

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mxz.fktsv.cn

[Q04] 修改列类型
来源：http://wyi.tian-w.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://xwf.ppjwa.cn

[Q05] 重命名列
来源：http://kjw.zhiwuduotai.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://axw.chenjidiqi.icu

[Q06] 删除列
来源：http://bvt.pycfn.com

ALTER TABLE users DROP COLUMN age;
来源：http://eqf.fanxiaobao.xyz

[Q07] 删除表
来源：http://vpt.chenjidiqi.icu

DROP TABLE IF EXISTS orders;
来源：http://rsd.bjfxy.top

[Q08] 创建普通索引
来源：http://vtu.52xcode.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://vbt.chenzaomai.com

[Q09] 创建唯一索引
来源：http://qih.sweek.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://bth.hongshengwenyu.top

[Q10] 插入单行
来源：http://tab.nanxinkj.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://aee.xuetiantiany.cn

[Q11] 一次插入多行
来源：http://qdl.sweek.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://rux.hesvh.cn

[Q12] 插入后取自增 ID
来源：http://xfb.zhiwuduotai.top

INSERT INTO users (name) VALUES ('C');
来源：http://znx.jqgufenzy.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://kih.zhongyouzk.top

[Q13] 忽略重复插入
来源：http://cno.gaohongyu789.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ngx.gzhubu.top

[Q14] 存在则更新（upsert）
来源：http://bbv.fanxiaobao.xyz

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://qwn.chenzaomai.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://pov.zhixingplan.top

[Q15] 查询全部
来源：http://xev.redwolf501.top

SELECT * FROM users;
来源：http://ywq.pycfn.com

[Q16] 查询指定列
来源：http://npf.wangshuangyany.cn

SELECT id, name FROM users;
来源：http://zhi.shanyushiyangkeji.top

[Q17] 条件查询
来源：http://ibt.cucudq.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://rro.ydzc1.top

[Q18] 模糊匹配
来源：http://pon.tanke756.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://jli.dianchejie.cn

[Q19] 范围查询
来源：http://oxn.zhengqikj.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ret.xuetiantiany.cn

[Q20] IN 列表
来源：http://zqb.yj20258.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://cik.fengsongda.top

[Q21] 空值判断
来源：http://iep.gzhubu.top

SELECT * FROM users WHERE email IS NULL;
来源：http://jqi.jiagoushi.top

[Q22] 排序
来源：http://tgx.yueranfly.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://vim.quarkkingdee.top

[Q23] 分页
来源：http://lao.c1oappe.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ifj.pycfn.com

[Q24] 去重
来源：http://trq.mhx1999.top

SELECT DISTINCT city FROM users;
来源：http://ipn.wangdashe.top

[Q25] 只取前 N 条
来源：http://mgb.jyoumei.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://lyc.chenjidiqi.icu

[Q26] 计数
来源：http://mrm.yj20258888.top

SELECT COUNT(*) FROM users;
来源：http://mqx.yuxming.cn

[Q27] 条件计数
来源：http://ciq.sweek.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://bkf.yanxiufei.cn

[Q28] 求和与平均
来源：http://qep.bjfxy.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wyh.zycfv.cn

[Q29] 最大最小值
来源：http://adz.meibo888.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://qtq.birdmap.top

[Q30] 分组统计
来源：http://hkj.yfazqb.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hyr.fengsongda.top

[Q31] 分组后过滤
来源：http://ken.jlsjyb.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://cyg.jinqigfzy.top

[Q32] 分组拼接字符串
来源：http://owf.fktsv.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://yxu.meibo888.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://bur.316326.xyz

[Q33] 多列分组
来源：http://nje.zdbjq.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://sdu.jiagoushi.top

[Q34] 每组取第一条
来源：http://fxp.yuxming.cn

SELECT * FROM (
来源：http://jwy.tianlin.xyz

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wmv.hysaishi.cn

) t WHERE rn = 1;
来源：http://aie.haohaochexian.top

[Q35] 内连接
来源：http://gpg.nanxuanxn.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wca.sjlbkw.cn

[Q36] 左连接
来源：http://qlc.hnqzz.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ytd.xziqi.cn

[Q37] 右连接
来源：http://lml.fengsongda.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://zpn.hywenlv.cn

[Q38] 全外连接（PostgreSQL）
来源：http://nsv.jqgufenzy.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://yhx.jiagoushi.top

[Q39] 自连接（查上下级）
来源：http://iuq.wangshuangyany.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://yki.andypj.xyz

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://etb.daxiang520.top

[Q40] 交叉连接（笛卡尔积）
来源：http://bde.jinghuilouyu.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mgf.9152youxi.cn

[Q41] 多表连接
来源：http://jvl.vehdjk.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://tlz.9152youxi.cn

JOIN users u ON u.id = o.user_id
来源：http://nrx.jqgfzy.top

JOIN products p ON p.id = o.product_id;
来源：http://sgm.xinyue.icu

[Q42] 连接条件附加过滤
来源：http://mbu.shzxlz.cn

SELECT u.name, o.amount FROM users u
来源：http://gly.jinghuilouyu.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://gpm.ctjpmb.com

[Q43] 标量子查询
来源：http://shn.sweek.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://oaq.jiagoushi.top

[Q44] IN 子查询
来源：http://cgg.bbcook.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://qcj.zhengqikj.top

[Q45] EXISTS 判断存在
来源：http://lxu.aizwys.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kmm.chenlongwang.top

[Q46] NOT EXISTS 判断不存在
来源：http://rjc.jinghuilouyu.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qyv.zhongyouzk.top

[Q47] 与平均值比较
来源：http://egl.fengsongda.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://kjw.fanxiaobao.xyz

[Q48] CTE 公用表表达式
来源：http://zzh.chenzaomai.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://bjl.pengpengdd.cyou

SELECT * FROM t WHERE c > 5;
来源：http://mzr.shanyushiyangtech.top

[Q49] 更新单行
来源：http://xyd.yonumen.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wvb.yonumen.top

[Q50] 批量更新
来源：http://lrd.hnqzz.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://efq.yongpay.top

[Q51] 用子查询更新
来源：http://dgx.ydjk.org.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://rmc.yj20258888.top

[Q52] 删除指定行
来源：http://dta.tarul.cn

DELETE FROM users WHERE id = 10;
来源：http://lui.jinyuanbaomall.cn

[Q53] 按条件删除
来源：http://eyl.hammf.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hss.bjfxy.top

[Q54] 清空表
来源：http://ngk.meibo888.top

TRUNCATE TABLE logs;
来源：http://iod.nanxinkj.top

[Q55] 排名（并列占位）
来源：http://klg.jiagoushi.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://pnf.vqdsnc.cn

[Q56] 密集排名（并列不占位）
来源：http://evg.gotoacloud.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://fpg.yonumen.top

[Q57] 行号
来源：http://lbw.jinqigfzy.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://sty.daria6918.cn

[Q58] 累计求和
来源：http://rxw.sweek.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://lzu.haohaochexian.top

[Q59] 分组内累计
来源：http://dgl.gogol.net.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wqo.hfpthk.cn

[Q60] 取上一行 / 下一行
来源：http://lnm.yj20258888.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://kwx.yuanzhike.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://bfr.jqgfzy.top

[Q61] 移动平均
来源：http://teb.jinqigfzy.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wct.ctjpmb.com

[Q62] 分组占比
来源：http://zpu.havefunace.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://vuj.sjlbkw.cn

[Q63] 开启事务
来源：http://zge.cdnleiting.top

START TRANSACTION;                -- 或 BEGIN
来源：http://zds.yanxiufei.cn

[Q64] 提交事务
来源：http://oee.vqdsnc.cn

COMMIT;
来源：http://ase.xylfe.cn

[Q65] 回滚事务
来源：http://yjq.hcnkem.com

ROLLBACK;
来源：http://sgl.jiagoushi.top

[Q66] 行锁查询
来源：http://kdc.vqdsnc.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://jdv.zhaomingkeji.xyz

[Q67] 设置隔离级别
来源：http://tvu.zhijiandao.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://xll.xuanzx.com

[Q68] 保存点
来源：http://hcq.jyoumei.cn

SAVEPOINT sp1;
来源：http://fdp.iojbl.cn

ROLLBACK TO sp1;
来源：http://xxt.xingfuxueyuan.xyz

[Q69] 查看执行计划
来源：http://cbw.xinyue.icu

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://puq.uphjek.com

[Q70] 更新统计信息
来源：http://hgf.pycfn.com

ANALYZE TABLE users;
来源：http://grm.nanxuanxn.top

[Q71] 查看建表语句
来源：http://syd.ybcxt.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://bel.yj20258888.top

[Q72] 查看索引
来源：http://hms.zhoulong.xyz

SHOW INDEX FROM users;
来源：http://bgu.nwbrower.top

[Q73] 查看表状态
来源：http://iei.gogol.net.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://jzb.cucudq.cn

[Q74] 强制使用索引
来源：http://nis.sjlbkw.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ice.hfpthk.cn

[Q75] 日期格式化
来源：http://umj.hnqzz.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://vhl.daxiang520.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://olf.ywan-chungtsiang.top

[Q76] 按天统计
来源：http://dbj.sysykeji.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://yiz.yueranfly.top

[Q77] 时间加减
来源：http://wwf.aibaodan.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://fud.shuidangran.top

[Q78] 当前时间
来源：http://ybd.vqdsnc.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mdy.hongshengwenyu.top

[Q79] 字符串拼接
来源：http://ctf.cashguo.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://rgk.kuanghao11.cn

[Q80] 字符串截取
来源：http://bvb.sxryk.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://bnd.9152youxi.cn

[Q81] 字符串替换
来源：http://tyn.nanxuanxn.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://den.guowangkeji.top

[Q82] 字符长度与字节长度
来源：http://svs.yvedp.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://umo.ppjwa.cn

[Q83] 大小写转换
来源：http://zif.jyoumei.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://gil.jiagoushi.top

[Q84] 去除首尾空格
来源：http://rwz.vehdjk.com

SELECT TRIM(name) FROM users;
来源：http://iud.dianchejie.cn

[Q85] 数值取整
来源：http://olo.bjfxy.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ekr.ydzc1.top

[Q86] 读取 JSON 字段
来源：http://lgk.guannengcc.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wie.yonumen.top

[Q87] JSON 字段做条件
来源：http://cda.jinqigfzy.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://aha.shangyingyoupin.top

[Q88] 行转列（条件聚合）
来源：http://spa.daria6918.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://usd.andypj.xyz

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://puq.zycfv.cn

[Q89] 判断表是否存在
来源：http://csi.ydjk.org.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://bak.pengpengdd.cyou

[Q90] 生成序号列
来源：http://zfd.aizwys.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://uxl.yuanzhike.top

================================================================================
来源：http://fsi.bbcook.cn

R. Bash 专题
来源：http://uhr.cashguo.top

================================================================================
来源：http://roi.shanyushiyangtech.top

[R01] shebang 与严格模式
来源：http://rjn.316326.xyz

#!/usr/bin/env bash
来源：http://jed.zhaomingkeji.xyz

set -euo pipefail
来源：http://zjf.dianchejie.cn

[R02] 变量赋值与使用
来源：http://rab.fehbvm.com

name="Tom"; echo "$name"
来源：http://grz.xylfe.cn

[R03] 只读变量
来源：http://dks.birdmap.top

readonly PI=3.14
来源：http://qoo.zhongyouzk.top

[R04] 位置参数
来源：http://qev.shuidangran.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://pms.yuxming.cn

[R05] 参数默认值
来源：http://hln.zdqjudy.top

name="${1:-default}"
来源：http://zff.sxryk.cn

[R06] 判断命令是否存在
来源：http://wwd.yueranfly.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://zqf.jyoumei.cn

[R07] if 判断文件
来源：http://gnw.gzhubu.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://kzd.xziqi.cn

[R08] 数值比较
来源：http://xll.yueranfly.top

if (( a > b )); then echo "a 更大"; fi
来源：http://pko.bjfxy.top

[R09] 字符串比较
来源：http://vui.birdmap.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://psf.uphjek.com

[R10] 正则匹配
来源：http://flg.birdmap.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://sza.xuanzx.com

[R11] case 多分支
来源：http://tjj.cdnleiting.top

case "$1" in
来源：http://sbo.sxryk.cn

start) echo "启动" ;;
来源：http://had.yj202588.top

stop)  echo "停止" ;;
来源：http://zmv.bjfxy.top

*)     echo "未知命令" ;;
来源：http://naw.fzhhl.top

esac
来源：http://qsl.tianlin.xyz

[R12] for 遍历文件
来源：http://tje.xuetiantiany.cn

for f in *.txt; do echo "$f"; done
来源：http://zue.fzhhl.top

[R13] for 计数循环
来源：http://jex.yj20258.top

for i in {1..10}; do echo "$i"; done
来源：http://gkk.gotoacloud.top

[R14] C 风格 for
来源：http://yfx.birdmap.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://skw.jinghuilouyu.cn

[R15] while 逐行读文件
来源：http://ahk.yongpay.top


<!-- 参考信息 -->