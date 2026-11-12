代发 wailian999

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://bws.yj202588.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hfx.kuanghao11.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://lsv.zhoulong.xyz

PHP:  if (empty($x)) {}
来源：http://yez.yanxiufei.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://keq.nanxinkj.top

TS:   if (x == null) {}
来源：http://cje.chenzaomai.com

Java: if (x == null || x.isEmpty()) {}
来源：http://sxx.cqqwz.cn

Go:   if x == nil {}
来源：http://vik.tanke756.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ieh.haohaochexian.top

C#:   if (x is null) {}
来源：http://taw.jianghu66.top

[P07] 防抖与节流
来源：http://iab.zhiwuduotai.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://rvd.yonumen.top

PHP:  // 手写时间戳比较
来源：http://osr.hnxiangtu.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://uxk.jinghuilouyu.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zqp.ppjwa.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://apy.yuanzhike.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://fgy.sxryk.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://tmj.chenzaomai.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://jml.yangfankeji.com

[P08] 处理浮点精度问题
来源：http://lwx.daxiang520.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://nao.zhongyouzk.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://nmg.chenzaomai.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://uhd.daxiang520.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ynn.gotoacloud.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://rbv.dashuyun.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://cbk.gzhubu.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://kff.fktsv.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://fuy.zdbjq.cn

================================================================================
来源：http://yda.shangyingyoupin.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ugq.ybcxt.top

================================================================================
来源：http://tql.jinqigfzy.top

[Q01] 创建表
来源：http://cfa.zhiwuduotai.top

CREATE TABLE users (
来源：http://uaj.hcnkem.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://olg.yfazqb.com

name VARCHAR(50) NOT NULL,
来源：http://cas.mhx1999.top

email VARCHAR(100) UNIQUE,
来源：http://dgz.nanxinkj.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://glr.chenlongwang.top

);
来源：http://ipx.fehbvm.com

[Q02] 创建带外键的表
来源：http://tez.cdnleiting.top

CREATE TABLE orders (
来源：http://htx.birdmap.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://lxa.ywan-chungtsiang.top

user_id INT NOT NULL,
来源：http://fdh.zhaomingkeji.xyz

amount DECIMAL(10, 2),
来源：http://vno.shanyushiyangkeji.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://rgg.ehwqpu.com

);
来源：http://vkx.sweek.top

[Q03] 增加列
来源：http://jtz.feifeiyinyue.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://rbq.zhixingplan.top

[Q04] 修改列类型
来源：http://qhh.svipenyu.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://poh.ydzc1.top

[Q05] 重命名列
来源：http://ddh.dashuyun.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://udp.snrcjt.cn

[Q06] 删除列
来源：http://eub.pengpengdd.cyou

ALTER TABLE users DROP COLUMN age;
来源：http://ytw.yj202588.top

[Q07] 删除表
来源：http://ezz.jlsjyb.cn

DROP TABLE IF EXISTS orders;
来源：http://xlk.cheryme.top

[Q08] 创建普通索引
来源：http://ynn.shuidangran.top

CREATE INDEX idx_users_email ON users(email);
来源：http://esz.zhengqikj.top

[Q09] 创建唯一索引
来源：http://ixd.aizwys.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://zaj.jinqigfzy.top

[Q10] 插入单行
来源：http://dfr.zhiwuduotai.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://fff.yuanzhike.top

[Q11] 一次插入多行
来源：http://ssc.fzhhl.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://yqh.chenlongwang.top

[Q12] 插入后取自增 ID
来源：http://tom.smart0.xyz

INSERT INTO users (name) VALUES ('C');
来源：http://sdo.xziqi.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://frd.sjlbkw.cn

[Q13] 忽略重复插入
来源：http://qum.ivvv.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://bzg.haohaochexian.top

[Q14] 存在则更新（upsert）
来源：http://flq.ybcxt.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://jsx.ctjpmb.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://kcd.gogol.net.cn

[Q15] 查询全部
来源：http://tlo.epnwcf.com

SELECT * FROM users;
来源：http://djc.dianchejie.cn

[Q16] 查询指定列
来源：http://jkd.gzhubu.top

SELECT id, name FROM users;
来源：http://duo.yj20258888.top

[Q17] 条件查询
来源：http://dah.tanke756.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ino.zhixingplan.top

[Q18] 模糊匹配
来源：http://cwf.fehbvm.com

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ugc.hesvh.cn

[Q19] 范围查询
来源：http://zqj.ctjpmb.com

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://vha.jianghu66.top

[Q20] IN 列表
来源：http://bep.yj20258888.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://jfo.epnwcf.com

[Q21] 空值判断
来源：http://vgt.hammf.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://wwy.hnqzz.top

[Q22] 排序
来源：http://rpe.fanxiaobao.xyz

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ugq.wangshuangyany.cn

[Q23] 分页
来源：http://lov.zhongyouzk.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://xqd.shanyushiyangtech.top

[Q24] 去重
来源：http://ngr.gaohongyu789.top

SELECT DISTINCT city FROM users;
来源：http://ugl.sxryk.cn

[Q25] 只取前 N 条
来源：http://dej.ydjk.org.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mva.meibo888.top

[Q26] 计数
来源：http://zud.zhijiandao.cn

SELECT COUNT(*) FROM users;
来源：http://hqs.jinghuilouyu.cn

[Q27] 条件计数
来源：http://zin.wangshuangyany.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://euh.aibaodan.cn

[Q28] 求和与平均
来源：http://hox.shanyushiyangkeji.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://flk.chenlongwang.top

[Q29] 最大最小值
来源：http://iji.ehwqpu.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://cyw.ctjpmb.com

[Q30] 分组统计
来源：http://pnj.aizwys.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wrd.52xcode.cn

[Q31] 分组后过滤
来源：http://lov.0kj1m.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ghg.wangdashe.top

[Q32] 分组拼接字符串
来源：http://bvo.fktsv.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://lnx.bbcook.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://xkv.sysykeji.top

[Q33] 多列分组
来源：http://pvh.hesvh.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://bya.jianghu66.top

[Q34] 每组取第一条
来源：http://ypt.ywan-chungtsiang.top

SELECT * FROM (
来源：http://eyd.zdbjq.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mua.shzxlz.cn

) t WHERE rn = 1;
来源：http://ufq.epnwcf.com

[Q35] 内连接
来源：http://mwp.sjlbkw.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://nno.yuxming.cn

[Q36] 左连接
来源：http://hgx.dashuyun.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://vfg.hnxiangtu.top

[Q37] 右连接
来源：http://mvc.yongpay.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://pir.jyoumei.cn

[Q38] 全外连接（PostgreSQL）
来源：http://stz.c1oappe.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mex.zhixingplan.top

[Q39] 自连接（查上下级）
来源：http://sef.sysykeji.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://aer.fehbvm.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://lgf.smart0.xyz

[Q40] 交叉连接（笛卡尔积）
来源：http://vdr.fanxiaobao.xyz

SELECT * FROM colors CROSS JOIN sizes;
来源：http://obk.feifeiyinyue.top

[Q41] 多表连接
来源：http://quo.yuxming.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://nyb.tian-w.cn

JOIN users u ON u.id = o.user_id
来源：http://fjy.ydzc1.top

JOIN products p ON p.id = o.product_id;
来源：http://csa.haohaochexian.top

[Q42] 连接条件附加过滤
来源：http://kyh.yuxming.cn

SELECT u.name, o.amount FROM users u
来源：http://avq.ehwqpu.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ipg.birdmap.top

[Q43] 标量子查询
来源：http://eru.yongpay.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://rze.zdqjudy.top

[Q44] IN 子查询
来源：http://num.jyoumei.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://qfs.redwolf501.top

[Q45] EXISTS 判断存在
来源：http://okl.andypj.xyz

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://krs.hywenlv.cn

[Q46] NOT EXISTS 判断不存在
来源：http://fjh.nwbrower.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://iqi.sjlbkw.cn

[Q47] 与平均值比较
来源：http://icx.shanyushiyangtech.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://xgm.bjfxy.top

[Q48] CTE 公用表表达式
来源：http://xki.hnxiangtu.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://kls.epnwcf.com

SELECT * FROM t WHERE c > 5;
来源：http://fyf.zdqjudy.top

[Q49] 更新单行
来源：http://yie.shanyushiyangtech.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://gys.pycfn.com

[Q50] 批量更新
来源：http://xvv.jqgufenzy.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://pfe.xinyue.icu

[Q51] 用子查询更新
来源：http://xnp.cqqwz.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wed.nwbrower.top

[Q52] 删除指定行
来源：http://bwe.mhx1999.top

DELETE FROM users WHERE id = 10;
来源：http://uys.zhijiandao.cn

[Q53] 按条件删除
来源：http://eha.fzhhl.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://jpb.zhoulong.xyz

[Q54] 清空表
来源：http://qnv.shzxlz.cn

TRUNCATE TABLE logs;
来源：http://nes.hnxiangtu.top

[Q55] 排名（并列占位）
来源：http://ovt.svipenyu.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://cqp.9152youxi.cn

[Q56] 密集排名（并列不占位）
来源：http://boi.jqgfzy.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hlj.daxiang520.top

[Q57] 行号
来源：http://pbi.iojbl.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://bfw.ivvv.top

[Q58] 累计求和
来源：http://hkx.tarul.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://dgk.chenjidiqi.icu

[Q59] 分组内累计
来源：http://qiy.pycfn.com

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://fya.zhongyouzk.top

[Q60] 取上一行 / 下一行
来源：http://jtd.ctjpmb.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://gvu.hfpthk.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ifq.birdmap.top

[Q61] 移动平均
来源：http://tme.epnwcf.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://lgt.gogol.net.cn

[Q62] 分组占比
来源：http://ymg.quarkkingdee.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ddj.bbcook.cn

[Q63] 开启事务
来源：http://bbo.jqgufenzy.top

START TRANSACTION;                -- 或 BEGIN
来源：http://iuu.jianghu66.top

[Q64] 提交事务
来源：http://gyw.jqgufenzy.top

COMMIT;
来源：http://ujq.0kj1m.cn

[Q65] 回滚事务
来源：http://uok.chenzaomai.com

ROLLBACK;
来源：http://qot.tanke756.top

[Q66] 行锁查询
来源：http://iry.ppjwa.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://xgi.cdnleiting.top

[Q67] 设置隔离级别
来源：http://vim.fengsongda.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://cpm.zhongyouzk.top

[Q68] 保存点
来源：http://gma.andypj.xyz

SAVEPOINT sp1;
来源：http://egt.feifeiyinyue.top

ROLLBACK TO sp1;
来源：http://orx.nanxinkj.top

[Q69] 查看执行计划
来源：http://vnf.nanxinkj.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://nea.hnxiangtu.top

[Q70] 更新统计信息
来源：http://evd.ybcxt.top

ANALYZE TABLE users;
来源：http://iyi.mhx1999.top

[Q71] 查看建表语句
来源：http://cxs.cucudq.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://khz.xuetiantiany.cn

[Q72] 查看索引
来源：http://gcl.xingfuxueyuan.xyz

SHOW INDEX FROM users;
来源：http://feu.nanxinkj.top

[Q73] 查看表状态
来源：http://rtc.mhx1999.top

SHOW TABLE STATUS LIKE 'users';
来源：http://noi.nwbrower.top

[Q74] 强制使用索引
来源：http://rbc.zycfv.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://xhd.dashuyun.cn

[Q75] 日期格式化
来源：http://wlm.gotoacloud.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://epr.chenlongwang.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://aax.sysykeji.top

[Q76] 按天统计
来源：http://dyw.ybcxt.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://zgz.yongpay.top

[Q77] 时间加减
来源：http://biz.yuanzhike.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://sry.zhongyouzk.top

[Q78] 当前时间
来源：http://szt.0kj1m.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hil.jqgufenzy.top

[Q79] 字符串拼接
来源：http://jjk.xylfe.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ybp.tarul.cn

[Q80] 字符串截取
来源：http://abp.shangyingyoupin.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://szb.sysykeji.top

[Q81] 字符串替换
来源：http://xyu.quarkkingdee.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://bwq.nanxinkj.top

[Q82] 字符长度与字节长度
来源：http://blf.tarul.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wom.gogol.net.cn

[Q83] 大小写转换
来源：http://iiq.daxiang520.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://byb.fehbvm.com

[Q84] 去除首尾空格
来源：http://stz.hysaishi.cn

SELECT TRIM(name) FROM users;
来源：http://ujh.sysykeji.top

[Q85] 数值取整
来源：http://rai.hcnkem.com

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://xlv.yueranfly.top

[Q86] 读取 JSON 字段
来源：http://ash.fktsv.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ueu.hnqzz.top

[Q87] JSON 字段做条件
来源：http://esu.zdqjudy.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://lhq.xingfuxueyuan.xyz

[Q88] 行转列（条件聚合）
来源：http://brw.zdqjudy.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://cjr.xuanzx.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://aix.hcnkem.com

[Q89] 判断表是否存在
来源：http://nbi.fengsongda.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://oxn.zhengqikj.top

[Q90] 生成序号列
来源：http://wts.sufxvd.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://bia.iojbl.cn

================================================================================
来源：http://psv.zhengqikj.top

R. Bash 专题
来源：http://waw.xziqi.cn

================================================================================
来源：http://kto.gaohongyu789.top

[R01] shebang 与严格模式
来源：http://dum.zdqjudy.top

#!/usr/bin/env bash
来源：http://jvy.svipenyu.cn

set -euo pipefail
来源：http://uok.jqgufenzy.top

[R02] 变量赋值与使用
来源：http://gfw.xuanzx.com

name="Tom"; echo "$name"
来源：http://wcz.hywenlv.cn

[R03] 只读变量
来源：http://wye.jqgufenzy.top

readonly PI=3.14
来源：http://bqs.jlsjyb.cn

[R04] 位置参数
来源：http://onv.ehwqpu.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://sop.xinyue.icu

[R05] 参数默认值
来源：http://lbd.xziqi.cn

name="${1:-default}"
来源：http://tal.sjlbkw.cn

[R06] 判断命令是否存在
来源：http://fbi.cdnleiting.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://xei.ehwqpu.com

[R07] if 判断文件
来源：http://dcm.nwbrower.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ulu.shuidangran.top

[R08] 数值比较
来源：http://koa.yonumen.top

if (( a > b )); then echo "a 更大"; fi
来源：http://fxu.uphjek.com

[R09] 字符串比较
来源：http://hxx.gzhubu.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://eqx.fzhhl.top

[R10] 正则匹配
来源：http://ksy.hysaishi.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://amq.hysaishi.cn

[R11] case 多分支
来源：http://hdb.ydzc1.top

case "$1" in
来源：http://rjr.uphjek.com

start) echo "启动" ;;
来源：http://ekr.hongshengwenyu.top

stop)  echo "停止" ;;
来源：http://jli.tian-w.cn

*)     echo "未知命令" ;;
来源：http://yot.yj20258.top

esac
来源：http://yaj.meibo888.top

[R12] for 遍历文件
来源：http://xvo.hysaishi.cn

for f in *.txt; do echo "$f"; done
来源：http://tic.yuanzhike.top

[R13] for 计数循环
来源：http://ykh.zhengqikj.top

for i in {1..10}; do echo "$i"; done
来源：http://ily.hywenlv.cn

[R14] C 风格 for
来源：http://qba.feifeiyinyue.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://omd.meibo888.top

[R15] while 逐行读文件
来源：http://gww.shzxlz.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://gvm.mhx1999.top

[R16] until 等待条件
来源：http://rth.xinyue.icu

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mkq.ydjk.org.cn

[R17] 数组定义与取值
来源：http://uak.xinyue.icu

arr=(a b c); echo "${arr[0]}"
来源：http://xjg.fzhhl.top

[R18] 遍历数组
来源：http://uga.zdbjq.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://lkf.aizwys.cn

[R19] 数组长度
来源：http://isq.yangfankeji.com

echo "${#arr[@]}"
来源：http://fex.dianchejie.cn

[R20] 关联数组（字典）
来源：http://qej.haohaochexian.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://pih.gotoacloud.top

[R21] 字符串长度
来源：http://gpk.sysykeji.top

echo "${#s}"
来源：http://rls.daxiang520.top

[R22] 截取子串
来源：http://yje.xingfuxueyuan.xyz

echo "${s:0:5}"
来源：http://odb.aizwys.cn

[R23] 字符串替换
来源：http://plq.fktsv.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://xzm.chenzaomai.com

[R24] 大小写转换
来源：http://krk.cheryme.top

echo "${s^^}"; echo "${s,,}"
来源：http://vzy.chenzaomai.com

[R25] 去后缀 / 去前缀
来源：http://und.redwolf501.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://psf.nanxuanxn.top

[R26] 命令替换
来源：http://mwz.yj20258.top

now=$(date +%F); echo "$now"
来源：http://rrl.fktsv.cn

[R27] 算术展开
来源：http://oid.redwolf501.top

echo $((1 + 2 * 3))
来源：http://tpf.pengpengdd.cyou

[R28] 浮点运算
来源：http://psl.52xcode.cn

echo "scale=2; 10/3" | bc
来源：http://mcy.nwbrower.top

[R29] 定义函数
来源：http://qyd.fehbvm.com


<!-- 参考信息 -->