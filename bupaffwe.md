代发 wailian999

Java: list.size();  map.size();  s.length()
来源：http://fyv.chenjidiqi.icu

Go:   len(arr);  len(m)
来源：http://ryb.ctjpmb.com

Ruby: x.length;  x.size
来源：http://rgi.yj20258888.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://acy.xuanzx.com

[P05] 判断两个对象内容是否相等
来源：http://ecu.nwbrower.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://ftv.zhongyouzk.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://kzc.yj20258.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://gzs.yuxming.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hey.andypj.xyz

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://cfi.haohaochexian.top

Go:   reflect.DeepEqual(a, b)
来源：http://ewt.yj20258888.top

Ruby: a == b
来源：http://ttp.jinghuilouyu.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://bcu.dashuyun.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://lgb.yj20258.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://lqn.cashguo.top

PHP:  if (empty($x)) {}
来源：http://vnk.fanxiaobao.xyz

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://dmw.jinyuanbaomall.cn

TS:   if (x == null) {}
来源：http://bfp.aizwys.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://uie.jianghu66.top

Go:   if x == nil {}
来源：http://wfv.fktsv.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hme.snrcjt.cn

C#:   if (x is null) {}
来源：http://zmp.jqgufenzy.top

[P07] 防抖与节流
来源：http://pwo.ydzc1.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ucy.yuanzhike.top

PHP:  // 手写时间戳比较
来源：http://pgu.zhoulong.xyz

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://efb.yanxiufei.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hus.yongpay.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mai.zhoulong.xyz

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://iyb.yanxiufei.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://dxh.daria6918.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://cpf.jinyuanbaomall.cn

[P08] 处理浮点精度问题
来源：http://pba.wangshuangyany.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://nvs.bjfxy.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://psg.zhijiandao.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://xab.svipenyu.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hsj.dianchejie.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://oqg.cheryme.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ezf.0kj1m.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://pkg.0kj1m.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://zfd.aibaodan.cn

================================================================================
来源：http://mwc.fehbvm.com

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://cck.hysaishi.cn

================================================================================
来源：http://tda.tian-w.cn

[Q01] 创建表
来源：http://ixc.ivvv.top

CREATE TABLE users (
来源：http://yva.iojbl.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://stm.316326.xyz

name VARCHAR(50) NOT NULL,
来源：http://flp.yj20258888.top

email VARCHAR(100) UNIQUE,
来源：http://wlp.feifeiyinyue.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://sgm.yj20258.top

);
来源：http://swt.zhixingplan.top

[Q02] 创建带外键的表
来源：http://xnn.uphjek.com

CREATE TABLE orders (
来源：http://vvl.hywenlv.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://uso.sjlbkw.cn

user_id INT NOT NULL,
来源：http://bga.cucudq.cn

amount DECIMAL(10, 2),
来源：http://ncv.shangyingyoupin.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ewh.aibaodan.cn

);
来源：http://ghw.pengpengdd.cyou

[Q03] 增加列
来源：http://prp.smart0.xyz

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ffu.hywenlv.cn

[Q04] 修改列类型
来源：http://vdb.fktsv.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://loe.xylfe.cn

[Q05] 重命名列
来源：http://xzo.52xcode.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://rtt.mhx1999.top

[Q06] 删除列
来源：http://sdl.yonumen.top

ALTER TABLE users DROP COLUMN age;
来源：http://fsr.hysaishi.cn

[Q07] 删除表
来源：http://rzf.zhongyouzk.top

DROP TABLE IF EXISTS orders;
来源：http://wzo.guannengcc.top

[Q08] 创建普通索引
来源：http://lho.jinghuilouyu.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://vfm.fzhhl.top

[Q09] 创建唯一索引
来源：http://qge.epnwcf.com

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://xcl.sysykeji.top

[Q10] 插入单行
来源：http://wra.zdqjudy.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://fkd.pycfn.com

[Q11] 一次插入多行
来源：http://bhz.hnxiangtu.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://opq.shuidangran.top

[Q12] 插入后取自增 ID
来源：http://ddd.snrcjt.cn

INSERT INTO users (name) VALUES ('C');
来源：http://wkl.yongpay.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ojy.havefunace.top

[Q13] 忽略重复插入
来源：http://tht.gogol.net.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://kmc.dianchejie.cn

[Q14] 存在则更新（upsert）
来源：http://rzw.cqqwz.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://dzy.jlsjyb.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://qfg.ivvv.top

[Q15] 查询全部
来源：http://whb.shanyushiyangtech.top

SELECT * FROM users;
来源：http://udg.ppjwa.cn

[Q16] 查询指定列
来源：http://bvc.xuetiantiany.cn

SELECT id, name FROM users;
来源：http://krv.c1oappe.top

[Q17] 条件查询
来源：http://van.yongpay.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://fax.iojbl.cn

[Q18] 模糊匹配
来源：http://fle.ppjwa.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://obi.zhoulong.xyz

[Q19] 范围查询
来源：http://bst.ywan-chungtsiang.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://bjm.xuetiantiany.cn

[Q20] IN 列表
来源：http://aig.jinqigfzy.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ndw.chenzaomai.com

[Q21] 空值判断
来源：http://glb.andypj.xyz

SELECT * FROM users WHERE email IS NULL;
来源：http://iog.316326.xyz

[Q22] 排序
来源：http://nvb.epnwcf.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://pov.haohaochexian.top

[Q23] 分页
来源：http://zsh.9152youxi.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://pzb.nanxinkj.top

[Q24] 去重
来源：http://ron.shzxlz.cn

SELECT DISTINCT city FROM users;
来源：http://pgk.yangfankeji.com

[Q25] 只取前 N 条
来源：http://eke.shuidangran.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://sjz.hammf.cn

[Q26] 计数
来源：http://aru.zdqjudy.top

SELECT COUNT(*) FROM users;
来源：http://chf.sjlbkw.cn

[Q27] 条件计数
来源：http://dvh.yvedp.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wtw.shangyingyoupin.top

[Q28] 求和与平均
来源：http://ddg.pycfn.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://gam.ctjpmb.com

[Q29] 最大最小值
来源：http://jkk.gaohongyu789.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://ipu.nanxinkj.top

[Q30] 分组统计
来源：http://ycz.guowangkeji.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://fmr.fktsv.cn

[Q31] 分组后过滤
来源：http://yjs.zhoulong.xyz

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hyf.yfazqb.com

[Q32] 分组拼接字符串
来源：http://pkw.cqqwz.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ihz.chenjidiqi.icu

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://bsr.jinqigufen.top

[Q33] 多列分组
来源：http://dvb.meibo888.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://phr.mhx1999.top

[Q34] 每组取第一条
来源：http://wwd.yfazqb.com

SELECT * FROM (
来源：http://hvm.yanxiufei.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ske.guannengcc.top

) t WHERE rn = 1;
来源：http://gcm.yuxming.cn

[Q35] 内连接
来源：http://ivt.zdbjq.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://gxs.bjfxy.top

[Q36] 左连接
来源：http://aln.yongpay.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://sxe.andypj.xyz

[Q37] 右连接
来源：http://pct.yj202588.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wws.hesvh.cn

[Q38] 全外连接（PostgreSQL）
来源：http://rdx.52xcode.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://naz.tarul.cn

[Q39] 自连接（查上下级）
来源：http://sbk.yueranfly.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://def.uphjek.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://nti.bbcook.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://mvk.cdnleiting.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://eha.andypj.xyz

[Q41] 多表连接
来源：http://hao.cqqwz.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://wvp.0kj1m.cn

JOIN users u ON u.id = o.user_id
来源：http://rcl.ctjpmb.com

JOIN products p ON p.id = o.product_id;
来源：http://ldt.ivvv.top

[Q42] 连接条件附加过滤
来源：http://klz.jyoumei.cn

SELECT u.name, o.amount FROM users u
来源：http://nla.zhengqikj.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://vny.fanxiaobao.xyz

[Q43] 标量子查询
来源：http://uza.feifeiyinyue.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://kne.shanyushiyangtech.top

[Q44] IN 子查询
来源：http://ouj.ybcxt.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ami.snrcjt.cn

[Q45] EXISTS 判断存在
来源：http://xpp.daxiang520.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vgm.cdnleiting.top

[Q46] NOT EXISTS 判断不存在
来源：http://lqt.ydzc1.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jfl.xuanzx.com

[Q47] 与平均值比较
来源：http://jbz.nwbrower.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://gnd.aizwys.cn

[Q48] CTE 公用表表达式
来源：http://lvo.zhaomingkeji.xyz

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://vni.pengpengdd.cyou

SELECT * FROM t WHERE c > 5;
来源：http://gzy.fengsongda.top

[Q49] 更新单行
来源：http://uyx.shanyushiyangkeji.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://rdc.zhoulong.xyz

[Q50] 批量更新
来源：http://iyx.yonumen.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://esi.wangdashe.top

[Q51] 用子查询更新
来源：http://oey.ppjwa.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ciz.gaohongyu789.top

[Q52] 删除指定行
来源：http://dwk.sxryk.cn

DELETE FROM users WHERE id = 10;
来源：http://mes.svipenyu.cn

[Q53] 按条件删除
来源：http://cbw.gogol.net.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ecw.9152youxi.cn

[Q54] 清空表
来源：http://ewr.svipenyu.cn

TRUNCATE TABLE logs;
来源：http://imp.cheryme.top

[Q55] 排名（并列占位）
来源：http://lmq.nanxinkj.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://yyy.chenzaomai.com

[Q56] 密集排名（并列不占位）
来源：http://rpr.hysaishi.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://fdu.cucudq.cn

[Q57] 行号
来源：http://epu.cheryme.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://zon.ivvv.top

[Q58] 累计求和
来源：http://pfo.xingfuxueyuan.xyz

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://uem.epnwcf.com

[Q59] 分组内累计
来源：http://wob.kuanghao11.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://pjc.sjlbkw.cn

[Q60] 取上一行 / 下一行
来源：http://vaw.snrcjt.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://vxo.yj20258.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://uub.nwbrower.top

[Q61] 移动平均
来源：http://ldd.daria6918.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://pnp.zhaomingkeji.xyz

[Q62] 分组占比
来源：http://jed.hesvh.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mul.xinyue.icu

[Q63] 开启事务
来源：http://qum.kuanghao11.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://wmp.zdbjq.cn

[Q64] 提交事务
来源：http://tbi.ywan-chungtsiang.top

COMMIT;
来源：http://hdd.sweek.top

[Q65] 回滚事务
来源：http://haa.tarul.cn

ROLLBACK;
来源：http://eog.dashuyun.cn

[Q66] 行锁查询
来源：http://gik.52xcode.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ier.jinyuanbaomall.cn

[Q67] 设置隔离级别
来源：http://idp.xuetiantiany.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://skr.nwbrower.top

[Q68] 保存点
来源：http://ftq.cdnleiting.top

SAVEPOINT sp1;
来源：http://bqn.hnqzz.top

ROLLBACK TO sp1;
来源：http://osy.birdmap.top

[Q69] 查看执行计划
来源：http://fol.shuidangran.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://bqs.ehwqpu.com

[Q70] 更新统计信息
来源：http://okm.pycfn.com

ANALYZE TABLE users;
来源：http://wri.sweek.top

[Q71] 查看建表语句
来源：http://mjn.sweek.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://lco.sxryk.cn

[Q72] 查看索引
来源：http://pmp.yonumen.top

SHOW INDEX FROM users;
来源：http://tjt.jqgfzy.top

[Q73] 查看表状态
来源：http://wbi.sufxvd.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://xkd.daxiang520.top

[Q74] 强制使用索引
来源：http://hov.hnqzz.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://rpm.xuetiantiany.cn

[Q75] 日期格式化
来源：http://vzc.gzhubu.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://tvg.gzhubu.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://cqa.zhixingplan.top

[Q76] 按天统计
来源：http://fhk.nanxuanxn.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://jee.ydjk.org.cn

[Q77] 时间加减
来源：http://pdc.sweek.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://tuf.nwbrower.top

[Q78] 当前时间
来源：http://rul.bbcook.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://rbj.zhoulong.xyz

[Q79] 字符串拼接
来源：http://ici.sjlbkw.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://vxi.jqgufenzy.top

[Q80] 字符串截取
来源：http://lne.ivvv.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hfk.sxryk.cn

[Q81] 字符串替换
来源：http://kqh.uphjek.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://erj.hammf.cn

[Q82] 字符长度与字节长度
来源：http://tud.chenzaomai.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ktt.9152youxi.cn

[Q83] 大小写转换
来源：http://rlx.ydjk.org.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://uky.xuanzx.com

[Q84] 去除首尾空格
来源：http://usp.xuetiantiany.cn

SELECT TRIM(name) FROM users;
来源：http://qcp.316326.xyz

[Q85] 数值取整
来源：http://jbl.xylfe.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://stc.cqqwz.cn

[Q86] 读取 JSON 字段
来源：http://fma.yuxming.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://xng.yj20258888.top

[Q87] JSON 字段做条件
来源：http://vqt.jinyuanbaomall.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://tui.zhengqikj.top

[Q88] 行转列（条件聚合）
来源：http://bhi.fehbvm.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wwv.cheryme.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://uae.birdmap.top

[Q89] 判断表是否存在
来源：http://jhr.zdbjq.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://tlh.pengpengdd.cyou

[Q90] 生成序号列
来源：http://kcp.hywenlv.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://xfk.smart0.xyz

================================================================================
来源：http://joz.hesvh.cn

R. Bash 专题
来源：http://lbh.zhoulong.xyz

================================================================================
来源：http://sbj.feifeiyinyue.top

[R01] shebang 与严格模式
来源：http://key.smart0.xyz

#!/usr/bin/env bash
来源：http://voo.zycfv.cn

set -euo pipefail
来源：http://lvu.aizwys.cn

[R02] 变量赋值与使用
来源：http://muk.xuanzx.com

name="Tom"; echo "$name"
来源：http://zzy.guannengcc.top

[R03] 只读变量
来源：http://lkm.haohaochexian.top

readonly PI=3.14
来源：http://xww.shzxlz.cn

[R04] 位置参数
来源：http://sdg.zhaomingkeji.xyz

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://lup.ehwqpu.com

[R05] 参数默认值
来源：http://fel.hammf.cn

name="${1:-default}"
来源：http://xui.redwolf501.top

[R06] 判断命令是否存在
来源：http://hro.hesvh.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://arj.iojbl.cn

[R07] if 判断文件
来源：http://hwv.aibaodan.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://plj.zhengqikj.top

[R08] 数值比较
来源：http://zsv.aizwys.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://wgd.bjfxy.top

[R09] 字符串比较
来源：http://rsl.shuidangran.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mbo.yvedp.cn

[R10] 正则匹配
来源：http://wrt.jinqigufen.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://grl.jinqigfzy.top

[R11] case 多分支
来源：http://gon.ctjpmb.com

case "$1" in
来源：http://kdc.fzhhl.top

start) echo "启动" ;;
来源：http://mze.yfazqb.com

stop)  echo "停止" ;;
来源：http://mbt.gzhubu.top

*)     echo "未知命令" ;;
来源：http://dfs.aibaodan.cn

esac
来源：http://tui.c1oappe.top

[R12] for 遍历文件
来源：http://xzj.9152youxi.cn

for f in *.txt; do echo "$f"; done
来源：http://dan.yuanzhike.top

[R13] for 计数循环
来源：http://cjn.hywenlv.cn

for i in {1..10}; do echo "$i"; done
来源：http://dex.aibaodan.cn

[R14] C 风格 for
来源：http://jgg.0kj1m.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://qot.kuanghao11.cn

[R15] while 逐行读文件
来源：http://uzu.bjfxy.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wwy.zycfv.cn

[R16] until 等待条件
来源：http://hkm.epnwcf.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://sre.fktsv.cn

[R17] 数组定义与取值
来源：http://rqh.jinqigufen.top

arr=(a b c); echo "${arr[0]}"
来源：http://qwc.yanxiufei.cn

[R18] 遍历数组
来源：http://mxs.quarkkingdee.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://snf.snrcjt.cn

[R19] 数组长度
来源：http://mbv.cheryme.top

echo "${#arr[@]}"
来源：http://wku.ydjk.org.cn

[R20] 关联数组（字典）
来源：http://emo.aibaodan.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://fcv.wangdashe.top

[R21] 字符串长度
来源：http://beb.zhoulong.xyz

echo "${#s}"
来源：http://kme.guowangkeji.top

[R22] 截取子串
来源：http://dca.vehdjk.com

echo "${s:0:5}"
来源：http://exh.jqgufenzy.top

[R23] 字符串替换
来源：http://wsj.zdbjq.cn


<!-- 参考信息 -->