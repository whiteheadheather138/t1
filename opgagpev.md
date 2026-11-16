代发 wailian999

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://xgj.ydzc1.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://zxs.vqdsnc.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://qjc.yj202588.top

[P04] 求长度
来源：http://egs.mhx1999.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://pgl.chenlongwang.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dwj.wangshuangyany.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hpk.zhoulong.xyz

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fgb.tarul.cn

Java: list.size();  map.size();  s.length()
来源：http://aoz.shangyingyoupin.top

Go:   len(arr);  len(m)
来源：http://oft.jinghuilouyu.cn

Ruby: x.length;  x.size
来源：http://tvl.cdnleiting.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://aok.iojbl.cn

[P05] 判断两个对象内容是否相等
来源：http://ity.nanxinkj.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://iib.zhixingplan.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://vdp.guowangkeji.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://git.jinqigfzy.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://vhl.svipenyu.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://oeq.ywan-chungtsiang.top

Go:   reflect.DeepEqual(a, b)
来源：http://pwg.9152youxi.cn

Ruby: a == b
来源：http://nmd.gzhubu.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://zqg.nwbrower.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://rjj.sweek.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://gcz.quarkkingdee.top

PHP:  if (empty($x)) {}
来源：http://fvz.jinghuilouyu.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://zgo.hysaishi.cn

TS:   if (x == null) {}
来源：http://jgt.zhongyouzk.top

Java: if (x == null || x.isEmpty()) {}
来源：http://nil.ydzc1.top

Go:   if x == nil {}
来源：http://aav.sxryk.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://zun.zhixingplan.top

C#:   if (x is null) {}
来源：http://nxl.yj202588.top

[P07] 防抖与节流
来源：http://gzq.ydjk.org.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://qju.ehwqpu.com

PHP:  // 手写时间戳比较
来源：http://dlg.nwbrower.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cmj.shuidangran.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://aoe.aibaodan.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://cle.yuanzhike.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://cjj.ywan-chungtsiang.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://ine.hongshengwenyu.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://fds.fktsv.cn

[P08] 处理浮点精度问题
来源：http://jlt.bjfxy.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://bwr.zhijiandao.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://jjg.yueranfly.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://gms.yj202588.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://phz.yongpay.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ddy.hnxiangtu.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://sfs.haohaochexian.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://kih.52xcode.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://dto.chenlongwang.top

================================================================================
来源：http://uue.zycfv.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://cbs.ydzc1.top

================================================================================
来源：http://znz.tian-w.cn

[Q01] 创建表
来源：http://ohk.gogol.net.cn

CREATE TABLE users (
来源：http://qrm.redwolf501.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://iuh.shanyushiyangtech.top

name VARCHAR(50) NOT NULL,
来源：http://rxt.jqgufenzy.top

email VARCHAR(100) UNIQUE,
来源：http://kuq.ydjk.org.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://qwk.fktsv.cn

);
来源：http://elr.hywenlv.cn

[Q02] 创建带外键的表
来源：http://jpn.jinghuilouyu.cn

CREATE TABLE orders (
来源：http://yhe.pycfn.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ukg.shanyushiyangkeji.top

user_id INT NOT NULL,
来源：http://dbl.jqgufenzy.top

amount DECIMAL(10, 2),
来源：http://wue.redwolf501.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://lcz.dashuyun.cn

);
来源：http://zsg.9152youxi.cn

[Q03] 增加列
来源：http://huu.shanyushiyangkeji.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://gsd.haohaochexian.top

[Q04] 修改列类型
来源：http://nhx.jinyuanbaomall.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wwj.sufxvd.cn

[Q05] 重命名列
来源：http://ukb.redwolf501.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://dum.kuanghao11.cn

[Q06] 删除列
来源：http://kky.yonumen.top

ALTER TABLE users DROP COLUMN age;
来源：http://jas.tian-w.cn

[Q07] 删除表
来源：http://yng.quarkkingdee.top

DROP TABLE IF EXISTS orders;
来源：http://ius.nwbrower.top

[Q08] 创建普通索引
来源：http://awd.9152youxi.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://jhi.jinqigufen.top

[Q09] 创建唯一索引
来源：http://hor.meibo888.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://toe.daxiang520.top

[Q10] 插入单行
来源：http://vcp.cqqwz.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://kda.birdmap.top

[Q11] 一次插入多行
来源：http://kse.xingfuxueyuan.xyz

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://lqn.cheryme.top

[Q12] 插入后取自增 ID
来源：http://lov.jinqigfzy.top

INSERT INTO users (name) VALUES ('C');
来源：http://pci.fzhhl.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wii.yuxming.cn

[Q13] 忽略重复插入
来源：http://uoe.fehbvm.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://oam.bjfxy.top

[Q14] 存在则更新（upsert）
来源：http://whn.daria6918.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://gdg.hnqzz.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://axk.bbcook.cn

[Q15] 查询全部
来源：http://lna.zdbjq.cn

SELECT * FROM users;
来源：http://pwe.sufxvd.cn

[Q16] 查询指定列
来源：http://frg.zhiwuduotai.top

SELECT id, name FROM users;
来源：http://sak.redwolf501.top

[Q17] 条件查询
来源：http://ndo.9152youxi.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://yzf.bbcook.cn

[Q18] 模糊匹配
来源：http://kho.jinqigfzy.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ceh.quarkkingdee.top

[Q19] 范围查询
来源：http://fwn.nanxinkj.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://nhr.iojbl.cn

[Q20] IN 列表
来源：http://jno.jyoumei.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://vfx.mhx1999.top

[Q21] 空值判断
来源：http://yce.zhongyouzk.top

SELECT * FROM users WHERE email IS NULL;
来源：http://akh.ydzc1.top

[Q22] 排序
来源：http://ynr.jyoumei.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://kqz.fehbvm.com

[Q23] 分页
来源：http://tcj.fengsongda.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://cur.hesvh.cn

[Q24] 去重
来源：http://nze.xuanzx.com

SELECT DISTINCT city FROM users;
来源：http://zjt.ppjwa.cn

[Q25] 只取前 N 条
来源：http://gdc.ydzc1.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wlb.nanxinkj.top

[Q26] 计数
来源：http://xqc.gotoacloud.top

SELECT COUNT(*) FROM users;
来源：http://hkg.pycfn.com

[Q27] 条件计数
来源：http://jix.aizwys.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://fwb.smart0.xyz

[Q28] 求和与平均
来源：http://mcr.sxryk.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://lht.jinghuilouyu.cn

[Q29] 最大最小值
来源：http://mys.zhoulong.xyz

SELECT MAX(age), MIN(age) FROM users;
来源：http://orx.daxiang520.top

[Q30] 分组统计
来源：http://lzm.svipenyu.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://dns.hnqzz.top

[Q31] 分组后过滤
来源：http://chk.svipenyu.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://vbq.daria6918.cn

[Q32] 分组拼接字符串
来源：http://kyu.zhaomingkeji.xyz

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://abe.gotoacloud.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://rfp.zdbjq.cn

[Q33] 多列分组
来源：http://kth.svipenyu.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://lvm.yvedp.cn

[Q34] 每组取第一条
来源：http://evb.tarul.cn

SELECT * FROM (
来源：http://hiz.xuanzx.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ahz.0kj1m.cn

) t WHERE rn = 1;
来源：http://gbw.haohaochexian.top

[Q35] 内连接
来源：http://uei.guowangkeji.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://now.52xcode.cn

[Q36] 左连接
来源：http://eca.xuetiantiany.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ppn.hnqzz.top

[Q37] 右连接
来源：http://xci.sysykeji.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://nxm.svipenyu.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ecf.jlsjyb.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://nzx.sweek.top

[Q39] 自连接（查上下级）
来源：http://uwl.ydzc1.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://bmd.316326.xyz

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://bwk.gotoacloud.top

[Q40] 交叉连接（笛卡尔积）
来源：http://egv.ctjpmb.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://jpw.yvedp.cn

[Q41] 多表连接
来源：http://nxu.yuxming.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://dbh.hesvh.cn

JOIN users u ON u.id = o.user_id
来源：http://tyl.birdmap.top

JOIN products p ON p.id = o.product_id;
来源：http://mwf.ydjk.org.cn

[Q42] 连接条件附加过滤
来源：http://opq.9152youxi.cn

SELECT u.name, o.amount FROM users u
来源：http://itw.fktsv.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://rsf.chenlongwang.top

[Q43] 标量子查询
来源：http://ajq.zhoulong.xyz

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ljp.quarkkingdee.top

[Q44] IN 子查询
来源：http://tyr.chenjidiqi.icu

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://cic.ydzc1.top

[Q45] EXISTS 判断存在
来源：http://bjv.yfazqb.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://dkd.gaohongyu789.top

[Q46] NOT EXISTS 判断不存在
来源：http://nth.hcnkem.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://azn.ydjk.org.cn

[Q47] 与平均值比较
来源：http://hha.hfpthk.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://rpe.zdqjudy.top

[Q48] CTE 公用表表达式
来源：http://hoz.kuanghao11.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://kxn.zhaomingkeji.xyz

SELECT * FROM t WHERE c > 5;
来源：http://apz.zhongyouzk.top

[Q49] 更新单行
来源：http://fmj.daria6918.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://egi.redwolf501.top

[Q50] 批量更新
来源：http://ezr.hnxiangtu.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://zbs.fengsongda.top

[Q51] 用子查询更新
来源：http://qln.xziqi.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://qij.chenzaomai.com

[Q52] 删除指定行
来源：http://pxx.jqgufenzy.top

DELETE FROM users WHERE id = 10;
来源：http://fxa.fehbvm.com

[Q53] 按条件删除
来源：http://ffu.tianlin.xyz

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://gtf.daxiang520.top

[Q54] 清空表
来源：http://mdp.ivvv.top

TRUNCATE TABLE logs;
来源：http://bji.nwbrower.top

[Q55] 排名（并列占位）
来源：http://lzv.iojbl.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ekc.xuetiantiany.cn

[Q56] 密集排名（并列不占位）
来源：http://gkj.xuanzx.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://iuq.cheryme.top

[Q57] 行号
来源：http://cek.xuanzx.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://msb.tian-w.cn

[Q58] 累计求和
来源：http://mux.chenjidiqi.icu

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://gzg.hnqzz.top

[Q59] 分组内累计
来源：http://avi.jinyuanbaomall.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://umo.chenlongwang.top

[Q60] 取上一行 / 下一行
来源：http://ouk.aizwys.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://lxt.meibo888.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://qfd.hcnkem.com

[Q61] 移动平均
来源：http://jmp.ctjpmb.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://adu.aizwys.cn

[Q62] 分组占比
来源：http://hiv.havefunace.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://pls.svipenyu.cn

[Q63] 开启事务
来源：http://mfu.zhiwuduotai.top

START TRANSACTION;                -- 或 BEGIN
来源：http://nkv.fehbvm.com

[Q64] 提交事务
来源：http://bwd.yj20258.top

COMMIT;
来源：http://kos.aibaodan.cn

[Q65] 回滚事务
来源：http://tsx.52xcode.cn

ROLLBACK;
来源：http://wsp.shzxlz.cn

[Q66] 行锁查询
来源：http://xbg.jinqigufen.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://kmc.yuanzhike.top

[Q67] 设置隔离级别
来源：http://yok.tarul.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://pog.daxiang520.top

[Q68] 保存点
来源：http://ffv.jinqigfzy.top

SAVEPOINT sp1;
来源：http://dlb.xylfe.cn

ROLLBACK TO sp1;
来源：http://bwg.ivvv.top

[Q69] 查看执行计划
来源：http://wsc.iojbl.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://htf.cucudq.cn

[Q70] 更新统计信息
来源：http://kxa.tanke756.top

ANALYZE TABLE users;
来源：http://rip.yongpay.top

[Q71] 查看建表语句
来源：http://nib.yfazqb.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://rwr.nwbrower.top

[Q72] 查看索引
来源：http://hyf.nanxinkj.top

SHOW INDEX FROM users;
来源：http://ruy.meibo888.top

[Q73] 查看表状态
来源：http://rzj.cashguo.top

SHOW TABLE STATUS LIKE 'users';
来源：http://oxa.nanxuanxn.top

[Q74] 强制使用索引
来源：http://yql.ehwqpu.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://fgc.guannengcc.top

[Q75] 日期格式化
来源：http://ffl.yfazqb.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://frl.xuanzx.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://atn.pengpengdd.cyou

[Q76] 按天统计
来源：http://pkf.snrcjt.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://jlr.sjlbkw.cn

[Q77] 时间加减
来源：http://ylo.shuidangran.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ojm.jinqigfzy.top

[Q78] 当前时间
来源：http://mll.fktsv.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://nra.hnxiangtu.top

[Q79] 字符串拼接
来源：http://ual.sysykeji.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://pyt.ehwqpu.com

[Q80] 字符串截取
来源：http://thz.fanxiaobao.xyz

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mhi.pengpengdd.cyou

[Q81] 字符串替换
来源：http://ehq.jyoumei.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://sce.fzhhl.top

[Q82] 字符长度与字节长度
来源：http://eqt.ctjpmb.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://rch.hywenlv.cn

[Q83] 大小写转换
来源：http://eay.wangdashe.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://cgr.tian-w.cn

[Q84] 去除首尾空格
来源：http://goa.smart0.xyz

SELECT TRIM(name) FROM users;
来源：http://tpe.hnqzz.top

[Q85] 数值取整
来源：http://eza.zhijiandao.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://xhl.fzhhl.top

[Q86] 读取 JSON 字段
来源：http://bxe.zhaomingkeji.xyz

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mqw.yj20258888.top

[Q87] JSON 字段做条件
来源：http://ehv.jyoumei.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://kpt.316326.xyz

[Q88] 行转列（条件聚合）
来源：http://wph.epnwcf.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://tzi.jiagoushi.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://rlw.fehbvm.com

[Q89] 判断表是否存在
来源：http://hbh.cdnleiting.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ifw.52xcode.cn

[Q90] 生成序号列
来源：http://ufv.pycfn.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://leo.jinqigfzy.top

================================================================================
来源：http://cac.jlsjyb.cn

R. Bash 专题
来源：http://ycc.zhixingplan.top

================================================================================
来源：http://pue.daxiang520.top

[R01] shebang 与严格模式
来源：http://tpb.havefunace.top

#!/usr/bin/env bash
来源：http://nrj.xylfe.cn

set -euo pipefail
来源：http://jcz.hfpthk.cn

[R02] 变量赋值与使用
来源：http://ype.birdmap.top

name="Tom"; echo "$name"
来源：http://lyi.jinqigufen.top

[R03] 只读变量
来源：http://axa.cdnleiting.top

readonly PI=3.14
来源：http://zqv.wangshuangyany.cn

[R04] 位置参数
来源：http://soo.pycfn.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://jga.guannengcc.top

[R05] 参数默认值
来源：http://bfh.mhx1999.top

name="${1:-default}"
来源：http://obo.jiagoushi.top

[R06] 判断命令是否存在
来源：http://let.xuetiantiany.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://vnb.shzxlz.cn

[R07] if 判断文件
来源：http://hfh.zhixingplan.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ngr.ybcxt.top

[R08] 数值比较
来源：http://ypu.zhiwuduotai.top

if (( a > b )); then echo "a 更大"; fi
来源：http://jdl.hnqzz.top

[R09] 字符串比较
来源：http://vcw.yvedp.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://tob.andypj.xyz

[R10] 正则匹配
来源：http://bks.zhijiandao.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://bsk.zhoulong.xyz

[R11] case 多分支
来源：http://aap.quarkkingdee.top

case "$1" in
来源：http://vto.gogol.net.cn

start) echo "启动" ;;
来源：http://olu.sufxvd.cn

stop)  echo "停止" ;;
来源：http://etr.ywan-chungtsiang.top

*)     echo "未知命令" ;;
来源：http://chs.hesvh.cn

esac
来源：http://jnp.jqgfzy.top

[R12] for 遍历文件
来源：http://doi.gotoacloud.top

for f in *.txt; do echo "$f"; done
来源：http://wtw.uphjek.com

[R13] for 计数循环
来源：http://vac.cashguo.top

for i in {1..10}; do echo "$i"; done
来源：http://nkq.yuxming.cn

[R14] C 风格 for
来源：http://hhf.xuanzx.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://uos.sjlbkw.cn

[R15] while 逐行读文件
来源：http://qko.zycfv.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://lmd.jinyuanbaomall.cn

[R16] until 等待条件
来源：http://sup.dashuyun.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://bwi.redwolf501.top

[R17] 数组定义与取值
来源：http://moj.jinghuilouyu.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ekz.zhoulong.xyz

[R18] 遍历数组
来源：http://ljq.zhongyouzk.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://eao.aibaodan.cn

[R19] 数组长度
来源：http://pml.cheryme.top


<!-- 参考信息 -->