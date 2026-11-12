代发 wailian999

Ruby: Digest::SHA256.hexdigest(s)
来源：http://rna.snrcjt.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://agc.cheryme.top

[P03] 生成短随机字符串
来源：http://unl.jinyuanbaomall.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://kgs.ydzc1.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://sur.bbcook.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kwe.hfpthk.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://yhv.yuanzhike.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://kao.xingfuxueyuan.xyz

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://tob.bbcook.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://itt.fehbvm.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://bok.chenlongwang.top

[P04] 求长度
来源：http://ced.havefunace.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wxl.hesvh.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://yji.xuetiantiany.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ejq.sysykeji.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://pma.nwbrower.top

Java: list.size();  map.size();  s.length()
来源：http://svv.wangdashe.top

Go:   len(arr);  len(m)
来源：http://obw.zdbjq.cn

Ruby: x.length;  x.size
来源：http://oeg.guowangkeji.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://fcp.sufxvd.cn

[P05] 判断两个对象内容是否相等
来源：http://mij.zhoulong.xyz

Py:   a == b              # 列表与字典递归比较内容
来源：http://dvb.zhoulong.xyz

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ghu.gogol.net.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hba.uphjek.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://jbj.ppjwa.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://irn.yuxming.cn

Go:   reflect.DeepEqual(a, b)
来源：http://trl.52xcode.cn

Ruby: a == b
来源：http://dgb.nanxinkj.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://bxd.zhixingplan.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://unk.yuanzhike.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://qdp.shzxlz.cn

PHP:  if (empty($x)) {}
来源：http://vbt.tianlin.xyz

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://xag.haohaochexian.top

TS:   if (x == null) {}
来源：http://rfn.iojbl.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://rfe.gaohongyu789.top

Go:   if x == nil {}
来源：http://yyc.bjfxy.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://xyk.wangshuangyany.cn

C#:   if (x is null) {}
来源：http://isa.gogol.net.cn

[P07] 防抖与节流
来源：http://ttx.bjfxy.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://prj.bbcook.cn

PHP:  // 手写时间戳比较
来源：http://nkn.shanyushiyangtech.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://seg.yuanzhike.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xxw.shanyushiyangkeji.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://zkg.gzhubu.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://jsr.birdmap.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://one.fengsongda.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hxg.fktsv.cn

[P08] 处理浮点精度问题
来源：http://dki.redwolf501.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mgf.cqqwz.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://xzp.cqqwz.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://seh.haohaochexian.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wli.sysykeji.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://xqs.guowangkeji.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://tjx.svipenyu.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://tuo.chenzaomai.com

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://nug.daxiang520.top

================================================================================
来源：http://kje.pengpengdd.cyou

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://vzx.bbcook.cn

================================================================================
来源：http://dag.tanke756.top

[Q01] 创建表
来源：http://thd.xylfe.cn

CREATE TABLE users (
来源：http://dze.hywenlv.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://bff.yj20258.top

name VARCHAR(50) NOT NULL,
来源：http://yku.zhengqikj.top

email VARCHAR(100) UNIQUE,
来源：http://aqo.yongpay.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mfy.0kj1m.cn

);
来源：http://dhl.yongpay.top

[Q02] 创建带外键的表
来源：http://bhi.cdnleiting.top

CREATE TABLE orders (
来源：http://alr.tanke756.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ngc.birdmap.top

user_id INT NOT NULL,
来源：http://sgk.fengsongda.top

amount DECIMAL(10, 2),
来源：http://gkp.chenjidiqi.icu

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://nif.epnwcf.com

);
来源：http://bpu.hnqzz.top

[Q03] 增加列
来源：http://ugn.zhaomingkeji.xyz

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://gth.sufxvd.cn

[Q04] 修改列类型
来源：http://aag.aizwys.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://utq.jinqigfzy.top

[Q05] 重命名列
来源：http://eol.cucudq.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ina.mhx1999.top

[Q06] 删除列
来源：http://cnt.9152youxi.cn

ALTER TABLE users DROP COLUMN age;
来源：http://efn.hfpthk.cn

[Q07] 删除表
来源：http://yng.snrcjt.cn

DROP TABLE IF EXISTS orders;
来源：http://oge.sysykeji.top

[Q08] 创建普通索引
来源：http://vfo.bbcook.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://yfv.smart0.xyz

[Q09] 创建唯一索引
来源：http://wjn.cheryme.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://srg.zhixingplan.top

[Q10] 插入单行
来源：http://yjg.svipenyu.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mrq.wangshuangyany.cn

[Q11] 一次插入多行
来源：http://cdl.jinqigufen.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ype.wangshuangyany.cn

[Q12] 插入后取自增 ID
来源：http://qtq.pycfn.com

INSERT INTO users (name) VALUES ('C');
来源：http://pof.chenlongwang.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://gdh.tanke756.top

[Q13] 忽略重复插入
来源：http://tib.vqdsnc.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wds.cashguo.top

[Q14] 存在则更新（upsert）
来源：http://eyo.andypj.xyz

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://jro.fengsongda.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://fgk.bbcook.cn

[Q15] 查询全部
来源：http://qpt.gzhubu.top

SELECT * FROM users;
来源：http://kee.yonumen.top

[Q16] 查询指定列
来源：http://dvr.wangshuangyany.cn

SELECT id, name FROM users;
来源：http://kmq.fehbvm.com

[Q17] 条件查询
来源：http://edt.guowangkeji.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://fss.redwolf501.top

[Q18] 模糊匹配
来源：http://pnr.shzxlz.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mxv.wangdashe.top

[Q19] 范围查询
来源：http://krw.nwbrower.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://lnz.yuanzhike.top

[Q20] IN 列表
来源：http://ubr.aibaodan.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://xes.haohaochexian.top

[Q21] 空值判断
来源：http://jrk.fzhhl.top

SELECT * FROM users WHERE email IS NULL;
来源：http://iby.andypj.xyz

[Q22] 排序
来源：http://ltz.mhx1999.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ouk.hammf.cn

[Q23] 分页
来源：http://dqo.tanke756.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ued.yj202588.top

[Q24] 去重
来源：http://vvb.zhijiandao.cn

SELECT DISTINCT city FROM users;
来源：http://czw.fehbvm.com

[Q25] 只取前 N 条
来源：http://syx.fktsv.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://fxh.yvedp.cn

[Q26] 计数
来源：http://zkn.sysykeji.top

SELECT COUNT(*) FROM users;
来源：http://lee.cqqwz.cn

[Q27] 条件计数
来源：http://ngk.chenjidiqi.icu

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wom.hcnkem.com

[Q28] 求和与平均
来源：http://qbo.xziqi.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://yoz.shuidangran.top

[Q29] 最大最小值
来源：http://whd.guowangkeji.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://ggh.hesvh.cn

[Q30] 分组统计
来源：http://tqu.ppjwa.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://vpf.dashuyun.cn

[Q31] 分组后过滤
来源：http://sui.haohaochexian.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://jkg.pycfn.com

[Q32] 分组拼接字符串
来源：http://bjq.fktsv.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ozy.hnxiangtu.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mqz.chenzaomai.com

[Q33] 多列分组
来源：http://mik.zdbjq.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://sut.gotoacloud.top

[Q34] 每组取第一条
来源：http://ynq.hcnkem.com

SELECT * FROM (
来源：http://hsx.hfpthk.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ora.aibaodan.cn

) t WHERE rn = 1;
来源：http://prl.fzhhl.top

[Q35] 内连接
来源：http://ito.yj202588.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://bwl.jianghu66.top

[Q36] 左连接
来源：http://qxv.cdnleiting.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://roj.ywan-chungtsiang.top

[Q37] 右连接
来源：http://jns.hysaishi.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://itg.sxryk.cn

[Q38] 全外连接（PostgreSQL）
来源：http://fog.ybcxt.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://doq.vqdsnc.cn

[Q39] 自连接（查上下级）
来源：http://vlv.wangshuangyany.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://fwf.yonumen.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://pfo.mhx1999.top

[Q40] 交叉连接（笛卡尔积）
来源：http://lke.xylfe.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://dwl.sweek.top

[Q41] 多表连接
来源：http://fpd.tarul.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://agb.jinyuanbaomall.cn

JOIN users u ON u.id = o.user_id
来源：http://gxa.xuetiantiany.cn

JOIN products p ON p.id = o.product_id;
来源：http://sgo.birdmap.top

[Q42] 连接条件附加过滤
来源：http://jpa.hnxiangtu.top

SELECT u.name, o.amount FROM users u
来源：http://oqf.zhongyouzk.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://zjt.shanyushiyangtech.top

[Q43] 标量子查询
来源：http://dfz.yueranfly.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://uew.ehwqpu.com

[Q44] IN 子查询
来源：http://ktn.zhengqikj.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://kju.yfazqb.com

[Q45] EXISTS 判断存在
来源：http://jid.cdnleiting.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ott.yanxiufei.cn

[Q46] NOT EXISTS 判断不存在
来源：http://yoo.aibaodan.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zff.zhiwuduotai.top

[Q47] 与平均值比较
来源：http://pzj.tarul.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wtc.xinyue.icu

[Q48] CTE 公用表表达式
来源：http://wzq.hnqzz.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://dga.aizwys.cn

SELECT * FROM t WHERE c > 5;
来源：http://zfx.cucudq.cn

[Q49] 更新单行
来源：http://tuu.hywenlv.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mus.sysykeji.top

[Q50] 批量更新
来源：http://ghv.havefunace.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://tuy.bjfxy.top

[Q51] 用子查询更新
来源：http://lle.shanyushiyangkeji.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://sjt.yuxming.cn

[Q52] 删除指定行
来源：http://ous.xziqi.cn

DELETE FROM users WHERE id = 10;
来源：http://wgd.fehbvm.com

[Q53] 按条件删除
来源：http://jjc.xinyue.icu

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ynv.zhoulong.xyz

[Q54] 清空表
来源：http://eod.pycfn.com

TRUNCATE TABLE logs;
来源：http://ezk.tarul.cn

[Q55] 排名（并列占位）
来源：http://cey.zhoulong.xyz

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://nal.dashuyun.cn

[Q56] 密集排名（并列不占位）
来源：http://wqp.dashuyun.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://bad.epnwcf.com

[Q57] 行号
来源：http://vos.ybcxt.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://xtt.shzxlz.cn

[Q58] 累计求和
来源：http://cgj.shanyushiyangkeji.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://sqx.gzhubu.top

[Q59] 分组内累计
来源：http://ovh.zhixingplan.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://han.yanxiufei.cn

[Q60] 取上一行 / 下一行
来源：http://mwt.yvedp.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://xft.xuetiantiany.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://pia.smart0.xyz

[Q61] 移动平均
来源：http://pvr.redwolf501.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://oas.yanxiufei.cn

[Q62] 分组占比
来源：http://njz.fanxiaobao.xyz

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://peq.yj20258888.top

[Q63] 开启事务
来源：http://rzu.fanxiaobao.xyz

START TRANSACTION;                -- 或 BEGIN
来源：http://xjq.ctjpmb.com

[Q64] 提交事务
来源：http://zoi.andypj.xyz

COMMIT;
来源：http://axr.jqgfzy.top

[Q65] 回滚事务
来源：http://kdr.9152youxi.cn

ROLLBACK;
来源：http://qht.jqgfzy.top

[Q66] 行锁查询
来源：http://gpy.xuetiantiany.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://qbn.zhiwuduotai.top

[Q67] 设置隔离级别
来源：http://wdx.sxryk.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://kqf.daria6918.cn

[Q68] 保存点
来源：http://ozz.9152youxi.cn

SAVEPOINT sp1;
来源：http://fjh.havefunace.top

ROLLBACK TO sp1;
来源：http://ouo.yj202588.top

[Q69] 查看执行计划
来源：http://nld.feifeiyinyue.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ucx.cheryme.top

[Q70] 更新统计信息
来源：http://jdz.yanxiufei.cn

ANALYZE TABLE users;
来源：http://nuu.hongshengwenyu.top

[Q71] 查看建表语句
来源：http://nsz.svipenyu.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://eme.sxryk.cn

[Q72] 查看索引
来源：http://czl.cdnleiting.top

SHOW INDEX FROM users;
来源：http://wqu.daria6918.cn

[Q73] 查看表状态
来源：http://hgm.jinyuanbaomall.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://vex.ybcxt.top

[Q74] 强制使用索引
来源：http://zoh.hfpthk.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://rdb.vehdjk.com

[Q75] 日期格式化
来源：http://kgr.ybcxt.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mke.shzxlz.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://twa.wangshuangyany.cn

[Q76] 按天统计
来源：http://bkt.cashguo.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ihg.ehwqpu.com

[Q77] 时间加减
来源：http://vrr.nanxuanxn.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://sco.fehbvm.com

[Q78] 当前时间
来源：http://awm.dashuyun.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://tnj.yangfankeji.com

[Q79] 字符串拼接
来源：http://cjo.aizwys.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://rdk.yj20258888.top

[Q80] 字符串截取
来源：http://zbj.0kj1m.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hsj.quarkkingdee.top

[Q81] 字符串替换
来源：http://ipe.bbcook.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mhc.hysaishi.cn

[Q82] 字符长度与字节长度
来源：http://pze.yangfankeji.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://qjl.wangdashe.top

[Q83] 大小写转换
来源：http://xuf.ivvv.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://zdc.nwbrower.top

[Q84] 去除首尾空格
来源：http://klb.fzhhl.top

SELECT TRIM(name) FROM users;
来源：http://irz.hongshengwenyu.top

[Q85] 数值取整
来源：http://wmj.jianghu66.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://qin.zhoulong.xyz

[Q86] 读取 JSON 字段
来源：http://gew.52xcode.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://bdg.xingfuxueyuan.xyz

[Q87] JSON 字段做条件
来源：http://plx.hongshengwenyu.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://eqb.gaohongyu789.top

[Q88] 行转列（条件聚合）
来源：http://pjy.gaohongyu789.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://uqf.bbcook.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://dmu.hywenlv.cn

[Q89] 判断表是否存在
来源：http://qty.iojbl.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ahb.dashuyun.cn

[Q90] 生成序号列
来源：http://ilb.ppjwa.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://zwa.yvedp.cn

================================================================================
来源：http://zah.yanxiufei.cn

R. Bash 专题
来源：http://xmh.vehdjk.com

================================================================================
来源：http://kcb.daxiang520.top

[R01] shebang 与严格模式
来源：http://jii.xingfuxueyuan.xyz

#!/usr/bin/env bash
来源：http://xcn.guannengcc.top

set -euo pipefail
来源：http://rtk.jyoumei.cn

[R02] 变量赋值与使用
来源：http://jgf.fktsv.cn

name="Tom"; echo "$name"
来源：http://lff.xuanzx.com

[R03] 只读变量
来源：http://ahv.0kj1m.cn

readonly PI=3.14
来源：http://byk.shzxlz.cn

[R04] 位置参数
来源：http://qtw.nanxinkj.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://iln.jianghu66.top

[R05] 参数默认值
来源：http://xqc.yueranfly.top

name="${1:-default}"
来源：http://wps.vqdsnc.cn

[R06] 判断命令是否存在
来源：http://nre.gotoacloud.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://lrh.chenjidiqi.icu

[R07] if 判断文件
来源：http://hte.cashguo.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mwk.xuetiantiany.cn

[R08] 数值比较
来源：http://sab.ivvv.top

if (( a > b )); then echo "a 更大"; fi
来源：http://rqg.daria6918.cn

[R09] 字符串比较
来源：http://nmm.nanxuanxn.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://xdr.yonumen.top

[R10] 正则匹配
来源：http://ohx.xingfuxueyuan.xyz

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://qub.sysykeji.top

[R11] case 多分支
来源：http://eby.xuetiantiany.cn

case "$1" in
来源：http://rvx.kuanghao11.cn

start) echo "启动" ;;
来源：http://mit.zdbjq.cn

stop)  echo "停止" ;;
来源：http://vhf.shangyingyoupin.top

*)     echo "未知命令" ;;
来源：http://sui.shzxlz.cn

esac
来源：http://gla.52xcode.cn

[R12] for 遍历文件
来源：http://mnb.daxiang520.top

for f in *.txt; do echo "$f"; done
来源：http://rbt.daria6918.cn

[R13] for 计数循环
来源：http://wgq.hywenlv.cn

for i in {1..10}; do echo "$i"; done
来源：http://iwm.yuxming.cn

[R14] C 风格 for
来源：http://okv.gaohongyu789.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://flp.nwbrower.top

[R15] while 逐行读文件
来源：http://mdi.quarkkingdee.top


<!-- 参考信息 -->