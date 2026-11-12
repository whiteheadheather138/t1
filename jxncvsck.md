代发 wailian999

Py:   len(x)            # 字符串、列表、字典通用
来源：http://tfo.yonumen.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wjy.snrcjt.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vap.jinyuanbaomall.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gna.uphjek.com

Java: list.size();  map.size();  s.length()
来源：http://nhq.jlsjyb.cn

Go:   len(arr);  len(m)
来源：http://eif.jyoumei.cn

Ruby: x.length;  x.size
来源：http://xtz.zhaomingkeji.xyz

C#:   list.Count;  dict.Count;  s.Length
来源：http://jjt.nanxinkj.top

[P05] 判断两个对象内容是否相等
来源：http://zzq.jianghu66.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://seo.sufxvd.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://fgq.yvedp.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hps.0kj1m.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ukm.sysykeji.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://bvm.shuidangran.top

Go:   reflect.DeepEqual(a, b)
来源：http://xzz.fanxiaobao.xyz

Ruby: a == b
来源：http://tij.fehbvm.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wel.zycfv.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://imh.redwolf501.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://lzx.kuanghao11.cn

PHP:  if (empty($x)) {}
来源：http://yyr.guowangkeji.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://bbc.daria6918.cn

TS:   if (x == null) {}
来源：http://hjc.jqgfzy.top

Java: if (x == null || x.isEmpty()) {}
来源：http://ipk.wangdashe.top

Go:   if x == nil {}
来源：http://nty.chenjidiqi.icu

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://vsw.fehbvm.com

C#:   if (x is null) {}
来源：http://mab.zhoulong.xyz

[P07] 防抖与节流
来源：http://cwa.zycfv.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ubi.sxryk.cn

PHP:  // 手写时间戳比较
来源：http://avz.wangdashe.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bkl.haohaochexian.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://isk.meibo888.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://jpb.sjlbkw.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://voz.uphjek.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://ekg.nanxinkj.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://spf.yuxming.cn

[P08] 处理浮点精度问题
来源：http://cum.shanyushiyangkeji.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://pje.zhiwuduotai.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://kgn.yj20258.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://zxm.sweek.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://zzr.xuetiantiany.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://qlu.c1oappe.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://tal.dashuyun.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://whj.yonumen.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://xcp.zhongyouzk.top

================================================================================
来源：http://tbo.nanxuanxn.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://xsf.shangyingyoupin.top

================================================================================
来源：http://mnf.ppjwa.cn

[Q01] 创建表
来源：http://jor.cdnleiting.top

CREATE TABLE users (
来源：http://bta.zhixingplan.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://cso.cashguo.top

name VARCHAR(50) NOT NULL,
来源：http://gng.cucudq.cn

email VARCHAR(100) UNIQUE,
来源：http://nvm.dashuyun.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://nam.redwolf501.top

);
来源：http://wsf.ppjwa.cn

[Q02] 创建带外键的表
来源：http://har.yanxiufei.cn

CREATE TABLE orders (
来源：http://uel.smart0.xyz

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://usn.316326.xyz

user_id INT NOT NULL,
来源：http://hpz.svipenyu.cn

amount DECIMAL(10, 2),
来源：http://foh.jqgufenzy.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://fuc.jqgufenzy.top

);
来源：http://egp.fktsv.cn

[Q03] 增加列
来源：http://msf.zhiwuduotai.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wib.cucudq.cn

[Q04] 修改列类型
来源：http://hpb.sjlbkw.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://caf.xingfuxueyuan.xyz

[Q05] 重命名列
来源：http://iza.nwbrower.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ucl.hysaishi.cn

[Q06] 删除列
来源：http://orx.xinyue.icu

ALTER TABLE users DROP COLUMN age;
来源：http://oqa.redwolf501.top

[Q07] 删除表
来源：http://ofb.jqgufenzy.top

DROP TABLE IF EXISTS orders;
来源：http://skv.cheryme.top

[Q08] 创建普通索引
来源：http://qdf.zdbjq.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://nxw.tanke756.top

[Q09] 创建唯一索引
来源：http://orw.quarkkingdee.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://dza.bbcook.cn

[Q10] 插入单行
来源：http://kxy.gogol.net.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://jft.zhaomingkeji.xyz

[Q11] 一次插入多行
来源：http://uox.hnxiangtu.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wju.hongshengwenyu.top

[Q12] 插入后取自增 ID
来源：http://aao.nwbrower.top

INSERT INTO users (name) VALUES ('C');
来源：http://vtk.pycfn.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://eao.tarul.cn

[Q13] 忽略重复插入
来源：http://aas.havefunace.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://nzy.fengsongda.top

[Q14] 存在则更新（upsert）
来源：http://hiw.hcnkem.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ldn.wangdashe.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://kup.yj20258.top

[Q15] 查询全部
来源：http://nkk.zhaomingkeji.xyz

SELECT * FROM users;
来源：http://qmj.mhx1999.top

[Q16] 查询指定列
来源：http://avb.shuidangran.top

SELECT id, name FROM users;
来源：http://bgj.sufxvd.cn

[Q17] 条件查询
来源：http://ozg.jinqigfzy.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://dhr.iojbl.cn

[Q18] 模糊匹配
来源：http://ukd.52xcode.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wuc.yvedp.cn

[Q19] 范围查询
来源：http://bgj.ivvv.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hyb.cqqwz.cn

[Q20] IN 列表
来源：http://tpz.vehdjk.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://zlo.jqgufenzy.top

[Q21] 空值判断
来源：http://aln.xuanzx.com

SELECT * FROM users WHERE email IS NULL;
来源：http://hsw.zycfv.cn

[Q22] 排序
来源：http://qbw.yuxming.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mta.jinghuilouyu.cn

[Q23] 分页
来源：http://fwo.guowangkeji.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ywv.jiagoushi.top

[Q24] 去重
来源：http://oiz.xuetiantiany.cn

SELECT DISTINCT city FROM users;
来源：http://pkj.yuxming.cn

[Q25] 只取前 N 条
来源：http://zup.shangyingyoupin.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://dek.xingfuxueyuan.xyz

[Q26] 计数
来源：http://fqb.daxiang520.top

SELECT COUNT(*) FROM users;
来源：http://ktk.c1oappe.top

[Q27] 条件计数
来源：http://dvc.zhaomingkeji.xyz

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://jem.nanxinkj.top

[Q28] 求和与平均
来源：http://adw.cqqwz.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://rsz.shanyushiyangtech.top

[Q29] 最大最小值
来源：http://rmd.jinqigufen.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://qxn.epnwcf.com

[Q30] 分组统计
来源：http://nsy.xinyue.icu

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://yhx.chenlongwang.top

[Q31] 分组后过滤
来源：http://ozx.yj20258888.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://gii.hfpthk.cn

[Q32] 分组拼接字符串
来源：http://lhx.yj20258888.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://tmg.hfpthk.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://kup.c1oappe.top

[Q33] 多列分组
来源：http://kfi.zhijiandao.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://oll.wangdashe.top

[Q34] 每组取第一条
来源：http://xjy.gaohongyu789.top

SELECT * FROM (
来源：http://tow.nwbrower.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ssn.chenzaomai.com

) t WHERE rn = 1;
来源：http://jky.fengsongda.top

[Q35] 内连接
来源：http://cir.zdqjudy.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://yjf.fzhhl.top

[Q36] 左连接
来源：http://xoq.zhengqikj.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://jov.yj202588.top

[Q37] 右连接
来源：http://bqd.tianlin.xyz

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://dmv.ywan-chungtsiang.top

[Q38] 全外连接（PostgreSQL）
来源：http://eqi.chenjidiqi.icu

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://cgz.haohaochexian.top

[Q39] 自连接（查上下级）
来源：http://pze.ywan-chungtsiang.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://hyl.uphjek.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://xyk.0kj1m.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://lnz.yj202588.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://sca.nanxuanxn.top

[Q41] 多表连接
来源：http://hhx.sjlbkw.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://nib.hnxiangtu.top

JOIN users u ON u.id = o.user_id
来源：http://gtt.shzxlz.cn

JOIN products p ON p.id = o.product_id;
来源：http://fmd.sufxvd.cn

[Q42] 连接条件附加过滤
来源：http://prm.daxiang520.top

SELECT u.name, o.amount FROM users u
来源：http://kbl.uphjek.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://xcn.shangyingyoupin.top

[Q43] 标量子查询
来源：http://rff.dashuyun.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ojn.redwolf501.top

[Q44] IN 子查询
来源：http://bda.ivvv.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://qht.guowangkeji.top

[Q45] EXISTS 判断存在
来源：http://ubh.nanxuanxn.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://loi.jianghu66.top

[Q46] NOT EXISTS 判断不存在
来源：http://vyt.cucudq.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zva.zhaomingkeji.xyz

[Q47] 与平均值比较
来源：http://bwd.c1oappe.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://vse.daria6918.cn

[Q48] CTE 公用表表达式
来源：http://hef.sxryk.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://yby.fanxiaobao.xyz

SELECT * FROM t WHERE c > 5;
来源：http://yym.cucudq.cn

[Q49] 更新单行
来源：http://gat.zhongyouzk.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://oza.tianlin.xyz

[Q50] 批量更新
来源：http://trp.zhijiandao.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://zhp.hysaishi.cn

[Q51] 用子查询更新
来源：http://dgk.nanxuanxn.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ffd.cashguo.top

[Q52] 删除指定行
来源：http://fja.zhoulong.xyz

DELETE FROM users WHERE id = 10;
来源：http://vxw.redwolf501.top

[Q53] 按条件删除
来源：http://xab.hongshengwenyu.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://saf.zdbjq.cn

[Q54] 清空表
来源：http://khp.fzhhl.top

TRUNCATE TABLE logs;
来源：http://eoa.epnwcf.com

[Q55] 排名（并列占位）
来源：http://itj.quarkkingdee.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://anr.yvedp.cn

[Q56] 密集排名（并列不占位）
来源：http://ekp.jyoumei.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://dgv.jianghu66.top

[Q57] 行号
来源：http://qjo.zdbjq.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://vei.zhixingplan.top

[Q58] 累计求和
来源：http://fxi.zhoulong.xyz

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://qoe.nanxinkj.top

[Q59] 分组内累计
来源：http://mly.0kj1m.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://qem.ydzc1.top

[Q60] 取上一行 / 下一行
来源：http://otg.vehdjk.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://dto.fzhhl.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ydu.jinyuanbaomall.cn

[Q61] 移动平均
来源：http://bxv.yvedp.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hah.yj20258.top

[Q62] 分组占比
来源：http://oie.yuxming.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://qmn.aizwys.cn

[Q63] 开启事务
来源：http://eva.zdbjq.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://qht.epnwcf.com

[Q64] 提交事务
来源：http://imp.fktsv.cn

COMMIT;
来源：http://nti.fehbvm.com

[Q65] 回滚事务
来源：http://wbp.zhixingplan.top

ROLLBACK;
来源：http://atx.havefunace.top

[Q66] 行锁查询
来源：http://fjx.yj202588.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://tkx.gaohongyu789.top

[Q67] 设置隔离级别
来源：http://boq.ppjwa.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://qie.chenlongwang.top

[Q68] 保存点
来源：http://com.yuanzhike.top

SAVEPOINT sp1;
来源：http://put.yongpay.top

ROLLBACK TO sp1;
来源：http://udx.sufxvd.cn

[Q69] 查看执行计划
来源：http://tfu.yangfankeji.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://lni.chenjidiqi.icu

[Q70] 更新统计信息
来源：http://hgb.xylfe.cn

ANALYZE TABLE users;
来源：http://uft.zdqjudy.top

[Q71] 查看建表语句
来源：http://jpx.zhixingplan.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://upv.svipenyu.cn

[Q72] 查看索引
来源：http://ndo.iojbl.cn

SHOW INDEX FROM users;
来源：http://uyn.jyoumei.cn

[Q73] 查看表状态
来源：http://uzh.aibaodan.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://mne.sweek.top

[Q74] 强制使用索引
来源：http://yup.guowangkeji.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://udx.cucudq.cn

[Q75] 日期格式化
来源：http://guv.dashuyun.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://snq.hesvh.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://tjw.feifeiyinyue.top

[Q76] 按天统计
来源：http://med.quarkkingdee.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://rtg.chenlongwang.top

[Q77] 时间加减
来源：http://zkd.pengpengdd.cyou

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ldx.dianchejie.cn

[Q78] 当前时间
来源：http://kfg.tarul.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://tvw.vqdsnc.cn

[Q79] 字符串拼接
来源：http://pgf.chenlongwang.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://iks.chenlongwang.top

[Q80] 字符串截取
来源：http://nfu.yongpay.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://tei.yonumen.top

[Q81] 字符串替换
来源：http://dcw.hcnkem.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://dbr.tanke756.top

[Q82] 字符长度与字节长度
来源：http://exs.ctjpmb.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://zrz.hysaishi.cn

[Q83] 大小写转换
来源：http://kst.ydjk.org.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://yjh.hnqzz.top

[Q84] 去除首尾空格
来源：http://lle.nanxinkj.top

SELECT TRIM(name) FROM users;
来源：http://kma.shanyushiyangkeji.top

[Q85] 数值取整
来源：http://iwj.gogol.net.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://jme.yuanzhike.top

[Q86] 读取 JSON 字段
来源：http://hiq.fzhhl.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://tbg.bjfxy.top

[Q87] JSON 字段做条件
来源：http://pmu.daxiang520.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://yai.vehdjk.com

[Q88] 行转列（条件聚合）
来源：http://rsb.xziqi.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://utc.ydjk.org.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://olk.jianghu66.top

[Q89] 判断表是否存在
来源：http://erv.jinghuilouyu.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://klp.jinqigufen.top

[Q90] 生成序号列
来源：http://zov.yj202588.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ekt.andypj.xyz

================================================================================
来源：http://qlq.yvedp.cn

R. Bash 专题
来源：http://xrj.vehdjk.com

================================================================================
来源：http://bcn.tian-w.cn

[R01] shebang 与严格模式
来源：http://ttt.wangshuangyany.cn

#!/usr/bin/env bash
来源：http://rkm.bjfxy.top

set -euo pipefail
来源：http://xra.cqqwz.cn

[R02] 变量赋值与使用
来源：http://emr.316326.xyz

name="Tom"; echo "$name"
来源：http://nos.jinyuanbaomall.cn

[R03] 只读变量
来源：http://pia.zhongyouzk.top

readonly PI=3.14
来源：http://ukz.gaohongyu789.top

[R04] 位置参数
来源：http://bdm.0kj1m.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://qfq.hongshengwenyu.top

[R05] 参数默认值
来源：http://fih.daria6918.cn

name="${1:-default}"
来源：http://gja.ydjk.org.cn

[R06] 判断命令是否存在
来源：http://faz.yonumen.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ubt.daxiang520.top

[R07] if 判断文件
来源：http://ssv.iojbl.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://frv.zhaomingkeji.xyz

[R08] 数值比较
来源：http://cav.bbcook.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://yiw.hfpthk.cn

[R09] 字符串比较
来源：http://hii.cashguo.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://was.xinyue.icu

[R10] 正则匹配
来源：http://rjj.shanyushiyangkeji.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://zzc.ydjk.org.cn

[R11] case 多分支
来源：http://mmx.zhongyouzk.top

case "$1" in
来源：http://dnb.xuetiantiany.cn

start) echo "启动" ;;
来源：http://jkx.haohaochexian.top

stop)  echo "停止" ;;
来源：http://vnv.dashuyun.cn

*)     echo "未知命令" ;;
来源：http://odm.aizwys.cn

esac
来源：http://jem.xziqi.cn

[R12] for 遍历文件
来源：http://fcb.smart0.xyz

for f in *.txt; do echo "$f"; done
来源：http://kii.gogol.net.cn

[R13] for 计数循环
来源：http://slo.hysaishi.cn

for i in {1..10}; do echo "$i"; done
来源：http://cwk.dashuyun.cn

[R14] C 风格 for
来源：http://mrz.fengsongda.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://bvf.zhaomingkeji.xyz

[R15] while 逐行读文件
来源：http://dpb.ydzc1.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ukk.pengpengdd.cyou

[R16] until 等待条件
来源：http://cnj.feifeiyinyue.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://oju.bbcook.cn

[R17] 数组定义与取值
来源：http://csx.haohaochexian.top

arr=(a b c); echo "${arr[0]}"
来源：http://ibq.yuxming.cn

[R18] 遍历数组
来源：http://wny.ctjpmb.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://zlx.9152youxi.cn

[R19] 数组长度
来源：http://bgq.jinqigufen.top

echo "${#arr[@]}"
来源：http://ctd.aizwys.cn

[R20] 关联数组（字典）
来源：http://uia.shangyingyoupin.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://zgt.andypj.xyz

[R21] 字符串长度
来源：http://kcu.yuanzhike.top


<!-- 参考信息 -->