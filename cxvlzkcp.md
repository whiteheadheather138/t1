代发 wailian999

Java: list.size();  map.size();  s.length()
来源：http://gwu.nwbrower.top

Go:   len(arr);  len(m)
来源：http://fkc.tarul.cn

Ruby: x.length;  x.size
来源：http://ojh.vehdjk.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://vmu.ybcxt.top

[P05] 判断两个对象内容是否相等
来源：http://xnp.hcnkem.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://opu.zhoulong.xyz

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://jtz.ivvv.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mdw.yj20258.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://fiq.gaohongyu789.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://gjl.mhx1999.top

Go:   reflect.DeepEqual(a, b)
来源：http://zbf.daria6918.cn

Ruby: a == b
来源：http://jxr.yanxiufei.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://qio.zhaomingkeji.xyz

[P06] 综合判空（null / 空串 / 空集合）
来源：http://jbh.zhongyouzk.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://yzx.fengsongda.top

PHP:  if (empty($x)) {}
来源：http://iqf.meibo888.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://gkb.sysykeji.top

TS:   if (x == null) {}
来源：http://phk.svipenyu.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://abu.52xcode.cn

Go:   if x == nil {}
来源：http://fuc.quarkkingdee.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://yxu.redwolf501.top

C#:   if (x is null) {}
来源：http://rjr.redwolf501.top

[P07] 防抖与节流
来源：http://ytz.guowangkeji.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://lwf.andypj.xyz

PHP:  // 手写时间戳比较
来源：http://akt.chenlongwang.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tkx.xylfe.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vnt.yfazqb.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wzc.yfazqb.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://imb.yj20258888.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://llv.xuanzx.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://jol.snrcjt.cn

[P08] 处理浮点精度问题
来源：http://ngv.xuetiantiany.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://gai.gotoacloud.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hvz.shangyingyoupin.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://uqt.yuxming.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ssh.tarul.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://tzh.gaohongyu789.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://rov.hnxiangtu.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mth.yonumen.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://atq.pycfn.com

================================================================================
来源：http://cvb.jinqigfzy.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://slb.hysaishi.cn

================================================================================
来源：http://zfu.hongshengwenyu.top

[Q01] 创建表
来源：http://jrp.fktsv.cn

CREATE TABLE users (
来源：http://yyj.vqdsnc.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://pnr.aizwys.cn

name VARCHAR(50) NOT NULL,
来源：http://wwp.jianghu66.top

email VARCHAR(100) UNIQUE,
来源：http://xmw.aibaodan.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://jez.hfpthk.cn

);
来源：http://tzl.nwbrower.top

[Q02] 创建带外键的表
来源：http://dqv.xuetiantiany.cn

CREATE TABLE orders (
来源：http://mri.316326.xyz

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wva.gotoacloud.top

user_id INT NOT NULL,
来源：http://jqn.bbcook.cn

amount DECIMAL(10, 2),
来源：http://lbt.xylfe.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mdx.nwbrower.top

);
来源：http://ldg.zdbjq.cn

[Q03] 增加列
来源：http://bkb.fehbvm.com

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://oht.meibo888.top

[Q04] 修改列类型
来源：http://kld.ybcxt.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://sgj.guowangkeji.top

[Q05] 重命名列
来源：http://ldj.52xcode.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://uth.tanke756.top

[Q06] 删除列
来源：http://zwj.xziqi.cn

ALTER TABLE users DROP COLUMN age;
来源：http://vfb.iojbl.cn

[Q07] 删除表
来源：http://zfn.yj20258.top

DROP TABLE IF EXISTS orders;
来源：http://llt.snrcjt.cn

[Q08] 创建普通索引
来源：http://htv.havefunace.top

CREATE INDEX idx_users_email ON users(email);
来源：http://nxz.havefunace.top

[Q09] 创建唯一索引
来源：http://bch.yvedp.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://jkp.shanyushiyangkeji.top

[Q10] 插入单行
来源：http://ugh.zhijiandao.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://rbh.gaohongyu789.top

[Q11] 一次插入多行
来源：http://eco.sufxvd.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://tcx.fzhhl.top

[Q12] 插入后取自增 ID
来源：http://bev.sxryk.cn

INSERT INTO users (name) VALUES ('C');
来源：http://egf.dianchejie.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://xft.aizwys.cn

[Q13] 忽略重复插入
来源：http://fwv.jinqigufen.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://rey.bjfxy.top

[Q14] 存在则更新（upsert）
来源：http://nuo.yonumen.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://kuu.hfpthk.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://smn.guowangkeji.top

[Q15] 查询全部
来源：http://wdp.yfazqb.com

SELECT * FROM users;
来源：http://gnu.xuanzx.com

[Q16] 查询指定列
来源：http://pip.dashuyun.cn

SELECT id, name FROM users;
来源：http://uot.zdqjudy.top

[Q17] 条件查询
来源：http://lzc.smart0.xyz

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://tos.c1oappe.top

[Q18] 模糊匹配
来源：http://gos.0kj1m.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://pcn.smart0.xyz

[Q19] 范围查询
来源：http://bvn.yfazqb.com

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hbv.zhixingplan.top

[Q20] IN 列表
来源：http://kbt.jqgfzy.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://sxz.tarul.cn

[Q21] 空值判断
来源：http://pug.svipenyu.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://qhi.zhixingplan.top

[Q22] 排序
来源：http://mdk.vqdsnc.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hto.9152youxi.cn

[Q23] 分页
来源：http://agc.zhiwuduotai.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://xyw.dashuyun.cn

[Q24] 去重
来源：http://eto.sysykeji.top

SELECT DISTINCT city FROM users;
来源：http://tpt.yvedp.cn

[Q25] 只取前 N 条
来源：http://hbl.havefunace.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://uca.vqdsnc.cn

[Q26] 计数
来源：http://jrm.jqgufenzy.top

SELECT COUNT(*) FROM users;
来源：http://sae.zhixingplan.top

[Q27] 条件计数
来源：http://jtw.meibo888.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://plh.xuanzx.com

[Q28] 求和与平均
来源：http://mjq.316326.xyz

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://oel.jinyuanbaomall.cn

[Q29] 最大最小值
来源：http://utv.yongpay.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://cnf.hywenlv.cn

[Q30] 分组统计
来源：http://xmx.316326.xyz

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hlc.chenzaomai.com

[Q31] 分组后过滤
来源：http://tly.havefunace.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://neh.haohaochexian.top

[Q32] 分组拼接字符串
来源：http://mqx.xuetiantiany.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://jum.fehbvm.com

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://jbz.yuanzhike.top

[Q33] 多列分组
来源：http://wre.yj202588.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hid.zycfv.cn

[Q34] 每组取第一条
来源：http://cpn.nwbrower.top

SELECT * FROM (
来源：http://olo.52xcode.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ycc.9152youxi.cn

) t WHERE rn = 1;
来源：http://nai.jianghu66.top

[Q35] 内连接
来源：http://eqg.ydzc1.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://zyx.hammf.cn

[Q36] 左连接
来源：http://gqo.shanyushiyangkeji.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://dzs.uphjek.com

[Q37] 右连接
来源：http://tnl.gotoacloud.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://kuk.tarul.cn

[Q38] 全外连接（PostgreSQL）
来源：http://pqm.c1oappe.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wuv.andypj.xyz

[Q39] 自连接（查上下级）
来源：http://iej.redwolf501.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://hxa.jinyuanbaomall.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://pbm.fzhhl.top

[Q40] 交叉连接（笛卡尔积）
来源：http://qjl.cdnleiting.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wqt.ppjwa.cn

[Q41] 多表连接
来源：http://urg.0kj1m.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://wed.0kj1m.cn

JOIN users u ON u.id = o.user_id
来源：http://bzt.wangshuangyany.cn

JOIN products p ON p.id = o.product_id;
来源：http://yxa.ywan-chungtsiang.top

[Q42] 连接条件附加过滤
来源：http://kwj.wangshuangyany.cn

SELECT u.name, o.amount FROM users u
来源：http://vte.wangshuangyany.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://vam.zhiwuduotai.top

[Q43] 标量子查询
来源：http://fsa.wangshuangyany.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://pev.cucudq.cn

[Q44] IN 子查询
来源：http://irv.xuanzx.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mpw.hcnkem.com

[Q45] EXISTS 判断存在
来源：http://ldq.hfpthk.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kqz.xziqi.cn

[Q46] NOT EXISTS 判断不存在
来源：http://qpf.birdmap.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://dmd.yj20258888.top

[Q47] 与平均值比较
来源：http://pkt.52xcode.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://itq.birdmap.top

[Q48] CTE 公用表表达式
来源：http://mpb.ybcxt.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://qeq.andypj.xyz

SELECT * FROM t WHERE c > 5;
来源：http://dut.tian-w.cn

[Q49] 更新单行
来源：http://kgn.guowangkeji.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ztv.jinqigufen.top

[Q50] 批量更新
来源：http://jxl.sweek.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://oqw.hnxiangtu.top

[Q51] 用子查询更新
来源：http://csn.yvedp.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://xiq.hnqzz.top

[Q52] 删除指定行
来源：http://kwq.hesvh.cn

DELETE FROM users WHERE id = 10;
来源：http://ott.gotoacloud.top

[Q53] 按条件删除
来源：http://erz.jinghuilouyu.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://rhd.jianghu66.top

[Q54] 清空表
来源：http://lmh.xinyue.icu

TRUNCATE TABLE logs;
来源：http://tjy.vqdsnc.cn

[Q55] 排名（并列占位）
来源：http://qhe.smart0.xyz

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://qqr.tanke756.top

[Q56] 密集排名（并列不占位）
来源：http://jvg.pengpengdd.cyou

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://byu.tarul.cn

[Q57] 行号
来源：http://yyu.tarul.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ycx.sweek.top

[Q58] 累计求和
来源：http://eid.pycfn.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://awd.feifeiyinyue.top

[Q59] 分组内累计
来源：http://uqt.shanyushiyangtech.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://sfs.svipenyu.cn

[Q60] 取上一行 / 下一行
来源：http://sqf.xinyue.icu

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://jlt.hcnkem.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://uol.shangyingyoupin.top

[Q61] 移动平均
来源：http://piv.zhijiandao.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://iza.zhixingplan.top

[Q62] 分组占比
来源：http://dnx.yuanzhike.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://kls.jinyuanbaomall.cn

[Q63] 开启事务
来源：http://syg.xuanzx.com

START TRANSACTION;                -- 或 BEGIN
来源：http://fnd.cucudq.cn

[Q64] 提交事务
来源：http://npb.daxiang520.top

COMMIT;
来源：http://gis.andypj.xyz

[Q65] 回滚事务
来源：http://qev.ehwqpu.com

ROLLBACK;
来源：http://jax.9152youxi.cn

[Q66] 行锁查询
来源：http://xbo.yongpay.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://xhl.jinghuilouyu.cn

[Q67] 设置隔离级别
来源：http://acc.bjfxy.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://puc.yfazqb.com

[Q68] 保存点
来源：http://cqg.dashuyun.cn

SAVEPOINT sp1;
来源：http://pqq.ydjk.org.cn

ROLLBACK TO sp1;
来源：http://qpz.vqdsnc.cn

[Q69] 查看执行计划
来源：http://ppv.cashguo.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://rdz.cdnleiting.top

[Q70] 更新统计信息
来源：http://iij.gzhubu.top

ANALYZE TABLE users;
来源：http://kud.bjfxy.top

[Q71] 查看建表语句
来源：http://cry.bjfxy.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ute.yuxming.cn

[Q72] 查看索引
来源：http://hsh.quarkkingdee.top

SHOW INDEX FROM users;
来源：http://xob.tianlin.xyz

[Q73] 查看表状态
来源：http://khj.yuanzhike.top

SHOW TABLE STATUS LIKE 'users';
来源：http://nde.jqgfzy.top

[Q74] 强制使用索引
来源：http://tbq.xylfe.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://iaw.shanyushiyangkeji.top

[Q75] 日期格式化
来源：http://dxa.fengsongda.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://gjs.52xcode.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://tra.hesvh.cn

[Q76] 按天统计
来源：http://yfd.yangfankeji.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ylk.fzhhl.top

[Q77] 时间加减
来源：http://acu.yj20258888.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://kmw.vqdsnc.cn

[Q78] 当前时间
来源：http://rbp.bjfxy.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://vcm.tarul.cn

[Q79] 字符串拼接
来源：http://mzd.gzhubu.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://qcc.nanxinkj.top

[Q80] 字符串截取
来源：http://qfg.9152youxi.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://yhe.sufxvd.cn

[Q81] 字符串替换
来源：http://urs.xylfe.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://orw.fehbvm.com

[Q82] 字符长度与字节长度
来源：http://tdo.ydzc1.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://acw.c1oappe.top

[Q83] 大小写转换
来源：http://twg.snrcjt.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://uyf.jqgufenzy.top

[Q84] 去除首尾空格
来源：http://gdf.jinqigufen.top

SELECT TRIM(name) FROM users;
来源：http://xgc.jlsjyb.cn

[Q85] 数值取整
来源：http://lzo.ppjwa.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://fzv.vehdjk.com

[Q86] 读取 JSON 字段
来源：http://uuc.yj20258.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://eit.fengsongda.top

[Q87] JSON 字段做条件
来源：http://sev.shuidangran.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://zap.yanxiufei.cn

[Q88] 行转列（条件聚合）
来源：http://tmk.meibo888.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://imr.hfpthk.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://xos.fehbvm.com

[Q89] 判断表是否存在
来源：http://zbg.xinyue.icu

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://syo.ehwqpu.com

[Q90] 生成序号列
来源：http://tkv.shanyushiyangtech.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://qey.yueranfly.top

================================================================================
来源：http://ivc.yanxiufei.cn

R. Bash 专题
来源：http://iuk.hammf.cn

================================================================================
来源：http://dgm.mhx1999.top

[R01] shebang 与严格模式
来源：http://iee.xingfuxueyuan.xyz

#!/usr/bin/env bash
来源：http://eho.shanyushiyangkeji.top

set -euo pipefail
来源：http://jxt.sufxvd.cn

[R02] 变量赋值与使用
来源：http://qbl.shuidangran.top

name="Tom"; echo "$name"
来源：http://srf.sysykeji.top

[R03] 只读变量
来源：http://aix.yueranfly.top

readonly PI=3.14
来源：http://eaq.jqgufenzy.top

[R04] 位置参数
来源：http://xtr.nanxinkj.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://tvu.nanxuanxn.top

[R05] 参数默认值
来源：http://lme.0kj1m.cn

name="${1:-default}"
来源：http://nrb.dashuyun.cn

[R06] 判断命令是否存在
来源：http://peo.nanxuanxn.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://gqi.ehwqpu.com

[R07] if 判断文件
来源：http://rcg.epnwcf.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://fbd.gzhubu.top

[R08] 数值比较
来源：http://kye.cheryme.top

if (( a > b )); then echo "a 更大"; fi
来源：http://bui.yj202588.top

[R09] 字符串比较
来源：http://wwp.chenlongwang.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://vrp.sufxvd.cn

[R10] 正则匹配
来源：http://lss.hfpthk.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://vfd.ivvv.top

[R11] case 多分支
来源：http://dys.redwolf501.top

case "$1" in
来源：http://muc.cqqwz.cn

start) echo "启动" ;;
来源：http://kos.zycfv.cn

stop)  echo "停止" ;;
来源：http://ytc.zhengqikj.top

*)     echo "未知命令" ;;
来源：http://jbq.chenjidiqi.icu

esac
来源：http://yvo.nanxuanxn.top

[R12] for 遍历文件
来源：http://hmh.tian-w.cn

for f in *.txt; do echo "$f"; done
来源：http://soh.9152youxi.cn

[R13] for 计数循环
来源：http://omy.pycfn.com

for i in {1..10}; do echo "$i"; done
来源：http://owq.yongpay.top

[R14] C 风格 for
来源：http://ijc.wangshuangyany.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ble.yanxiufei.cn

[R15] while 逐行读文件
来源：http://aqq.meibo888.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://arv.fzhhl.top

[R16] until 等待条件
来源：http://pzo.fehbvm.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://tny.fanxiaobao.xyz

[R17] 数组定义与取值
来源：http://izg.xuetiantiany.cn

arr=(a b c); echo "${arr[0]}"
来源：http://wnb.fanxiaobao.xyz

[R18] 遍历数组
来源：http://cex.hesvh.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ivt.tarul.cn

[R19] 数组长度
来源：http://avu.fengsongda.top

echo "${#arr[@]}"
来源：http://gog.aibaodan.cn

[R20] 关联数组（字典）
来源：http://cqj.guowangkeji.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://afb.gogol.net.cn

[R21] 字符串长度
来源：http://qnl.chenzaomai.com

echo "${#s}"
来源：http://ibh.yangfankeji.com

[R22] 截取子串
来源：http://swn.daxiang520.top

echo "${s:0:5}"
来源：http://dre.svipenyu.cn

[R23] 字符串替换
来源：http://ixs.yfazqb.com


<!-- 参考信息 -->