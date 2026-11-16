代发 wailian999

[P05] 判断两个对象内容是否相等
来源：http://aqe.gotoacloud.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://lfq.jlsjyb.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ptc.mhx1999.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://prp.uphjek.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://tfs.fengsongda.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ztb.316326.xyz

Go:   reflect.DeepEqual(a, b)
来源：http://ksf.daria6918.cn

Ruby: a == b
来源：http://vud.aizwys.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://sis.sjlbkw.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mmd.hnxiangtu.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://tkb.havefunace.top

PHP:  if (empty($x)) {}
来源：http://asi.gaohongyu789.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://icl.chenlongwang.top

TS:   if (x == null) {}
来源：http://gkx.xuanzx.com

Java: if (x == null || x.isEmpty()) {}
来源：http://mro.316326.xyz

Go:   if x == nil {}
来源：http://wfc.wangdashe.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://zjv.zhengqikj.top

C#:   if (x is null) {}
来源：http://liz.yvedp.cn

[P07] 防抖与节流
来源：http://cbq.havefunace.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mfw.quarkkingdee.top

PHP:  // 手写时间戳比较
来源：http://gfz.jyoumei.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gkh.yj202588.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://loj.c1oappe.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://qlz.sysykeji.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://dzt.xuanzx.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://aza.jqgfzy.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://yjx.zycfv.cn

[P08] 处理浮点精度问题
来源：http://hqc.zycfv.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://vva.chenzaomai.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://pyz.pengpengdd.cyou

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://zpp.cheryme.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://duk.sxryk.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://yrc.zhongyouzk.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://cti.yangfankeji.com

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://dem.hongshengwenyu.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hnv.ppjwa.cn

================================================================================
来源：http://lxp.cheryme.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://bxd.jinyuanbaomall.cn

================================================================================
来源：http://uco.dashuyun.cn

[Q01] 创建表
来源：http://tbj.ydjk.org.cn

CREATE TABLE users (
来源：http://xal.hnxiangtu.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://dbi.fzhhl.top

name VARCHAR(50) NOT NULL,
来源：http://aee.svipenyu.cn

email VARCHAR(100) UNIQUE,
来源：http://hoy.xziqi.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://cvt.iojbl.cn

);
来源：http://cec.snrcjt.cn

[Q02] 创建带外键的表
来源：http://pzy.yonumen.top

CREATE TABLE orders (
来源：http://uvr.gaohongyu789.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hzt.dashuyun.cn

user_id INT NOT NULL,
来源：http://brx.jlsjyb.cn

amount DECIMAL(10, 2),
来源：http://bpp.shangyingyoupin.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://zgq.bbcook.cn

);
来源：http://buq.feifeiyinyue.top

[Q03] 增加列
来源：http://nou.yanxiufei.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://pnr.zdqjudy.top

[Q04] 修改列类型
来源：http://tdr.cqqwz.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mmv.xylfe.cn

[Q05] 重命名列
来源：http://xlj.52xcode.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wes.cqqwz.cn

[Q06] 删除列
来源：http://gzx.hcnkem.com

ALTER TABLE users DROP COLUMN age;
来源：http://rsp.xuetiantiany.cn

[Q07] 删除表
来源：http://pay.sjlbkw.cn

DROP TABLE IF EXISTS orders;
来源：http://llu.sysykeji.top

[Q08] 创建普通索引
来源：http://mxm.fzhhl.top

CREATE INDEX idx_users_email ON users(email);
来源：http://rjq.xingfuxueyuan.xyz

[Q09] 创建唯一索引
来源：http://etc.shanyushiyangtech.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ssw.cqqwz.cn

[Q10] 插入单行
来源：http://akn.yj20258.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://rtp.fanxiaobao.xyz

[Q11] 一次插入多行
来源：http://jml.andypj.xyz

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://qqe.yvedp.cn

[Q12] 插入后取自增 ID
来源：http://xyp.ydzc1.top

INSERT INTO users (name) VALUES ('C');
来源：http://lgj.52xcode.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://bqg.pycfn.com

[Q13] 忽略重复插入
来源：http://sgs.guowangkeji.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://txs.0kj1m.cn

[Q14] 存在则更新（upsert）
来源：http://wnq.mhx1999.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://dnl.jinqigfzy.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://fqg.vqdsnc.cn

[Q15] 查询全部
来源：http://hfd.jqgfzy.top

SELECT * FROM users;
来源：http://sfm.fehbvm.com

[Q16] 查询指定列
来源：http://jtn.yueranfly.top

SELECT id, name FROM users;
来源：http://vbn.daxiang520.top

[Q17] 条件查询
来源：http://mjt.meibo888.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://kqu.aibaodan.cn

[Q18] 模糊匹配
来源：http://uvg.zdqjudy.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://fnc.tian-w.cn

[Q19] 范围查询
来源：http://mov.yanxiufei.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hef.yanxiufei.cn

[Q20] IN 列表
来源：http://rfu.yonumen.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://cit.ppjwa.cn

[Q21] 空值判断
来源：http://kks.gzhubu.top

SELECT * FROM users WHERE email IS NULL;
来源：http://tqo.feifeiyinyue.top

[Q22] 排序
来源：http://xaq.kuanghao11.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://nqx.pycfn.com

[Q23] 分页
来源：http://fpc.zhoulong.xyz

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://slg.dianchejie.cn

[Q24] 去重
来源：http://rgn.tanke756.top

SELECT DISTINCT city FROM users;
来源：http://svq.epnwcf.com

[Q25] 只取前 N 条
来源：http://tgl.uphjek.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://vbu.jyoumei.cn

[Q26] 计数
来源：http://jzv.chenlongwang.top

SELECT COUNT(*) FROM users;
来源：http://lxj.ybcxt.top

[Q27] 条件计数
来源：http://srq.ivvv.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://enf.zhaomingkeji.xyz

[Q28] 求和与平均
来源：http://geo.jqgufenzy.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://fwk.kuanghao11.cn

[Q29] 最大最小值
来源：http://scd.yongpay.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://orq.dashuyun.cn

[Q30] 分组统计
来源：http://wag.zhongyouzk.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ybr.jinyuanbaomall.cn

[Q31] 分组后过滤
来源：http://ewx.sxryk.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://eji.jinqigufen.top

[Q32] 分组拼接字符串
来源：http://lif.hnqzz.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://yau.jyoumei.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://xul.epnwcf.com

[Q33] 多列分组
来源：http://lkv.jianghu66.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://nlw.epnwcf.com

[Q34] 每组取第一条
来源：http://khu.jlsjyb.cn

SELECT * FROM (
来源：http://cdg.gogol.net.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hdg.yanxiufei.cn

) t WHERE rn = 1;
来源：http://skz.shzxlz.cn

[Q35] 内连接
来源：http://fix.yonumen.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://yrf.zhengqikj.top

[Q36] 左连接
来源：http://mrk.316326.xyz

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mln.gaohongyu789.top

[Q37] 右连接
来源：http://gls.sweek.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://jvz.yangfankeji.com

[Q38] 全外连接（PostgreSQL）
来源：http://vku.yj20258.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ypb.bbcook.cn

[Q39] 自连接（查上下级）
来源：http://srd.nanxinkj.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://jdc.xziqi.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://cqx.vqdsnc.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://aak.0kj1m.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wat.epnwcf.com

[Q41] 多表连接
来源：http://zfw.zhixingplan.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://dkj.yuxming.cn

JOIN users u ON u.id = o.user_id
来源：http://fbt.yfazqb.com

JOIN products p ON p.id = o.product_id;
来源：http://xby.tian-w.cn

[Q42] 连接条件附加过滤
来源：http://qiq.sufxvd.cn

SELECT u.name, o.amount FROM users u
来源：http://tfa.xingfuxueyuan.xyz

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://pcv.snrcjt.cn

[Q43] 标量子查询
来源：http://rbl.shanyushiyangkeji.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://anr.shangyingyoupin.top

[Q44] IN 子查询
来源：http://pxg.feifeiyinyue.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://zux.yvedp.cn

[Q45] EXISTS 判断存在
来源：http://aku.guowangkeji.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://gta.svipenyu.cn

[Q46] NOT EXISTS 判断不存在
来源：http://dca.tarul.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ptx.xinyue.icu

[Q47] 与平均值比较
来源：http://eph.chenlongwang.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://gzw.wangshuangyany.cn

[Q48] CTE 公用表表达式
来源：http://ant.xylfe.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://bau.fzhhl.top

SELECT * FROM t WHERE c > 5;
来源：http://clb.nanxuanxn.top

[Q49] 更新单行
来源：http://xzp.cqqwz.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://tod.jinyuanbaomall.cn

[Q50] 批量更新
来源：http://anz.ppjwa.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ltl.jinqigfzy.top

[Q51] 用子查询更新
来源：http://cxz.vqdsnc.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://eun.cqqwz.cn

[Q52] 删除指定行
来源：http://kbv.ywan-chungtsiang.top

DELETE FROM users WHERE id = 10;
来源：http://ifc.cdnleiting.top

[Q53] 按条件删除
来源：http://tfk.xziqi.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ypk.snrcjt.cn

[Q54] 清空表
来源：http://fnr.yj202588.top

TRUNCATE TABLE logs;
来源：http://wxg.sweek.top

[Q55] 排名（并列占位）
来源：http://hus.gotoacloud.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://qzh.meibo888.top

[Q56] 密集排名（并列不占位）
来源：http://uuc.bbcook.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://doo.nwbrower.top

[Q57] 行号
来源：http://zjh.xylfe.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://fkl.shzxlz.cn

[Q58] 累计求和
来源：http://hwx.xinyue.icu

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://iav.zhiwuduotai.top

[Q59] 分组内累计
来源：http://pyl.ywan-chungtsiang.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://fzt.jinyuanbaomall.cn

[Q60] 取上一行 / 下一行
来源：http://msl.yonumen.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ekk.zhoulong.xyz

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://bfq.cucudq.cn

[Q61] 移动平均
来源：http://whq.shuidangran.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://olr.gogol.net.cn

[Q62] 分组占比
来源：http://fqh.zhongyouzk.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ubh.sufxvd.cn

[Q63] 开启事务
来源：http://csa.yvedp.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://yuv.haohaochexian.top

[Q64] 提交事务
来源：http://eyj.jqgfzy.top

COMMIT;
来源：http://zdp.yj20258888.top

[Q65] 回滚事务
来源：http://egl.epnwcf.com

ROLLBACK;
来源：http://fbd.uphjek.com

[Q66] 行锁查询
来源：http://qyn.havefunace.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://kby.vqdsnc.cn

[Q67] 设置隔离级别
来源：http://hmy.daria6918.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ooa.tarul.cn

[Q68] 保存点
来源：http://rys.xylfe.cn

SAVEPOINT sp1;
来源：http://khm.yj202588.top

ROLLBACK TO sp1;
来源：http://rzc.tianlin.xyz

[Q69] 查看执行计划
来源：http://hjb.zhijiandao.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://kfb.meibo888.top

[Q70] 更新统计信息
来源：http://xbx.hnqzz.top

ANALYZE TABLE users;
来源：http://pii.tarul.cn

[Q71] 查看建表语句
来源：http://ana.haohaochexian.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ptj.zycfv.cn

[Q72] 查看索引
来源：http://hqf.zhiwuduotai.top

SHOW INDEX FROM users;
来源：http://qsj.nanxuanxn.top

[Q73] 查看表状态
来源：http://rdi.iojbl.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://vas.quarkkingdee.top

[Q74] 强制使用索引
来源：http://orm.zhongyouzk.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://lix.sxryk.cn

[Q75] 日期格式化
来源：http://kro.haohaochexian.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://jyu.yueranfly.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://myy.ctjpmb.com

[Q76] 按天统计
来源：http://blu.hnxiangtu.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://sti.zhengqikj.top

[Q77] 时间加减
来源：http://pzx.dashuyun.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wem.ywan-chungtsiang.top

[Q78] 当前时间
来源：http://ffy.yj202588.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://nev.jqgufenzy.top

[Q79] 字符串拼接
来源：http://fom.quarkkingdee.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wna.hammf.cn

[Q80] 字符串截取
来源：http://juv.jqgfzy.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ytm.sxryk.cn

[Q81] 字符串替换
来源：http://bhb.aibaodan.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://xan.jqgfzy.top

[Q82] 字符长度与字节长度
来源：http://obf.hammf.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://dzn.smart0.xyz

[Q83] 大小写转换
来源：http://coo.gaohongyu789.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://oqb.tianlin.xyz

[Q84] 去除首尾空格
来源：http://kam.shzxlz.cn

SELECT TRIM(name) FROM users;
来源：http://fso.ehwqpu.com

[Q85] 数值取整
来源：http://otq.fehbvm.com

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://egf.cheryme.top

[Q86] 读取 JSON 字段
来源：http://ybh.jianghu66.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://zgd.dashuyun.cn

[Q87] JSON 字段做条件
来源：http://kjb.andypj.xyz

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hsg.ywan-chungtsiang.top

[Q88] 行转列（条件聚合）
来源：http://mzb.nanxinkj.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://pqh.ivvv.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://zfv.wangdashe.top

[Q89] 判断表是否存在
来源：http://gae.gotoacloud.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://gsu.meibo888.top

[Q90] 生成序号列
来源：http://jwi.ehwqpu.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://kzr.xylfe.cn

================================================================================
来源：http://mcm.shanyushiyangkeji.top

R. Bash 专题
来源：http://weh.jinqigufen.top

================================================================================
来源：http://phw.jinghuilouyu.cn

[R01] shebang 与严格模式
来源：http://ztc.zhongyouzk.top

#!/usr/bin/env bash
来源：http://gfb.jyoumei.cn

set -euo pipefail
来源：http://cax.jlsjyb.cn

[R02] 变量赋值与使用
来源：http://epv.yuanzhike.top

name="Tom"; echo "$name"
来源：http://xzz.yuxming.cn

[R03] 只读变量
来源：http://koq.vehdjk.com

readonly PI=3.14
来源：http://pxv.cqqwz.cn

[R04] 位置参数
来源：http://uvc.pengpengdd.cyou

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://aly.yj202588.top

[R05] 参数默认值
来源：http://bdd.9152youxi.cn

name="${1:-default}"
来源：http://jio.yanxiufei.cn

[R06] 判断命令是否存在
来源：http://nra.bjfxy.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wwp.chenzaomai.com

[R07] if 判断文件
来源：http://sor.zhongyouzk.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://qoj.jinqigfzy.top

[R08] 数值比较
来源：http://mum.hcnkem.com

if (( a > b )); then echo "a 更大"; fi
来源：http://yqu.zhengqikj.top

[R09] 字符串比较
来源：http://enu.gogol.net.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://aoq.yangfankeji.com

[R10] 正则匹配
来源：http://bui.nanxinkj.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://bco.jlsjyb.cn

[R11] case 多分支
来源：http://yhu.zycfv.cn

case "$1" in
来源：http://ktf.0kj1m.cn

start) echo "启动" ;;
来源：http://kap.yongpay.top

stop)  echo "停止" ;;
来源：http://idq.hysaishi.cn

*)     echo "未知命令" ;;
来源：http://mzy.wangdashe.top

esac
来源：http://iww.fanxiaobao.xyz

[R12] for 遍历文件
来源：http://xxb.haohaochexian.top

for f in *.txt; do echo "$f"; done
来源：http://hzs.yj202588.top

[R13] for 计数循环
来源：http://tft.yonumen.top

for i in {1..10}; do echo "$i"; done
来源：http://pyi.zhaomingkeji.xyz

[R14] C 风格 for
来源：http://vxy.nanxuanxn.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://pxf.svipenyu.cn

[R15] while 逐行读文件
来源：http://ygg.wangshuangyany.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://zrf.dianchejie.cn

[R16] until 等待条件
来源：http://cdb.shangyingyoupin.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wrp.dashuyun.cn

[R17] 数组定义与取值
来源：http://grx.jyoumei.cn

arr=(a b c); echo "${arr[0]}"
来源：http://eef.iojbl.cn

[R18] 遍历数组
来源：http://oia.shanyushiyangkeji.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://fho.cucudq.cn

[R19] 数组长度
来源：http://zgg.tian-w.cn

echo "${#arr[@]}"
来源：http://raf.yuanzhike.top

[R20] 关联数组（字典）
来源：http://slv.ivvv.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://uqc.jlsjyb.cn

[R21] 字符串长度
来源：http://vmf.aibaodan.cn

echo "${#s}"
来源：http://dhd.hammf.cn

[R22] 截取子串
来源：http://twn.fanxiaobao.xyz

echo "${s:0:5}"
来源：http://weh.nanxuanxn.top

[R23] 字符串替换
来源：http://zcx.tarul.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://rpn.dashuyun.cn

[R24] 大小写转换
来源：http://qpq.cucudq.cn

echo "${s^^}"; echo "${s,,}"
来源：http://qgb.nwbrower.top

[R25] 去后缀 / 去前缀
来源：http://wuq.cucudq.cn


<!-- 参考信息 -->