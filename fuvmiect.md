代发 wailian999

[P05] 判断两个对象内容是否相等
来源：http://jht.ctjpmb.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://yaf.vqdsnc.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://qvm.vqdsnc.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://xof.jinyuanbaomall.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://csz.xingfuxueyuan.xyz

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://oaz.redwolf501.top

Go:   reflect.DeepEqual(a, b)
来源：http://gzg.smart0.xyz

Ruby: a == b
来源：http://jcy.bjfxy.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://pyj.sxryk.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://kex.9152youxi.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://qee.shangyingyoupin.top

PHP:  if (empty($x)) {}
来源：http://plo.kuanghao11.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ahh.bjfxy.top

TS:   if (x == null) {}
来源：http://rid.hywenlv.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ejw.nwbrower.top

Go:   if x == nil {}
来源：http://nhd.uphjek.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mpj.yanxiufei.cn

C#:   if (x is null) {}
来源：http://ist.shanyushiyangkeji.top

[P07] 防抖与节流
来源：http://uyg.pengpengdd.cyou

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://svy.zhixingplan.top

PHP:  // 手写时间戳比较
来源：http://vcx.xingfuxueyuan.xyz

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ggt.fanxiaobao.xyz

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tog.jinyuanbaomall.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://kpn.ivvv.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://std.yj20258.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://azj.tanke756.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ifh.0kj1m.cn

[P08] 处理浮点精度问题
来源：http://lwx.jqgfzy.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://akb.hysaishi.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://sxm.nwbrower.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://knm.vehdjk.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://lqs.havefunace.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://suz.guannengcc.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://xct.hfpthk.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://xcg.shuidangran.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://tll.yj20258.top

================================================================================
来源：http://rln.316326.xyz

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://sab.gzhubu.top

================================================================================
来源：http://uvp.tarul.cn

[Q01] 创建表
来源：http://kni.yongpay.top

CREATE TABLE users (
来源：http://ucq.cqqwz.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://fdt.jqgufenzy.top

name VARCHAR(50) NOT NULL,
来源：http://vjz.ivvv.top

email VARCHAR(100) UNIQUE,
来源：http://cyx.jinqigufen.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://yrp.nanxinkj.top

);
来源：http://kcp.hesvh.cn

[Q02] 创建带外键的表
来源：http://vkf.yongpay.top

CREATE TABLE orders (
来源：http://joq.sjlbkw.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://iie.chenlongwang.top

user_id INT NOT NULL,
来源：http://akf.gzhubu.top

amount DECIMAL(10, 2),
来源：http://zgy.hesvh.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://vlf.sufxvd.cn

);
来源：http://xtg.nanxinkj.top

[Q03] 增加列
来源：http://wbb.svipenyu.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://tcz.yvedp.cn

[Q04] 修改列类型
来源：http://zqh.wangdashe.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://bea.nanxinkj.top

[Q05] 重命名列
来源：http://xfx.zdbjq.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://qbb.cqqwz.cn

[Q06] 删除列
来源：http://zki.nwbrower.top

ALTER TABLE users DROP COLUMN age;
来源：http://gyn.zhengqikj.top

[Q07] 删除表
来源：http://omx.yj20258888.top

DROP TABLE IF EXISTS orders;
来源：http://lqq.cqqwz.cn

[Q08] 创建普通索引
来源：http://gyb.xuanzx.com

CREATE INDEX idx_users_email ON users(email);
来源：http://rbf.fanxiaobao.xyz

[Q09] 创建唯一索引
来源：http://hud.zhiwuduotai.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://pfl.hesvh.cn

[Q10] 插入单行
来源：http://rtq.yuxming.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://rtk.xziqi.cn

[Q11] 一次插入多行
来源：http://fsr.sxryk.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://myh.tarul.cn

[Q12] 插入后取自增 ID
来源：http://ieh.yj202588.top

INSERT INTO users (name) VALUES ('C');
来源：http://dwm.jqgufenzy.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://qga.hywenlv.cn

[Q13] 忽略重复插入
来源：http://eia.wangdashe.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://uin.xingfuxueyuan.xyz

[Q14] 存在则更新（upsert）
来源：http://ipp.jyoumei.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://iif.fanxiaobao.xyz

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://zwn.fengsongda.top

[Q15] 查询全部
来源：http://gsu.shuidangran.top

SELECT * FROM users;
来源：http://wbh.nanxinkj.top

[Q16] 查询指定列
来源：http://aui.hysaishi.cn

SELECT id, name FROM users;
来源：http://vwz.hnqzz.top

[Q17] 条件查询
来源：http://oyr.guowangkeji.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://jle.jyoumei.cn

[Q18] 模糊匹配
来源：http://sva.fzhhl.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://umk.jqgufenzy.top

[Q19] 范围查询
来源：http://nlj.yj20258.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://imu.kuanghao11.cn

[Q20] IN 列表
来源：http://ltt.fktsv.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ylv.jianghu66.top

[Q21] 空值判断
来源：http://poa.gogol.net.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://dlx.hnxiangtu.top

[Q22] 排序
来源：http://iwh.havefunace.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://gra.yangfankeji.com

[Q23] 分页
来源：http://moi.ywan-chungtsiang.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://nau.smart0.xyz

[Q24] 去重
来源：http://xqx.shuidangran.top

SELECT DISTINCT city FROM users;
来源：http://hjg.zhijiandao.cn

[Q25] 只取前 N 条
来源：http://jyr.yj202588.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://fib.0kj1m.cn

[Q26] 计数
来源：http://szv.uphjek.com

SELECT COUNT(*) FROM users;
来源：http://uwg.316326.xyz

[Q27] 条件计数
来源：http://twa.hysaishi.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://xmk.yonumen.top

[Q28] 求和与平均
来源：http://aca.fanxiaobao.xyz

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://enu.pycfn.com

[Q29] 最大最小值
来源：http://vfc.gaohongyu789.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://jcz.zhoulong.xyz

[Q30] 分组统计
来源：http://her.zhaomingkeji.xyz

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://vuo.jqgfzy.top

[Q31] 分组后过滤
来源：http://jbp.316326.xyz

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://dvp.birdmap.top

[Q32] 分组拼接字符串
来源：http://spd.smart0.xyz

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ned.xuanzx.com

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://iya.quarkkingdee.top

[Q33] 多列分组
来源：http://cpj.daxiang520.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://dst.xuanzx.com

[Q34] 每组取第一条
来源：http://hmo.birdmap.top

SELECT * FROM (
来源：http://tih.shanyushiyangkeji.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://rvh.jyoumei.cn

) t WHERE rn = 1;
来源：http://fsi.yanxiufei.cn

[Q35] 内连接
来源：http://pcf.nanxuanxn.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ukc.yueranfly.top

[Q36] 左连接
来源：http://rch.haohaochexian.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://clk.zhaomingkeji.xyz

[Q37] 右连接
来源：http://hbt.zhongyouzk.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://xxi.jianghu66.top

[Q38] 全外连接（PostgreSQL）
来源：http://tlg.zhoulong.xyz

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://btf.xinyue.icu

[Q39] 自连接（查上下级）
来源：http://wed.haohaochexian.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://dpw.bjfxy.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://dgj.yuxming.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://opn.redwolf501.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ntj.iojbl.cn

[Q41] 多表连接
来源：http://okz.nanxuanxn.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://qix.feifeiyinyue.top

JOIN users u ON u.id = o.user_id
来源：http://oyh.daria6918.cn

JOIN products p ON p.id = o.product_id;
来源：http://qgs.0kj1m.cn

[Q42] 连接条件附加过滤
来源：http://ljq.havefunace.top

SELECT u.name, o.amount FROM users u
来源：http://yoi.zhijiandao.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ata.hcnkem.com

[Q43] 标量子查询
来源：http://gkd.52xcode.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://tmh.hnxiangtu.top

[Q44] IN 子查询
来源：http://cne.gotoacloud.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://dls.jinyuanbaomall.cn

[Q45] EXISTS 判断存在
来源：http://mak.sysykeji.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blt.chenzaomai.com

[Q46] NOT EXISTS 判断不存在
来源：http://dyf.svipenyu.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://dtw.tarul.cn

[Q47] 与平均值比较
来源：http://dva.sysykeji.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mmh.ydjk.org.cn

[Q48] CTE 公用表表达式
来源：http://lhn.ehwqpu.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://pfc.yj20258888.top

SELECT * FROM t WHERE c > 5;
来源：http://zut.zycfv.cn

[Q49] 更新单行
来源：http://nxz.yonumen.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://tpy.tarul.cn

[Q50] 批量更新
来源：http://xiu.yangfankeji.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://lsx.bjfxy.top

[Q51] 用子查询更新
来源：http://kgb.pengpengdd.cyou

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://yai.shanyushiyangkeji.top

[Q52] 删除指定行
来源：http://fta.yanxiufei.cn

DELETE FROM users WHERE id = 10;
来源：http://vsz.haohaochexian.top

[Q53] 按条件删除
来源：http://pxc.jinqigfzy.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://lpq.ydzc1.top

[Q54] 清空表
来源：http://gxj.tarul.cn

TRUNCATE TABLE logs;
来源：http://fxw.tarul.cn

[Q55] 排名（并列占位）
来源：http://gnw.tarul.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://fcf.zdbjq.cn

[Q56] 密集排名（并列不占位）
来源：http://iof.xuanzx.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://rjo.feifeiyinyue.top

[Q57] 行号
来源：http://xab.316326.xyz

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://huf.pycfn.com

[Q58] 累计求和
来源：http://sgy.xuanzx.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://bno.ctjpmb.com

[Q59] 分组内累计
来源：http://tga.tarul.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://uij.yj20258.top

[Q60] 取上一行 / 下一行
来源：http://xxy.yueranfly.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://xia.jinqigfzy.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://vje.shanyushiyangtech.top

[Q61] 移动平均
来源：http://moq.tianlin.xyz

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blt.hywenlv.cn

[Q62] 分组占比
来源：http://qgb.52xcode.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://jbl.jianghu66.top

[Q63] 开启事务
来源：http://nao.sjlbkw.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://jeg.kuanghao11.cn

[Q64] 提交事务
来源：http://kdu.hammf.cn

COMMIT;
来源：http://eqn.ywan-chungtsiang.top

[Q65] 回滚事务
来源：http://qel.nanxuanxn.top

ROLLBACK;
来源：http://gdh.sjlbkw.cn

[Q66] 行锁查询
来源：http://pwv.sjlbkw.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://znn.yanxiufei.cn

[Q67] 设置隔离级别
来源：http://pcq.pycfn.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://rng.vqdsnc.cn

[Q68] 保存点
来源：http://cjh.yanxiufei.cn

SAVEPOINT sp1;
来源：http://wst.yj20258888.top

ROLLBACK TO sp1;
来源：http://wuo.yuanzhike.top

[Q69] 查看执行计划
来源：http://imo.yj202588.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://uqj.gotoacloud.top

[Q70] 更新统计信息
来源：http://qla.tanke756.top

ANALYZE TABLE users;
来源：http://cdr.sxryk.cn

[Q71] 查看建表语句
来源：http://wnf.bbcook.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://vbv.snrcjt.cn

[Q72] 查看索引
来源：http://ftg.jinqigfzy.top

SHOW INDEX FROM users;
来源：http://pmw.hammf.cn

[Q73] 查看表状态
来源：http://xza.zhengqikj.top

SHOW TABLE STATUS LIKE 'users';
来源：http://vvh.ctjpmb.com

[Q74] 强制使用索引
来源：http://tdi.ydjk.org.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://lxf.birdmap.top

[Q75] 日期格式化
来源：http://nty.shanyushiyangkeji.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://fnd.52xcode.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hsf.hfpthk.cn

[Q76] 按天统计
来源：http://krk.feifeiyinyue.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://rud.xuetiantiany.cn

[Q77] 时间加减
来源：http://yyv.dashuyun.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://gkr.hnxiangtu.top

[Q78] 当前时间
来源：http://ios.andypj.xyz

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://rsi.xuetiantiany.cn

[Q79] 字符串拼接
来源：http://rra.jinyuanbaomall.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://kam.yangfankeji.com

[Q80] 字符串截取
来源：http://vqg.zhongyouzk.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://yio.ivvv.top

[Q81] 字符串替换
来源：http://esv.kuanghao11.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://paz.cheryme.top

[Q82] 字符长度与字节长度
来源：http://ezc.sjlbkw.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ggq.birdmap.top

[Q83] 大小写转换
来源：http://ktb.nanxuanxn.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://rjs.zhaomingkeji.xyz

[Q84] 去除首尾空格
来源：http://bet.birdmap.top

SELECT TRIM(name) FROM users;
来源：http://kpu.kuanghao11.cn

[Q85] 数值取整
来源：http://tlm.pengpengdd.cyou

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://kqu.316326.xyz

[Q86] 读取 JSON 字段
来源：http://cqr.vehdjk.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://yqy.zhongyouzk.top

[Q87] JSON 字段做条件
来源：http://oki.yfazqb.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://bbi.jinqigfzy.top

[Q88] 行转列（条件聚合）
来源：http://wks.zhaomingkeji.xyz

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://paz.hesvh.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://eeq.yfazqb.com

[Q89] 判断表是否存在
来源：http://ucr.redwolf501.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://zqa.sufxvd.cn

[Q90] 生成序号列
来源：http://ogj.zdqjudy.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://cyj.ydzc1.top

================================================================================
来源：http://bpy.shuidangran.top

R. Bash 专题
来源：http://aiv.yangfankeji.com

================================================================================
来源：http://xof.wangdashe.top

[R01] shebang 与严格模式
来源：http://ppu.kuanghao11.cn

#!/usr/bin/env bash
来源：http://dht.fengsongda.top

set -euo pipefail
来源：http://rbi.iojbl.cn

[R02] 变量赋值与使用
来源：http://lop.gaohongyu789.top

name="Tom"; echo "$name"
来源：http://knf.yvedp.cn

[R03] 只读变量
来源：http://cqi.andypj.xyz

readonly PI=3.14
来源：http://buu.havefunace.top

[R04] 位置参数
来源：http://wls.xylfe.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ghf.wangdashe.top

[R05] 参数默认值
来源：http://two.wangdashe.top

name="${1:-default}"
来源：http://wfq.tarul.cn

[R06] 判断命令是否存在
来源：http://oun.shanyushiyangkeji.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://uhe.ivvv.top

[R07] if 判断文件
来源：http://qzh.gotoacloud.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://kcs.guowangkeji.top

[R08] 数值比较
来源：http://rij.vehdjk.com

if (( a > b )); then echo "a 更大"; fi
来源：http://qmw.shangyingyoupin.top

[R09] 字符串比较
来源：http://xdl.52xcode.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://gmo.xziqi.cn

[R10] 正则匹配
来源：http://zmv.zhoulong.xyz

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://uwg.nanxuanxn.top

[R11] case 多分支
来源：http://nyt.jinqigufen.top

case "$1" in
来源：http://iis.guannengcc.top

start) echo "启动" ;;
来源：http://xlt.feifeiyinyue.top

stop)  echo "停止" ;;
来源：http://dgd.shanyushiyangkeji.top

*)     echo "未知命令" ;;
来源：http://rif.fzhhl.top

esac
来源：http://rum.mhx1999.top

[R12] for 遍历文件
来源：http://bre.c1oappe.top

for f in *.txt; do echo "$f"; done
来源：http://pzt.chenzaomai.com

[R13] for 计数循环
来源：http://gcm.zhengqikj.top

for i in {1..10}; do echo "$i"; done
来源：http://ora.cdnleiting.top

[R14] C 风格 for
来源：http://dfq.ppjwa.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://fpi.ybcxt.top

[R15] while 逐行读文件
来源：http://bvn.c1oappe.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://adp.iojbl.cn

[R16] until 等待条件
来源：http://xqq.hywenlv.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://was.ywan-chungtsiang.top

[R17] 数组定义与取值
来源：http://qer.9152youxi.cn

arr=(a b c); echo "${arr[0]}"
来源：http://zsv.quarkkingdee.top

[R18] 遍历数组
来源：http://cna.kuanghao11.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://kup.wangshuangyany.cn

[R19] 数组长度
来源：http://iye.kuanghao11.cn

echo "${#arr[@]}"
来源：http://zuj.jinyuanbaomall.cn

[R20] 关联数组（字典）
来源：http://nra.xingfuxueyuan.xyz

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://eyb.pycfn.com

[R21] 字符串长度
来源：http://fvd.cashguo.top

echo "${#s}"
来源：http://zcm.aizwys.cn

[R22] 截取子串
来源：http://cgg.hfpthk.cn

echo "${s:0:5}"
来源：http://dkq.hammf.cn

[R23] 字符串替换
来源：http://gei.nwbrower.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://vns.cheryme.top

[R24] 大小写转换
来源：http://zcl.wangdashe.top

echo "${s^^}"; echo "${s,,}"
来源：http://ujl.zhijiandao.cn

[R25] 去后缀 / 去前缀
来源：http://jro.hnqzz.top


<!-- 参考信息 -->