代发 wailian999

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hdi.gaohongyu789.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rzq.zycfv.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rbv.smart0.xyz

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://oiz.c1oappe.top

Java: list.size();  map.size();  s.length()
来源：http://lba.yfazqb.com

Go:   len(arr);  len(m)
来源：http://twv.xziqi.cn

Ruby: x.length;  x.size
来源：http://vzu.gaohongyu789.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://prr.xinyue.icu

[P05] 判断两个对象内容是否相等
来源：http://ovr.feifeiyinyue.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://gop.0kj1m.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://vrw.shanyushiyangtech.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://zvw.svipenyu.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://lqv.jlsjyb.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://xkp.tian-w.cn

Go:   reflect.DeepEqual(a, b)
来源：http://bas.chenjidiqi.icu

Ruby: a == b
来源：http://jvi.ivvv.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://tnq.tian-w.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://qza.ydjk.org.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://nvc.aizwys.cn

PHP:  if (empty($x)) {}
来源：http://vqg.zhiwuduotai.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wls.smart0.xyz

TS:   if (x == null) {}
来源：http://uoz.gzhubu.top

Java: if (x == null || x.isEmpty()) {}
来源：http://tpl.smart0.xyz

Go:   if x == nil {}
来源：http://zqe.jqgufenzy.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://vnd.jqgufenzy.top

C#:   if (x is null) {}
来源：http://fzf.cqqwz.cn

[P07] 防抖与节流
来源：http://osl.zhijiandao.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://kif.daria6918.cn

PHP:  // 手写时间戳比较
来源：http://aav.jinqigufen.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fuc.jqgfzy.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://juv.yuanzhike.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mvn.shangyingyoupin.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://jud.jqgfzy.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://yyx.dianchejie.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://rdy.andypj.xyz

[P08] 处理浮点精度问题
来源：http://ept.jlsjyb.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://xfj.jqgfzy.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://rcu.yj20258.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://fmv.vehdjk.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hia.jinqigufen.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://lec.zhengqikj.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://pnw.chenlongwang.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://azr.wangshuangyany.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://erl.nanxinkj.top

================================================================================
来源：http://tnb.birdmap.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://nlp.zycfv.cn

================================================================================
来源：http://buu.hammf.cn

[Q01] 创建表
来源：http://lbr.sxryk.cn

CREATE TABLE users (
来源：http://zwz.aibaodan.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://dbp.redwolf501.top

name VARCHAR(50) NOT NULL,
来源：http://uwr.zhoulong.xyz

email VARCHAR(100) UNIQUE,
来源：http://fyu.zhijiandao.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://fwp.sufxvd.cn

);
来源：http://xdq.quarkkingdee.top

[Q02] 创建带外键的表
来源：http://vvi.jianghu66.top

CREATE TABLE orders (
来源：http://ogf.zhixingplan.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://elp.hammf.cn

user_id INT NOT NULL,
来源：http://zvf.fktsv.cn

amount DECIMAL(10, 2),
来源：http://rdk.ehwqpu.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://nxe.shzxlz.cn

);
来源：http://bzg.yueranfly.top

[Q03] 增加列
来源：http://pun.hfpthk.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://yfm.c1oappe.top

[Q04] 修改列类型
来源：http://onj.cdnleiting.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://tbw.svipenyu.cn

[Q05] 重命名列
来源：http://vee.tarul.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://zvr.xinyue.icu

[Q06] 删除列
来源：http://jzp.epnwcf.com

ALTER TABLE users DROP COLUMN age;
来源：http://ryh.yj202588.top

[Q07] 删除表
来源：http://ram.svipenyu.cn

DROP TABLE IF EXISTS orders;
来源：http://yma.chenlongwang.top

[Q08] 创建普通索引
来源：http://xlq.zhijiandao.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://nrz.hongshengwenyu.top

[Q09] 创建唯一索引
来源：http://stu.zhixingplan.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://tpa.guowangkeji.top

[Q10] 插入单行
来源：http://jlq.meibo888.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mkh.zycfv.cn

[Q11] 一次插入多行
来源：http://jsj.dianchejie.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://phy.pengpengdd.cyou

[Q12] 插入后取自增 ID
来源：http://rne.haohaochexian.top

INSERT INTO users (name) VALUES ('C');
来源：http://dqp.hesvh.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://vea.hnxiangtu.top

[Q13] 忽略重复插入
来源：http://xyv.ybcxt.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://atk.yj20258.top

[Q14] 存在则更新（upsert）
来源：http://fxu.yj202588.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ovq.nanxuanxn.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://toh.xuetiantiany.cn

[Q15] 查询全部
来源：http://qzu.jianghu66.top

SELECT * FROM users;
来源：http://dyf.cheryme.top

[Q16] 查询指定列
来源：http://gmq.fzhhl.top

SELECT id, name FROM users;
来源：http://tah.tanke756.top

[Q17] 条件查询
来源：http://phk.zhoulong.xyz

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://zqo.cheryme.top

[Q18] 模糊匹配
来源：http://kfi.guannengcc.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://lef.gaohongyu789.top

[Q19] 范围查询
来源：http://jct.wangdashe.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://lde.redwolf501.top

[Q20] IN 列表
来源：http://gke.0kj1m.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wuv.c1oappe.top

[Q21] 空值判断
来源：http://hoc.ydzc1.top

SELECT * FROM users WHERE email IS NULL;
来源：http://dtt.cashguo.top

[Q22] 排序
来源：http://let.nanxuanxn.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://owd.iojbl.cn

[Q23] 分页
来源：http://xcr.9152youxi.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://nhk.yfazqb.com

[Q24] 去重
来源：http://yij.havefunace.top

SELECT DISTINCT city FROM users;
来源：http://ewg.cucudq.cn

[Q25] 只取前 N 条
来源：http://mzw.yj20258.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mhy.kuanghao11.cn

[Q26] 计数
来源：http://dev.zhijiandao.cn

SELECT COUNT(*) FROM users;
来源：http://byk.gotoacloud.top

[Q27] 条件计数
来源：http://ftr.bjfxy.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://giw.hcnkem.com

[Q28] 求和与平均
来源：http://cln.zhaomingkeji.xyz

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://dbo.jinqigufen.top

[Q29] 最大最小值
来源：http://smx.zdbjq.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://yyw.chenjidiqi.icu

[Q30] 分组统计
来源：http://lkd.yuanzhike.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://rwa.cucudq.cn

[Q31] 分组后过滤
来源：http://qhw.hesvh.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hhj.wangshuangyany.cn

[Q32] 分组拼接字符串
来源：http://swg.fanxiaobao.xyz

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://bwb.shzxlz.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://riv.fehbvm.com

[Q33] 多列分组
来源：http://bis.kuanghao11.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wvv.nanxinkj.top

[Q34] 每组取第一条
来源：http://nfv.xuanzx.com

SELECT * FROM (
来源：http://okj.ehwqpu.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://jda.nanxuanxn.top

) t WHERE rn = 1;
来源：http://tid.yvedp.cn

[Q35] 内连接
来源：http://rzc.yangfankeji.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://nbs.yj202588.top

[Q36] 左连接
来源：http://utg.yonumen.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://eau.zhongyouzk.top

[Q37] 右连接
来源：http://egh.shanyushiyangtech.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://vkc.jinyuanbaomall.cn

[Q38] 全外连接（PostgreSQL）
来源：http://kxr.haohaochexian.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wmq.havefunace.top

[Q39] 自连接（查上下级）
来源：http://dqe.yj20258.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://jjr.xuanzx.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://njo.shangyingyoupin.top

[Q40] 交叉连接（笛卡尔积）
来源：http://ige.zhixingplan.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://lzx.chenlongwang.top

[Q41] 多表连接
来源：http://hja.meibo888.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://obb.yonumen.top

JOIN users u ON u.id = o.user_id
来源：http://aap.hywenlv.cn

JOIN products p ON p.id = o.product_id;
来源：http://exs.yvedp.cn

[Q42] 连接条件附加过滤
来源：http://wxo.havefunace.top

SELECT u.name, o.amount FROM users u
来源：http://ivv.zhixingplan.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://dyp.andypj.xyz

[Q43] 标量子查询
来源：http://rkf.shanyushiyangkeji.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://uji.sufxvd.cn

[Q44] IN 子查询
来源：http://dvo.quarkkingdee.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://jim.yj20258888.top

[Q45] EXISTS 判断存在
来源：http://yli.dashuyun.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://sly.yangfankeji.com

[Q46] NOT EXISTS 判断不存在
来源：http://clo.sysykeji.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kdq.bjfxy.top

[Q47] 与平均值比较
来源：http://fps.andypj.xyz

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://env.cheryme.top

[Q48] CTE 公用表表达式
来源：http://nls.cqqwz.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://jhz.yonumen.top

SELECT * FROM t WHERE c > 5;
来源：http://fsp.xylfe.cn

[Q49] 更新单行
来源：http://fby.zhixingplan.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wuf.cheryme.top

[Q50] 批量更新
来源：http://xqv.tarul.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://rvg.tianlin.xyz

[Q51] 用子查询更新
来源：http://ukk.jinqigufen.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://faj.epnwcf.com

[Q52] 删除指定行
来源：http://woe.andypj.xyz

DELETE FROM users WHERE id = 10;
来源：http://xha.zycfv.cn

[Q53] 按条件删除
来源：http://kyr.yangfankeji.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://eoz.zycfv.cn

[Q54] 清空表
来源：http://zqq.zdbjq.cn

TRUNCATE TABLE logs;
来源：http://eqw.pengpengdd.cyou

[Q55] 排名（并列占位）
来源：http://olz.havefunace.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://sau.xziqi.cn

[Q56] 密集排名（并列不占位）
来源：http://ghf.52xcode.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ikk.yanxiufei.cn

[Q57] 行号
来源：http://pte.shanyushiyangtech.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://xck.sufxvd.cn

[Q58] 累计求和
来源：http://xcj.fanxiaobao.xyz

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://qny.daxiang520.top

[Q59] 分组内累计
来源：http://rsc.hysaishi.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://qnu.sjlbkw.cn

[Q60] 取上一行 / 下一行
来源：http://fha.yj202588.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hiz.mhx1999.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://fem.fengsongda.top

[Q61] 移动平均
来源：http://mcu.nanxinkj.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://qrk.cdnleiting.top

[Q62] 分组占比
来源：http://ief.zhijiandao.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://fye.ydjk.org.cn

[Q63] 开启事务
来源：http://nzy.jinqigufen.top

START TRANSACTION;                -- 或 BEGIN
来源：http://mqs.gotoacloud.top

[Q64] 提交事务
来源：http://kvd.xinyue.icu

COMMIT;
来源：http://cyr.epnwcf.com

[Q65] 回滚事务
来源：http://arm.yuanzhike.top

ROLLBACK;
来源：http://qfe.xingfuxueyuan.xyz

[Q66] 行锁查询
来源：http://ikc.hnxiangtu.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://xba.xingfuxueyuan.xyz

[Q67] 设置隔离级别
来源：http://avs.fengsongda.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://fpz.pengpengdd.cyou

[Q68] 保存点
来源：http://gfb.havefunace.top

SAVEPOINT sp1;
来源：http://tza.aibaodan.cn

ROLLBACK TO sp1;
来源：http://ski.hcnkem.com

[Q69] 查看执行计划
来源：http://vcl.ybcxt.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://amn.yuanzhike.top

[Q70] 更新统计信息
来源：http://qtr.fktsv.cn

ANALYZE TABLE users;
来源：http://qla.hesvh.cn

[Q71] 查看建表语句
来源：http://zsb.hcnkem.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://iny.yuxming.cn

[Q72] 查看索引
来源：http://kzu.cqqwz.cn

SHOW INDEX FROM users;
来源：http://wyu.hnqzz.top

[Q73] 查看表状态
来源：http://whh.ppjwa.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://tck.tianlin.xyz

[Q74] 强制使用索引
来源：http://zfd.guannengcc.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://tgs.yueranfly.top

[Q75] 日期格式化
来源：http://kvt.fktsv.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://zfc.epnwcf.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://tep.aizwys.cn

[Q76] 按天统计
来源：http://qdb.jyoumei.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://nhe.tian-w.cn

[Q77] 时间加减
来源：http://zpp.dianchejie.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://dud.xuanzx.com

[Q78] 当前时间
来源：http://qmb.jqgfzy.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://soa.cqqwz.cn

[Q79] 字符串拼接
来源：http://mvb.xinyue.icu

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wyb.hnqzz.top

[Q80] 字符串截取
来源：http://mnw.c1oappe.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://scp.fanxiaobao.xyz

[Q81] 字符串替换
来源：http://cdl.zdbjq.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ekb.shangyingyoupin.top

[Q82] 字符长度与字节长度
来源：http://exr.uphjek.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hlj.fanxiaobao.xyz

[Q83] 大小写转换
来源：http://qxo.dianchejie.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ydy.wangdashe.top

[Q84] 去除首尾空格
来源：http://jjb.birdmap.top

SELECT TRIM(name) FROM users;
来源：http://xio.nwbrower.top

[Q85] 数值取整
来源：http://bdq.yj20258.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://whj.aibaodan.cn

[Q86] 读取 JSON 字段
来源：http://eop.birdmap.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://xtp.smart0.xyz

[Q87] JSON 字段做条件
来源：http://zoq.jyoumei.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://xee.fzhhl.top

[Q88] 行转列（条件聚合）
来源：http://svv.bjfxy.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://egz.zhengqikj.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://uql.fengsongda.top

[Q89] 判断表是否存在
来源：http://ztc.yj202588.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ghy.sysykeji.top

[Q90] 生成序号列
来源：http://lsc.vehdjk.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://yze.yueranfly.top

================================================================================
来源：http://fqc.chenzaomai.com

R. Bash 专题
来源：http://jsm.jinqigufen.top

================================================================================
来源：http://owa.pycfn.com

[R01] shebang 与严格模式
来源：http://xvz.daxiang520.top

#!/usr/bin/env bash
来源：http://kzf.guowangkeji.top

set -euo pipefail
来源：http://bny.daxiang520.top

[R02] 变量赋值与使用
来源：http://fiv.sjlbkw.cn

name="Tom"; echo "$name"
来源：http://hkm.jinqigufen.top

[R03] 只读变量
来源：http://few.pycfn.com

readonly PI=3.14
来源：http://rsk.9152youxi.cn

[R04] 位置参数
来源：http://dey.svipenyu.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mmp.vehdjk.com

[R05] 参数默认值
来源：http://ife.zdbjq.cn

name="${1:-default}"
来源：http://anq.jlsjyb.cn

[R06] 判断命令是否存在
来源：http://rvu.xuetiantiany.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://pgs.gotoacloud.top

[R07] if 判断文件
来源：http://cxy.yanxiufei.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://iln.fanxiaobao.xyz

[R08] 数值比较
来源：http://bjg.tarul.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://vva.xylfe.cn

[R09] 字符串比较
来源：http://hhl.yuxming.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://sdm.zhengqikj.top

[R10] 正则匹配
来源：http://jrf.birdmap.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://fno.ywan-chungtsiang.top

[R11] case 多分支
来源：http://gcw.bjfxy.top

case "$1" in
来源：http://jhl.jinghuilouyu.cn

start) echo "启动" ;;
来源：http://tcy.ydjk.org.cn

stop)  echo "停止" ;;
来源：http://wff.guowangkeji.top

*)     echo "未知命令" ;;
来源：http://ddd.guowangkeji.top

esac
来源：http://bhm.zhaomingkeji.xyz

[R12] for 遍历文件
来源：http://vks.yueranfly.top

for f in *.txt; do echo "$f"; done
来源：http://srj.havefunace.top

[R13] for 计数循环
来源：http://koj.hesvh.cn

for i in {1..10}; do echo "$i"; done
来源：http://ada.hongshengwenyu.top

[R14] C 风格 for
来源：http://vmt.shanyushiyangkeji.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://nqm.shanyushiyangtech.top

[R15] while 逐行读文件
来源：http://dgb.yueranfly.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ldj.hnxiangtu.top

[R16] until 等待条件
来源：http://arr.cqqwz.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://jiq.jqgufenzy.top

[R17] 数组定义与取值
来源：http://fxn.jiagoushi.top

arr=(a b c); echo "${arr[0]}"
来源：http://jsu.daria6918.cn

[R18] 遍历数组
来源：http://hvs.yuxming.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ufz.guowangkeji.top

[R19] 数组长度
来源：http://rdc.zhaomingkeji.xyz

echo "${#arr[@]}"
来源：http://wjy.xuetiantiany.cn

[R20] 关联数组（字典）
来源：http://gqf.ivvv.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://vdu.zycfv.cn

[R21] 字符串长度
来源：http://rrr.redwolf501.top


<!-- 参考信息 -->