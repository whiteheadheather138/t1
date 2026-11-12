代发 wailian999

Java: list.size();  map.size();  s.length()
来源：http://yun.hnqzz.top

Go:   len(arr);  len(m)
来源：http://sba.yueranfly.top

Ruby: x.length;  x.size
来源：http://xda.guowangkeji.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://kxw.vqdsnc.cn

[P05] 判断两个对象内容是否相等
来源：http://mdo.hnqzz.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://noy.cucudq.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ytj.c1oappe.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ozb.jianghu66.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ewk.jqgfzy.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://efg.0kj1m.cn

Go:   reflect.DeepEqual(a, b)
来源：http://geb.uphjek.com

Ruby: a == b
来源：http://tla.nanxuanxn.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://nap.sxryk.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://vaf.bjfxy.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://zzq.zdqjudy.top

PHP:  if (empty($x)) {}
来源：http://nks.cdnleiting.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://cno.316326.xyz

TS:   if (x == null) {}
来源：http://oua.meibo888.top

Java: if (x == null || x.isEmpty()) {}
来源：http://afu.cqqwz.cn

Go:   if x == nil {}
来源：http://pit.hnxiangtu.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://qmi.haohaochexian.top

C#:   if (x is null) {}
来源：http://czu.yj20258.top

[P07] 防抖与节流
来源：http://xhs.fanxiaobao.xyz

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://xyg.cashguo.top

PHP:  // 手写时间戳比较
来源：http://qfz.shuidangran.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vil.yj20258888.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jyq.andypj.xyz

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://tsc.vehdjk.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://qhk.zhiwuduotai.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://yrw.havefunace.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://btp.yueranfly.top

[P08] 处理浮点精度问题
来源：http://uzy.xziqi.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mzx.pycfn.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://fvx.jlsjyb.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://jdo.sufxvd.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://lqs.jinyuanbaomall.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://dal.fanxiaobao.xyz

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ahz.bbcook.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://sjq.hnqzz.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://olq.hammf.cn

================================================================================
来源：http://pvb.shuidangran.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://gwp.dianchejie.cn

================================================================================
来源：http://pdr.yvedp.cn

[Q01] 创建表
来源：http://fkp.sufxvd.cn

CREATE TABLE users (
来源：http://pno.xylfe.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://pmv.shangyingyoupin.top

name VARCHAR(50) NOT NULL,
来源：http://jgo.cashguo.top

email VARCHAR(100) UNIQUE,
来源：http://euy.meibo888.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://jfd.cqqwz.cn

);
来源：http://qej.andypj.xyz

[Q02] 创建带外键的表
来源：http://dej.hywenlv.cn

CREATE TABLE orders (
来源：http://bjm.jinqigufen.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ics.vqdsnc.cn

user_id INT NOT NULL,
来源：http://lka.wangshuangyany.cn

amount DECIMAL(10, 2),
来源：http://ycf.yanxiufei.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ldh.guowangkeji.top

);
来源：http://slw.jinqigufen.top

[Q03] 增加列
来源：http://gdw.pengpengdd.cyou

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mmt.fzhhl.top

[Q04] 修改列类型
来源：http://mzc.jinghuilouyu.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mzs.chenlongwang.top

[Q05] 重命名列
来源：http://thl.vqdsnc.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://bvk.chenzaomai.com

[Q06] 删除列
来源：http://tcn.xingfuxueyuan.xyz

ALTER TABLE users DROP COLUMN age;
来源：http://jro.zhongyouzk.top

[Q07] 删除表
来源：http://kyi.jinqigufen.top

DROP TABLE IF EXISTS orders;
来源：http://ipo.hammf.cn

[Q08] 创建普通索引
来源：http://pqm.daria6918.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://rop.wangshuangyany.cn

[Q09] 创建唯一索引
来源：http://hah.fzhhl.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://gna.ydjk.org.cn

[Q10] 插入单行
来源：http://ikf.shangyingyoupin.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://gfe.fengsongda.top

[Q11] 一次插入多行
来源：http://zlr.chenjidiqi.icu

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://gec.zycfv.cn

[Q12] 插入后取自增 ID
来源：http://kba.bjfxy.top

INSERT INTO users (name) VALUES ('C');
来源：http://kbm.shangyingyoupin.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://npp.jinqigfzy.top

[Q13] 忽略重复插入
来源：http://niv.cucudq.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://qvb.jqgufenzy.top

[Q14] 存在则更新（upsert）
来源：http://bpb.sufxvd.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://uyy.jlsjyb.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://jmf.gzhubu.top

[Q15] 查询全部
来源：http://dqn.yvedp.cn

SELECT * FROM users;
来源：http://ldk.jiagoushi.top

[Q16] 查询指定列
来源：http://god.jinqigufen.top

SELECT id, name FROM users;
来源：http://jyi.cheryme.top

[Q17] 条件查询
来源：http://rfp.haohaochexian.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://dfy.ybcxt.top

[Q18] 模糊匹配
来源：http://vow.zhiwuduotai.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://jlw.sxryk.cn

[Q19] 范围查询
来源：http://sho.feifeiyinyue.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ezo.nwbrower.top

[Q20] IN 列表
来源：http://rgq.zhengqikj.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://fts.iojbl.cn

[Q21] 空值判断
来源：http://ihs.sjlbkw.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://lta.birdmap.top

[Q22] 排序
来源：http://yft.sweek.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://iki.nwbrower.top

[Q23] 分页
来源：http://rtt.pengpengdd.cyou

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://jwh.nanxuanxn.top

[Q24] 去重
来源：http://hmv.tian-w.cn

SELECT DISTINCT city FROM users;
来源：http://tnr.jiagoushi.top

[Q25] 只取前 N 条
来源：http://imb.hysaishi.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://elx.yongpay.top

[Q26] 计数
来源：http://dlb.jinyuanbaomall.cn

SELECT COUNT(*) FROM users;
来源：http://edn.zdbjq.cn

[Q27] 条件计数
来源：http://ggd.dianchejie.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://nka.hfpthk.cn

[Q28] 求和与平均
来源：http://xsv.gogol.net.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://axk.yonumen.top

[Q29] 最大最小值
来源：http://vyn.hcnkem.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://lir.tanke756.top

[Q30] 分组统计
来源：http://mrx.hnqzz.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://bff.ehwqpu.com

[Q31] 分组后过滤
来源：http://ijy.hywenlv.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://nzk.ppjwa.cn

[Q32] 分组拼接字符串
来源：http://xzd.svipenyu.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://gux.jinyuanbaomall.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://pae.yj20258.top

[Q33] 多列分组
来源：http://iop.jinqigfzy.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://rgt.yj20258.top

[Q34] 每组取第一条
来源：http://zrq.yonumen.top

SELECT * FROM (
来源：http://yco.kuanghao11.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://tmm.fengsongda.top

) t WHERE rn = 1;
来源：http://pye.meibo888.top

[Q35] 内连接
来源：http://zjc.yuxming.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://zws.0kj1m.cn

[Q36] 左连接
来源：http://amu.sxryk.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://cef.yonumen.top

[Q37] 右连接
来源：http://tej.fktsv.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://bnb.bbcook.cn

[Q38] 全外连接（PostgreSQL）
来源：http://kbx.uphjek.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://xvu.feifeiyinyue.top

[Q39] 自连接（查上下级）
来源：http://lbw.52xcode.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://vtl.snrcjt.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://caz.gotoacloud.top

[Q40] 交叉连接（笛卡尔积）
来源：http://qau.zhijiandao.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://aut.jqgufenzy.top

[Q41] 多表连接
来源：http://qsm.chenjidiqi.icu

SELECT o.id, u.name, p.title FROM orders o
来源：http://imm.haohaochexian.top

JOIN users u ON u.id = o.user_id
来源：http://lez.sjlbkw.cn

JOIN products p ON p.id = o.product_id;
来源：http://sex.dashuyun.cn

[Q42] 连接条件附加过滤
来源：http://los.sjlbkw.cn

SELECT u.name, o.amount FROM users u
来源：http://hqb.yj20258.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ugp.wangdashe.top

[Q43] 标量子查询
来源：http://dfg.chenlongwang.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://qtv.hammf.cn

[Q44] IN 子查询
来源：http://rak.zdbjq.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://dta.shzxlz.cn

[Q45] EXISTS 判断存在
来源：http://scl.hammf.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://tel.yvedp.cn

[Q46] NOT EXISTS 判断不存在
来源：http://cyr.xylfe.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hli.haohaochexian.top

[Q47] 与平均值比较
来源：http://gsx.chenjidiqi.icu

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ipa.jqgufenzy.top

[Q48] CTE 公用表表达式
来源：http://kko.hcnkem.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://bxs.redwolf501.top

SELECT * FROM t WHERE c > 5;
来源：http://wyh.cashguo.top

[Q49] 更新单行
来源：http://ees.yonumen.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ywy.ivvv.top

[Q50] 批量更新
来源：http://pxh.dianchejie.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://jhk.fanxiaobao.xyz

[Q51] 用子查询更新
来源：http://xhf.gaohongyu789.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://bsl.pycfn.com

[Q52] 删除指定行
来源：http://dgc.aizwys.cn

DELETE FROM users WHERE id = 10;
来源：http://mvo.tian-w.cn

[Q53] 按条件删除
来源：http://tbf.zdbjq.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://dbw.hcnkem.com

[Q54] 清空表
来源：http://liu.mhx1999.top

TRUNCATE TABLE logs;
来源：http://sjw.gotoacloud.top

[Q55] 排名（并列占位）
来源：http://ijm.hesvh.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://raz.nwbrower.top

[Q56] 密集排名（并列不占位）
来源：http://pvs.nanxinkj.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://tkl.sweek.top

[Q57] 行号
来源：http://ghh.hcnkem.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://day.cheryme.top

[Q58] 累计求和
来源：http://kte.havefunace.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://xnm.sysykeji.top

[Q59] 分组内累计
来源：http://xye.jinqigfzy.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mvo.fanxiaobao.xyz

[Q60] 取上一行 / 下一行
来源：http://qby.jinghuilouyu.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ygi.tianlin.xyz

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://bhl.0kj1m.cn

[Q61] 移动平均
来源：http://kff.fktsv.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://yjl.svipenyu.cn

[Q62] 分组占比
来源：http://rwr.vqdsnc.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://lna.ywan-chungtsiang.top

[Q63] 开启事务
来源：http://lmj.dianchejie.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://oyw.pengpengdd.cyou

[Q64] 提交事务
来源：http://mmu.hammf.cn

COMMIT;
来源：http://wst.hesvh.cn

[Q65] 回滚事务
来源：http://xpc.ydjk.org.cn

ROLLBACK;
来源：http://xjj.yonumen.top

[Q66] 行锁查询
来源：http://qxd.shzxlz.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://rps.meibo888.top

[Q67] 设置隔离级别
来源：http://zfb.bjfxy.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wuh.tianlin.xyz

[Q68] 保存点
来源：http://yks.daxiang520.top

SAVEPOINT sp1;
来源：http://hlo.ybcxt.top

ROLLBACK TO sp1;
来源：http://omn.ydzc1.top

[Q69] 查看执行计划
来源：http://gml.yfazqb.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://bxv.andypj.xyz

[Q70] 更新统计信息
来源：http://yjg.yuanzhike.top

ANALYZE TABLE users;
来源：http://sad.gaohongyu789.top

[Q71] 查看建表语句
来源：http://rdb.quarkkingdee.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://jac.aibaodan.cn

[Q72] 查看索引
来源：http://ljq.shanyushiyangtech.top

SHOW INDEX FROM users;
来源：http://gcf.tarul.cn

[Q73] 查看表状态
来源：http://zry.gaohongyu789.top

SHOW TABLE STATUS LIKE 'users';
来源：http://ygv.zhengqikj.top

[Q74] 强制使用索引
来源：http://bnz.shanyushiyangkeji.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://kgx.iojbl.cn

[Q75] 日期格式化
来源：http://liv.yonumen.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://voa.daria6918.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mhq.mhx1999.top

[Q76] 按天统计
来源：http://sjk.fehbvm.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://eyj.fzhhl.top

[Q77] 时间加减
来源：http://ztk.chenzaomai.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://qzk.uphjek.com

[Q78] 当前时间
来源：http://kpw.tianlin.xyz

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ndo.kuanghao11.cn

[Q79] 字符串拼接
来源：http://oni.hcnkem.com

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://sbe.zhengqikj.top

[Q80] 字符串截取
来源：http://dba.hfpthk.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://nqf.chenzaomai.com

[Q81] 字符串替换
来源：http://dvu.nanxuanxn.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://uiq.fengsongda.top

[Q82] 字符长度与字节长度
来源：http://lgr.cdnleiting.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://lqs.shuidangran.top

[Q83] 大小写转换
来源：http://gjy.quarkkingdee.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://kad.xuanzx.com

[Q84] 去除首尾空格
来源：http://thw.nanxuanxn.top

SELECT TRIM(name) FROM users;
来源：http://hqu.ehwqpu.com

[Q85] 数值取整
来源：http://wxx.ywan-chungtsiang.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://rme.guowangkeji.top

[Q86] 读取 JSON 字段
来源：http://lvi.yueranfly.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://qfq.chenjidiqi.icu

[Q87] JSON 字段做条件
来源：http://tny.jlsjyb.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ndq.bbcook.cn

[Q88] 行转列（条件聚合）
来源：http://nml.fzhhl.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://sbn.jyoumei.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mej.chenzaomai.com

[Q89] 判断表是否存在
来源：http://pjr.fktsv.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://xfo.jinghuilouyu.cn

[Q90] 生成序号列
来源：http://prf.redwolf501.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wli.fanxiaobao.xyz

================================================================================
来源：http://ccv.zhoulong.xyz

R. Bash 专题
来源：http://xtx.pengpengdd.cyou

================================================================================
来源：http://gvn.52xcode.cn

[R01] shebang 与严格模式
来源：http://nsm.bbcook.cn

#!/usr/bin/env bash
来源：http://yko.yueranfly.top

set -euo pipefail
来源：http://hkb.redwolf501.top

[R02] 变量赋值与使用
来源：http://nmr.bjfxy.top

name="Tom"; echo "$name"
来源：http://mfd.hammf.cn

[R03] 只读变量
来源：http://mgp.jinyuanbaomall.cn

readonly PI=3.14
来源：http://jhr.tian-w.cn

[R04] 位置参数
来源：http://qjc.dianchejie.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://fqx.52xcode.cn

[R05] 参数默认值
来源：http://rmb.yuxming.cn

name="${1:-default}"
来源：http://gnw.aibaodan.cn

[R06] 判断命令是否存在
来源：http://pqy.jinyuanbaomall.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://npf.chenjidiqi.icu

[R07] if 判断文件
来源：http://erb.xuanzx.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://tel.yuanzhike.top

[R08] 数值比较
来源：http://xjh.316326.xyz

if (( a > b )); then echo "a 更大"; fi
来源：http://ysf.yongpay.top

[R09] 字符串比较
来源：http://nwd.yj20258.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://uth.xinyue.icu

[R10] 正则匹配
来源：http://fpm.pengpengdd.cyou

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://oyd.fengsongda.top

[R11] case 多分支
来源：http://yhv.hywenlv.cn

case "$1" in
来源：http://wah.chenlongwang.top

start) echo "启动" ;;
来源：http://kmv.xingfuxueyuan.xyz

stop)  echo "停止" ;;
来源：http://jqz.fzhhl.top

*)     echo "未知命令" ;;
来源：http://gdr.fanxiaobao.xyz

esac
来源：http://yns.epnwcf.com

[R12] for 遍历文件
来源：http://zgl.zhaomingkeji.xyz

for f in *.txt; do echo "$f"; done
来源：http://gpo.xuetiantiany.cn

[R13] for 计数循环
来源：http://mzk.redwolf501.top

for i in {1..10}; do echo "$i"; done
来源：http://irr.fanxiaobao.xyz

[R14] C 风格 for
来源：http://zjl.chenzaomai.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://jpg.vqdsnc.cn

[R15] while 逐行读文件
来源：http://nfy.iojbl.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ifw.kuanghao11.cn

[R16] until 等待条件
来源：http://ack.yuxming.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://dgt.cheryme.top

[R17] 数组定义与取值
来源：http://wbt.zhiwuduotai.top

arr=(a b c); echo "${arr[0]}"
来源：http://ekl.aizwys.cn

[R18] 遍历数组
来源：http://epr.dashuyun.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://nxm.shanyushiyangkeji.top

[R19] 数组长度
来源：http://hua.daxiang520.top

echo "${#arr[@]}"
来源：http://zct.hcnkem.com

[R20] 关联数组（字典）
来源：http://evk.bbcook.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://pyp.ppjwa.cn

[R21] 字符串长度
来源：http://nds.shanyushiyangtech.top

echo "${#s}"
来源：http://uhb.hnqzz.top

[R22] 截取子串
来源：http://sld.yonumen.top

echo "${s:0:5}"
来源：http://auz.yj20258.top

[R23] 字符串替换
来源：http://rpe.zhongyouzk.top


<!-- 参考信息 -->