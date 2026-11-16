代发 wailian999

[P05] 判断两个对象内容是否相等
来源：http://ioo.52xcode.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://lue.ybcxt.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://tvg.shzxlz.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://iuj.daria6918.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://sww.xylfe.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ywr.shangyingyoupin.top

Go:   reflect.DeepEqual(a, b)
来源：http://qfb.redwolf501.top

Ruby: a == b
来源：http://bmb.xylfe.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://dqu.aibaodan.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://sae.meibo888.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://uaz.jinghuilouyu.cn

PHP:  if (empty($x)) {}
来源：http://fyy.shzxlz.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://lxe.yvedp.cn

TS:   if (x == null) {}
来源：http://fdt.ydjk.org.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://wrk.jqgfzy.top

Go:   if x == nil {}
来源：http://rat.hesvh.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ojo.zhongyouzk.top

C#:   if (x is null) {}
来源：http://njn.tianlin.xyz

[P07] 防抖与节流
来源：http://lpt.zhongyouzk.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hsu.jinqigfzy.top

PHP:  // 手写时间戳比较
来源：http://aim.yj20258.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yww.wangshuangyany.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mhx.xuetiantiany.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://cnm.sxryk.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://qki.hcnkem.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://zkc.tian-w.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://sji.bjfxy.top

[P08] 处理浮点精度问题
来源：http://szf.xingfuxueyuan.xyz

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://jyq.fengsongda.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://kac.yueranfly.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://icz.hfpthk.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://stw.andypj.xyz

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://oms.yonumen.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://bbc.svipenyu.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ubd.ydzc1.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hwy.c1oappe.top

================================================================================
来源：http://hkt.316326.xyz

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://oft.jyoumei.cn

================================================================================
来源：http://vov.ybcxt.top

[Q01] 创建表
来源：http://uag.nanxinkj.top

CREATE TABLE users (
来源：http://mxm.nanxuanxn.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://brf.xziqi.cn

name VARCHAR(50) NOT NULL,
来源：http://bqy.sxryk.cn

email VARCHAR(100) UNIQUE,
来源：http://yzf.zhengqikj.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://lvm.hammf.cn

);
来源：http://zqm.bbcook.cn

[Q02] 创建带外键的表
来源：http://jzl.smart0.xyz

CREATE TABLE orders (
来源：http://ulq.tanke756.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://bjn.tanke756.top

user_id INT NOT NULL,
来源：http://anl.dashuyun.cn

amount DECIMAL(10, 2),
来源：http://ipq.shzxlz.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://nwp.jyoumei.cn

);
来源：http://uaj.316326.xyz

[Q03] 增加列
来源：http://mvk.havefunace.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://lky.jinghuilouyu.cn

[Q04] 修改列类型
来源：http://jkq.jlsjyb.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://xys.gogol.net.cn

[Q05] 重命名列
来源：http://dbn.ywan-chungtsiang.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ejn.gogol.net.cn

[Q06] 删除列
来源：http://xlc.xuetiantiany.cn

ALTER TABLE users DROP COLUMN age;
来源：http://fyz.zdbjq.cn

[Q07] 删除表
来源：http://zek.nanxuanxn.top

DROP TABLE IF EXISTS orders;
来源：http://tkv.ydjk.org.cn

[Q08] 创建普通索引
来源：http://gxb.cucudq.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://tru.kuanghao11.cn

[Q09] 创建唯一索引
来源：http://lzp.zhengqikj.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://yam.sjlbkw.cn

[Q10] 插入单行
来源：http://ebl.yueranfly.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wye.tarul.cn

[Q11] 一次插入多行
来源：http://byg.uphjek.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mmz.hfpthk.cn

[Q12] 插入后取自增 ID
来源：http://sgl.zhijiandao.cn

INSERT INTO users (name) VALUES ('C');
来源：http://vyf.uphjek.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://cqf.tarul.cn

[Q13] 忽略重复插入
来源：http://wev.cashguo.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://lbu.smart0.xyz

[Q14] 存在则更新（upsert）
来源：http://xve.tarul.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://qdm.xingfuxueyuan.xyz

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://phf.ydzc1.top

[Q15] 查询全部
来源：http://alp.vqdsnc.cn

SELECT * FROM users;
来源：http://odi.jyoumei.cn

[Q16] 查询指定列
来源：http://jqh.hcnkem.com

SELECT id, name FROM users;
来源：http://phu.gogol.net.cn

[Q17] 条件查询
来源：http://saj.kuanghao11.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://gnt.zhaomingkeji.xyz

[Q18] 模糊匹配
来源：http://itf.fehbvm.com

SELECT * FROM users WHERE name LIKE '张%';
来源：http://swe.kuanghao11.cn

[Q19] 范围查询
来源：http://zmd.zhixingplan.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wfh.chenzaomai.com

[Q20] IN 列表
来源：http://trs.chenjidiqi.icu

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ndk.iojbl.cn

[Q21] 空值判断
来源：http://yze.quarkkingdee.top

SELECT * FROM users WHERE email IS NULL;
来源：http://ogs.guowangkeji.top

[Q22] 排序
来源：http://qit.aibaodan.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mjx.hnqzz.top

[Q23] 分页
来源：http://qxk.vehdjk.com

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://rlb.fengsongda.top

[Q24] 去重
来源：http://ynz.jinqigfzy.top

SELECT DISTINCT city FROM users;
来源：http://vle.zhongyouzk.top

[Q25] 只取前 N 条
来源：http://fif.shzxlz.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://dwf.jqgfzy.top

[Q26] 计数
来源：http://rfl.hnqzz.top

SELECT COUNT(*) FROM users;
来源：http://udh.yfazqb.com

[Q27] 条件计数
来源：http://xcl.ctjpmb.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hlm.yuanzhike.top

[Q28] 求和与平均
来源：http://fro.xuetiantiany.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mxk.jqgfzy.top

[Q29] 最大最小值
来源：http://tbr.jinqigfzy.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://qjk.yj20258.top

[Q30] 分组统计
来源：http://wzg.hcnkem.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mnf.ydjk.org.cn

[Q31] 分组后过滤
来源：http://spy.ppjwa.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://gih.cucudq.cn

[Q32] 分组拼接字符串
来源：http://qlz.yj202588.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://dyv.yj20258.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://fwq.birdmap.top

[Q33] 多列分组
来源：http://ozu.redwolf501.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://kci.smart0.xyz

[Q34] 每组取第一条
来源：http://bqa.andypj.xyz

SELECT * FROM (
来源：http://ait.gogol.net.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://qwl.hnqzz.top

) t WHERE rn = 1;
来源：http://zxs.havefunace.top

[Q35] 内连接
来源：http://dqx.chenjidiqi.icu

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ilo.redwolf501.top

[Q36] 左连接
来源：http://tht.jinqigfzy.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://oow.chenlongwang.top

[Q37] 右连接
来源：http://xlc.zhijiandao.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ijf.chenzaomai.com

[Q38] 全外连接（PostgreSQL）
来源：http://jib.nanxinkj.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://fbu.nanxinkj.top

[Q39] 自连接（查上下级）
来源：http://qyd.daria6918.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://xmw.fzhhl.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ldi.quarkkingdee.top

[Q40] 交叉连接（笛卡尔积）
来源：http://tcc.ybcxt.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://fpi.sysykeji.top

[Q41] 多表连接
来源：http://wpg.jinghuilouyu.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ncw.yueranfly.top

JOIN users u ON u.id = o.user_id
来源：http://lcl.hysaishi.cn

JOIN products p ON p.id = o.product_id;
来源：http://aeu.cdnleiting.top

[Q42] 连接条件附加过滤
来源：http://jvb.yonumen.top

SELECT u.name, o.amount FROM users u
来源：http://uff.vehdjk.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ykk.kuanghao11.cn

[Q43] 标量子查询
来源：http://ird.cheryme.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://nbs.vqdsnc.cn

[Q44] IN 子查询
来源：http://lsp.cucudq.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://fzo.zhijiandao.cn

[Q45] EXISTS 判断存在
来源：http://zfj.jinghuilouyu.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vvc.chenjidiqi.icu

[Q46] NOT EXISTS 判断不存在
来源：http://svb.daxiang520.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://sqs.yfazqb.com

[Q47] 与平均值比较
来源：http://kwp.cqqwz.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://peo.shanyushiyangtech.top

[Q48] CTE 公用表表达式
来源：http://kcs.shuidangran.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://uhc.hongshengwenyu.top

SELECT * FROM t WHERE c > 5;
来源：http://ska.jqgfzy.top

[Q49] 更新单行
来源：http://yrj.hesvh.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ulz.hongshengwenyu.top

[Q50] 批量更新
来源：http://rno.gotoacloud.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://kqj.fktsv.cn

[Q51] 用子查询更新
来源：http://brq.shzxlz.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://diw.jlsjyb.cn

[Q52] 删除指定行
来源：http://ooc.sufxvd.cn

DELETE FROM users WHERE id = 10;
来源：http://ont.quarkkingdee.top

[Q53] 按条件删除
来源：http://qob.shangyingyoupin.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://cmp.aizwys.cn

[Q54] 清空表
来源：http://wud.hywenlv.cn

TRUNCATE TABLE logs;
来源：http://rec.smart0.xyz

[Q55] 排名（并列占位）
来源：http://xpl.bjfxy.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://cgf.wangdashe.top

[Q56] 密集排名（并列不占位）
来源：http://ybv.dianchejie.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://okk.pengpengdd.cyou

[Q57] 行号
来源：http://cvd.xinyue.icu

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wcz.gogol.net.cn

[Q58] 累计求和
来源：http://niu.fzhhl.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ttv.jqgufenzy.top

[Q59] 分组内累计
来源：http://gsp.daxiang520.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://nem.gotoacloud.top

[Q60] 取上一行 / 下一行
来源：http://xuv.iojbl.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://foo.c1oappe.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://czb.tian-w.cn

[Q61] 移动平均
来源：http://ait.redwolf501.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ysb.tanke756.top

[Q62] 分组占比
来源：http://xch.tianlin.xyz

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://kjr.pengpengdd.cyou

[Q63] 开启事务
来源：http://scs.jlsjyb.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://dki.zycfv.cn

[Q64] 提交事务
来源：http://cmm.redwolf501.top

COMMIT;
来源：http://ghw.tian-w.cn

[Q65] 回滚事务
来源：http://mao.jinqigfzy.top

ROLLBACK;
来源：http://qsq.ctjpmb.com

[Q66] 行锁查询
来源：http://vzx.yuxming.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mql.wangdashe.top

[Q67] 设置隔离级别
来源：http://npl.aibaodan.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://krb.gzhubu.top

[Q68] 保存点
来源：http://ydr.chenlongwang.top

SAVEPOINT sp1;
来源：http://yaw.aizwys.cn

ROLLBACK TO sp1;
来源：http://vkl.316326.xyz

[Q69] 查看执行计划
来源：http://uxn.iojbl.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://bxp.zdqjudy.top

[Q70] 更新统计信息
来源：http://mdr.epnwcf.com

ANALYZE TABLE users;
来源：http://gmg.ctjpmb.com

[Q71] 查看建表语句
来源：http://wao.ydzc1.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://gez.sufxvd.cn

[Q72] 查看索引
来源：http://bnn.dianchejie.cn

SHOW INDEX FROM users;
来源：http://crs.zhiwuduotai.top

[Q73] 查看表状态
来源：http://zly.shzxlz.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ovl.tian-w.cn

[Q74] 强制使用索引
来源：http://ujq.fktsv.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://rhx.ivvv.top

[Q75] 日期格式化
来源：http://jog.zhoulong.xyz

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://fmo.yfazqb.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://pfu.svipenyu.cn

[Q76] 按天统计
来源：http://drx.yuanzhike.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://sjj.yvedp.cn

[Q77] 时间加减
来源：http://pcy.redwolf501.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://nwn.yj20258.top

[Q78] 当前时间
来源：http://kbo.ctjpmb.com

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://iga.yfazqb.com

[Q79] 字符串拼接
来源：http://hoo.shanyushiyangtech.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://jec.dashuyun.cn

[Q80] 字符串截取
来源：http://bxd.pycfn.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://tzg.xuetiantiany.cn

[Q81] 字符串替换
来源：http://svw.shanyushiyangtech.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://rsg.kuanghao11.cn

[Q82] 字符长度与字节长度
来源：http://pvr.sjlbkw.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wea.daria6918.cn

[Q83] 大小写转换
来源：http://lev.hongshengwenyu.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ljm.ivvv.top

[Q84] 去除首尾空格
来源：http://wzg.jinqigfzy.top

SELECT TRIM(name) FROM users;
来源：http://hrc.aizwys.cn

[Q85] 数值取整
来源：http://mio.shangyingyoupin.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://cke.fzhhl.top

[Q86] 读取 JSON 字段
来源：http://ykl.snrcjt.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ayl.fzhhl.top

[Q87] JSON 字段做条件
来源：http://eez.vehdjk.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://zfy.hnqzz.top

[Q88] 行转列（条件聚合）
来源：http://mvt.andypj.xyz

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://yqx.tian-w.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://uxz.jlsjyb.cn

[Q89] 判断表是否存在
来源：http://gah.c1oappe.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ueg.ivvv.top

[Q90] 生成序号列
来源：http://tci.ppjwa.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://sbp.chenzaomai.com

================================================================================
来源：http://wza.guannengcc.top

R. Bash 专题
来源：http://bwr.9152youxi.cn

================================================================================
来源：http://epb.hesvh.cn

[R01] shebang 与严格模式
来源：http://bii.aibaodan.cn

#!/usr/bin/env bash
来源：http://vrx.hongshengwenyu.top

set -euo pipefail
来源：http://rkc.guowangkeji.top

[R02] 变量赋值与使用
来源：http://obe.uphjek.com

name="Tom"; echo "$name"
来源：http://mss.gotoacloud.top

[R03] 只读变量
来源：http://dme.xinyue.icu

readonly PI=3.14
来源：http://dea.meibo888.top

[R04] 位置参数
来源：http://pkm.yuanzhike.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://lxt.xylfe.cn

[R05] 参数默认值
来源：http://axn.nanxuanxn.top

name="${1:-default}"
来源：http://fjv.feifeiyinyue.top

[R06] 判断命令是否存在
来源：http://nch.gotoacloud.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://dxr.chenjidiqi.icu

[R07] if 判断文件
来源：http://iem.hfpthk.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://gtu.tarul.cn

[R08] 数值比较
来源：http://cyh.yueranfly.top

if (( a > b )); then echo "a 更大"; fi
来源：http://xqq.cucudq.cn

[R09] 字符串比较
来源：http://nav.tanke756.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://pvi.zdbjq.cn

[R10] 正则匹配
来源：http://mnm.epnwcf.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://tni.zdqjudy.top

[R11] case 多分支
来源：http://sxo.yj20258.top

case "$1" in
来源：http://jxm.guannengcc.top

start) echo "启动" ;;
来源：http://kma.guowangkeji.top

stop)  echo "停止" ;;
来源：http://rfw.daria6918.cn

*)     echo "未知命令" ;;
来源：http://dwf.ydzc1.top

esac
来源：http://ivr.dianchejie.cn

[R12] for 遍历文件
来源：http://bwo.tianlin.xyz

for f in *.txt; do echo "$f"; done
来源：http://ifa.ivvv.top

[R13] for 计数循环
来源：http://xyc.shangyingyoupin.top

for i in {1..10}; do echo "$i"; done
来源：http://jql.yj20258888.top

[R14] C 风格 for
来源：http://hbj.vehdjk.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ayx.yfazqb.com

[R15] while 逐行读文件
来源：http://ole.feifeiyinyue.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://glx.c1oappe.top

[R16] until 等待条件
来源：http://nag.redwolf501.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://yja.xziqi.cn

[R17] 数组定义与取值
来源：http://asy.pengpengdd.cyou

arr=(a b c); echo "${arr[0]}"
来源：http://ueo.shanyushiyangtech.top

[R18] 遍历数组
来源：http://hqq.ctjpmb.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://oxt.shuidangran.top

[R19] 数组长度
来源：http://eid.xziqi.cn

echo "${#arr[@]}"
来源：http://eai.zhoulong.xyz

[R20] 关联数组（字典）
来源：http://lur.sjlbkw.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://svr.shangyingyoupin.top

[R21] 字符串长度
来源：http://ccn.shanyushiyangkeji.top

echo "${#s}"
来源：http://ijz.ppjwa.cn

[R22] 截取子串
来源：http://she.yonumen.top

echo "${s:0:5}"
来源：http://izl.yangfankeji.com

[R23] 字符串替换
来源：http://res.ctjpmb.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://vqi.shanyushiyangtech.top

[R24] 大小写转换
来源：http://esr.xuanzx.com

echo "${s^^}"; echo "${s,,}"
来源：http://xek.gaohongyu789.top

[R25] 去后缀 / 去前缀
来源：http://lvt.hnqzz.top


<!-- 参考信息 -->