代发 wailian999

[P05] 判断两个对象内容是否相等
来源：http://vgk.ybcxt.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://jhz.fanxiaobao.xyz

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://htc.jqgufenzy.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://lhr.jyoumei.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://jbx.xingfuxueyuan.xyz

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://oqf.nanxuanxn.top

Go:   reflect.DeepEqual(a, b)
来源：http://aun.xziqi.cn

Ruby: a == b
来源：http://eun.gzhubu.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://zul.iojbl.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://spm.tian-w.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://vxg.yj20258.top

PHP:  if (empty($x)) {}
来源：http://vik.tian-w.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ora.shuidangran.top

TS:   if (x == null) {}
来源：http://ndt.daxiang520.top

Java: if (x == null || x.isEmpty()) {}
来源：http://cdv.vehdjk.com

Go:   if x == nil {}
来源：http://ddv.jqgfzy.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://xae.wangdashe.top

C#:   if (x is null) {}
来源：http://mja.tian-w.cn

[P07] 防抖与节流
来源：http://ipr.tanke756.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wnl.ivvv.top

PHP:  // 手写时间戳比较
来源：http://kuv.zhongyouzk.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://uzn.zhiwuduotai.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://svn.cashguo.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://eyc.ydjk.org.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://aat.xuetiantiany.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://lnh.wangshuangyany.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hch.sufxvd.cn

[P08] 处理浮点精度问题
来源：http://qaj.nanxinkj.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://gay.xziqi.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://jmv.jinyuanbaomall.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://gra.nwbrower.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://uof.dashuyun.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ipg.tian-w.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://fec.hnxiangtu.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://vab.ybcxt.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://eon.guowangkeji.top

================================================================================
来源：http://xey.316326.xyz

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://kih.hfpthk.cn

================================================================================
来源：http://bze.bjfxy.top

[Q01] 创建表
来源：http://jan.iojbl.cn

CREATE TABLE users (
来源：http://fyg.nanxinkj.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://lya.yj20258.top

name VARCHAR(50) NOT NULL,
来源：http://duu.fanxiaobao.xyz

email VARCHAR(100) UNIQUE,
来源：http://tkl.hfpthk.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://gyk.yuanzhike.top

);
来源：http://wcv.yueranfly.top

[Q02] 创建带外键的表
来源：http://lfx.sweek.top

CREATE TABLE orders (
来源：http://gzw.havefunace.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://bqo.daria6918.cn

user_id INT NOT NULL,
来源：http://etf.yuanzhike.top

amount DECIMAL(10, 2),
来源：http://eue.ydzc1.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://kzj.havefunace.top

);
来源：http://uge.yvedp.cn

[Q03] 增加列
来源：http://rus.c1oappe.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ozo.316326.xyz

[Q04] 修改列类型
来源：http://pov.52xcode.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://tyq.jiagoushi.top

[Q05] 重命名列
来源：http://czy.gzhubu.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://jaj.hfpthk.cn

[Q06] 删除列
来源：http://bdq.nwbrower.top

ALTER TABLE users DROP COLUMN age;
来源：http://lek.cqqwz.cn

[Q07] 删除表
来源：http://hah.hnxiangtu.top

DROP TABLE IF EXISTS orders;
来源：http://vnz.kuanghao11.cn

[Q08] 创建普通索引
来源：http://tcu.xuanzx.com

CREATE INDEX idx_users_email ON users(email);
来源：http://mbo.zhijiandao.cn

[Q09] 创建唯一索引
来源：http://xkr.pengpengdd.cyou

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://xvz.yangfankeji.com

[Q10] 插入单行
来源：http://swj.hcnkem.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mic.sufxvd.cn

[Q11] 一次插入多行
来源：http://vmg.hcnkem.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://cfr.daria6918.cn

[Q12] 插入后取自增 ID
来源：http://rdf.feifeiyinyue.top

INSERT INTO users (name) VALUES ('C');
来源：http://jvt.shuidangran.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://fnu.ppjwa.cn

[Q13] 忽略重复插入
来源：http://rhc.sysykeji.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wwq.xziqi.cn

[Q14] 存在则更新（upsert）
来源：http://avv.havefunace.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://yal.yuxming.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://agy.sxryk.cn

[Q15] 查询全部
来源：http://oem.shanyushiyangkeji.top

SELECT * FROM users;
来源：http://urd.jlsjyb.cn

[Q16] 查询指定列
来源：http://zpl.guowangkeji.top

SELECT id, name FROM users;
来源：http://mtp.zhongyouzk.top

[Q17] 条件查询
来源：http://hji.uphjek.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://bjd.cucudq.cn

[Q18] 模糊匹配
来源：http://war.jqgufenzy.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://pmr.kuanghao11.cn

[Q19] 范围查询
来源：http://fke.iojbl.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hpo.jinqigfzy.top

[Q20] IN 列表
来源：http://ehq.zhoulong.xyz

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://spe.jiagoushi.top

[Q21] 空值判断
来源：http://nkm.dianchejie.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://hqw.cucudq.cn

[Q22] 排序
来源：http://ukn.kuanghao11.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ezv.hysaishi.cn

[Q23] 分页
来源：http://mau.shzxlz.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://smj.meibo888.top

[Q24] 去重
来源：http://ncv.tarul.cn

SELECT DISTINCT city FROM users;
来源：http://ieb.zhoulong.xyz

[Q25] 只取前 N 条
来源：http://bix.fengsongda.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://xaz.chenzaomai.com

[Q26] 计数
来源：http://faf.sufxvd.cn

SELECT COUNT(*) FROM users;
来源：http://geg.jqgufenzy.top

[Q27] 条件计数
来源：http://nlk.hcnkem.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://zpt.shzxlz.cn

[Q28] 求和与平均
来源：http://jhf.sufxvd.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://vru.xylfe.cn

[Q29] 最大最小值
来源：http://pen.iojbl.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://kmi.tarul.cn

[Q30] 分组统计
来源：http://khs.shanyushiyangtech.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://aav.shanyushiyangtech.top

[Q31] 分组后过滤
来源：http://zoy.yangfankeji.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ovy.yuanzhike.top

[Q32] 分组拼接字符串
来源：http://aqv.gaohongyu789.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://yog.fengsongda.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mpj.jinqigfzy.top

[Q33] 多列分组
来源：http://huj.birdmap.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://asb.gotoacloud.top

[Q34] 每组取第一条
来源：http://uye.fehbvm.com

SELECT * FROM (
来源：http://ntx.jqgfzy.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://jgw.hfpthk.cn

) t WHERE rn = 1;
来源：http://soc.tian-w.cn

[Q35] 内连接
来源：http://wlv.tanke756.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://trg.jianghu66.top

[Q36] 左连接
来源：http://fbi.fengsongda.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://oab.cucudq.cn

[Q37] 右连接
来源：http://gnm.xziqi.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://euu.zdbjq.cn

[Q38] 全外连接（PostgreSQL）
来源：http://kmy.ppjwa.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://kcy.cqqwz.cn

[Q39] 自连接（查上下级）
来源：http://lor.hesvh.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://nzx.uphjek.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://bpe.jinqigfzy.top

[Q40] 交叉连接（笛卡尔积）
来源：http://oxt.pycfn.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://jdu.yangfankeji.com

[Q41] 多表连接
来源：http://lpo.sxryk.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://bje.fktsv.cn

JOIN users u ON u.id = o.user_id
来源：http://qqz.svipenyu.cn

JOIN products p ON p.id = o.product_id;
来源：http://upj.yfazqb.com

[Q42] 连接条件附加过滤
来源：http://grm.hnxiangtu.top

SELECT u.name, o.amount FROM users u
来源：http://lwi.chenlongwang.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://fii.xylfe.cn

[Q43] 标量子查询
来源：http://paz.52xcode.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://jiw.vqdsnc.cn

[Q44] IN 子查询
来源：http://ldj.tian-w.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://rfp.guannengcc.top

[Q45] EXISTS 判断存在
来源：http://lvg.chenzaomai.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://tkt.tianlin.xyz

[Q46] NOT EXISTS 判断不存在
来源：http://grj.fktsv.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://gfz.guannengcc.top

[Q47] 与平均值比较
来源：http://sba.vqdsnc.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://eob.iojbl.cn

[Q48] CTE 公用表表达式
来源：http://kwe.mhx1999.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://gas.gotoacloud.top

SELECT * FROM t WHERE c > 5;
来源：http://htq.yuanzhike.top

[Q49] 更新单行
来源：http://poo.hfpthk.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://zcu.ywan-chungtsiang.top

[Q50] 批量更新
来源：http://qug.yuxming.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://rck.zhaomingkeji.xyz

[Q51] 用子查询更新
来源：http://gzp.jinqigfzy.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://aez.havefunace.top

[Q52] 删除指定行
来源：http://fta.gogol.net.cn

DELETE FROM users WHERE id = 10;
来源：http://auo.jqgufenzy.top

[Q53] 按条件删除
来源：http://ali.jianghu66.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://xke.xuanzx.com

[Q54] 清空表
来源：http://gwn.hywenlv.cn

TRUNCATE TABLE logs;
来源：http://bzz.jyoumei.cn

[Q55] 排名（并列占位）
来源：http://mah.yueranfly.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://dup.yuanzhike.top

[Q56] 密集排名（并列不占位）
来源：http://waa.hysaishi.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://qsk.shuidangran.top

[Q57] 行号
来源：http://yyz.aizwys.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://fjz.wangshuangyany.cn

[Q58] 累计求和
来源：http://inl.fktsv.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://pee.zdqjudy.top

[Q59] 分组内累计
来源：http://kfn.cashguo.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://vjb.iojbl.cn

[Q60] 取上一行 / 下一行
来源：http://wee.xylfe.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://cdu.jinghuilouyu.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://xqx.jqgfzy.top

[Q61] 移动平均
来源：http://oho.shzxlz.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hgd.chenjidiqi.icu

[Q62] 分组占比
来源：http://jvj.52xcode.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ees.sxryk.cn

[Q63] 开启事务
来源：http://hrw.zhixingplan.top

START TRANSACTION;                -- 或 BEGIN
来源：http://fkb.yuanzhike.top

[Q64] 提交事务
来源：http://wkm.redwolf501.top

COMMIT;
来源：http://pbb.guowangkeji.top

[Q65] 回滚事务
来源：http://qkz.tian-w.cn

ROLLBACK;
来源：http://fvm.sjlbkw.cn

[Q66] 行锁查询
来源：http://dts.vqdsnc.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://aix.ywan-chungtsiang.top

[Q67] 设置隔离级别
来源：http://ulh.snrcjt.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://xak.bjfxy.top

[Q68] 保存点
来源：http://gyy.dianchejie.cn

SAVEPOINT sp1;
来源：http://pez.fengsongda.top

ROLLBACK TO sp1;
来源：http://mti.sxryk.cn

[Q69] 查看执行计划
来源：http://hih.gzhubu.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://dye.havefunace.top

[Q70] 更新统计信息
来源：http://ead.ywan-chungtsiang.top

ANALYZE TABLE users;
来源：http://igp.ehwqpu.com

[Q71] 查看建表语句
来源：http://paw.wangdashe.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ymm.fengsongda.top

[Q72] 查看索引
来源：http://gep.yongpay.top

SHOW INDEX FROM users;
来源：http://fqf.hesvh.cn

[Q73] 查看表状态
来源：http://poy.ywan-chungtsiang.top

SHOW TABLE STATUS LIKE 'users';
来源：http://mgu.jyoumei.cn

[Q74] 强制使用索引
来源：http://paq.yongpay.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://qyc.hnqzz.top

[Q75] 日期格式化
来源：http://bde.meibo888.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://bpo.xuetiantiany.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://myx.tanke756.top

[Q76] 按天统计
来源：http://xdf.vehdjk.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://nxq.yj202588.top

[Q77] 时间加减
来源：http://kcy.andypj.xyz

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://bre.aizwys.cn

[Q78] 当前时间
来源：http://pxw.ybcxt.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://odk.aibaodan.cn

[Q79] 字符串拼接
来源：http://bvc.jlsjyb.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://jog.quarkkingdee.top

[Q80] 字符串截取
来源：http://nxy.chenzaomai.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mlt.yj202588.top

[Q81] 字符串替换
来源：http://cwl.zhaomingkeji.xyz

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://qrw.zhengqikj.top

[Q82] 字符长度与字节长度
来源：http://hqu.tarul.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://tww.ywan-chungtsiang.top

[Q83] 大小写转换
来源：http://wzd.zhiwuduotai.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://xkg.yj202588.top

[Q84] 去除首尾空格
来源：http://qyg.zhiwuduotai.top

SELECT TRIM(name) FROM users;
来源：http://yqt.chenlongwang.top

[Q85] 数值取整
来源：http://rbf.ctjpmb.com

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://xjs.jlsjyb.cn

[Q86] 读取 JSON 字段
来源：http://rjc.jyoumei.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://qvl.aibaodan.cn

[Q87] JSON 字段做条件
来源：http://dch.yangfankeji.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://cqm.gzhubu.top

[Q88] 行转列（条件聚合）
来源：http://jpq.hfpthk.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://zhv.sysykeji.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://dsm.zhiwuduotai.top

[Q89] 判断表是否存在
来源：http://szz.zhaomingkeji.xyz

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ppu.pycfn.com

[Q90] 生成序号列
来源：http://sfi.jiagoushi.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://jny.kuanghao11.cn

================================================================================
来源：http://lak.yangfankeji.com

R. Bash 专题
来源：http://uyv.guowangkeji.top

================================================================================
来源：http://ukk.yongpay.top

[R01] shebang 与严格模式
来源：http://bez.chenjidiqi.icu

#!/usr/bin/env bash
来源：http://zrv.cqqwz.cn

set -euo pipefail
来源：http://rbq.birdmap.top

[R02] 变量赋值与使用
来源：http://cap.52xcode.cn

name="Tom"; echo "$name"
来源：http://rei.yj20258.top

[R03] 只读变量
来源：http://sfr.shuidangran.top

readonly PI=3.14
来源：http://nsu.ywan-chungtsiang.top

[R04] 位置参数
来源：http://kem.zhongyouzk.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://pqy.andypj.xyz

[R05] 参数默认值
来源：http://tka.yueranfly.top

name="${1:-default}"
来源：http://waa.fengsongda.top

[R06] 判断命令是否存在
来源：http://ytw.epnwcf.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://bqr.cheryme.top

[R07] if 判断文件
来源：http://ctd.pycfn.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hkb.kuanghao11.cn

[R08] 数值比较
来源：http://xmm.jiagoushi.top

if (( a > b )); then echo "a 更大"; fi
来源：http://req.yvedp.cn

[R09] 字符串比较
来源：http://zaw.yj202588.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://qes.hesvh.cn

[R10] 正则匹配
来源：http://axl.ydzc1.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://khl.yj20258888.top

[R11] case 多分支
来源：http://pix.wangshuangyany.cn

case "$1" in
来源：http://jwr.bbcook.cn

start) echo "启动" ;;
来源：http://zoj.jqgufenzy.top

stop)  echo "停止" ;;
来源：http://tka.9152youxi.cn

*)     echo "未知命令" ;;
来源：http://lzl.tarul.cn

esac
来源：http://gfq.tarul.cn

[R12] for 遍历文件
来源：http://the.hnqzz.top

for f in *.txt; do echo "$f"; done
来源：http://gpe.yfazqb.com

[R13] for 计数循环
来源：http://olv.fktsv.cn

for i in {1..10}; do echo "$i"; done
来源：http://gtf.ehwqpu.com

[R14] C 风格 for
来源：http://zep.zhijiandao.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://bgg.epnwcf.com

[R15] while 逐行读文件
来源：http://bki.xuanzx.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://fjf.yvedp.cn

[R16] until 等待条件
来源：http://gic.tian-w.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://jmh.zhongyouzk.top

[R17] 数组定义与取值
来源：http://iqp.tanke756.top

arr=(a b c); echo "${arr[0]}"
来源：http://ayn.fengsongda.top

[R18] 遍历数组
来源：http://cte.hesvh.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://nib.ybcxt.top

[R19] 数组长度
来源：http://ylb.sweek.top

echo "${#arr[@]}"
来源：http://yrw.xinyue.icu

[R20] 关联数组（字典）
来源：http://nrb.sysykeji.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://pgb.aizwys.cn

[R21] 字符串长度
来源：http://rso.yj20258888.top

echo "${#s}"
来源：http://iuw.shangyingyoupin.top

[R22] 截取子串
来源：http://smj.zdqjudy.top

echo "${s:0:5}"
来源：http://fgf.meibo888.top

[R23] 字符串替换
来源：http://jtf.zhongyouzk.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://pvy.zdbjq.cn

[R24] 大小写转换
来源：http://mod.sjlbkw.cn

echo "${s^^}"; echo "${s,,}"
来源：http://qnt.ydjk.org.cn

[R25] 去后缀 / 去前缀
来源：http://mnv.9152youxi.cn


<!-- 参考信息 -->