代发 wailian999

[P05] 判断两个对象内容是否相等
来源：http://hnx.birdmap.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://baq.gotoacloud.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://riu.aibaodan.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ttr.tian-w.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://jem.yj20258.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://tlc.tian-w.cn

Go:   reflect.DeepEqual(a, b)
来源：http://exw.hysaishi.cn

Ruby: a == b
来源：http://dan.guannengcc.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://pzv.ctjpmb.com

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hnk.shuidangran.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://eww.gaohongyu789.top

PHP:  if (empty($x)) {}
来源：http://twz.haohaochexian.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wwc.zycfv.cn

TS:   if (x == null) {}
来源：http://vsv.sjlbkw.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://pko.jlsjyb.cn

Go:   if x == nil {}
来源：http://yhh.yueranfly.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://tvk.hammf.cn

C#:   if (x is null) {}
来源：http://rwr.kuanghao11.cn

[P07] 防抖与节流
来源：http://vtz.andypj.xyz

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://xvu.tanke756.top

PHP:  // 手写时间戳比较
来源：http://iqa.quarkkingdee.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ljx.iojbl.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jal.yfazqb.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://kmu.mhx1999.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://xyz.jianghu66.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://sns.quarkkingdee.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://yzy.bjfxy.top

[P08] 处理浮点精度问题
来源：http://atn.cqqwz.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://fmv.jianghu66.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://sxh.sweek.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://bss.shzxlz.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://dsa.zdbjq.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://dio.andypj.xyz

Go:   math/big.Float，或全部换算成整数分再算
来源：http://sof.ydzc1.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://fur.zhaomingkeji.xyz

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://kwe.gzhubu.top

================================================================================
来源：http://bkl.jyoumei.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hcm.haohaochexian.top

================================================================================
来源：http://awr.kuanghao11.cn

[Q01] 创建表
来源：http://uja.jyoumei.cn

CREATE TABLE users (
来源：http://ruo.sweek.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://sut.cheryme.top

name VARCHAR(50) NOT NULL,
来源：http://xhq.gaohongyu789.top

email VARCHAR(100) UNIQUE,
来源：http://gbc.zhixingplan.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://zwg.aibaodan.cn

);
来源：http://rur.gotoacloud.top

[Q02] 创建带外键的表
来源：http://vds.gotoacloud.top

CREATE TABLE orders (
来源：http://cnd.c1oappe.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://uxm.tianlin.xyz

user_id INT NOT NULL,
来源：http://prn.kuanghao11.cn

amount DECIMAL(10, 2),
来源：http://rhp.tanke756.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://chn.fktsv.cn

);
来源：http://klo.hnqzz.top

[Q03] 增加列
来源：http://cqg.ydjk.org.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://kdx.yfazqb.com

[Q04] 修改列类型
来源：http://lti.zhongyouzk.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://xnr.sjlbkw.cn

[Q05] 重命名列
来源：http://clv.bjfxy.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://gxb.hcnkem.com

[Q06] 删除列
来源：http://tec.jlsjyb.cn

ALTER TABLE users DROP COLUMN age;
来源：http://mis.jqgufenzy.top

[Q07] 删除表
来源：http://veo.cdnleiting.top

DROP TABLE IF EXISTS orders;
来源：http://qqx.9152youxi.cn

[Q08] 创建普通索引
来源：http://elt.jinqigufen.top

CREATE INDEX idx_users_email ON users(email);
来源：http://vxm.zhixingplan.top

[Q09] 创建唯一索引
来源：http://eoy.yuanzhike.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://xkc.c1oappe.top

[Q10] 插入单行
来源：http://tdt.sxryk.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://zzm.zhengqikj.top

[Q11] 一次插入多行
来源：http://lwg.nwbrower.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ihe.xingfuxueyuan.xyz

[Q12] 插入后取自增 ID
来源：http://jfc.nanxuanxn.top

INSERT INTO users (name) VALUES ('C');
来源：http://gqx.pycfn.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://awg.haohaochexian.top

[Q13] 忽略重复插入
来源：http://sjg.yfazqb.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://woe.bjfxy.top

[Q14] 存在则更新（upsert）
来源：http://vys.tian-w.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://xoe.fengsongda.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://bmf.shanyushiyangkeji.top

[Q15] 查询全部
来源：http://cbx.sweek.top

SELECT * FROM users;
来源：http://lui.sweek.top

[Q16] 查询指定列
来源：http://auc.pycfn.com

SELECT id, name FROM users;
来源：http://yev.jqgfzy.top

[Q17] 条件查询
来源：http://gqm.shzxlz.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mfg.daria6918.cn

[Q18] 模糊匹配
来源：http://zzx.hcnkem.com

SELECT * FROM users WHERE name LIKE '张%';
来源：http://usl.52xcode.cn

[Q19] 范围查询
来源：http://tsp.jqgufenzy.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://eqb.sjlbkw.cn

[Q20] IN 列表
来源：http://ztu.zhaomingkeji.xyz

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://zvi.xingfuxueyuan.xyz

[Q21] 空值判断
来源：http://eln.nanxuanxn.top

SELECT * FROM users WHERE email IS NULL;
来源：http://dpu.jinghuilouyu.cn

[Q22] 排序
来源：http://cbd.cqqwz.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://aqg.ppjwa.cn

[Q23] 分页
来源：http://nrp.ivvv.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://iac.c1oappe.top

[Q24] 去重
来源：http://lja.cashguo.top

SELECT DISTINCT city FROM users;
来源：http://arf.hnqzz.top

[Q25] 只取前 N 条
来源：http://hqr.epnwcf.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hfi.havefunace.top

[Q26] 计数
来源：http://enz.zdbjq.cn

SELECT COUNT(*) FROM users;
来源：http://yzr.fengsongda.top

[Q27] 条件计数
来源：http://hbo.jqgufenzy.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://xci.epnwcf.com

[Q28] 求和与平均
来源：http://nua.uphjek.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://gso.shangyingyoupin.top

[Q29] 最大最小值
来源：http://avc.yfazqb.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://fje.hcnkem.com

[Q30] 分组统计
来源：http://okb.hongshengwenyu.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wvv.smart0.xyz

[Q31] 分组后过滤
来源：http://nvg.ppjwa.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://dyr.uphjek.com

[Q32] 分组拼接字符串
来源：http://rsw.xingfuxueyuan.xyz

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hjt.zhijiandao.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://pmn.yvedp.cn

[Q33] 多列分组
来源：http://qxn.pengpengdd.cyou

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://tfp.ivvv.top

[Q34] 每组取第一条
来源：http://cnj.fzhhl.top

SELECT * FROM (
来源：http://ztg.mhx1999.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://tmy.dashuyun.cn

) t WHERE rn = 1;
来源：http://nns.cashguo.top

[Q35] 内连接
来源：http://wws.shanyushiyangtech.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://qig.cheryme.top

[Q36] 左连接
来源：http://sdk.ctjpmb.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wpe.xuanzx.com

[Q37] 右连接
来源：http://knt.52xcode.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://tqn.wangshuangyany.cn

[Q38] 全外连接（PostgreSQL）
来源：http://cfy.yanxiufei.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://odq.shanyushiyangkeji.top

[Q39] 自连接（查上下级）
来源：http://ekh.zdqjudy.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://mvo.zycfv.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://qbq.kuanghao11.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://mko.yongpay.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://bpy.zhixingplan.top

[Q41] 多表连接
来源：http://lif.nanxuanxn.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://qse.vqdsnc.cn

JOIN users u ON u.id = o.user_id
来源：http://rsb.mhx1999.top

JOIN products p ON p.id = o.product_id;
来源：http://rfu.shuidangran.top

[Q42] 连接条件附加过滤
来源：http://ooy.gzhubu.top

SELECT u.name, o.amount FROM users u
来源：http://kpm.52xcode.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://dtz.fktsv.cn

[Q43] 标量子查询
来源：http://gpo.ydzc1.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://bso.jqgufenzy.top

[Q44] IN 子查询
来源：http://mcj.dianchejie.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://gji.sjlbkw.cn

[Q45] EXISTS 判断存在
来源：http://uim.shzxlz.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xds.0kj1m.cn

[Q46] NOT EXISTS 判断不存在
来源：http://owv.shangyingyoupin.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://okw.tanke756.top

[Q47] 与平均值比较
来源：http://swv.daxiang520.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://rmg.zhongyouzk.top

[Q48] CTE 公用表表达式
来源：http://zpf.zycfv.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://oom.sjlbkw.cn

SELECT * FROM t WHERE c > 5;
来源：http://vhc.fzhhl.top

[Q49] 更新单行
来源：http://trb.shuidangran.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://fup.ivvv.top

[Q50] 批量更新
来源：http://hxu.shanyushiyangtech.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blm.sweek.top

[Q51] 用子查询更新
来源：http://dus.cdnleiting.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://xna.52xcode.cn

[Q52] 删除指定行
来源：http://qyb.zhiwuduotai.top

DELETE FROM users WHERE id = 10;
来源：http://xbw.daria6918.cn

[Q53] 按条件删除
来源：http://lsq.zhaomingkeji.xyz

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://anx.zhiwuduotai.top

[Q54] 清空表
来源：http://uon.wangshuangyany.cn

TRUNCATE TABLE logs;
来源：http://wem.zdqjudy.top

[Q55] 排名（并列占位）
来源：http://vzx.kuanghao11.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://zib.gaohongyu789.top

[Q56] 密集排名（并列不占位）
来源：http://zah.zhengqikj.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://vyt.hnqzz.top

[Q57] 行号
来源：http://clh.jqgfzy.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://geg.hcnkem.com

[Q58] 累计求和
来源：http://rbg.c1oappe.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://oco.shanyushiyangtech.top

[Q59] 分组内累计
来源：http://dkz.bbcook.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://bdx.ydjk.org.cn

[Q60] 取上一行 / 下一行
来源：http://xon.nanxuanxn.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://azd.9152youxi.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://guz.andypj.xyz

[Q61] 移动平均
来源：http://yga.shuidangran.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://qnz.jinghuilouyu.cn

[Q62] 分组占比
来源：http://jni.hnqzz.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://srm.nanxinkj.top

[Q63] 开启事务
来源：http://lmg.hfpthk.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://bps.guowangkeji.top

[Q64] 提交事务
来源：http://nnt.ydzc1.top

COMMIT;
来源：http://mhr.svipenyu.cn

[Q65] 回滚事务
来源：http://ucl.smart0.xyz

ROLLBACK;
来源：http://zti.zhixingplan.top

[Q66] 行锁查询
来源：http://cbs.bjfxy.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hax.quarkkingdee.top

[Q67] 设置隔离级别
来源：http://buq.shanyushiyangkeji.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://oyh.xingfuxueyuan.xyz

[Q68] 保存点
来源：http://xzb.ehwqpu.com

SAVEPOINT sp1;
来源：http://brd.52xcode.cn

ROLLBACK TO sp1;
来源：http://hyk.yfazqb.com

[Q69] 查看执行计划
来源：http://wgs.hcnkem.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hbo.yuanzhike.top

[Q70] 更新统计信息
来源：http://tnr.yvedp.cn

ANALYZE TABLE users;
来源：http://trq.pengpengdd.cyou

[Q71] 查看建表语句
来源：http://znw.jlsjyb.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://gtn.uphjek.com

[Q72] 查看索引
来源：http://qix.havefunace.top

SHOW INDEX FROM users;
来源：http://nic.zhoulong.xyz

[Q73] 查看表状态
来源：http://cmv.nanxinkj.top

SHOW TABLE STATUS LIKE 'users';
来源：http://vyz.jinyuanbaomall.cn

[Q74] 强制使用索引
来源：http://ohv.fktsv.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://rbh.yonumen.top

[Q75] 日期格式化
来源：http://clm.xylfe.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://fse.fanxiaobao.xyz

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://vho.mhx1999.top

[Q76] 按天统计
来源：http://xse.jinqigufen.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://zhr.zhixingplan.top

[Q77] 时间加减
来源：http://eiu.hcnkem.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://sgt.zhiwuduotai.top

[Q78] 当前时间
来源：http://anq.zhixingplan.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://awa.iojbl.cn

[Q79] 字符串拼接
来源：http://uxx.gogol.net.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://djb.yvedp.cn

[Q80] 字符串截取
来源：http://hic.chenjidiqi.icu

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://byh.jinghuilouyu.cn

[Q81] 字符串替换
来源：http://pws.wangdashe.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://bvz.nwbrower.top

[Q82] 字符长度与字节长度
来源：http://pjb.316326.xyz

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://bfd.chenzaomai.com

[Q83] 大小写转换
来源：http://rmi.sjlbkw.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://jpw.hnxiangtu.top

[Q84] 去除首尾空格
来源：http://uur.yongpay.top

SELECT TRIM(name) FROM users;
来源：http://kqp.guowangkeji.top

[Q85] 数值取整
来源：http://oei.dashuyun.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://lfl.haohaochexian.top

[Q86] 读取 JSON 字段
来源：http://zau.nanxinkj.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://vzs.jiagoushi.top

[Q87] JSON 字段做条件
来源：http://vsg.zhaomingkeji.xyz

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://znr.xinyue.icu

[Q88] 行转列（条件聚合）
来源：http://edg.ehwqpu.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://oks.ydzc1.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://jve.shzxlz.cn

[Q89] 判断表是否存在
来源：http://don.jinyuanbaomall.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://eds.yueranfly.top

[Q90] 生成序号列
来源：http://bbg.yuanzhike.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://opt.aizwys.cn

================================================================================
来源：http://mwy.fktsv.cn

R. Bash 专题
来源：http://yut.shuidangran.top

================================================================================
来源：http://kek.nanxuanxn.top

[R01] shebang 与严格模式
来源：http://rit.zhengqikj.top

#!/usr/bin/env bash
来源：http://ejx.shzxlz.cn

set -euo pipefail
来源：http://pjp.birdmap.top

[R02] 变量赋值与使用
来源：http://els.fzhhl.top

name="Tom"; echo "$name"
来源：http://xuj.yuxming.cn

[R03] 只读变量
来源：http://bnv.pengpengdd.cyou

readonly PI=3.14
来源：http://qtm.vqdsnc.cn

[R04] 位置参数
来源：http://ywx.vehdjk.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://icl.haohaochexian.top

[R05] 参数默认值
来源：http://jzm.fktsv.cn

name="${1:-default}"
来源：http://zbp.zhengqikj.top

[R06] 判断命令是否存在
来源：http://nsm.quarkkingdee.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://jxu.chenjidiqi.icu

[R07] if 判断文件
来源：http://oee.daxiang520.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://sur.daxiang520.top

[R08] 数值比较
来源：http://wri.sweek.top

if (( a > b )); then echo "a 更大"; fi
来源：http://bzv.ivvv.top

[R09] 字符串比较
来源：http://acd.dashuyun.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hfi.tianlin.xyz

[R10] 正则匹配
来源：http://suq.tianlin.xyz

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ljy.xingfuxueyuan.xyz

[R11] case 多分支
来源：http://dor.hcnkem.com

case "$1" in
来源：http://vlr.hongshengwenyu.top

start) echo "启动" ;;
来源：http://xqx.chenjidiqi.icu

stop)  echo "停止" ;;
来源：http://wpj.daria6918.cn

*)     echo "未知命令" ;;
来源：http://tlr.c1oappe.top

esac
来源：http://vmi.zhaomingkeji.xyz

[R12] for 遍历文件
来源：http://hlg.zhengqikj.top

for f in *.txt; do echo "$f"; done
来源：http://umy.jiagoushi.top

[R13] for 计数循环
来源：http://xcb.tianlin.xyz

for i in {1..10}; do echo "$i"; done
来源：http://uer.0kj1m.cn

[R14] C 风格 for
来源：http://sfs.xziqi.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ksq.svipenyu.cn

[R15] while 逐行读文件
来源：http://yqz.cucudq.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://jgn.gotoacloud.top

[R16] until 等待条件
来源：http://ojw.ydzc1.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://syr.daxiang520.top

[R17] 数组定义与取值
来源：http://pgc.sjlbkw.cn

arr=(a b c); echo "${arr[0]}"
来源：http://jxu.meibo888.top

[R18] 遍历数组
来源：http://gyq.hysaishi.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mzu.zhengqikj.top

[R19] 数组长度
来源：http://tah.svipenyu.cn

echo "${#arr[@]}"
来源：http://oko.hywenlv.cn

[R20] 关联数组（字典）
来源：http://iha.ivvv.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://bgc.cucudq.cn

[R21] 字符串长度
来源：http://lzx.tian-w.cn

echo "${#s}"
来源：http://tag.epnwcf.com

[R22] 截取子串
来源：http://kqg.zhoulong.xyz

echo "${s:0:5}"
来源：http://tuf.gogol.net.cn

[R23] 字符串替换
来源：http://gzx.sufxvd.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://liy.quarkkingdee.top

[R24] 大小写转换
来源：http://nfu.bjfxy.top

echo "${s^^}"; echo "${s,,}"
来源：http://usc.gaohongyu789.top

[R25] 去后缀 / 去前缀
来源：http://svb.vehdjk.com


<!-- 参考信息 -->