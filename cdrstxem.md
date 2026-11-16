代发 wailian999

Java: list.size();  map.size();  s.length()
来源：http://tcq.haohaochexian.top

Go:   len(arr);  len(m)
来源：http://kup.gaohongyu789.top

Ruby: x.length;  x.size
来源：http://pfs.zhiwuduotai.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://aln.jqgufenzy.top

[P05] 判断两个对象内容是否相等
来源：http://wup.jinghuilouyu.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://yky.jiagoushi.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ern.yj202588.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://uep.zhengqikj.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://duv.kuanghao11.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wjm.cheryme.top

Go:   reflect.DeepEqual(a, b)
来源：http://osy.jinyuanbaomall.cn

Ruby: a == b
来源：http://uaq.nanxuanxn.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://eet.yuanzhike.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://kgj.fktsv.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://fij.meibo888.top

PHP:  if (empty($x)) {}
来源：http://hcj.chenjidiqi.icu

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://fzb.jinyuanbaomall.cn

TS:   if (x == null) {}
来源：http://mzk.cqqwz.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://owt.hywenlv.cn

Go:   if x == nil {}
来源：http://yvi.iojbl.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://bxh.ehwqpu.com

C#:   if (x is null) {}
来源：http://gjc.yuxming.cn

[P07] 防抖与节流
来源：http://dmh.xuanzx.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://gbu.yongpay.top

PHP:  // 手写时间戳比较
来源：http://faj.kuanghao11.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qtb.chenjidiqi.icu

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dyw.yfazqb.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wkc.zhongyouzk.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://izz.gaohongyu789.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://giv.zhijiandao.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://dzo.tianlin.xyz

[P08] 处理浮点精度问题
来源：http://jeg.yongpay.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://pyr.xuanzx.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://pgx.gaohongyu789.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ceq.gotoacloud.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ckb.xuetiantiany.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://gso.shangyingyoupin.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://jle.redwolf501.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://afm.yanxiufei.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://bkw.daxiang520.top

================================================================================
来源：http://ptt.jinghuilouyu.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mkn.quarkkingdee.top

================================================================================
来源：http://bkh.hysaishi.cn

[Q01] 创建表
来源：http://rhh.kuanghao11.cn

CREATE TABLE users (
来源：http://gqb.zycfv.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ygf.hongshengwenyu.top

name VARCHAR(50) NOT NULL,
来源：http://cie.snrcjt.cn

email VARCHAR(100) UNIQUE,
来源：http://cjf.daria6918.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ovk.yj20258888.top

);
来源：http://ver.pengpengdd.cyou

[Q02] 创建带外键的表
来源：http://vsc.jlsjyb.cn

CREATE TABLE orders (
来源：http://bae.nanxinkj.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ipx.fzhhl.top

user_id INT NOT NULL,
来源：http://zpg.shuidangran.top

amount DECIMAL(10, 2),
来源：http://gwj.bbcook.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://kfr.daxiang520.top

);
来源：http://yxf.smart0.xyz

[Q03] 增加列
来源：http://qqw.ivvv.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://zkz.guannengcc.top

[Q04] 修改列类型
来源：http://xkr.ppjwa.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://lgu.yj20258888.top

[Q05] 重命名列
来源：http://usy.fanxiaobao.xyz

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://xjq.0kj1m.cn

[Q06] 删除列
来源：http://ehj.hnxiangtu.top

ALTER TABLE users DROP COLUMN age;
来源：http://vxp.yfazqb.com

[Q07] 删除表
来源：http://knn.hfpthk.cn

DROP TABLE IF EXISTS orders;
来源：http://gel.zhongyouzk.top

[Q08] 创建普通索引
来源：http://scr.daxiang520.top

CREATE INDEX idx_users_email ON users(email);
来源：http://loo.tian-w.cn

[Q09] 创建唯一索引
来源：http://ray.aizwys.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://lyc.ydjk.org.cn

[Q10] 插入单行
来源：http://wyc.9152youxi.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://unv.ppjwa.cn

[Q11] 一次插入多行
来源：http://sxs.ctjpmb.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ane.shuidangran.top

[Q12] 插入后取自增 ID
来源：http://udz.tian-w.cn

INSERT INTO users (name) VALUES ('C');
来源：http://erf.redwolf501.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ynf.hesvh.cn

[Q13] 忽略重复插入
来源：http://uel.jinghuilouyu.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://yhm.shuidangran.top

[Q14] 存在则更新（upsert）
来源：http://uhc.epnwcf.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://gru.feifeiyinyue.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://sri.daxiang520.top

[Q15] 查询全部
来源：http://wro.vqdsnc.cn

SELECT * FROM users;
来源：http://nmq.zhijiandao.cn

[Q16] 查询指定列
来源：http://kju.zhengqikj.top

SELECT id, name FROM users;
来源：http://gqk.chenlongwang.top

[Q17] 条件查询
来源：http://grn.pycfn.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://jhi.zdbjq.cn

[Q18] 模糊匹配
来源：http://qye.yongpay.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ots.shanyushiyangtech.top

[Q19] 范围查询
来源：http://xez.cucudq.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mfo.sysykeji.top

[Q20] IN 列表
来源：http://fjx.hesvh.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://anl.ivvv.top

[Q21] 空值判断
来源：http://jat.guowangkeji.top

SELECT * FROM users WHERE email IS NULL;
来源：http://lrw.jlsjyb.cn

[Q22] 排序
来源：http://grr.uphjek.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hqo.zhixingplan.top

[Q23] 分页
来源：http://rps.feifeiyinyue.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://rsc.yongpay.top

[Q24] 去重
来源：http://lvu.chenlongwang.top

SELECT DISTINCT city FROM users;
来源：http://rce.cqqwz.cn

[Q25] 只取前 N 条
来源：http://nco.yvedp.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://dkw.xylfe.cn

[Q26] 计数
来源：http://jrs.cashguo.top

SELECT COUNT(*) FROM users;
来源：http://mxj.ivvv.top

[Q27] 条件计数
来源：http://ybh.sysykeji.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://umj.cucudq.cn

[Q28] 求和与平均
来源：http://fmq.hongshengwenyu.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://jgy.sjlbkw.cn

[Q29] 最大最小值
来源：http://abl.pycfn.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://zam.sysykeji.top

[Q30] 分组统计
来源：http://iwg.tanke756.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://nyk.uphjek.com

[Q31] 分组后过滤
来源：http://jxj.yanxiufei.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hnc.zhoulong.xyz

[Q32] 分组拼接字符串
来源：http://bze.tianlin.xyz

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://kvo.bjfxy.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://gjk.havefunace.top

[Q33] 多列分组
来源：http://phk.yj20258888.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://oyl.fzhhl.top

[Q34] 每组取第一条
来源：http://mjy.ctjpmb.com

SELECT * FROM (
来源：http://qvg.hcnkem.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://dsp.vehdjk.com

) t WHERE rn = 1;
来源：http://gkm.zycfv.cn

[Q35] 内连接
来源：http://rnf.redwolf501.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://cht.epnwcf.com

[Q36] 左连接
来源：http://rku.ydjk.org.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://era.zycfv.cn

[Q37] 右连接
来源：http://rso.ydzc1.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://yjh.xingfuxueyuan.xyz

[Q38] 全外连接（PostgreSQL）
来源：http://zff.jlsjyb.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://vga.jqgfzy.top

[Q39] 自连接（查上下级）
来源：http://sjd.gotoacloud.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://ybq.vehdjk.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://vih.yangfankeji.com

[Q40] 交叉连接（笛卡尔积）
来源：http://zkl.jinqigfzy.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://clj.zhongyouzk.top

[Q41] 多表连接
来源：http://zmi.jianghu66.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://lfi.cdnleiting.top

JOIN users u ON u.id = o.user_id
来源：http://pad.zhiwuduotai.top

JOIN products p ON p.id = o.product_id;
来源：http://tok.ydzc1.top

[Q42] 连接条件附加过滤
来源：http://fem.cqqwz.cn

SELECT u.name, o.amount FROM users u
来源：http://mhy.gzhubu.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://qpw.daxiang520.top

[Q43] 标量子查询
来源：http://nkc.andypj.xyz

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://rxn.gogol.net.cn

[Q44] IN 子查询
来源：http://oge.tian-w.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://tnn.cucudq.cn

[Q45] EXISTS 判断存在
来源：http://uxt.fehbvm.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://pnp.jiagoushi.top

[Q46] NOT EXISTS 判断不存在
来源：http://fls.hnqzz.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xon.mhx1999.top

[Q47] 与平均值比较
来源：http://cmy.cqqwz.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://tuj.jinyuanbaomall.cn

[Q48] CTE 公用表表达式
来源：http://str.sweek.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://vnz.yj20258888.top

SELECT * FROM t WHERE c > 5;
来源：http://uge.fktsv.cn

[Q49] 更新单行
来源：http://gki.iojbl.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://gke.cdnleiting.top

[Q50] 批量更新
来源：http://tox.fktsv.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://tcp.iojbl.cn

[Q51] 用子查询更新
来源：http://vvy.jiagoushi.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://sxm.xylfe.cn

[Q52] 删除指定行
来源：http://uxd.hysaishi.cn

DELETE FROM users WHERE id = 10;
来源：http://xno.ctjpmb.com

[Q53] 按条件删除
来源：http://ghg.meibo888.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ovk.jinghuilouyu.cn

[Q54] 清空表
来源：http://qns.gotoacloud.top

TRUNCATE TABLE logs;
来源：http://ljq.vehdjk.com

[Q55] 排名（并列占位）
来源：http://cbc.xziqi.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://dmu.dashuyun.cn

[Q56] 密集排名（并列不占位）
来源：http://ioj.yuxming.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ylf.xziqi.cn

[Q57] 行号
来源：http://lsy.xziqi.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://bup.chenzaomai.com

[Q58] 累计求和
来源：http://gyj.guannengcc.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://pyu.svipenyu.cn

[Q59] 分组内累计
来源：http://ewy.hfpthk.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://nca.shanyushiyangtech.top

[Q60] 取上一行 / 下一行
来源：http://jwd.c1oappe.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://onv.pycfn.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://qlp.fktsv.cn

[Q61] 移动平均
来源：http://zby.fktsv.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://fur.guowangkeji.top

[Q62] 分组占比
来源：http://rit.jqgfzy.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://kid.hywenlv.cn

[Q63] 开启事务
来源：http://yzc.jyoumei.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://mln.tarul.cn

[Q64] 提交事务
来源：http://lwt.jqgfzy.top

COMMIT;
来源：http://jsr.wangdashe.top

[Q65] 回滚事务
来源：http://bui.mhx1999.top

ROLLBACK;
来源：http://txg.zhongyouzk.top

[Q66] 行锁查询
来源：http://gea.ppjwa.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hww.ydzc1.top

[Q67] 设置隔离级别
来源：http://vdn.cashguo.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://cxj.birdmap.top

[Q68] 保存点
来源：http://wmr.ppjwa.cn

SAVEPOINT sp1;
来源：http://mrk.guannengcc.top

ROLLBACK TO sp1;
来源：http://urm.yonumen.top

[Q69] 查看执行计划
来源：http://ayy.aibaodan.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mba.hywenlv.cn

[Q70] 更新统计信息
来源：http://ukh.jyoumei.cn

ANALYZE TABLE users;
来源：http://leq.gogol.net.cn

[Q71] 查看建表语句
来源：http://fct.daxiang520.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://qty.hnxiangtu.top

[Q72] 查看索引
来源：http://nri.sxryk.cn

SHOW INDEX FROM users;
来源：http://ktf.daria6918.cn

[Q73] 查看表状态
来源：http://fae.316326.xyz

SHOW TABLE STATUS LIKE 'users';
来源：http://kwg.ywan-chungtsiang.top

[Q74] 强制使用索引
来源：http://dyc.316326.xyz

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://vig.tian-w.cn

[Q75] 日期格式化
来源：http://igg.pycfn.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ayp.hammf.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wxg.svipenyu.cn

[Q76] 按天统计
来源：http://whn.uphjek.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://vec.iojbl.cn

[Q77] 时间加减
来源：http://wqt.shzxlz.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ezo.xziqi.cn

[Q78] 当前时间
来源：http://aau.hongshengwenyu.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://now.yueranfly.top

[Q79] 字符串拼接
来源：http://wcy.316326.xyz

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://tno.iojbl.cn

[Q80] 字符串截取
来源：http://hol.fehbvm.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://uav.ydjk.org.cn

[Q81] 字符串替换
来源：http://mmy.yongpay.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://lix.bbcook.cn

[Q82] 字符长度与字节长度
来源：http://vae.haohaochexian.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://pph.hongshengwenyu.top

[Q83] 大小写转换
来源：http://jfa.svipenyu.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://uvw.tarul.cn

[Q84] 去除首尾空格
来源：http://nus.yvedp.cn

SELECT TRIM(name) FROM users;
来源：http://dhu.tian-w.cn

[Q85] 数值取整
来源：http://hah.yj20258.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://aml.tanke756.top

[Q86] 读取 JSON 字段
来源：http://qzs.aizwys.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://nwx.cdnleiting.top

[Q87] JSON 字段做条件
来源：http://ndn.nwbrower.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://obz.zhaomingkeji.xyz

[Q88] 行转列（条件聚合）
来源：http://uil.hywenlv.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ixu.dashuyun.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://bcv.zycfv.cn

[Q89] 判断表是否存在
来源：http://ymd.ydjk.org.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://brb.cheryme.top

[Q90] 生成序号列
来源：http://lif.jinqigufen.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://zbk.jianghu66.top

================================================================================
来源：http://lmc.ehwqpu.com

R. Bash 专题
来源：http://kqf.redwolf501.top

================================================================================
来源：http://eqj.0kj1m.cn

[R01] shebang 与严格模式
来源：http://qrd.xingfuxueyuan.xyz

#!/usr/bin/env bash
来源：http://jra.bjfxy.top

set -euo pipefail
来源：http://eif.hcnkem.com

[R02] 变量赋值与使用
来源：http://yba.mhx1999.top

name="Tom"; echo "$name"
来源：http://dik.fanxiaobao.xyz

[R03] 只读变量
来源：http://yxs.hnqzz.top

readonly PI=3.14
来源：http://eev.hcnkem.com

[R04] 位置参数
来源：http://fvy.jinghuilouyu.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ckj.xziqi.cn

[R05] 参数默认值
来源：http://jgw.ybcxt.top

name="${1:-default}"
来源：http://tvc.epnwcf.com

[R06] 判断命令是否存在
来源：http://fkw.hywenlv.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://cvz.9152youxi.cn

[R07] if 判断文件
来源：http://qnp.ydzc1.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://vop.ydjk.org.cn

[R08] 数值比较
来源：http://aaq.jinghuilouyu.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://dsk.xinyue.icu

[R09] 字符串比较
来源：http://ksg.aibaodan.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://tnq.jinghuilouyu.cn

[R10] 正则匹配
来源：http://zfl.guannengcc.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://rpj.wangshuangyany.cn

[R11] case 多分支
来源：http://zvi.9152youxi.cn

case "$1" in
来源：http://dtg.yangfankeji.com

start) echo "启动" ;;
来源：http://uzc.guowangkeji.top

stop)  echo "停止" ;;
来源：http://fzm.tanke756.top

*)     echo "未知命令" ;;
来源：http://ngs.jinqigufen.top

esac
来源：http://xyu.gogol.net.cn

[R12] for 遍历文件
来源：http://egf.xuanzx.com

for f in *.txt; do echo "$f"; done
来源：http://zmh.chenjidiqi.icu

[R13] for 计数循环
来源：http://iia.vqdsnc.cn

for i in {1..10}; do echo "$i"; done
来源：http://rsn.shzxlz.cn

[R14] C 风格 for
来源：http://fsv.zhixingplan.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wdw.jinqigfzy.top

[R15] while 逐行读文件
来源：http://enj.ydjk.org.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://vpr.ctjpmb.com

[R16] until 等待条件
来源：http://ndb.haohaochexian.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://rep.zycfv.cn

[R17] 数组定义与取值
来源：http://tlo.jqgfzy.top

arr=(a b c); echo "${arr[0]}"
来源：http://kdm.epnwcf.com

[R18] 遍历数组
来源：http://gmj.nanxuanxn.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://krh.ivvv.top

[R19] 数组长度
来源：http://xhh.pycfn.com

echo "${#arr[@]}"
来源：http://agd.nanxuanxn.top

[R20] 关联数组（字典）
来源：http://czt.uphjek.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://qel.tanke756.top

[R21] 字符串长度
来源：http://roe.yfazqb.com

echo "${#s}"
来源：http://jcr.yj20258.top

[R22] 截取子串
来源：http://bcg.jianghu66.top

echo "${s:0:5}"
来源：http://gfm.chenlongwang.top

[R23] 字符串替换
来源：http://oky.tarul.cn


<!-- 参考信息 -->