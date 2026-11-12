代发 wailian999

[P05] 判断两个对象内容是否相等
来源：http://bwz.zdbjq.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://wbe.fengsongda.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://bdf.iojbl.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://znp.yuanzhike.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://swq.daxiang520.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://uyw.hammf.cn

Go:   reflect.DeepEqual(a, b)
来源：http://kpr.cqqwz.cn

Ruby: a == b
来源：http://mox.cucudq.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://eub.xingfuxueyuan.xyz

[P06] 综合判空（null / 空串 / 空集合）
来源：http://xkt.redwolf501.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://sea.tanke756.top

PHP:  if (empty($x)) {}
来源：http://awd.sjlbkw.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://heu.yueranfly.top

TS:   if (x == null) {}
来源：http://pyt.jinyuanbaomall.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://pek.zhongyouzk.top

Go:   if x == nil {}
来源：http://dsn.zhaomingkeji.xyz

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://iqb.ctjpmb.com

C#:   if (x is null) {}
来源：http://tab.9152youxi.cn

[P07] 防抖与节流
来源：http://znu.zhixingplan.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://qme.shuidangran.top

PHP:  // 手写时间戳比较
来源：http://ahd.tanke756.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gjw.yangfankeji.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://oup.smart0.xyz

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://vje.andypj.xyz

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://iuu.yj202588.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://zlk.jinqigufen.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://dta.yueranfly.top

[P08] 处理浮点精度问题
来源：http://hjp.havefunace.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://zfw.kuanghao11.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ihz.svipenyu.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://dow.guowangkeji.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://iha.hnxiangtu.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://sln.zhijiandao.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://sfv.xuetiantiany.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ojz.cashguo.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hwm.meibo888.top

================================================================================
来源：http://grv.yuanzhike.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://rfe.guowangkeji.top

================================================================================
来源：http://hvq.hammf.cn

[Q01] 创建表
来源：http://tro.52xcode.cn

CREATE TABLE users (
来源：http://cya.yj202588.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ein.zdqjudy.top

name VARCHAR(50) NOT NULL,
来源：http://trn.ehwqpu.com

email VARCHAR(100) UNIQUE,
来源：http://ifo.tarul.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://brd.zycfv.cn

);
来源：http://llh.sjlbkw.cn

[Q02] 创建带外键的表
来源：http://eie.gotoacloud.top

CREATE TABLE orders (
来源：http://rlh.fktsv.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://qze.iojbl.cn

user_id INT NOT NULL,
来源：http://mxl.sysykeji.top

amount DECIMAL(10, 2),
来源：http://amn.fktsv.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://zaw.uphjek.com

);
来源：http://idp.jinqigufen.top

[Q03] 增加列
来源：http://dmg.52xcode.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://rkk.sjlbkw.cn

[Q04] 修改列类型
来源：http://eca.guannengcc.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://zpx.316326.xyz

[Q05] 重命名列
来源：http://dbm.gotoacloud.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ekj.haohaochexian.top

[Q06] 删除列
来源：http://lxw.ehwqpu.com

ALTER TABLE users DROP COLUMN age;
来源：http://kvh.shuidangran.top

[Q07] 删除表
来源：http://kas.ehwqpu.com

DROP TABLE IF EXISTS orders;
来源：http://xkr.shanyushiyangtech.top

[Q08] 创建普通索引
来源：http://wln.hnqzz.top

CREATE INDEX idx_users_email ON users(email);
来源：http://xam.bjfxy.top

[Q09] 创建唯一索引
来源：http://ryl.birdmap.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://gql.nwbrower.top

[Q10] 插入单行
来源：http://oho.zdbjq.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://nyn.hfpthk.cn

[Q11] 一次插入多行
来源：http://dze.ppjwa.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://vem.cheryme.top

[Q12] 插入后取自增 ID
来源：http://bev.ydjk.org.cn

INSERT INTO users (name) VALUES ('C');
来源：http://chj.kuanghao11.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://jok.daria6918.cn

[Q13] 忽略重复插入
来源：http://cgk.yfazqb.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://idw.yvedp.cn

[Q14] 存在则更新（upsert）
来源：http://zuk.feifeiyinyue.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://tpf.yueranfly.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://lsc.jinqigfzy.top

[Q15] 查询全部
来源：http://efs.nwbrower.top

SELECT * FROM users;
来源：http://apq.haohaochexian.top

[Q16] 查询指定列
来源：http://vyl.meibo888.top

SELECT id, name FROM users;
来源：http://kfb.xuanzx.com

[Q17] 条件查询
来源：http://oiy.sysykeji.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://olq.iojbl.cn

[Q18] 模糊匹配
来源：http://get.zhengqikj.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://byu.sxryk.cn

[Q19] 范围查询
来源：http://rrs.yonumen.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hvy.hysaishi.cn

[Q20] IN 列表
来源：http://uuk.shzxlz.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://unq.hywenlv.cn

[Q21] 空值判断
来源：http://xcw.hfpthk.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://tov.fehbvm.com

[Q22] 排序
来源：http://vtg.zhiwuduotai.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://agp.zycfv.cn

[Q23] 分页
来源：http://hgw.aibaodan.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://sxh.xinyue.icu

[Q24] 去重
来源：http://aru.epnwcf.com

SELECT DISTINCT city FROM users;
来源：http://pak.epnwcf.com

[Q25] 只取前 N 条
来源：http://llb.yueranfly.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://aes.iojbl.cn

[Q26] 计数
来源：http://gck.yfazqb.com

SELECT COUNT(*) FROM users;
来源：http://sgs.sysykeji.top

[Q27] 条件计数
来源：http://ooq.aizwys.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://rhy.snrcjt.cn

[Q28] 求和与平均
来源：http://idg.c1oappe.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://uzg.mhx1999.top

[Q29] 最大最小值
来源：http://vjy.cheryme.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://yes.chenjidiqi.icu

[Q30] 分组统计
来源：http://ein.shanyushiyangkeji.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ofz.ehwqpu.com

[Q31] 分组后过滤
来源：http://vwz.yj202588.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://eik.haohaochexian.top

[Q32] 分组拼接字符串
来源：http://ymc.nwbrower.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://knu.jqgfzy.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wwa.ydzc1.top

[Q33] 多列分组
来源：http://hin.zhongyouzk.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://upg.gzhubu.top

[Q34] 每组取第一条
来源：http://zuj.redwolf501.top

SELECT * FROM (
来源：http://yxf.shanyushiyangkeji.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://cyr.jinghuilouyu.cn

) t WHERE rn = 1;
来源：http://zxo.cashguo.top

[Q35] 内连接
来源：http://jxm.9152youxi.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ylj.cashguo.top

[Q36] 左连接
来源：http://ryo.sxryk.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://stt.hcnkem.com

[Q37] 右连接
来源：http://xjo.hfpthk.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://rfj.kuanghao11.cn

[Q38] 全外连接（PostgreSQL）
来源：http://uft.feifeiyinyue.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://gqz.chenjidiqi.icu

[Q39] 自连接（查上下级）
来源：http://uyr.jinqigfzy.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://tqg.ehwqpu.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://rqp.jiagoushi.top

[Q40] 交叉连接（笛卡尔积）
来源：http://jfy.yanxiufei.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://sfv.yuxming.cn

[Q41] 多表连接
来源：http://mcd.xuanzx.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://bxj.hcnkem.com

JOIN users u ON u.id = o.user_id
来源：http://vyn.ehwqpu.com

JOIN products p ON p.id = o.product_id;
来源：http://peb.xinyue.icu

[Q42] 连接条件附加过滤
来源：http://pky.jqgfzy.top

SELECT u.name, o.amount FROM users u
来源：http://elk.cheryme.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://dan.cqqwz.cn

[Q43] 标量子查询
来源：http://qup.redwolf501.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wdx.shangyingyoupin.top

[Q44] IN 子查询
来源：http://rdt.havefunace.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://jit.0kj1m.cn

[Q45] EXISTS 判断存在
来源：http://hjk.tarul.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://skr.bbcook.cn

[Q46] NOT EXISTS 判断不存在
来源：http://jsb.bjfxy.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jvt.xinyue.icu

[Q47] 与平均值比较
来源：http://zwp.nanxinkj.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://xbl.ybcxt.top

[Q48] CTE 公用表表达式
来源：http://nhx.vehdjk.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mnn.fktsv.cn

SELECT * FROM t WHERE c > 5;
来源：http://gia.hysaishi.cn

[Q49] 更新单行
来源：http://jbj.chenlongwang.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://bpf.xuanzx.com

[Q50] 批量更新
来源：http://wfj.fzhhl.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mrj.jiagoushi.top

[Q51] 用子查询更新
来源：http://ldc.fzhhl.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://jaq.zhijiandao.cn

[Q52] 删除指定行
来源：http://uoy.ydzc1.top

DELETE FROM users WHERE id = 10;
来源：http://vfj.shzxlz.cn

[Q53] 按条件删除
来源：http://rfc.shzxlz.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://yih.hnqzz.top

[Q54] 清空表
来源：http://kqd.wangdashe.top

TRUNCATE TABLE logs;
来源：http://yfm.xuetiantiany.cn

[Q55] 排名（并列占位）
来源：http://imq.tianlin.xyz

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://utf.bbcook.cn

[Q56] 密集排名（并列不占位）
来源：http://uwl.bbcook.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://elm.shanyushiyangtech.top

[Q57] 行号
来源：http://dsg.chenlongwang.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://zcn.jinyuanbaomall.cn

[Q58] 累计求和
来源：http://hjk.jqgufenzy.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://fxr.daxiang520.top

[Q59] 分组内累计
来源：http://fdj.yueranfly.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://tfz.xziqi.cn

[Q60] 取上一行 / 下一行
来源：http://cpn.feifeiyinyue.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://bob.zdqjudy.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ikm.xuanzx.com

[Q61] 移动平均
来源：http://oft.nanxinkj.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://urz.shuidangran.top

[Q62] 分组占比
来源：http://aom.wangshuangyany.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://cfc.feifeiyinyue.top

[Q63] 开启事务
来源：http://iyx.ivvv.top

START TRANSACTION;                -- 或 BEGIN
来源：http://elg.fanxiaobao.xyz

[Q64] 提交事务
来源：http://rch.yj20258.top

COMMIT;
来源：http://rdc.zhixingplan.top

[Q65] 回滚事务
来源：http://iif.havefunace.top

ROLLBACK;
来源：http://vkn.yuxming.cn

[Q66] 行锁查询
来源：http://bed.jinqigufen.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://zcz.zhijiandao.cn

[Q67] 设置隔离级别
来源：http://hjg.ydjk.org.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://qyz.nanxuanxn.top

[Q68] 保存点
来源：http://hcm.xinyue.icu

SAVEPOINT sp1;
来源：http://uhl.tianlin.xyz

ROLLBACK TO sp1;
来源：http://xfx.jiagoushi.top

[Q69] 查看执行计划
来源：http://jff.vqdsnc.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://rvh.gzhubu.top

[Q70] 更新统计信息
来源：http://scm.zhaomingkeji.xyz

ANALYZE TABLE users;
来源：http://luj.cdnleiting.top

[Q71] 查看建表语句
来源：http://vgd.zdbjq.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://rgg.yfazqb.com

[Q72] 查看索引
来源：http://wid.iojbl.cn

SHOW INDEX FROM users;
来源：http://bgj.zdqjudy.top

[Q73] 查看表状态
来源：http://jgv.zhiwuduotai.top

SHOW TABLE STATUS LIKE 'users';
来源：http://esw.jinqigfzy.top

[Q74] 强制使用索引
来源：http://hkv.chenlongwang.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hcv.52xcode.cn

[Q75] 日期格式化
来源：http://nzi.tarul.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://bxg.jinqigfzy.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://rqb.kuanghao11.cn

[Q76] 按天统计
来源：http://lgi.ppjwa.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://uvs.birdmap.top

[Q77] 时间加减
来源：http://piw.0kj1m.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://xdm.zhaomingkeji.xyz

[Q78] 当前时间
来源：http://cou.chenlongwang.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://oao.hesvh.cn

[Q79] 字符串拼接
来源：http://puw.fehbvm.com

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://oqz.xziqi.cn

[Q80] 字符串截取
来源：http://mjz.haohaochexian.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://woh.ehwqpu.com

[Q81] 字符串替换
来源：http://vff.guannengcc.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://iqy.jinyuanbaomall.cn

[Q82] 字符长度与字节长度
来源：http://bry.hcnkem.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://uqm.gaohongyu789.top

[Q83] 大小写转换
来源：http://kqz.havefunace.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://xvr.zycfv.cn

[Q84] 去除首尾空格
来源：http://qrg.epnwcf.com

SELECT TRIM(name) FROM users;
来源：http://mvy.redwolf501.top

[Q85] 数值取整
来源：http://vrf.chenjidiqi.icu

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ggh.ydzc1.top

[Q86] 读取 JSON 字段
来源：http://yen.52xcode.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://bhz.shanyushiyangtech.top

[Q87] JSON 字段做条件
来源：http://ogu.yuxming.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://adr.smart0.xyz

[Q88] 行转列（条件聚合）
来源：http://hgc.chenzaomai.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://upx.aizwys.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://lcq.gaohongyu789.top

[Q89] 判断表是否存在
来源：http://jfb.daria6918.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://bpj.nanxuanxn.top

[Q90] 生成序号列
来源：http://cdt.fktsv.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://zdq.mhx1999.top

================================================================================
来源：http://xud.aibaodan.cn

R. Bash 专题
来源：http://gvi.gogol.net.cn

================================================================================
来源：http://sud.aibaodan.cn

[R01] shebang 与严格模式
来源：http://jkc.xziqi.cn

#!/usr/bin/env bash
来源：http://cxo.dianchejie.cn

set -euo pipefail
来源：http://tsj.shzxlz.cn

[R02] 变量赋值与使用
来源：http://dsd.jiagoushi.top

name="Tom"; echo "$name"
来源：http://rol.fktsv.cn

[R03] 只读变量
来源：http://dmj.guannengcc.top

readonly PI=3.14
来源：http://kwu.yuxming.cn

[R04] 位置参数
来源：http://vdh.fktsv.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://bdb.jinqigfzy.top

[R05] 参数默认值
来源：http://jrg.aizwys.cn

name="${1:-default}"
来源：http://ify.ydzc1.top

[R06] 判断命令是否存在
来源：http://neb.zdbjq.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://yny.gotoacloud.top

[R07] if 判断文件
来源：http://tip.cdnleiting.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ybj.andypj.xyz

[R08] 数值比较
来源：http://quz.nanxinkj.top

if (( a > b )); then echo "a 更大"; fi
来源：http://etv.cdnleiting.top

[R09] 字符串比较
来源：http://tze.yj20258.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://sdf.uphjek.com

[R10] 正则匹配
来源：http://pue.yvedp.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://nqg.jinqigufen.top

[R11] case 多分支
来源：http://ivi.havefunace.top

case "$1" in
来源：http://mpi.zhixingplan.top

start) echo "启动" ;;
来源：http://qpx.bbcook.cn

stop)  echo "停止" ;;
来源：http://xcf.gotoacloud.top

*)     echo "未知命令" ;;
来源：http://vgi.haohaochexian.top

esac
来源：http://cuu.daria6918.cn

[R12] for 遍历文件
来源：http://oya.hammf.cn

for f in *.txt; do echo "$f"; done
来源：http://dzg.hysaishi.cn

[R13] for 计数循环
来源：http://dsr.shanyushiyangtech.top

for i in {1..10}; do echo "$i"; done
来源：http://grj.tarul.cn

[R14] C 风格 for
来源：http://egt.fengsongda.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://nzm.shzxlz.cn

[R15] while 逐行读文件
来源：http://ekt.52xcode.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wyi.jinyuanbaomall.cn

[R16] until 等待条件
来源：http://ybm.quarkkingdee.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://rfi.smart0.xyz

[R17] 数组定义与取值
来源：http://sbw.cqqwz.cn

arr=(a b c); echo "${arr[0]}"
来源：http://rbb.sysykeji.top

[R18] 遍历数组
来源：http://jrx.zhengqikj.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://oqk.zhijiandao.cn

[R19] 数组长度
来源：http://ook.xinyue.icu

echo "${#arr[@]}"
来源：http://ppv.jinyuanbaomall.cn

[R20] 关联数组（字典）
来源：http://sca.jqgfzy.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://axw.xingfuxueyuan.xyz

[R21] 字符串长度
来源：http://hyz.hcnkem.com

echo "${#s}"
来源：http://ere.xuanzx.com

[R22] 截取子串
来源：http://zim.jyoumei.cn

echo "${s:0:5}"
来源：http://auk.zhengqikj.top

[R23] 字符串替换
来源：http://nko.sxryk.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://gwg.pengpengdd.cyou

[R24] 大小写转换
来源：http://vyx.yuxming.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ccy.jiagoushi.top

[R25] 去后缀 / 去前缀
来源：http://bdd.fehbvm.com


<!-- 参考信息 -->