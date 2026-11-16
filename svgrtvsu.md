代发 wailian999

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mbq.mhx1999.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hbe.hfpthk.cn

Go:   reflect.DeepEqual(a, b)
来源：http://kvt.fzhhl.top

Ruby: a == b
来源：http://nue.bjfxy.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://dza.yuxming.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://rfb.fengsongda.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://qix.yfazqb.com

PHP:  if (empty($x)) {}
来源：http://idn.hcnkem.com

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://pie.sysykeji.top

TS:   if (x == null) {}
来源：http://cta.kuanghao11.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://gey.zhijiandao.cn

Go:   if x == nil {}
来源：http://oeq.yongpay.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mnm.xinyue.icu

C#:   if (x is null) {}
来源：http://vyi.xziqi.cn

[P07] 防抖与节流
来源：http://wph.xuanzx.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://box.shanyushiyangtech.top

PHP:  // 手写时间戳比较
来源：http://rfs.ctjpmb.com

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://frh.jyoumei.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rjf.zhoulong.xyz

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://fhn.tanke756.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hpv.yueranfly.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://okd.xingfuxueyuan.xyz

C#:   // 用 System.Timers.Timer 重置实现
来源：http://oou.hesvh.cn

[P08] 处理浮点精度问题
来源：http://zlk.sufxvd.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://dpo.ctjpmb.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://fft.snrcjt.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://biy.yfazqb.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://jhl.yanxiufei.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://cmp.sufxvd.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://zjp.mhx1999.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://sza.0kj1m.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://fpd.hesvh.cn

================================================================================
来源：http://mtp.yongpay.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wrg.chenjidiqi.icu

================================================================================
来源：http://zxw.yfazqb.com

[Q01] 创建表
来源：http://jde.jinqigfzy.top

CREATE TABLE users (
来源：http://rmc.jinghuilouyu.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://uoc.fengsongda.top

name VARCHAR(50) NOT NULL,
来源：http://dfo.c1oappe.top

email VARCHAR(100) UNIQUE,
来源：http://qag.daria6918.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://prv.0kj1m.cn

);
来源：http://ejm.daria6918.cn

[Q02] 创建带外键的表
来源：http://zlz.52xcode.cn

CREATE TABLE orders (
来源：http://bvz.c1oappe.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://csl.nanxinkj.top

user_id INT NOT NULL,
来源：http://dqj.nanxuanxn.top

amount DECIMAL(10, 2),
来源：http://dtg.pengpengdd.cyou

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://yxr.shangyingyoupin.top

);
来源：http://ple.daria6918.cn

[Q03] 增加列
来源：http://gdu.chenjidiqi.icu

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://psw.yj202588.top

[Q04] 修改列类型
来源：http://jbm.ybcxt.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://nnu.52xcode.cn

[Q05] 重命名列
来源：http://vah.52xcode.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://erb.guannengcc.top

[Q06] 删除列
来源：http://foi.tarul.cn

ALTER TABLE users DROP COLUMN age;
来源：http://xlz.nanxuanxn.top

[Q07] 删除表
来源：http://shm.yj20258888.top

DROP TABLE IF EXISTS orders;
来源：http://jan.zdbjq.cn

[Q08] 创建普通索引
来源：http://ufb.shzxlz.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://tqj.jqgfzy.top

[Q09] 创建唯一索引
来源：http://uvi.daxiang520.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://dug.tarul.cn

[Q10] 插入单行
来源：http://bcw.jyoumei.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://udl.hammf.cn

[Q11] 一次插入多行
来源：http://ldw.sysykeji.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://fbk.vehdjk.com

[Q12] 插入后取自增 ID
来源：http://acq.jqgufenzy.top

INSERT INTO users (name) VALUES ('C');
来源：http://fia.hfpthk.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://qzk.gaohongyu789.top

[Q13] 忽略重复插入
来源：http://hui.yuanzhike.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://vww.zhixingplan.top

[Q14] 存在则更新（upsert）
来源：http://brk.ydjk.org.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wcm.tarul.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://jlh.yj20258.top

[Q15] 查询全部
来源：http://vxk.yonumen.top

SELECT * FROM users;
来源：http://hvr.jyoumei.cn

[Q16] 查询指定列
来源：http://xwd.jinyuanbaomall.cn

SELECT id, name FROM users;
来源：http://bds.gaohongyu789.top

[Q17] 条件查询
来源：http://epe.guowangkeji.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://jrb.nwbrower.top

[Q18] 模糊匹配
来源：http://wnu.jlsjyb.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://zds.ydjk.org.cn

[Q19] 范围查询
来源：http://qrz.jinqigfzy.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://vva.hammf.cn

[Q20] IN 列表
来源：http://hvi.jianghu66.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://koq.gogol.net.cn

[Q21] 空值判断
来源：http://eok.ydjk.org.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ocv.daria6918.cn

[Q22] 排序
来源：http://dbe.chenlongwang.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ixb.jqgufenzy.top

[Q23] 分页
来源：http://grj.hcnkem.com

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://djf.fanxiaobao.xyz

[Q24] 去重
来源：http://aos.gogol.net.cn

SELECT DISTINCT city FROM users;
来源：http://vpg.zhengqikj.top

[Q25] 只取前 N 条
来源：http://cjo.shuidangran.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://oly.bbcook.cn

[Q26] 计数
来源：http://mad.ctjpmb.com

SELECT COUNT(*) FROM users;
来源：http://udv.chenzaomai.com

[Q27] 条件计数
来源：http://rwy.yj202588.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wue.ppjwa.cn

[Q28] 求和与平均
来源：http://zho.havefunace.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ztb.mhx1999.top

[Q29] 最大最小值
来源：http://rma.yj20258888.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://ipi.hesvh.cn

[Q30] 分组统计
来源：http://lnd.zhengqikj.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ple.jqgfzy.top

[Q31] 分组后过滤
来源：http://yux.sysykeji.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://vic.sysykeji.top

[Q32] 分组拼接字符串
来源：http://bzp.yangfankeji.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://pnb.yongpay.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://zya.cqqwz.cn

[Q33] 多列分组
来源：http://yop.hysaishi.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://lli.hywenlv.cn

[Q34] 每组取第一条
来源：http://zvd.yongpay.top

SELECT * FROM (
来源：http://wef.shanyushiyangtech.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mkh.aizwys.cn

) t WHERE rn = 1;
来源：http://fke.ppjwa.cn

[Q35] 内连接
来源：http://ciq.cdnleiting.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wih.hnxiangtu.top

[Q36] 左连接
来源：http://mms.jinqigufen.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://uqf.ydzc1.top

[Q37] 右连接
来源：http://lbg.iojbl.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://sfg.ehwqpu.com

[Q38] 全外连接（PostgreSQL）
来源：http://pmr.aizwys.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://nwi.iojbl.cn

[Q39] 自连接（查上下级）
来源：http://ohb.yj20258888.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://ymj.chenlongwang.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://jkm.ehwqpu.com

[Q40] 交叉连接（笛卡尔积）
来源：http://zvb.snrcjt.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://jmj.birdmap.top

[Q41] 多表连接
来源：http://nym.sjlbkw.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ilg.wangdashe.top

JOIN users u ON u.id = o.user_id
来源：http://zjz.iojbl.cn

JOIN products p ON p.id = o.product_id;
来源：http://zcb.hysaishi.cn

[Q42] 连接条件附加过滤
来源：http://ept.vqdsnc.cn

SELECT u.name, o.amount FROM users u
来源：http://kes.hfpthk.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mmi.ppjwa.cn

[Q43] 标量子查询
来源：http://dno.fehbvm.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://oig.pycfn.com

[Q44] IN 子查询
来源：http://mhq.meibo888.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://qos.cqqwz.cn

[Q45] EXISTS 判断存在
来源：http://afv.hnqzz.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fob.shanyushiyangtech.top

[Q46] NOT EXISTS 判断不存在
来源：http://jsg.jianghu66.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kct.jinyuanbaomall.cn

[Q47] 与平均值比较
来源：http://vpe.tianlin.xyz

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ssg.iojbl.cn

[Q48] CTE 公用表表达式
来源：http://wsz.yueranfly.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://rje.tianlin.xyz

SELECT * FROM t WHERE c > 5;
来源：http://qjx.hnxiangtu.top

[Q49] 更新单行
来源：http://ifq.52xcode.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://tdf.zdqjudy.top

[Q50] 批量更新
来源：http://cox.aibaodan.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://erf.aizwys.cn

[Q51] 用子查询更新
来源：http://odt.chenlongwang.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mjy.jqgufenzy.top

[Q52] 删除指定行
来源：http://jwq.jinyuanbaomall.cn

DELETE FROM users WHERE id = 10;
来源：http://qpz.sufxvd.cn

[Q53] 按条件删除
来源：http://moz.hysaishi.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://rrk.cdnleiting.top

[Q54] 清空表
来源：http://dvm.zhiwuduotai.top

TRUNCATE TABLE logs;
来源：http://nwt.cdnleiting.top

[Q55] 排名（并列占位）
来源：http://mwt.gogol.net.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hgq.cdnleiting.top

[Q56] 密集排名（并列不占位）
来源：http://oqy.yanxiufei.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://vwy.yanxiufei.cn

[Q57] 行号
来源：http://ezk.zhixingplan.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hoy.chenjidiqi.icu

[Q58] 累计求和
来源：http://gup.tian-w.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://sui.kuanghao11.cn

[Q59] 分组内累计
来源：http://acw.yuxming.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://xai.zhiwuduotai.top

[Q60] 取上一行 / 下一行
来源：http://frm.aizwys.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://gcz.yanxiufei.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://uvy.c1oappe.top

[Q61] 移动平均
来源：http://wwq.svipenyu.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ola.pycfn.com

[Q62] 分组占比
来源：http://lfd.0kj1m.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://dio.zhixingplan.top

[Q63] 开启事务
来源：http://qej.sweek.top

START TRANSACTION;                -- 或 BEGIN
来源：http://moy.fanxiaobao.xyz

[Q64] 提交事务
来源：http://mki.guowangkeji.top

COMMIT;
来源：http://kch.wangdashe.top

[Q65] 回滚事务
来源：http://zby.jqgfzy.top

ROLLBACK;
来源：http://zqe.cashguo.top

[Q66] 行锁查询
来源：http://veh.xuanzx.com

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://fyo.guowangkeji.top

[Q67] 设置隔离级别
来源：http://kcw.yj202588.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://sqf.jlsjyb.cn

[Q68] 保存点
来源：http://eoq.kuanghao11.cn

SAVEPOINT sp1;
来源：http://yya.yvedp.cn

ROLLBACK TO sp1;
来源：http://hud.zhoulong.xyz

[Q69] 查看执行计划
来源：http://hrd.shanyushiyangtech.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://cyi.hysaishi.cn

[Q70] 更新统计信息
来源：http://nba.cqqwz.cn

ANALYZE TABLE users;
来源：http://izc.smart0.xyz

[Q71] 查看建表语句
来源：http://nmo.vqdsnc.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://htj.ehwqpu.com

[Q72] 查看索引
来源：http://eza.yanxiufei.cn

SHOW INDEX FROM users;
来源：http://fdb.nanxinkj.top

[Q73] 查看表状态
来源：http://kbs.gogol.net.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://oin.vehdjk.com

[Q74] 强制使用索引
来源：http://qki.yonumen.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://jbh.feifeiyinyue.top

[Q75] 日期格式化
来源：http://len.bbcook.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wdc.iojbl.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://pkw.ydjk.org.cn

[Q76] 按天统计
来源：http://aeg.yonumen.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://zgp.hesvh.cn

[Q77] 时间加减
来源：http://cil.yj202588.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://xao.jiagoushi.top

[Q78] 当前时间
来源：http://mvb.bbcook.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://eqn.zhongyouzk.top

[Q79] 字符串拼接
来源：http://vbw.dianchejie.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mgu.hysaishi.cn

[Q80] 字符串截取
来源：http://mje.wangdashe.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://gnr.ppjwa.cn

[Q81] 字符串替换
来源：http://ubl.chenlongwang.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wyh.zhoulong.xyz

[Q82] 字符长度与字节长度
来源：http://ptt.smart0.xyz

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://vij.haohaochexian.top

[Q83] 大小写转换
来源：http://qlr.fanxiaobao.xyz

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ztg.ppjwa.cn

[Q84] 去除首尾空格
来源：http://npv.yj20258888.top

SELECT TRIM(name) FROM users;
来源：http://fqi.ybcxt.top

[Q85] 数值取整
来源：http://pwy.pengpengdd.cyou

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://lra.gotoacloud.top

[Q86] 读取 JSON 字段
来源：http://lqa.uphjek.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mtu.ybcxt.top

[Q87] JSON 字段做条件
来源：http://swq.cqqwz.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://phr.fzhhl.top

[Q88] 行转列（条件聚合）
来源：http://qpa.pycfn.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://gqd.gaohongyu789.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://xrp.zdbjq.cn

[Q89] 判断表是否存在
来源：http://eda.chenjidiqi.icu

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ikh.xingfuxueyuan.xyz

[Q90] 生成序号列
来源：http://hwf.yueranfly.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://muc.52xcode.cn

================================================================================
来源：http://qae.zhiwuduotai.top

R. Bash 专题
来源：http://ifo.iojbl.cn

================================================================================
来源：http://kks.zhaomingkeji.xyz

[R01] shebang 与严格模式
来源：http://aue.jlsjyb.cn

#!/usr/bin/env bash
来源：http://cqa.shanyushiyangtech.top

set -euo pipefail
来源：http://bqg.hfpthk.cn

[R02] 变量赋值与使用
来源：http://emx.yj20258.top

name="Tom"; echo "$name"
来源：http://gil.tarul.cn

[R03] 只读变量
来源：http://iiy.guannengcc.top

readonly PI=3.14
来源：http://rfs.zdbjq.cn

[R04] 位置参数
来源：http://gol.dianchejie.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://etr.jinyuanbaomall.cn

[R05] 参数默认值
来源：http://iph.smart0.xyz

name="${1:-default}"
来源：http://eud.aizwys.cn

[R06] 判断命令是否存在
来源：http://hfl.cucudq.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hdb.jinqigufen.top

[R07] if 判断文件
来源：http://nyy.xuetiantiany.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://zud.sxryk.cn

[R08] 数值比较
来源：http://jdu.yj20258888.top

if (( a > b )); then echo "a 更大"; fi
来源：http://jgi.ydjk.org.cn

[R09] 字符串比较
来源：http://fcq.cashguo.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://djx.chenlongwang.top

[R10] 正则匹配
来源：http://hnh.zdqjudy.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hxa.yj202588.top

[R11] case 多分支
来源：http://jzv.xingfuxueyuan.xyz

case "$1" in
来源：http://dhz.zdqjudy.top

start) echo "启动" ;;
来源：http://xnl.ydzc1.top

stop)  echo "停止" ;;
来源：http://ewf.zdbjq.cn

*)     echo "未知命令" ;;
来源：http://zju.hcnkem.com

esac
来源：http://ebj.aizwys.cn

[R12] for 遍历文件
来源：http://efu.zhixingplan.top

for f in *.txt; do echo "$f"; done
来源：http://xui.yvedp.cn

[R13] for 计数循环
来源：http://cbx.jqgufenzy.top

for i in {1..10}; do echo "$i"; done
来源：http://hbr.dashuyun.cn

[R14] C 风格 for
来源：http://ctg.yonumen.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mke.zhongyouzk.top

[R15] while 逐行读文件
来源：http://jei.yvedp.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://jmy.9152youxi.cn

[R16] until 等待条件
来源：http://mkt.sweek.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://jvm.birdmap.top

[R17] 数组定义与取值
来源：http://xln.tanke756.top

arr=(a b c); echo "${arr[0]}"
来源：http://wyx.tianlin.xyz

[R18] 遍历数组
来源：http://yku.sysykeji.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://rby.shangyingyoupin.top

[R19] 数组长度
来源：http://xjd.hammf.cn

echo "${#arr[@]}"
来源：http://bhp.yvedp.cn

[R20] 关联数组（字典）
来源：http://foi.wangdashe.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://fwt.pengpengdd.cyou

[R21] 字符串长度
来源：http://ipy.yuxming.cn

echo "${#s}"
来源：http://ozl.xuetiantiany.cn

[R22] 截取子串
来源：http://ezs.fanxiaobao.xyz

echo "${s:0:5}"
来源：http://ovt.zdbjq.cn

[R23] 字符串替换
来源：http://ypc.xuanzx.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hid.xylfe.cn

[R24] 大小写转换
来源：http://qsc.yfazqb.com

echo "${s^^}"; echo "${s,,}"
来源：http://fmv.zhijiandao.cn

[R25] 去后缀 / 去前缀
来源：http://iqh.zhijiandao.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://eig.zdqjudy.top

[R26] 命令替换
来源：http://mji.jinghuilouyu.cn

now=$(date +%F); echo "$now"
来源：http://hca.andypj.xyz

[R27] 算术展开
来源：http://yin.fengsongda.top


<!-- 参考信息 -->