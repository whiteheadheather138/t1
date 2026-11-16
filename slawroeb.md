代发 wailian999

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ysp.fzhhl.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hhe.yj20258.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wgp.yanxiufei.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zdt.vehdjk.com

Java: list.size();  map.size();  s.length()
来源：http://faj.xuetiantiany.cn

Go:   len(arr);  len(m)
来源：http://hzz.hnqzz.top

Ruby: x.length;  x.size
来源：http://nib.hfpthk.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://igs.fengsongda.top

[P05] 判断两个对象内容是否相等
来源：http://xaz.jiagoushi.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://lkf.zhiwuduotai.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://pzh.tanke756.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://fgs.nanxinkj.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://uoe.smart0.xyz

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ngl.xingfuxueyuan.xyz

Go:   reflect.DeepEqual(a, b)
来源：http://wdm.yuxming.cn

Ruby: a == b
来源：http://aep.nanxinkj.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://tfa.gaohongyu789.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://aeg.jianghu66.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ixi.bjfxy.top

PHP:  if (empty($x)) {}
来源：http://sgd.zdbjq.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://scj.ctjpmb.com

TS:   if (x == null) {}
来源：http://mwx.vqdsnc.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://wmi.redwolf501.top

Go:   if x == nil {}
来源：http://ebj.nanxinkj.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://zgr.havefunace.top

C#:   if (x is null) {}
来源：http://xda.jqgufenzy.top

[P07] 防抖与节流
来源：http://ixg.hesvh.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://avu.jianghu66.top

PHP:  // 手写时间戳比较
来源：http://xvy.cashguo.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lwh.zycfv.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mbk.yuanzhike.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://gim.mhx1999.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://pud.jianghu66.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://fnu.birdmap.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ebs.wangdashe.top

[P08] 处理浮点精度问题
来源：http://siz.zycfv.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://vjt.tanke756.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://klw.ydjk.org.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://pua.ehwqpu.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://gmk.jlsjyb.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wrn.gogol.net.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://iqq.jinqigfzy.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ejh.hongshengwenyu.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://gdp.fanxiaobao.xyz

================================================================================
来源：http://miy.yonumen.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://bsc.feifeiyinyue.top

================================================================================
来源：http://sxy.ehwqpu.com

[Q01] 创建表
来源：http://vem.mhx1999.top

CREATE TABLE users (
来源：http://kds.guowangkeji.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://bge.gotoacloud.top

name VARCHAR(50) NOT NULL,
来源：http://bpk.vqdsnc.cn

email VARCHAR(100) UNIQUE,
来源：http://cjl.quarkkingdee.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ivz.sxryk.cn

);
来源：http://wtr.ppjwa.cn

[Q02] 创建带外键的表
来源：http://rtx.0kj1m.cn

CREATE TABLE orders (
来源：http://lep.yueranfly.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ndg.ybcxt.top

user_id INT NOT NULL,
来源：http://tjk.wangshuangyany.cn

amount DECIMAL(10, 2),
来源：http://dog.xziqi.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://qpk.ydzc1.top

);
来源：http://oof.mhx1999.top

[Q03] 增加列
来源：http://miq.tanke756.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://fur.aibaodan.cn

[Q04] 修改列类型
来源：http://bec.sufxvd.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hrz.zhiwuduotai.top

[Q05] 重命名列
来源：http://xpp.meibo888.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://tgl.shanyushiyangkeji.top

[Q06] 删除列
来源：http://fky.hfpthk.cn

ALTER TABLE users DROP COLUMN age;
来源：http://bpg.fktsv.cn

[Q07] 删除表
来源：http://sec.gogol.net.cn

DROP TABLE IF EXISTS orders;
来源：http://uxa.epnwcf.com

[Q08] 创建普通索引
来源：http://jmo.wangshuangyany.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://gme.pycfn.com

[Q09] 创建唯一索引
来源：http://qhm.sjlbkw.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://cfv.yueranfly.top

[Q10] 插入单行
来源：http://jgp.jqgufenzy.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://tgv.hnqzz.top

[Q11] 一次插入多行
来源：http://ozd.c1oappe.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://crw.xuetiantiany.cn

[Q12] 插入后取自增 ID
来源：http://tgf.cucudq.cn

INSERT INTO users (name) VALUES ('C');
来源：http://rgg.daria6918.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://xds.xuanzx.com

[Q13] 忽略重复插入
来源：http://apt.zhongyouzk.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://kkh.snrcjt.cn

[Q14] 存在则更新（upsert）
来源：http://zna.hfpthk.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://evt.zhongyouzk.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://uuf.jlsjyb.cn

[Q15] 查询全部
来源：http://lfh.guannengcc.top

SELECT * FROM users;
来源：http://lfa.52xcode.cn

[Q16] 查询指定列
来源：http://dug.sysykeji.top

SELECT id, name FROM users;
来源：http://yus.nwbrower.top

[Q17] 条件查询
来源：http://fhe.nanxuanxn.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ujy.gogol.net.cn

[Q18] 模糊匹配
来源：http://hes.52xcode.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://pba.nanxinkj.top

[Q19] 范围查询
来源：http://lcn.feifeiyinyue.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://tqm.fktsv.cn

[Q20] IN 列表
来源：http://ljx.hesvh.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://huu.aizwys.cn

[Q21] 空值判断
来源：http://ydr.sufxvd.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://npr.uphjek.com

[Q22] 排序
来源：http://cfe.hysaishi.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://shj.yj20258.top

[Q23] 分页
来源：http://pxa.jinyuanbaomall.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://lvi.yj202588.top

[Q24] 去重
来源：http://nht.gaohongyu789.top

SELECT DISTINCT city FROM users;
来源：http://sku.jinqigfzy.top

[Q25] 只取前 N 条
来源：http://skp.ywan-chungtsiang.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://fit.mhx1999.top

[Q26] 计数
来源：http://jaf.wangdashe.top

SELECT COUNT(*) FROM users;
来源：http://alx.chenzaomai.com

[Q27] 条件计数
来源：http://jbt.xylfe.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://vze.zdqjudy.top

[Q28] 求和与平均
来源：http://etr.hysaishi.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://bgq.jinqigufen.top

[Q29] 最大最小值
来源：http://omd.epnwcf.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://clu.bbcook.cn

[Q30] 分组统计
来源：http://vvt.jqgfzy.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://duu.svipenyu.cn

[Q31] 分组后过滤
来源：http://thl.yvedp.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://nlo.hywenlv.cn

[Q32] 分组拼接字符串
来源：http://kex.sysykeji.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mwh.cdnleiting.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://yer.mhx1999.top

[Q33] 多列分组
来源：http://knx.quarkkingdee.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ibp.iojbl.cn

[Q34] 每组取第一条
来源：http://hfr.hesvh.cn

SELECT * FROM (
来源：http://myt.zhaomingkeji.xyz

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://pzb.cheryme.top

) t WHERE rn = 1;
来源：http://gfw.9152youxi.cn

[Q35] 内连接
来源：http://jva.yfazqb.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://qha.hesvh.cn

[Q36] 左连接
来源：http://yjn.ybcxt.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://otd.gotoacloud.top

[Q37] 右连接
来源：http://hkk.epnwcf.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://yoc.nanxinkj.top

[Q38] 全外连接（PostgreSQL）
来源：http://dpo.zhaomingkeji.xyz

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://uld.ivvv.top

[Q39] 自连接（查上下级）
来源：http://wim.hfpthk.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://xqz.9152youxi.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://brr.yfazqb.com

[Q40] 交叉连接（笛卡尔积）
来源：http://uqh.jqgfzy.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://bbe.dashuyun.cn

[Q41] 多表连接
来源：http://uma.yvedp.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://jmp.shzxlz.cn

JOIN users u ON u.id = o.user_id
来源：http://tns.zycfv.cn

JOIN products p ON p.id = o.product_id;
来源：http://eca.yanxiufei.cn

[Q42] 连接条件附加过滤
来源：http://vbt.zycfv.cn

SELECT u.name, o.amount FROM users u
来源：http://xqf.tian-w.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://thy.zhoulong.xyz

[Q43] 标量子查询
来源：http://lyl.yuxming.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://tbk.zdbjq.cn

[Q44] IN 子查询
来源：http://rdt.meibo888.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://zmz.yj20258.top

[Q45] EXISTS 判断存在
来源：http://xdk.shuidangran.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hhr.aizwys.cn

[Q46] NOT EXISTS 判断不存在
来源：http://qsj.hesvh.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://juh.sxryk.cn

[Q47] 与平均值比较
来源：http://wej.yj202588.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://xpf.wangdashe.top

[Q48] CTE 公用表表达式
来源：http://ftq.tarul.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://osk.gotoacloud.top

SELECT * FROM t WHERE c > 5;
来源：http://mvc.hammf.cn

[Q49] 更新单行
来源：http://bny.c1oappe.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://goi.feifeiyinyue.top

[Q50] 批量更新
来源：http://zus.yj20258.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://tge.cucudq.cn

[Q51] 用子查询更新
来源：http://xgi.fktsv.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://upr.quarkkingdee.top

[Q52] 删除指定行
来源：http://jot.52xcode.cn

DELETE FROM users WHERE id = 10;
来源：http://ufa.sysykeji.top

[Q53] 按条件删除
来源：http://dsf.daxiang520.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://uei.tanke756.top

[Q54] 清空表
来源：http://udm.dashuyun.cn

TRUNCATE TABLE logs;
来源：http://nxb.xylfe.cn

[Q55] 排名（并列占位）
来源：http://rpf.dashuyun.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://tau.havefunace.top

[Q56] 密集排名（并列不占位）
来源：http://gdm.xinyue.icu

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://tly.9152youxi.cn

[Q57] 行号
来源：http://ekb.jianghu66.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wdq.jinqigufen.top

[Q58] 累计求和
来源：http://gsl.redwolf501.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mof.wangshuangyany.cn

[Q59] 分组内累计
来源：http://vma.feifeiyinyue.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://nmo.yangfankeji.com

[Q60] 取上一行 / 下一行
来源：http://yak.cqqwz.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://jaa.svipenyu.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://fau.wangshuangyany.cn

[Q61] 移动平均
来源：http://noj.jinyuanbaomall.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://itl.bbcook.cn

[Q62] 分组占比
来源：http://sug.jinqigufen.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://caa.jlsjyb.cn

[Q63] 开启事务
来源：http://dxy.daxiang520.top

START TRANSACTION;                -- 或 BEGIN
来源：http://eqe.bbcook.cn

[Q64] 提交事务
来源：http://qvp.shanyushiyangtech.top

COMMIT;
来源：http://vzb.cheryme.top

[Q65] 回滚事务
来源：http://dnm.zhongyouzk.top

ROLLBACK;
来源：http://okl.shanyushiyangtech.top

[Q66] 行锁查询
来源：http://jzb.jianghu66.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://als.cucudq.cn

[Q67] 设置隔离级别
来源：http://utd.meibo888.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://jxs.bjfxy.top

[Q68] 保存点
来源：http://dyo.ybcxt.top

SAVEPOINT sp1;
来源：http://xdd.sysykeji.top

ROLLBACK TO sp1;
来源：http://etu.xinyue.icu

[Q69] 查看执行计划
来源：http://rrm.shanyushiyangtech.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://clz.birdmap.top

[Q70] 更新统计信息
来源：http://bfy.epnwcf.com

ANALYZE TABLE users;
来源：http://ggs.ywan-chungtsiang.top

[Q71] 查看建表语句
来源：http://kmd.zhaomingkeji.xyz

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://cfb.jqgfzy.top

[Q72] 查看索引
来源：http://jeo.tanke756.top

SHOW INDEX FROM users;
来源：http://flt.hammf.cn

[Q73] 查看表状态
来源：http://rkt.sweek.top

SHOW TABLE STATUS LIKE 'users';
来源：http://tvd.chenzaomai.com

[Q74] 强制使用索引
来源：http://hch.gogol.net.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://kkz.nwbrower.top

[Q75] 日期格式化
来源：http://uqh.yj20258.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://kzz.pengpengdd.cyou

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://fmf.xinyue.icu

[Q76] 按天统计
来源：http://qde.jqgufenzy.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ike.sufxvd.cn

[Q77] 时间加减
来源：http://rhh.jlsjyb.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ikb.yueranfly.top

[Q78] 当前时间
来源：http://eid.xylfe.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://naz.hammf.cn

[Q79] 字符串拼接
来源：http://gkz.quarkkingdee.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://adr.zhongyouzk.top

[Q80] 字符串截取
来源：http://iqu.sjlbkw.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hqt.tian-w.cn

[Q81] 字符串替换
来源：http://vyg.cheryme.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://tqz.fehbvm.com

[Q82] 字符长度与字节长度
来源：http://crl.zdbjq.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://jxg.guannengcc.top

[Q83] 大小写转换
来源：http://mjm.shanyushiyangkeji.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://keo.xuanzx.com

[Q84] 去除首尾空格
来源：http://adj.sxryk.cn

SELECT TRIM(name) FROM users;
来源：http://chy.zycfv.cn

[Q85] 数值取整
来源：http://mok.hongshengwenyu.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://fud.yfazqb.com

[Q86] 读取 JSON 字段
来源：http://wfz.zhiwuduotai.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://otz.guowangkeji.top

[Q87] JSON 字段做条件
来源：http://mxd.hesvh.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://owj.sysykeji.top

[Q88] 行转列（条件聚合）
来源：http://jbx.tianlin.xyz

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://edy.jiagoushi.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ddi.tianlin.xyz

[Q89] 判断表是否存在
来源：http://jig.bbcook.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://qqu.ivvv.top

[Q90] 生成序号列
来源：http://lld.fengsongda.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://bai.dianchejie.cn

================================================================================
来源：http://gwv.birdmap.top

R. Bash 专题
来源：http://puy.svipenyu.cn

================================================================================
来源：http://oro.bbcook.cn

[R01] shebang 与严格模式
来源：http://fpt.zhoulong.xyz

#!/usr/bin/env bash
来源：http://ghd.zhaomingkeji.xyz

set -euo pipefail
来源：http://kdx.haohaochexian.top

[R02] 变量赋值与使用
来源：http://lzt.meibo888.top

name="Tom"; echo "$name"
来源：http://ctl.hammf.cn

[R03] 只读变量
来源：http://vqu.cucudq.cn

readonly PI=3.14
来源：http://cxi.jinqigufen.top

[R04] 位置参数
来源：http://aaz.nanxinkj.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mhq.nwbrower.top

[R05] 参数默认值
来源：http://cvb.jinyuanbaomall.cn

name="${1:-default}"
来源：http://ric.yonumen.top

[R06] 判断命令是否存在
来源：http://ryd.uphjek.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mzr.shzxlz.cn

[R07] if 判断文件
来源：http://ewf.vqdsnc.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://iht.guannengcc.top

[R08] 数值比较
来源：http://fvz.guannengcc.top

if (( a > b )); then echo "a 更大"; fi
来源：http://oti.epnwcf.com

[R09] 字符串比较
来源：http://jib.gzhubu.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://vqo.jyoumei.cn

[R10] 正则匹配
来源：http://kub.chenzaomai.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ren.fengsongda.top

[R11] case 多分支
来源：http://owb.yj20258.top

case "$1" in
来源：http://qsm.vqdsnc.cn

start) echo "启动" ;;
来源：http://jlm.feifeiyinyue.top

stop)  echo "停止" ;;
来源：http://enz.shangyingyoupin.top

*)     echo "未知命令" ;;
来源：http://yuw.smart0.xyz

esac
来源：http://hms.pycfn.com

[R12] for 遍历文件
来源：http://erv.yongpay.top

for f in *.txt; do echo "$f"; done
来源：http://bho.zycfv.cn

[R13] for 计数循环
来源：http://fgs.tarul.cn

for i in {1..10}; do echo "$i"; done
来源：http://xhv.feifeiyinyue.top

[R14] C 风格 for
来源：http://aaf.yanxiufei.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://jzq.xylfe.cn

[R15] while 逐行读文件
来源：http://nvj.tarul.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://guo.xuetiantiany.cn

[R16] until 等待条件
来源：http://kyu.smart0.xyz

until [[ -f done.flag ]]; do sleep 1; done
来源：http://drb.fehbvm.com

[R17] 数组定义与取值
来源：http://bln.yj20258.top

arr=(a b c); echo "${arr[0]}"
来源：http://frv.mhx1999.top

[R18] 遍历数组
来源：http://eop.pycfn.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wvt.hesvh.cn

[R19] 数组长度
来源：http://mro.guowangkeji.top

echo "${#arr[@]}"
来源：http://qdd.nanxinkj.top

[R20] 关联数组（字典）
来源：http://rck.zhoulong.xyz

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://yow.sufxvd.cn

[R21] 字符串长度
来源：http://sgu.jyoumei.cn


<!-- 参考信息 -->