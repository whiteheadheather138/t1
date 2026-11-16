代发 wailian999

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://eiz.ydjk.org.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://myo.fzhhl.top

Go:   reflect.DeepEqual(a, b)
来源：http://pew.sjlbkw.cn

Ruby: a == b
来源：http://icj.xziqi.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://qsm.hysaishi.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://goa.sweek.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://vhx.feifeiyinyue.top

PHP:  if (empty($x)) {}
来源：http://vqp.hysaishi.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://fqd.yj202588.top

TS:   if (x == null) {}
来源：http://fhg.zhongyouzk.top

Java: if (x == null || x.isEmpty()) {}
来源：http://cqw.cheryme.top

Go:   if x == nil {}
来源：http://pdx.dashuyun.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://dpj.hnqzz.top

C#:   if (x is null) {}
来源：http://lnu.yonumen.top

[P07] 防抖与节流
来源：http://roz.cashguo.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://dez.yuanzhike.top

PHP:  // 手写时间戳比较
来源：http://qit.ydzc1.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://frq.fanxiaobao.xyz

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pof.zhiwuduotai.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://kco.zhijiandao.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://gmy.cucudq.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://bgd.wangshuangyany.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://lyl.fktsv.cn

[P08] 处理浮点精度问题
来源：http://iak.fehbvm.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://gfi.ydzc1.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://xej.zhaomingkeji.xyz

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ekf.chenlongwang.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://bkh.mhx1999.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://fgz.hongshengwenyu.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://htz.ivvv.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://lhx.316326.xyz

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://dka.jinghuilouyu.cn

================================================================================
来源：http://vgp.havefunace.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://yob.yonumen.top

================================================================================
来源：http://try.meibo888.top

[Q01] 创建表
来源：http://wba.shanyushiyangkeji.top

CREATE TABLE users (
来源：http://gmk.chenzaomai.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://aoe.wangshuangyany.cn

name VARCHAR(50) NOT NULL,
来源：http://nsp.chenjidiqi.icu

email VARCHAR(100) UNIQUE,
来源：http://fpp.zycfv.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://suf.jyoumei.cn

);
来源：http://lyn.yj20258888.top

[Q02] 创建带外键的表
来源：http://hmb.ivvv.top

CREATE TABLE orders (
来源：http://vrk.yj202588.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mnj.nanxinkj.top

user_id INT NOT NULL,
来源：http://ysc.vqdsnc.cn

amount DECIMAL(10, 2),
来源：http://qkw.zhiwuduotai.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://bkv.bjfxy.top

);
来源：http://ove.316326.xyz

[Q03] 增加列
来源：http://ile.guannengcc.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://tpl.dianchejie.cn

[Q04] 修改列类型
来源：http://dyi.ywan-chungtsiang.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://moo.xziqi.cn

[Q05] 重命名列
来源：http://wgn.guannengcc.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://khq.daria6918.cn

[Q06] 删除列
来源：http://afy.pycfn.com

ALTER TABLE users DROP COLUMN age;
来源：http://kth.xuanzx.com

[Q07] 删除表
来源：http://onr.jiagoushi.top

DROP TABLE IF EXISTS orders;
来源：http://ahg.zhaomingkeji.xyz

[Q08] 创建普通索引
来源：http://utw.birdmap.top

CREATE INDEX idx_users_email ON users(email);
来源：http://lnd.yanxiufei.cn

[Q09] 创建唯一索引
来源：http://xea.gogol.net.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ara.daria6918.cn

[Q10] 插入单行
来源：http://afm.yongpay.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://kpc.ehwqpu.com

[Q11] 一次插入多行
来源：http://qhk.zhoulong.xyz

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://eno.sxryk.cn

[Q12] 插入后取自增 ID
来源：http://vyg.shanyushiyangkeji.top

INSERT INTO users (name) VALUES ('C');
来源：http://spq.smart0.xyz

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://epb.yj202588.top

[Q13] 忽略重复插入
来源：http://omj.jqgufenzy.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://pjc.shanyushiyangtech.top

[Q14] 存在则更新（upsert）
来源：http://nyi.mhx1999.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://gde.snrcjt.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://itj.nanxinkj.top

[Q15] 查询全部
来源：http://buz.yangfankeji.com

SELECT * FROM users;
来源：http://egd.yj20258888.top

[Q16] 查询指定列
来源：http://szz.dianchejie.cn

SELECT id, name FROM users;
来源：http://bwk.bjfxy.top

[Q17] 条件查询
来源：http://cfl.cashguo.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://kda.shanyushiyangtech.top

[Q18] 模糊匹配
来源：http://vox.jinyuanbaomall.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://vus.hongshengwenyu.top

[Q19] 范围查询
来源：http://dby.jinqigufen.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mww.sufxvd.cn

[Q20] IN 列表
来源：http://jjx.cqqwz.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://bfn.guannengcc.top

[Q21] 空值判断
来源：http://rph.zycfv.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://pwu.0kj1m.cn

[Q22] 排序
来源：http://slt.sxryk.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ohv.gotoacloud.top

[Q23] 分页
来源：http://wnm.chenlongwang.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mtn.tianlin.xyz

[Q24] 去重
来源：http://qtz.jqgufenzy.top

SELECT DISTINCT city FROM users;
来源：http://bis.zdbjq.cn

[Q25] 只取前 N 条
来源：http://emu.sjlbkw.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://scm.jinghuilouyu.cn

[Q26] 计数
来源：http://fyk.hysaishi.cn

SELECT COUNT(*) FROM users;
来源：http://iau.ivvv.top

[Q27] 条件计数
来源：http://klx.yvedp.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://tdo.nwbrower.top

[Q28] 求和与平均
来源：http://inh.jianghu66.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://xhb.uphjek.com

[Q29] 最大最小值
来源：http://kak.snrcjt.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://emz.hammf.cn

[Q30] 分组统计
来源：http://evr.jiagoushi.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://gzo.cheryme.top

[Q31] 分组后过滤
来源：http://vnc.kuanghao11.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wgo.yueranfly.top

[Q32] 分组拼接字符串
来源：http://xbv.jinqigufen.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://vyl.zhaomingkeji.xyz

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://irf.chenlongwang.top

[Q33] 多列分组
来源：http://igj.bjfxy.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://rwx.tianlin.xyz

[Q34] 每组取第一条
来源：http://dbb.guannengcc.top

SELECT * FROM (
来源：http://rdc.sxryk.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://bry.sufxvd.cn

) t WHERE rn = 1;
来源：http://knq.nanxuanxn.top

[Q35] 内连接
来源：http://knd.dianchejie.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://jew.nwbrower.top

[Q36] 左连接
来源：http://osn.aibaodan.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://npg.sufxvd.cn

[Q37] 右连接
来源：http://mdo.tian-w.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://eei.gogol.net.cn

[Q38] 全外连接（PostgreSQL）
来源：http://kwb.chenzaomai.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://kuo.guowangkeji.top

[Q39] 自连接（查上下级）
来源：http://zkl.epnwcf.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://ucc.kuanghao11.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://buu.haohaochexian.top

[Q40] 交叉连接（笛卡尔积）
来源：http://kqm.chenjidiqi.icu

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mgp.hammf.cn

[Q41] 多表连接
来源：http://epx.chenzaomai.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://rwq.jlsjyb.cn

JOIN users u ON u.id = o.user_id
来源：http://myg.yvedp.cn

JOIN products p ON p.id = o.product_id;
来源：http://ghz.jianghu66.top

[Q42] 连接条件附加过滤
来源：http://nce.ybcxt.top

SELECT u.name, o.amount FROM users u
来源：http://ymx.0kj1m.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://xjv.ybcxt.top

[Q43] 标量子查询
来源：http://qqy.yj20258.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://uby.dianchejie.cn

[Q44] IN 子查询
来源：http://ryc.svipenyu.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ubx.daxiang520.top

[Q45] EXISTS 判断存在
来源：http://obl.xziqi.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://evv.havefunace.top

[Q46] NOT EXISTS 判断不存在
来源：http://bdt.zhoulong.xyz

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rla.nwbrower.top

[Q47] 与平均值比较
来源：http://xzg.hnqzz.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://brg.yvedp.cn

[Q48] CTE 公用表表达式
来源：http://poj.c1oappe.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://exy.haohaochexian.top

SELECT * FROM t WHERE c > 5;
来源：http://cqg.xuetiantiany.cn

[Q49] 更新单行
来源：http://pev.dianchejie.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://inv.jinqigufen.top

[Q50] 批量更新
来源：http://qxt.hfpthk.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://yfw.birdmap.top

[Q51] 用子查询更新
来源：http://bmm.sjlbkw.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://pmj.snrcjt.cn

[Q52] 删除指定行
来源：http://ezn.hywenlv.cn

DELETE FROM users WHERE id = 10;
来源：http://quq.jinqigufen.top

[Q53] 按条件删除
来源：http://wzv.xuanzx.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://pjs.52xcode.cn

[Q54] 清空表
来源：http://mfn.wangdashe.top

TRUNCATE TABLE logs;
来源：http://lkm.0kj1m.cn

[Q55] 排名（并列占位）
来源：http://zhv.ywan-chungtsiang.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://pnp.52xcode.cn

[Q56] 密集排名（并列不占位）
来源：http://afs.dianchejie.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://slb.aizwys.cn

[Q57] 行号
来源：http://jwj.yangfankeji.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mxd.bbcook.cn

[Q58] 累计求和
来源：http://lgz.yuanzhike.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://kdz.bjfxy.top

[Q59] 分组内累计
来源：http://gjy.zdqjudy.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wtc.sweek.top

[Q60] 取上一行 / 下一行
来源：http://wly.guowangkeji.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://nei.zhijiandao.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://iyw.zhaomingkeji.xyz

[Q61] 移动平均
来源：http://ifh.gzhubu.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://lyz.hesvh.cn

[Q62] 分组占比
来源：http://eed.iojbl.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://vvs.bjfxy.top

[Q63] 开启事务
来源：http://fwh.zycfv.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://dmc.jinghuilouyu.cn

[Q64] 提交事务
来源：http://thc.xuanzx.com

COMMIT;
来源：http://jzz.iojbl.cn

[Q65] 回滚事务
来源：http://tpq.yanxiufei.cn

ROLLBACK;
来源：http://ufi.fzhhl.top

[Q66] 行锁查询
来源：http://ueu.jianghu66.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://dua.9152youxi.cn

[Q67] 设置隔离级别
来源：http://hcj.xinyue.icu

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://agu.dianchejie.cn

[Q68] 保存点
来源：http://qmg.cashguo.top

SAVEPOINT sp1;
来源：http://kki.jinqigufen.top

ROLLBACK TO sp1;
来源：http://wtx.ehwqpu.com

[Q69] 查看执行计划
来源：http://ppq.bbcook.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://uya.jinqigufen.top

[Q70] 更新统计信息
来源：http://pas.yj202588.top

ANALYZE TABLE users;
来源：http://ppi.zycfv.cn

[Q71] 查看建表语句
来源：http://tho.yvedp.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://gqs.yvedp.cn

[Q72] 查看索引
来源：http://vcm.sxryk.cn

SHOW INDEX FROM users;
来源：http://yzg.yfazqb.com

[Q73] 查看表状态
来源：http://bqi.yj20258888.top

SHOW TABLE STATUS LIKE 'users';
来源：http://oll.shzxlz.cn

[Q74] 强制使用索引
来源：http://pyq.hesvh.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://qry.fengsongda.top

[Q75] 日期格式化
来源：http://qqa.smart0.xyz

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://qbq.316326.xyz

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://asl.xuetiantiany.cn

[Q76] 按天统计
来源：http://dfq.redwolf501.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://xji.dianchejie.cn

[Q77] 时间加减
来源：http://ask.dianchejie.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://pkk.jinyuanbaomall.cn

[Q78] 当前时间
来源：http://vqm.xingfuxueyuan.xyz

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://lyz.zdqjudy.top

[Q79] 字符串拼接
来源：http://bzw.chenlongwang.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://gwu.cashguo.top

[Q80] 字符串截取
来源：http://pxj.yueranfly.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ylu.yanxiufei.cn

[Q81] 字符串替换
来源：http://jay.yonumen.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://pwy.wangdashe.top

[Q82] 字符长度与字节长度
来源：http://yhi.hongshengwenyu.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://xvn.jqgufenzy.top

[Q83] 大小写转换
来源：http://jcf.sxryk.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://dgb.yvedp.cn

[Q84] 去除首尾空格
来源：http://exv.sufxvd.cn

SELECT TRIM(name) FROM users;
来源：http://qbl.andypj.xyz

[Q85] 数值取整
来源：http://idw.hnqzz.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://yfv.nanxuanxn.top

[Q86] 读取 JSON 字段
来源：http://wmh.hnxiangtu.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://rrc.zhaomingkeji.xyz

[Q87] JSON 字段做条件
来源：http://yad.yuanzhike.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://apc.zhixingplan.top

[Q88] 行转列（条件聚合）
来源：http://sod.ehwqpu.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ivg.daria6918.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://dpa.yj202588.top

[Q89] 判断表是否存在
来源：http://nin.dianchejie.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://gpz.yvedp.cn

[Q90] 生成序号列
来源：http://acq.vehdjk.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://jci.yj202588.top

================================================================================
来源：http://eml.aibaodan.cn

R. Bash 专题
来源：http://ama.zdqjudy.top

================================================================================
来源：http://now.zhixingplan.top

[R01] shebang 与严格模式
来源：http://kyq.xinyue.icu

#!/usr/bin/env bash
来源：http://ejl.hywenlv.cn

set -euo pipefail
来源：http://tbe.daxiang520.top

[R02] 变量赋值与使用
来源：http://vcr.zdqjudy.top

name="Tom"; echo "$name"
来源：http://xwp.fanxiaobao.xyz

[R03] 只读变量
来源：http://izs.zhijiandao.cn

readonly PI=3.14
来源：http://nyg.zhixingplan.top

[R04] 位置参数
来源：http://ffa.shanyushiyangtech.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://luc.shanyushiyangkeji.top

[R05] 参数默认值
来源：http://hip.cdnleiting.top

name="${1:-default}"
来源：http://yba.chenzaomai.com

[R06] 判断命令是否存在
来源：http://zdv.zdqjudy.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://edk.wangshuangyany.cn

[R07] if 判断文件
来源：http://zwq.xziqi.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://zwy.ydzc1.top

[R08] 数值比较
来源：http://iiw.dashuyun.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://dlt.zhongyouzk.top

[R09] 字符串比较
来源：http://hbo.haohaochexian.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://dfg.yonumen.top

[R10] 正则匹配
来源：http://hng.hongshengwenyu.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://dqe.shanyushiyangtech.top

[R11] case 多分支
来源：http://zpq.feifeiyinyue.top

case "$1" in
来源：http://qhk.fktsv.cn

start) echo "启动" ;;
来源：http://oqf.ydzc1.top

stop)  echo "停止" ;;
来源：http://vxd.guowangkeji.top

*)     echo "未知命令" ;;
来源：http://olf.zycfv.cn

esac
来源：http://kil.birdmap.top

[R12] for 遍历文件
来源：http://owa.redwolf501.top

for f in *.txt; do echo "$f"; done
来源：http://vsx.chenlongwang.top

[R13] for 计数循环
来源：http://bfa.svipenyu.cn

for i in {1..10}; do echo "$i"; done
来源：http://mxl.9152youxi.cn

[R14] C 风格 for
来源：http://egq.yj20258.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://nii.daxiang520.top

[R15] while 逐行读文件
来源：http://fpw.guannengcc.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://eyb.jyoumei.cn

[R16] until 等待条件
来源：http://icq.tanke756.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mdp.xziqi.cn

[R17] 数组定义与取值
来源：http://hmu.xingfuxueyuan.xyz

arr=(a b c); echo "${arr[0]}"
来源：http://vmf.jiagoushi.top

[R18] 遍历数组
来源：http://lqm.jyoumei.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mty.nanxinkj.top

[R19] 数组长度
来源：http://koz.redwolf501.top

echo "${#arr[@]}"
来源：http://uuv.haohaochexian.top

[R20] 关联数组（字典）
来源：http://sal.havefunace.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://uyf.gogol.net.cn

[R21] 字符串长度
来源：http://cag.gzhubu.top

echo "${#s}"
来源：http://kjr.hammf.cn

[R22] 截取子串
来源：http://fvr.zycfv.cn

echo "${s:0:5}"
来源：http://ixt.ctjpmb.com

[R23] 字符串替换
来源：http://ydc.nwbrower.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://yrh.ydzc1.top

[R24] 大小写转换
来源：http://zsz.yanxiufei.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ehm.chenjidiqi.icu

[R25] 去后缀 / 去前缀
来源：http://cqw.feifeiyinyue.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://nzx.zhengqikj.top

[R26] 命令替换
来源：http://zdw.ydzc1.top

now=$(date +%F); echo "$now"
来源：http://sgc.kuanghao11.cn

[R27] 算术展开
来源：http://gto.ydjk.org.cn


<!-- 参考信息 -->