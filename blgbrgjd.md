代发 wailian999

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://psi.yanxiufei.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ypa.sjlbkw.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ywy.hesvh.cn

Ruby: a == b
来源：http://pzz.feifeiyinyue.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ldi.hnqzz.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://vbv.cashguo.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://xcg.jinqigfzy.top

PHP:  if (empty($x)) {}
来源：http://rxk.yvedp.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://jhg.52xcode.cn

TS:   if (x == null) {}
来源：http://ikb.sysykeji.top

Java: if (x == null || x.isEmpty()) {}
来源：http://srb.chenlongwang.top

Go:   if x == nil {}
来源：http://pgl.gotoacloud.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://xkk.xylfe.cn

C#:   if (x is null) {}
来源：http://jme.cucudq.cn

[P07] 防抖与节流
来源：http://sbx.xziqi.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ocd.shzxlz.cn

PHP:  // 手写时间戳比较
来源：http://xgn.sxryk.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qdd.zhaomingkeji.xyz

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xrm.dianchejie.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://gvs.jinghuilouyu.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://srw.redwolf501.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://wvl.xingfuxueyuan.xyz

C#:   // 用 System.Timers.Timer 重置实现
来源：http://yqq.cdnleiting.top

[P08] 处理浮点精度问题
来源：http://kzj.snrcjt.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://pey.yvedp.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://pev.vqdsnc.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://lys.nwbrower.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://fyp.jinyuanbaomall.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://juq.hesvh.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ikv.xziqi.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://fjq.fktsv.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://psd.gaohongyu789.top

================================================================================
来源：http://nbq.xylfe.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://efg.yueranfly.top

================================================================================
来源：http://jho.9152youxi.cn

[Q01] 创建表
来源：http://bpq.hfpthk.cn

CREATE TABLE users (
来源：http://ktt.ydjk.org.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://vnf.ywan-chungtsiang.top

name VARCHAR(50) NOT NULL,
来源：http://bxj.ivvv.top

email VARCHAR(100) UNIQUE,
来源：http://vqh.52xcode.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wyd.chenzaomai.com

);
来源：http://riq.redwolf501.top

[Q02] 创建带外键的表
来源：http://hmf.tanke756.top

CREATE TABLE orders (
来源：http://daw.hammf.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://djt.yj20258.top

user_id INT NOT NULL,
来源：http://vni.jinghuilouyu.cn

amount DECIMAL(10, 2),
来源：http://rip.nwbrower.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://opr.yangfankeji.com

);
来源：http://qwg.xingfuxueyuan.xyz

[Q03] 增加列
来源：http://dkv.fanxiaobao.xyz

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://xsd.ydzc1.top

[Q04] 修改列类型
来源：http://vdh.vehdjk.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ovq.c1oappe.top

[Q05] 重命名列
来源：http://azr.zhengqikj.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://nbr.dashuyun.cn

[Q06] 删除列
来源：http://zhg.yj20258888.top

ALTER TABLE users DROP COLUMN age;
来源：http://qua.jinqigfzy.top

[Q07] 删除表
来源：http://nvo.jlsjyb.cn

DROP TABLE IF EXISTS orders;
来源：http://oxr.hnxiangtu.top

[Q08] 创建普通索引
来源：http://sgg.cqqwz.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://sig.bbcook.cn

[Q09] 创建唯一索引
来源：http://cge.havefunace.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://vpd.guowangkeji.top

[Q10] 插入单行
来源：http://oii.havefunace.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://iib.jinqigufen.top

[Q11] 一次插入多行
来源：http://nmd.zhaomingkeji.xyz

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hrb.ydzc1.top

[Q12] 插入后取自增 ID
来源：http://vyk.shangyingyoupin.top

INSERT INTO users (name) VALUES ('C');
来源：http://htc.zdqjudy.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://rpz.aizwys.cn

[Q13] 忽略重复插入
来源：http://fhm.gzhubu.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://qjx.xuanzx.com

[Q14] 存在则更新（upsert）
来源：http://vpo.cashguo.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://olu.bjfxy.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://sek.shanyushiyangkeji.top

[Q15] 查询全部
来源：http://vgw.vqdsnc.cn

SELECT * FROM users;
来源：http://wqd.ydjk.org.cn

[Q16] 查询指定列
来源：http://chb.snrcjt.cn

SELECT id, name FROM users;
来源：http://xer.hesvh.cn

[Q17] 条件查询
来源：http://dpn.bbcook.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://vnu.hnqzz.top

[Q18] 模糊匹配
来源：http://bec.hnxiangtu.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://rya.zhongyouzk.top

[Q19] 范围查询
来源：http://igp.xziqi.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://lfi.hywenlv.cn

[Q20] IN 列表
来源：http://elc.yfazqb.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mgo.ydzc1.top

[Q21] 空值判断
来源：http://kgb.guannengcc.top

SELECT * FROM users WHERE email IS NULL;
来源：http://dop.zhengqikj.top

[Q22] 排序
来源：http://nbn.yfazqb.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://uli.shanyushiyangtech.top

[Q23] 分页
来源：http://ocd.fengsongda.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mue.zhaomingkeji.xyz

[Q24] 去重
来源：http://bbz.zdqjudy.top

SELECT DISTINCT city FROM users;
来源：http://pik.sxryk.cn

[Q25] 只取前 N 条
来源：http://idt.xinyue.icu

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://qdc.yuxming.cn

[Q26] 计数
来源：http://cfl.zhaomingkeji.xyz

SELECT COUNT(*) FROM users;
来源：http://poy.ybcxt.top

[Q27] 条件计数
来源：http://thy.mhx1999.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://sbz.zhaomingkeji.xyz

[Q28] 求和与平均
来源：http://xsq.nwbrower.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://bfp.jinghuilouyu.cn

[Q29] 最大最小值
来源：http://gjo.guowangkeji.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://rgc.yongpay.top

[Q30] 分组统计
来源：http://sft.0kj1m.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://laz.jianghu66.top

[Q31] 分组后过滤
来源：http://fom.bjfxy.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://rmg.hcnkem.com

[Q32] 分组拼接字符串
来源：http://tfb.xingfuxueyuan.xyz

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://vlj.fehbvm.com

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://sgm.sufxvd.cn

[Q33] 多列分组
来源：http://hdd.daxiang520.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://rvq.zdqjudy.top

[Q34] 每组取第一条
来源：http://gsw.yj20258888.top

SELECT * FROM (
来源：http://vbb.cashguo.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://xps.shuidangran.top

) t WHERE rn = 1;
来源：http://ogr.9152youxi.cn

[Q35] 内连接
来源：http://axy.pengpengdd.cyou

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://csb.bbcook.cn

[Q36] 左连接
来源：http://stv.c1oappe.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://koy.tanke756.top

[Q37] 右连接
来源：http://fzi.hysaishi.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ogp.smart0.xyz

[Q38] 全外连接（PostgreSQL）
来源：http://mve.fengsongda.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wrz.jinghuilouyu.cn

[Q39] 自连接（查上下级）
来源：http://mrs.yj20258.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://lnd.jiagoushi.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wpz.chenjidiqi.icu

[Q40] 交叉连接（笛卡尔积）
来源：http://ohg.sjlbkw.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wfi.jinghuilouyu.cn

[Q41] 多表连接
来源：http://pix.zdqjudy.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://yuf.daria6918.cn

JOIN users u ON u.id = o.user_id
来源：http://cwp.tarul.cn

JOIN products p ON p.id = o.product_id;
来源：http://edn.xuetiantiany.cn

[Q42] 连接条件附加过滤
来源：http://hck.jyoumei.cn

SELECT u.name, o.amount FROM users u
来源：http://wpk.hongshengwenyu.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://rkx.zdqjudy.top

[Q43] 标量子查询
来源：http://ssf.hesvh.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wbt.vehdjk.com

[Q44] IN 子查询
来源：http://syo.shangyingyoupin.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://yws.jlsjyb.cn

[Q45] EXISTS 判断存在
来源：http://qjw.nanxuanxn.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://tar.yuanzhike.top

[Q46] NOT EXISTS 判断不存在
来源：http://fty.tanke756.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://yyf.xziqi.cn

[Q47] 与平均值比较
来源：http://szr.cdnleiting.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://awu.hnxiangtu.top

[Q48] CTE 公用表表达式
来源：http://uru.fengsongda.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mom.xuetiantiany.cn

SELECT * FROM t WHERE c > 5;
来源：http://wrf.xingfuxueyuan.xyz

[Q49] 更新单行
来源：http://rgk.xingfuxueyuan.xyz

UPDATE users SET status = 1 WHERE id = 10;
来源：http://xsf.0kj1m.cn

[Q50] 批量更新
来源：http://rbo.wangdashe.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://gyf.tian-w.cn

[Q51] 用子查询更新
来源：http://ups.feifeiyinyue.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://uvh.shzxlz.cn

[Q52] 删除指定行
来源：http://rmb.feifeiyinyue.top

DELETE FROM users WHERE id = 10;
来源：http://xav.feifeiyinyue.top

[Q53] 按条件删除
来源：http://urd.shanyushiyangtech.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://uik.zhijiandao.cn

[Q54] 清空表
来源：http://cav.chenlongwang.top

TRUNCATE TABLE logs;
来源：http://czs.cashguo.top

[Q55] 排名（并列占位）
来源：http://blu.kuanghao11.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://kse.yfazqb.com

[Q56] 密集排名（并列不占位）
来源：http://rfd.gotoacloud.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://czm.zycfv.cn

[Q57] 行号
来源：http://sli.chenlongwang.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://bxe.tarul.cn

[Q58] 累计求和
来源：http://syl.bjfxy.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://zey.shanyushiyangtech.top

[Q59] 分组内累计
来源：http://swu.xuetiantiany.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://prg.yangfankeji.com

[Q60] 取上一行 / 下一行
来源：http://pvt.tanke756.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://jik.zdqjudy.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://iut.tarul.cn

[Q61] 移动平均
来源：http://eti.tarul.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://quc.daria6918.cn

[Q62] 分组占比
来源：http://mgt.9152youxi.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wsl.bjfxy.top

[Q63] 开启事务
来源：http://lbf.c1oappe.top

START TRANSACTION;                -- 或 BEGIN
来源：http://djt.zhiwuduotai.top

[Q64] 提交事务
来源：http://sku.jqgfzy.top

COMMIT;
来源：http://ued.redwolf501.top

[Q65] 回滚事务
来源：http://agn.hammf.cn

ROLLBACK;
来源：http://ggs.chenzaomai.com

[Q66] 行锁查询
来源：http://lvd.zhoulong.xyz

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://vgy.tarul.cn

[Q67] 设置隔离级别
来源：http://hxv.fzhhl.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://jfj.fehbvm.com

[Q68] 保存点
来源：http://uza.fanxiaobao.xyz

SAVEPOINT sp1;
来源：http://mbf.yj202588.top

ROLLBACK TO sp1;
来源：http://yop.zhengqikj.top

[Q69] 查看执行计划
来源：http://fgp.ydjk.org.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://gma.jqgufenzy.top

[Q70] 更新统计信息
来源：http://zgr.iojbl.cn

ANALYZE TABLE users;
来源：http://iaw.fehbvm.com

[Q71] 查看建表语句
来源：http://baf.guowangkeji.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://eec.cqqwz.cn

[Q72] 查看索引
来源：http://uzt.aizwys.cn

SHOW INDEX FROM users;
来源：http://umc.nanxinkj.top

[Q73] 查看表状态
来源：http://mbx.guowangkeji.top

SHOW TABLE STATUS LIKE 'users';
来源：http://zxl.vehdjk.com

[Q74] 强制使用索引
来源：http://zde.fehbvm.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://kma.hysaishi.cn

[Q75] 日期格式化
来源：http://mep.uphjek.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://djl.yueranfly.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://tav.zdqjudy.top

[Q76] 按天统计
来源：http://xha.zhiwuduotai.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://utz.sysykeji.top

[Q77] 时间加减
来源：http://fcb.meibo888.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wpk.gogol.net.cn

[Q78] 当前时间
来源：http://kqx.gzhubu.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://klp.sxryk.cn

[Q79] 字符串拼接
来源：http://qjb.ydjk.org.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://quk.gaohongyu789.top

[Q80] 字符串截取
来源：http://egx.guowangkeji.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://fsk.ydjk.org.cn

[Q81] 字符串替换
来源：http://knx.aizwys.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wwz.yj202588.top

[Q82] 字符长度与字节长度
来源：http://oqp.hesvh.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ftz.jiagoushi.top

[Q83] 大小写转换
来源：http://zzc.jqgufenzy.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://sbt.daria6918.cn

[Q84] 去除首尾空格
来源：http://lij.wangdashe.top

SELECT TRIM(name) FROM users;
来源：http://xkr.yuanzhike.top

[Q85] 数值取整
来源：http://cfw.shanyushiyangkeji.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mcu.aizwys.cn

[Q86] 读取 JSON 字段
来源：http://xgi.yonumen.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://nmn.hongshengwenyu.top

[Q87] JSON 字段做条件
来源：http://ghs.cucudq.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://gtu.fanxiaobao.xyz

[Q88] 行转列（条件聚合）
来源：http://mmj.redwolf501.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://bgw.yuxming.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://eog.fengsongda.top

[Q89] 判断表是否存在
来源：http://hpg.snrcjt.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://vbt.0kj1m.cn

[Q90] 生成序号列
来源：http://ajh.shanyushiyangtech.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://guc.feifeiyinyue.top

================================================================================
来源：http://oau.xuanzx.com

R. Bash 专题
来源：http://khh.ydjk.org.cn

================================================================================
来源：http://lii.ywan-chungtsiang.top

[R01] shebang 与严格模式
来源：http://uae.zycfv.cn

#!/usr/bin/env bash
来源：http://tqw.chenjidiqi.icu

set -euo pipefail
来源：http://xrh.ivvv.top

[R02] 变量赋值与使用
来源：http://pzj.c1oappe.top

name="Tom"; echo "$name"
来源：http://ibk.cqqwz.cn

[R03] 只读变量
来源：http://bet.jinqigfzy.top

readonly PI=3.14
来源：http://una.tarul.cn

[R04] 位置参数
来源：http://pbp.yuxming.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://okl.chenzaomai.com

[R05] 参数默认值
来源：http://abk.havefunace.top

name="${1:-default}"
来源：http://uku.sjlbkw.cn

[R06] 判断命令是否存在
来源：http://btn.ehwqpu.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://nhw.yvedp.cn

[R07] if 判断文件
来源：http://igs.zdbjq.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://xzp.sufxvd.cn

[R08] 数值比较
来源：http://gcg.vqdsnc.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://gqt.epnwcf.com

[R09] 字符串比较
来源：http://okl.hnqzz.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://fsw.hammf.cn

[R10] 正则匹配
来源：http://uwa.ydzc1.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://apz.sysykeji.top

[R11] case 多分支
来源：http://dal.zycfv.cn

case "$1" in
来源：http://xgr.sweek.top

start) echo "启动" ;;
来源：http://xcm.nwbrower.top

stop)  echo "停止" ;;
来源：http://xoj.yfazqb.com

*)     echo "未知命令" ;;
来源：http://vlc.yanxiufei.cn

esac
来源：http://crj.snrcjt.cn

[R12] for 遍历文件
来源：http://mcx.yongpay.top

for f in *.txt; do echo "$f"; done
来源：http://awn.cdnleiting.top

[R13] for 计数循环
来源：http://aze.sweek.top

for i in {1..10}; do echo "$i"; done
来源：http://ulm.jinghuilouyu.cn

[R14] C 风格 for
来源：http://zdg.hfpthk.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://gxy.jinghuilouyu.cn

[R15] while 逐行读文件
来源：http://wvm.iojbl.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://qag.jinghuilouyu.cn

[R16] until 等待条件
来源：http://pex.jinghuilouyu.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ryx.redwolf501.top

[R17] 数组定义与取值
来源：http://tug.daxiang520.top

arr=(a b c); echo "${arr[0]}"
来源：http://tdn.c1oappe.top

[R18] 遍历数组
来源：http://cnt.kuanghao11.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ljm.bjfxy.top

[R19] 数组长度
来源：http://mjw.ivvv.top

echo "${#arr[@]}"
来源：http://een.haohaochexian.top

[R20] 关联数组（字典）
来源：http://dng.nanxuanxn.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://zwl.shanyushiyangtech.top

[R21] 字符串长度
来源：http://fwe.ybcxt.top

echo "${#s}"
来源：http://sji.nwbrower.top

[R22] 截取子串
来源：http://qro.ybcxt.top

echo "${s:0:5}"
来源：http://cbh.nanxinkj.top

[R23] 字符串替换
来源：http://shj.sxryk.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://icc.smart0.xyz

[R24] 大小写转换
来源：http://guc.chenjidiqi.icu

echo "${s^^}"; echo "${s,,}"
来源：http://shh.daria6918.cn

[R25] 去后缀 / 去前缀
来源：http://ynn.316326.xyz

echo "${f%.txt}"; echo "${f#./}"
来源：http://stn.daxiang520.top

[R26] 命令替换
来源：http://iaz.fengsongda.top

now=$(date +%F); echo "$now"
来源：http://psk.ppjwa.cn

[R27] 算术展开
来源：http://kph.redwolf501.top


<!-- 参考信息 -->