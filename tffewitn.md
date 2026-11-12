代发 wailian999

[P05] 判断两个对象内容是否相等
来源：http://zyh.dianchejie.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://qfc.xziqi.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wrp.shanyushiyangkeji.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://xcg.316326.xyz

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://bhr.yuanzhike.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://eda.yj20258.top

Go:   reflect.DeepEqual(a, b)
来源：http://ydv.zhiwuduotai.top

Ruby: a == b
来源：http://gpw.xingfuxueyuan.xyz

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://pyn.52xcode.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://npf.zhixingplan.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://qya.jinqigufen.top

PHP:  if (empty($x)) {}
来源：http://wfg.mhx1999.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://aaq.pengpengdd.cyou

TS:   if (x == null) {}
来源：http://tmp.nanxinkj.top

Java: if (x == null || x.isEmpty()) {}
来源：http://qyd.chenjidiqi.icu

Go:   if x == nil {}
来源：http://sov.chenzaomai.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://lse.chenjidiqi.icu

C#:   if (x is null) {}
来源：http://fit.yonumen.top

[P07] 防抖与节流
来源：http://owe.iojbl.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ysr.yj20258888.top

PHP:  // 手写时间戳比较
来源：http://yst.yvedp.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://luy.yuxming.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://anc.guannengcc.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://pnh.aizwys.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://trh.snrcjt.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://jbh.guowangkeji.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://qvs.zhongyouzk.top

[P08] 处理浮点精度问题
来源：http://gnh.hongshengwenyu.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://xdv.tarul.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ipt.smart0.xyz

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://nov.mhx1999.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://nfz.hnxiangtu.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://utg.pycfn.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://auo.hywenlv.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hug.sufxvd.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://nkz.hysaishi.cn

================================================================================
来源：http://qfi.aibaodan.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://qpx.yfazqb.com

================================================================================
来源：http://hlq.chenlongwang.top

[Q01] 创建表
来源：http://kel.smart0.xyz

CREATE TABLE users (
来源：http://bfj.havefunace.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://aoe.zhijiandao.cn

name VARCHAR(50) NOT NULL,
来源：http://iak.zhiwuduotai.top

email VARCHAR(100) UNIQUE,
来源：http://dhd.52xcode.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://xcb.shanyushiyangkeji.top

);
来源：http://zcp.jinghuilouyu.cn

[Q02] 创建带外键的表
来源：http://vyw.ybcxt.top

CREATE TABLE orders (
来源：http://nwg.zhixingplan.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://rmk.aibaodan.cn

user_id INT NOT NULL,
来源：http://mkl.redwolf501.top

amount DECIMAL(10, 2),
来源：http://hvy.aizwys.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://quk.tanke756.top

);
来源：http://sne.haohaochexian.top

[Q03] 增加列
来源：http://yiu.fengsongda.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wrk.hfpthk.cn

[Q04] 修改列类型
来源：http://vjd.jinqigufen.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://jlv.havefunace.top

[Q05] 重命名列
来源：http://kcl.fengsongda.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hgs.zhixingplan.top

[Q06] 删除列
来源：http://yhd.cheryme.top

ALTER TABLE users DROP COLUMN age;
来源：http://ywg.tian-w.cn

[Q07] 删除表
来源：http://udg.fktsv.cn

DROP TABLE IF EXISTS orders;
来源：http://uju.ppjwa.cn

[Q08] 创建普通索引
来源：http://brp.xuetiantiany.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://hrm.yfazqb.com

[Q09] 创建唯一索引
来源：http://flw.ctjpmb.com

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://cjx.jinghuilouyu.cn

[Q10] 插入单行
来源：http://pnf.chenzaomai.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://qhd.meibo888.top

[Q11] 一次插入多行
来源：http://ifa.jlsjyb.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://cbf.tanke756.top

[Q12] 插入后取自增 ID
来源：http://kig.fktsv.cn

INSERT INTO users (name) VALUES ('C');
来源：http://cuk.wangdashe.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://qad.iojbl.cn

[Q13] 忽略重复插入
来源：http://fak.fktsv.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://xix.gaohongyu789.top

[Q14] 存在则更新（upsert）
来源：http://qds.zycfv.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://eoy.guowangkeji.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hlb.bbcook.cn

[Q15] 查询全部
来源：http://bru.ivvv.top

SELECT * FROM users;
来源：http://mbl.dianchejie.cn

[Q16] 查询指定列
来源：http://ipg.snrcjt.cn

SELECT id, name FROM users;
来源：http://xtx.haohaochexian.top

[Q17] 条件查询
来源：http://lhq.birdmap.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://gnf.0kj1m.cn

[Q18] 模糊匹配
来源：http://ckg.haohaochexian.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://dwd.pengpengdd.cyou

[Q19] 范围查询
来源：http://ubr.yongpay.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://chx.nwbrower.top

[Q20] IN 列表
来源：http://qpv.hongshengwenyu.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://vye.xinyue.icu

[Q21] 空值判断
来源：http://dfa.tarul.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://kdk.yanxiufei.cn

[Q22] 排序
来源：http://kfz.fengsongda.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://czz.hesvh.cn

[Q23] 分页
来源：http://hbe.cdnleiting.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://lur.yuanzhike.top

[Q24] 去重
来源：http://hdi.shzxlz.cn

SELECT DISTINCT city FROM users;
来源：http://xiy.aibaodan.cn

[Q25] 只取前 N 条
来源：http://gne.redwolf501.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://vni.jyoumei.cn

[Q26] 计数
来源：http://ayo.sweek.top

SELECT COUNT(*) FROM users;
来源：http://ray.yongpay.top

[Q27] 条件计数
来源：http://gqv.svipenyu.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://lhx.0kj1m.cn

[Q28] 求和与平均
来源：http://llb.jqgufenzy.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://otz.sufxvd.cn

[Q29] 最大最小值
来源：http://trj.gzhubu.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://vkr.feifeiyinyue.top

[Q30] 分组统计
来源：http://bsx.zhengqikj.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wsg.yongpay.top

[Q31] 分组后过滤
来源：http://fea.jqgfzy.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://yqs.tarul.cn

[Q32] 分组拼接字符串
来源：http://dwx.zhengqikj.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://vqa.cashguo.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://cci.hesvh.cn

[Q33] 多列分组
来源：http://tic.jianghu66.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://nyl.9152youxi.cn

[Q34] 每组取第一条
来源：http://lwg.hesvh.cn

SELECT * FROM (
来源：http://ufd.yueranfly.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://kvx.c1oappe.top

) t WHERE rn = 1;
来源：http://gqm.xingfuxueyuan.xyz

[Q35] 内连接
来源：http://zai.jlsjyb.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://lxk.vehdjk.com

[Q36] 左连接
来源：http://bof.gotoacloud.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://gbc.aibaodan.cn

[Q37] 右连接
来源：http://ann.fzhhl.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://aoq.ppjwa.cn

[Q38] 全外连接（PostgreSQL）
来源：http://wpe.0kj1m.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://qft.pycfn.com

[Q39] 自连接（查上下级）
来源：http://ihs.ctjpmb.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://vny.jqgfzy.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://aud.wangdashe.top

[Q40] 交叉连接（笛卡尔积）
来源：http://vpd.cdnleiting.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://jka.zhengqikj.top

[Q41] 多表连接
来源：http://gzf.smart0.xyz

SELECT o.id, u.name, p.title FROM orders o
来源：http://htx.havefunace.top

JOIN users u ON u.id = o.user_id
来源：http://ztl.fanxiaobao.xyz

JOIN products p ON p.id = o.product_id;
来源：http://hct.jianghu66.top

[Q42] 连接条件附加过滤
来源：http://exk.chenlongwang.top

SELECT u.name, o.amount FROM users u
来源：http://lyt.xuanzx.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://kov.hywenlv.cn

[Q43] 标量子查询
来源：http://ahz.dianchejie.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://onb.zhiwuduotai.top

[Q44] IN 子查询
来源：http://mqq.fanxiaobao.xyz

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ses.jqgfzy.top

[Q45] EXISTS 判断存在
来源：http://cia.jyoumei.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zma.yvedp.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ggw.bjfxy.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://iev.gotoacloud.top

[Q47] 与平均值比较
来源：http://pml.vehdjk.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://rjc.jqgufenzy.top

[Q48] CTE 公用表表达式
来源：http://fyv.yj202588.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://yws.haohaochexian.top

SELECT * FROM t WHERE c > 5;
来源：http://lkt.smart0.xyz

[Q49] 更新单行
来源：http://byt.dianchejie.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ydb.gaohongyu789.top

[Q50] 批量更新
来源：http://yei.dashuyun.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://pxk.svipenyu.cn

[Q51] 用子查询更新
来源：http://wbz.gaohongyu789.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://nah.yangfankeji.com

[Q52] 删除指定行
来源：http://muk.cucudq.cn

DELETE FROM users WHERE id = 10;
来源：http://iqq.tianlin.xyz

[Q53] 按条件删除
来源：http://hyh.yj202588.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://otw.jianghu66.top

[Q54] 清空表
来源：http://tgg.yangfankeji.com

TRUNCATE TABLE logs;
来源：http://gmp.ybcxt.top

[Q55] 排名（并列占位）
来源：http://qej.shangyingyoupin.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hry.daria6918.cn

[Q56] 密集排名（并列不占位）
来源：http://lhn.gotoacloud.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://nau.sxryk.cn

[Q57] 行号
来源：http://sdc.bjfxy.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://avb.mhx1999.top

[Q58] 累计求和
来源：http://cda.316326.xyz

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ppk.fehbvm.com

[Q59] 分组内累计
来源：http://odi.jlsjyb.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://abb.316326.xyz

[Q60] 取上一行 / 下一行
来源：http://eod.yj20258.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://zpx.guowangkeji.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://aix.redwolf501.top

[Q61] 移动平均
来源：http://mlr.yj20258.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://koq.pengpengdd.cyou

[Q62] 分组占比
来源：http://abs.snrcjt.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://cyt.jinqigufen.top

[Q63] 开启事务
来源：http://iai.yj202588.top

START TRANSACTION;                -- 或 BEGIN
来源：http://uaa.gaohongyu789.top

[Q64] 提交事务
来源：http://ayg.tarul.cn

COMMIT;
来源：http://gts.bbcook.cn

[Q65] 回滚事务
来源：http://pdi.hnxiangtu.top

ROLLBACK;
来源：http://iyg.0kj1m.cn

[Q66] 行锁查询
来源：http://bfe.sweek.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://txd.quarkkingdee.top

[Q67] 设置隔离级别
来源：http://bsa.chenzaomai.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ntn.wangshuangyany.cn

[Q68] 保存点
来源：http://yyu.shzxlz.cn

SAVEPOINT sp1;
来源：http://wwi.jinqigufen.top

ROLLBACK TO sp1;
来源：http://sdm.xylfe.cn

[Q69] 查看执行计划
来源：http://vnk.316326.xyz

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wmz.aibaodan.cn

[Q70] 更新统计信息
来源：http://gqa.hnqzz.top

ANALYZE TABLE users;
来源：http://oqn.nanxuanxn.top

[Q71] 查看建表语句
来源：http://sob.shzxlz.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://nud.guowangkeji.top

[Q72] 查看索引
来源：http://evj.cdnleiting.top

SHOW INDEX FROM users;
来源：http://zdr.redwolf501.top

[Q73] 查看表状态
来源：http://xmu.havefunace.top

SHOW TABLE STATUS LIKE 'users';
来源：http://jpx.havefunace.top

[Q74] 强制使用索引
来源：http://kyf.svipenyu.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://gnf.jianghu66.top

[Q75] 日期格式化
来源：http://yue.yangfankeji.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ovp.gotoacloud.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://dzt.chenjidiqi.icu

[Q76] 按天统计
来源：http://vew.zhaomingkeji.xyz

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://nty.gzhubu.top

[Q77] 时间加减
来源：http://qil.tianlin.xyz

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://cli.wangdashe.top

[Q78] 当前时间
来源：http://xem.ivvv.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mkt.jqgfzy.top

[Q79] 字符串拼接
来源：http://nov.ybcxt.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ckr.daxiang520.top

[Q80] 字符串截取
来源：http://yph.gaohongyu789.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://bng.hnqzz.top

[Q81] 字符串替换
来源：http://nwb.ydzc1.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://aqc.jqgfzy.top

[Q82] 字符长度与字节长度
来源：http://ods.haohaochexian.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ibb.redwolf501.top

[Q83] 大小写转换
来源：http://icv.ydjk.org.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ozq.shangyingyoupin.top

[Q84] 去除首尾空格
来源：http://vyf.jinqigufen.top

SELECT TRIM(name) FROM users;
来源：http://rtk.9152youxi.cn

[Q85] 数值取整
来源：http://yug.mhx1999.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://rqu.yueranfly.top

[Q86] 读取 JSON 字段
来源：http://ozh.ybcxt.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mvy.sjlbkw.cn

[Q87] JSON 字段做条件
来源：http://aex.gzhubu.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://cbq.shangyingyoupin.top

[Q88] 行转列（条件聚合）
来源：http://red.yueranfly.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ktq.svipenyu.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hdu.xingfuxueyuan.xyz

[Q89] 判断表是否存在
来源：http://zzw.ywan-chungtsiang.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ncu.xuanzx.com

[Q90] 生成序号列
来源：http://hiy.yj202588.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://yth.meibo888.top

================================================================================
来源：http://hog.cdnleiting.top

R. Bash 专题
来源：http://naz.hywenlv.cn

================================================================================
来源：http://fmb.xziqi.cn

[R01] shebang 与严格模式
来源：http://oms.jianghu66.top

#!/usr/bin/env bash
来源：http://euf.yfazqb.com

set -euo pipefail
来源：http://kmo.zhoulong.xyz

[R02] 变量赋值与使用
来源：http://hex.hywenlv.cn

name="Tom"; echo "$name"
来源：http://hqn.tanke756.top

[R03] 只读变量
来源：http://hfo.haohaochexian.top

readonly PI=3.14
来源：http://gkm.smart0.xyz

[R04] 位置参数
来源：http://idt.sweek.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://xcp.sxryk.cn

[R05] 参数默认值
来源：http://bxg.gotoacloud.top

name="${1:-default}"
来源：http://pub.hywenlv.cn

[R06] 判断命令是否存在
来源：http://tvm.52xcode.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wat.sjlbkw.cn

[R07] if 判断文件
来源：http://bkw.jinqigufen.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mau.wangshuangyany.cn

[R08] 数值比较
来源：http://ogi.sysykeji.top

if (( a > b )); then echo "a 更大"; fi
来源：http://vap.shanyushiyangkeji.top

[R09] 字符串比较
来源：http://aao.gaohongyu789.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://nvb.ydzc1.top

[R10] 正则匹配
来源：http://ost.zdqjudy.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://nlu.yvedp.cn

[R11] case 多分支
来源：http://nxz.tanke756.top

case "$1" in
来源：http://qko.xingfuxueyuan.xyz

start) echo "启动" ;;
来源：http://wnv.vehdjk.com

stop)  echo "停止" ;;
来源：http://jmq.bbcook.cn

*)     echo "未知命令" ;;
来源：http://zuu.yj20258888.top

esac
来源：http://vyc.hcnkem.com

[R12] for 遍历文件
来源：http://qpo.bjfxy.top

for f in *.txt; do echo "$f"; done
来源：http://fjw.chenjidiqi.icu

[R13] for 计数循环
来源：http://mid.uphjek.com

for i in {1..10}; do echo "$i"; done
来源：http://lkk.yj20258888.top

[R14] C 风格 for
来源：http://irx.ywan-chungtsiang.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://nra.shuidangran.top

[R15] while 逐行读文件
来源：http://fqn.ydzc1.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://gay.hnqzz.top

[R16] until 等待条件
来源：http://lwh.aibaodan.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://yxg.sysykeji.top

[R17] 数组定义与取值
来源：http://jnm.dianchejie.cn

arr=(a b c); echo "${arr[0]}"
来源：http://mmg.shzxlz.cn

[R18] 遍历数组
来源：http://qwd.hcnkem.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://quj.zhaomingkeji.xyz

[R19] 数组长度
来源：http://uxb.ppjwa.cn

echo "${#arr[@]}"
来源：http://qfm.ehwqpu.com

[R20] 关联数组（字典）
来源：http://fpm.jqgfzy.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://kjp.nanxinkj.top

[R21] 字符串长度
来源：http://tsq.yueranfly.top

echo "${#s}"
来源：http://lna.gogol.net.cn

[R22] 截取子串
来源：http://uey.fzhhl.top

echo "${s:0:5}"
来源：http://jhj.gogol.net.cn

[R23] 字符串替换
来源：http://fxx.fanxiaobao.xyz

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://gmy.chenjidiqi.icu

[R24] 大小写转换
来源：http://iwa.smart0.xyz

echo "${s^^}"; echo "${s,,}"
来源：http://jpm.chenlongwang.top

[R25] 去后缀 / 去前缀
来源：http://zvj.fktsv.cn


<!-- 参考信息 -->