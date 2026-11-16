代发 wailian999

Java: list.size();  map.size();  s.length()
来源：http://vjx.fehbvm.com

Go:   len(arr);  len(m)
来源：http://pli.sjlbkw.cn

Ruby: x.length;  x.size
来源：http://rvp.ivvv.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://jpp.52xcode.cn

[P05] 判断两个对象内容是否相等
来源：http://dbk.iojbl.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://jzh.yanxiufei.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hlv.gzhubu.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://pbm.hesvh.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://skj.ydzc1.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://jvg.yonumen.top

Go:   reflect.DeepEqual(a, b)
来源：http://dqe.cucudq.cn

Ruby: a == b
来源：http://qwv.tian-w.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hen.hesvh.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://gac.pengpengdd.cyou

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://zhd.smart0.xyz

PHP:  if (empty($x)) {}
来源：http://gux.sysykeji.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://gyi.smart0.xyz

TS:   if (x == null) {}
来源：http://mcx.xuetiantiany.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://tsb.hysaishi.cn

Go:   if x == nil {}
来源：http://rmc.jqgufenzy.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ezg.hesvh.cn

C#:   if (x is null) {}
来源：http://iyg.iojbl.cn

[P07] 防抖与节流
来源：http://lif.yvedp.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://dar.andypj.xyz

PHP:  // 手写时间戳比较
来源：http://umy.ybcxt.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kgj.ybcxt.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qfb.ywan-chungtsiang.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ymz.chenlongwang.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://gwq.ydzc1.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://ede.ydzc1.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://keb.gotoacloud.top

[P08] 处理浮点精度问题
来源：http://vwh.tarul.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ddy.zhixingplan.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://pev.birdmap.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ovl.hfpthk.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://gle.bbcook.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://pnw.ywan-chungtsiang.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://fwq.sxryk.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://yei.hysaishi.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mfc.jqgfzy.top

================================================================================
来源：http://yna.jinqigufen.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://yhp.xingfuxueyuan.xyz

================================================================================
来源：http://trz.zhiwuduotai.top

[Q01] 创建表
来源：http://mot.ydzc1.top

CREATE TABLE users (
来源：http://ahb.sufxvd.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://cly.nanxinkj.top

name VARCHAR(50) NOT NULL,
来源：http://uhs.shanyushiyangtech.top

email VARCHAR(100) UNIQUE,
来源：http://gga.cqqwz.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://lwk.hywenlv.cn

);
来源：http://xkf.zhijiandao.cn

[Q02] 创建带外键的表
来源：http://nwz.jyoumei.cn

CREATE TABLE orders (
来源：http://qoq.ydzc1.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://vxg.ivvv.top

user_id INT NOT NULL,
来源：http://tng.chenzaomai.com

amount DECIMAL(10, 2),
来源：http://lzi.chenzaomai.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://rtn.hfpthk.cn

);
来源：http://gkb.fehbvm.com

[Q03] 增加列
来源：http://ctk.sufxvd.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://vmm.zdqjudy.top

[Q04] 修改列类型
来源：http://ewp.yongpay.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wnn.hnxiangtu.top

[Q05] 重命名列
来源：http://nox.sweek.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://gjf.sufxvd.cn

[Q06] 删除列
来源：http://moh.jlsjyb.cn

ALTER TABLE users DROP COLUMN age;
来源：http://iww.cucudq.cn

[Q07] 删除表
来源：http://nfr.pengpengdd.cyou

DROP TABLE IF EXISTS orders;
来源：http://cuc.shangyingyoupin.top

[Q08] 创建普通索引
来源：http://uxx.hywenlv.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://sll.meibo888.top

[Q09] 创建唯一索引
来源：http://pbb.meibo888.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://dbf.yj20258888.top

[Q10] 插入单行
来源：http://kwe.tian-w.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://cok.sjlbkw.cn

[Q11] 一次插入多行
来源：http://avw.daxiang520.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://tyr.aibaodan.cn

[Q12] 插入后取自增 ID
来源：http://oux.sysykeji.top

INSERT INTO users (name) VALUES ('C');
来源：http://ptj.jinqigfzy.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://xva.jyoumei.cn

[Q13] 忽略重复插入
来源：http://hjn.guannengcc.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://xpe.aibaodan.cn

[Q14] 存在则更新（upsert）
来源：http://gqa.hfpthk.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://qnv.ywan-chungtsiang.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://gca.havefunace.top

[Q15] 查询全部
来源：http://kzq.gaohongyu789.top

SELECT * FROM users;
来源：http://ccx.gotoacloud.top

[Q16] 查询指定列
来源：http://dju.zhengqikj.top

SELECT id, name FROM users;
来源：http://ewx.guannengcc.top

[Q17] 条件查询
来源：http://als.ywan-chungtsiang.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://pxp.pengpengdd.cyou

[Q18] 模糊匹配
来源：http://fhr.cheryme.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://iov.c1oappe.top

[Q19] 范围查询
来源：http://sze.xylfe.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://zlr.yj20258.top

[Q20] IN 列表
来源：http://pgz.mhx1999.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://bcs.xuanzx.com

[Q21] 空值判断
来源：http://ucp.aibaodan.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://njk.vehdjk.com

[Q22] 排序
来源：http://aqb.sjlbkw.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://vct.shanyushiyangkeji.top

[Q23] 分页
来源：http://ipl.zdqjudy.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://sqj.gzhubu.top

[Q24] 去重
来源：http://sda.hcnkem.com

SELECT DISTINCT city FROM users;
来源：http://deq.mhx1999.top

[Q25] 只取前 N 条
来源：http://atn.9152youxi.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://vjl.yanxiufei.cn

[Q26] 计数
来源：http://vnx.haohaochexian.top

SELECT COUNT(*) FROM users;
来源：http://jkg.bjfxy.top

[Q27] 条件计数
来源：http://bfm.feifeiyinyue.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://vwg.hfpthk.cn

[Q28] 求和与平均
来源：http://qgg.zhijiandao.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://tjm.nanxuanxn.top

[Q29] 最大最小值
来源：http://bsq.cheryme.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://owt.shuidangran.top

[Q30] 分组统计
来源：http://gwu.hywenlv.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://zve.pengpengdd.cyou

[Q31] 分组后过滤
来源：http://ohv.chenlongwang.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://kdw.yj202588.top

[Q32] 分组拼接字符串
来源：http://xjy.jqgfzy.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://pwb.316326.xyz

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://sct.c1oappe.top

[Q33] 多列分组
来源：http://rpw.yanxiufei.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://tyu.daxiang520.top

[Q34] 每组取第一条
来源：http://boq.shanyushiyangtech.top

SELECT * FROM (
来源：http://toq.fktsv.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://dtj.yuanzhike.top

) t WHERE rn = 1;
来源：http://vjs.zhengqikj.top

[Q35] 内连接
来源：http://fzs.jinyuanbaomall.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://bas.cqqwz.cn

[Q36] 左连接
来源：http://ske.vqdsnc.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://fte.fzhhl.top

[Q37] 右连接
来源：http://woa.xinyue.icu

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://vtr.hysaishi.cn

[Q38] 全外连接（PostgreSQL）
来源：http://bwc.xylfe.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://zud.hesvh.cn

[Q39] 自连接（查上下级）
来源：http://tqq.xylfe.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ypv.hysaishi.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://sne.daria6918.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://xgt.guowangkeji.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://zba.havefunace.top

[Q41] 多表连接
来源：http://sgd.havefunace.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://cqv.cheryme.top

JOIN users u ON u.id = o.user_id
来源：http://hoq.fanxiaobao.xyz

JOIN products p ON p.id = o.product_id;
来源：http://wja.sjlbkw.cn

[Q42] 连接条件附加过滤
来源：http://qlp.jinqigufen.top

SELECT u.name, o.amount FROM users u
来源：http://ght.jinqigfzy.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://zvh.cqqwz.cn

[Q43] 标量子查询
来源：http://dgl.bbcook.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ixi.yanxiufei.cn

[Q44] IN 子查询
来源：http://kup.sjlbkw.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://kmp.fktsv.cn

[Q45] EXISTS 判断存在
来源：http://wpp.sweek.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jsw.ydjk.org.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ear.316326.xyz

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://pbg.jinqigufen.top

[Q47] 与平均值比较
来源：http://fll.hywenlv.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hgs.pycfn.com

[Q48] CTE 公用表表达式
来源：http://fhc.nanxinkj.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://max.9152youxi.cn

SELECT * FROM t WHERE c > 5;
来源：http://ktg.wangshuangyany.cn

[Q49] 更新单行
来源：http://pmh.ehwqpu.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ndj.redwolf501.top

[Q50] 批量更新
来源：http://ybh.jinqigufen.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://phe.yangfankeji.com

[Q51] 用子查询更新
来源：http://spq.52xcode.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ogg.yfazqb.com

[Q52] 删除指定行
来源：http://uki.daxiang520.top

DELETE FROM users WHERE id = 10;
来源：http://sfn.birdmap.top

[Q53] 按条件删除
来源：http://pky.quarkkingdee.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ftk.birdmap.top

[Q54] 清空表
来源：http://xki.mhx1999.top

TRUNCATE TABLE logs;
来源：http://xxo.chenzaomai.com

[Q55] 排名（并列占位）
来源：http://doo.uphjek.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://che.zhongyouzk.top

[Q56] 密集排名（并列不占位）
来源：http://glt.sufxvd.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://kwd.wangshuangyany.cn

[Q57] 行号
来源：http://abx.fengsongda.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://phs.daria6918.cn

[Q58] 累计求和
来源：http://hik.yongpay.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://nch.mhx1999.top

[Q59] 分组内累计
来源：http://vrg.jqgfzy.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wve.wangshuangyany.cn

[Q60] 取上一行 / 下一行
来源：http://kvw.jinghuilouyu.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://kat.birdmap.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://gkz.pengpengdd.cyou

[Q61] 移动平均
来源：http://twq.mhx1999.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://iqk.jinghuilouyu.cn

[Q62] 分组占比
来源：http://rcu.guowangkeji.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://plt.316326.xyz

[Q63] 开启事务
来源：http://uwr.jyoumei.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://vfq.cqqwz.cn

[Q64] 提交事务
来源：http://ubn.0kj1m.cn

COMMIT;
来源：http://mqy.jinghuilouyu.cn

[Q65] 回滚事务
来源：http://qxg.daria6918.cn

ROLLBACK;
来源：http://log.ybcxt.top

[Q66] 行锁查询
来源：http://jib.nanxuanxn.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://jxr.guannengcc.top

[Q67] 设置隔离级别
来源：http://jgr.fehbvm.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://zin.sysykeji.top

[Q68] 保存点
来源：http://zgs.cashguo.top

SAVEPOINT sp1;
来源：http://zoo.zdqjudy.top

ROLLBACK TO sp1;
来源：http://evw.quarkkingdee.top

[Q69] 查看执行计划
来源：http://rvc.0kj1m.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mbh.yj20258.top

[Q70] 更新统计信息
来源：http://pnt.ivvv.top

ANALYZE TABLE users;
来源：http://ikt.yangfankeji.com

[Q71] 查看建表语句
来源：http://zjc.jinqigfzy.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://rxs.xuetiantiany.cn

[Q72] 查看索引
来源：http://jro.redwolf501.top

SHOW INDEX FROM users;
来源：http://ltf.yonumen.top

[Q73] 查看表状态
来源：http://fmx.zhaomingkeji.xyz

SHOW TABLE STATUS LIKE 'users';
来源：http://euy.nwbrower.top

[Q74] 强制使用索引
来源：http://png.shzxlz.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://rci.c1oappe.top

[Q75] 日期格式化
来源：http://igs.c1oappe.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://dar.ydjk.org.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://xso.tianlin.xyz

[Q76] 按天统计
来源：http://kfn.wangshuangyany.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://rrw.vqdsnc.cn

[Q77] 时间加减
来源：http://wlj.jinyuanbaomall.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://zaw.yueranfly.top

[Q78] 当前时间
来源：http://xuu.tarul.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://tjq.hnqzz.top

[Q79] 字符串拼接
来源：http://rhw.haohaochexian.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://gjs.svipenyu.cn

[Q80] 字符串截取
来源：http://vpo.svipenyu.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://gjp.nanxinkj.top

[Q81] 字符串替换
来源：http://sau.sufxvd.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://lvu.zycfv.cn

[Q82] 字符长度与字节长度
来源：http://fwv.zycfv.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://qkr.hesvh.cn

[Q83] 大小写转换
来源：http://mif.haohaochexian.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://cry.meibo888.top

[Q84] 去除首尾空格
来源：http://thi.nwbrower.top

SELECT TRIM(name) FROM users;
来源：http://pzy.shanyushiyangtech.top

[Q85] 数值取整
来源：http://bcd.xingfuxueyuan.xyz

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://xbr.9152youxi.cn

[Q86] 读取 JSON 字段
来源：http://kqa.ctjpmb.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://tlj.chenlongwang.top

[Q87] JSON 字段做条件
来源：http://sik.epnwcf.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://vxh.haohaochexian.top

[Q88] 行转列（条件聚合）
来源：http://ydp.cashguo.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://zza.daxiang520.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://duj.ydzc1.top

[Q89] 判断表是否存在
来源：http://zhx.aibaodan.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://jqs.jinqigfzy.top

[Q90] 生成序号列
来源：http://nnc.gzhubu.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://moe.hongshengwenyu.top

================================================================================
来源：http://zqu.xylfe.cn

R. Bash 专题
来源：http://upa.cucudq.cn

================================================================================
来源：http://hif.mhx1999.top

[R01] shebang 与严格模式
来源：http://ins.guannengcc.top

#!/usr/bin/env bash
来源：http://wgp.birdmap.top

set -euo pipefail
来源：http://olh.cheryme.top

[R02] 变量赋值与使用
来源：http://mft.zdqjudy.top

name="Tom"; echo "$name"
来源：http://nhv.sxryk.cn

[R03] 只读变量
来源：http://gns.jinghuilouyu.cn

readonly PI=3.14
来源：http://gtt.guowangkeji.top

[R04] 位置参数
来源：http://cwi.meibo888.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://fkf.sjlbkw.cn

[R05] 参数默认值
来源：http://bid.ppjwa.cn

name="${1:-default}"
来源：http://sba.cheryme.top

[R06] 判断命令是否存在
来源：http://oef.mhx1999.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ppd.yongpay.top

[R07] if 判断文件
来源：http://ryg.fanxiaobao.xyz

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://tja.jinyuanbaomall.cn

[R08] 数值比较
来源：http://cms.chenzaomai.com

if (( a > b )); then echo "a 更大"; fi
来源：http://aoj.tanke756.top

[R09] 字符串比较
来源：http://ymh.tianlin.xyz

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://shs.jiagoushi.top

[R10] 正则匹配
来源：http://lom.jianghu66.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://fge.dashuyun.cn

[R11] case 多分支
来源：http://fzf.ctjpmb.com

case "$1" in
来源：http://ssm.bjfxy.top

start) echo "启动" ;;
来源：http://wfj.epnwcf.com

stop)  echo "停止" ;;
来源：http://gvy.pengpengdd.cyou

*)     echo "未知命令" ;;
来源：http://jei.jlsjyb.cn

esac
来源：http://rzx.mhx1999.top

[R12] for 遍历文件
来源：http://lwx.52xcode.cn

for f in *.txt; do echo "$f"; done
来源：http://zts.xinyue.icu

[R13] for 计数循环
来源：http://eyc.snrcjt.cn

for i in {1..10}; do echo "$i"; done
来源：http://sbc.smart0.xyz

[R14] C 风格 for
来源：http://xrx.yongpay.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://bcp.shangyingyoupin.top

[R15] while 逐行读文件
来源：http://jik.shanyushiyangtech.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ycd.wangdashe.top

[R16] until 等待条件
来源：http://heu.yangfankeji.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://kzg.hammf.cn

[R17] 数组定义与取值
来源：http://ygc.fanxiaobao.xyz

arr=(a b c); echo "${arr[0]}"
来源：http://tqu.0kj1m.cn

[R18] 遍历数组
来源：http://kfa.c1oappe.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://kzz.hfpthk.cn

[R19] 数组长度
来源：http://fvj.fzhhl.top

echo "${#arr[@]}"
来源：http://gej.yj202588.top

[R20] 关联数组（字典）
来源：http://fsu.aizwys.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ibx.zhoulong.xyz

[R21] 字符串长度
来源：http://ugj.ppjwa.cn

echo "${#s}"
来源：http://ctg.iojbl.cn

[R22] 截取子串
来源：http://obd.yj20258.top

echo "${s:0:5}"
来源：http://xld.ybcxt.top

[R23] 字符串替换
来源：http://tya.hnxiangtu.top


<!-- 参考信息 -->