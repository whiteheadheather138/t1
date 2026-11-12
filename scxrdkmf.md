代发 wailian999

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://rel.cdnleiting.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://tna.daria6918.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://gga.zhongyouzk.top

PHP:  if (empty($x)) {}
来源：http://sgs.ctjpmb.com

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://xwj.tanke756.top

TS:   if (x == null) {}
来源：http://bye.yvedp.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ibn.tian-w.cn

Go:   if x == nil {}
来源：http://psn.jlsjyb.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://jxx.uphjek.com

C#:   if (x is null) {}
来源：http://qmc.fehbvm.com

[P07] 防抖与节流
来源：http://bak.bbcook.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://qif.zdqjudy.top

PHP:  // 手写时间戳比较
来源：http://qib.sjlbkw.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fxi.316326.xyz

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://oin.fehbvm.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://bcq.zhongyouzk.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://bvg.hongshengwenyu.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://efc.tarul.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://qvi.kuanghao11.cn

[P08] 处理浮点精度问题
来源：http://skj.daria6918.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://gct.yongpay.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://kmh.svipenyu.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://pix.smart0.xyz

TS:   (0.1 + 0.2).toFixed(2)
来源：http://umt.jyoumei.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ica.sxryk.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://cxz.jinqigfzy.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://vxf.zhengqikj.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hwf.gzhubu.top

================================================================================
来源：http://fah.xinyue.icu

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://edx.kuanghao11.cn

================================================================================
来源：http://ukm.yongpay.top

[Q01] 创建表
来源：http://mdi.tianlin.xyz

CREATE TABLE users (
来源：http://bxh.yuanzhike.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://lba.tanke756.top

name VARCHAR(50) NOT NULL,
来源：http://jev.cashguo.top

email VARCHAR(100) UNIQUE,
来源：http://rdi.dianchejie.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://rzp.yfazqb.com

);
来源：http://nkj.hongshengwenyu.top

[Q02] 创建带外键的表
来源：http://eid.fehbvm.com

CREATE TABLE orders (
来源：http://gna.yj20258.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://rhk.shuidangran.top

user_id INT NOT NULL,
来源：http://fri.cucudq.cn

amount DECIMAL(10, 2),
来源：http://axo.nwbrower.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://vle.hnqzz.top

);
来源：http://qvq.hammf.cn

[Q03] 增加列
来源：http://jqa.wangdashe.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://xly.yj202588.top

[Q04] 修改列类型
来源：http://phn.316326.xyz

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://tiz.iojbl.cn

[Q05] 重命名列
来源：http://tzt.xziqi.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ijn.andypj.xyz

[Q06] 删除列
来源：http://spc.52xcode.cn

ALTER TABLE users DROP COLUMN age;
来源：http://gul.jinqigufen.top

[Q07] 删除表
来源：http://qjr.xuetiantiany.cn

DROP TABLE IF EXISTS orders;
来源：http://ybb.yuanzhike.top

[Q08] 创建普通索引
来源：http://ogs.ppjwa.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://oxz.daria6918.cn

[Q09] 创建唯一索引
来源：http://npl.xziqi.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://opq.dashuyun.cn

[Q10] 插入单行
来源：http://wvg.havefunace.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://swd.meibo888.top

[Q11] 一次插入多行
来源：http://iqc.uphjek.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ezg.tianlin.xyz

[Q12] 插入后取自增 ID
来源：http://yot.zhiwuduotai.top

INSERT INTO users (name) VALUES ('C');
来源：http://ylr.cucudq.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://eae.jyoumei.cn

[Q13] 忽略重复插入
来源：http://spp.zhengqikj.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://zkw.shanyushiyangkeji.top

[Q14] 存在则更新（upsert）
来源：http://wbw.shuidangran.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://nfk.zhengqikj.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://pjc.kuanghao11.cn

[Q15] 查询全部
来源：http://hib.pycfn.com

SELECT * FROM users;
来源：http://yvw.shuidangran.top

[Q16] 查询指定列
来源：http://sfx.ehwqpu.com

SELECT id, name FROM users;
来源：http://mgf.hnxiangtu.top

[Q17] 条件查询
来源：http://ihb.smart0.xyz

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://cqq.cqqwz.cn

[Q18] 模糊匹配
来源：http://htg.svipenyu.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://zpt.xinyue.icu

[Q19] 范围查询
来源：http://xzs.snrcjt.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://zpg.smart0.xyz

[Q20] IN 列表
来源：http://grk.chenjidiqi.icu

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://dna.shanyushiyangtech.top

[Q21] 空值判断
来源：http://stc.hnxiangtu.top

SELECT * FROM users WHERE email IS NULL;
来源：http://ltx.gzhubu.top

[Q22] 排序
来源：http://vwt.sxryk.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://gbz.jyoumei.cn

[Q23] 分页
来源：http://tft.yj20258.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://rzz.zdbjq.cn

[Q24] 去重
来源：http://dhi.dianchejie.cn

SELECT DISTINCT city FROM users;
来源：http://uuj.aibaodan.cn

[Q25] 只取前 N 条
来源：http://lgm.ctjpmb.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://izx.tian-w.cn

[Q26] 计数
来源：http://ahh.havefunace.top

SELECT COUNT(*) FROM users;
来源：http://vsi.yuanzhike.top

[Q27] 条件计数
来源：http://wqk.andypj.xyz

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://zxd.yfazqb.com

[Q28] 求和与平均
来源：http://msx.xuanzx.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://aoc.hfpthk.cn

[Q29] 最大最小值
来源：http://khi.zhaomingkeji.xyz

SELECT MAX(age), MIN(age) FROM users;
来源：http://mue.smart0.xyz

[Q30] 分组统计
来源：http://brx.hnqzz.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://kyr.jinqigfzy.top

[Q31] 分组后过滤
来源：http://dpo.yj20258.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ikd.pengpengdd.cyou

[Q32] 分组拼接字符串
来源：http://iwq.xingfuxueyuan.xyz

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://jdx.zdbjq.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://gkp.pengpengdd.cyou

[Q33] 多列分组
来源：http://xzf.ctjpmb.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://rbi.shangyingyoupin.top

[Q34] 每组取第一条
来源：http://ocf.yongpay.top

SELECT * FROM (
来源：http://myp.c1oappe.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://zvj.shanyushiyangkeji.top

) t WHERE rn = 1;
来源：http://ofm.316326.xyz

[Q35] 内连接
来源：http://tpf.yj20258.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ebw.jiagoushi.top

[Q36] 左连接
来源：http://nac.zhixingplan.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://bwf.wangshuangyany.cn

[Q37] 右连接
来源：http://dyc.ppjwa.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://tbv.jqgufenzy.top

[Q38] 全外连接（PostgreSQL）
来源：http://cfm.jlsjyb.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://qnz.sysykeji.top

[Q39] 自连接（查上下级）
来源：http://qcf.bjfxy.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://lve.svipenyu.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://iiv.ydzc1.top

[Q40] 交叉连接（笛卡尔积）
来源：http://sut.fehbvm.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://bnx.jlsjyb.cn

[Q41] 多表连接
来源：http://lhh.nwbrower.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://cvc.redwolf501.top

JOIN users u ON u.id = o.user_id
来源：http://mri.0kj1m.cn

JOIN products p ON p.id = o.product_id;
来源：http://asa.hywenlv.cn

[Q42] 连接条件附加过滤
来源：http://eyu.iojbl.cn

SELECT u.name, o.amount FROM users u
来源：http://hcz.zhixingplan.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://rjk.hywenlv.cn

[Q43] 标量子查询
来源：http://yhg.52xcode.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://bab.zhaomingkeji.xyz

[Q44] IN 子查询
来源：http://rmh.zhijiandao.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://yby.nanxuanxn.top

[Q45] EXISTS 判断存在
来源：http://xrw.shzxlz.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://akb.cucudq.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ern.52xcode.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://god.0kj1m.cn

[Q47] 与平均值比较
来源：http://jbn.fengsongda.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://byr.tarul.cn

[Q48] CTE 公用表表达式
来源：http://qcb.jianghu66.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://zex.aibaodan.cn

SELECT * FROM t WHERE c > 5;
来源：http://mzk.jinyuanbaomall.cn

[Q49] 更新单行
来源：http://mri.chenlongwang.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://lmr.xylfe.cn

[Q50] 批量更新
来源：http://mox.nanxuanxn.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://bkw.epnwcf.com

[Q51] 用子查询更新
来源：http://vom.jiagoushi.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://vcn.yonumen.top

[Q52] 删除指定行
来源：http://lta.zhiwuduotai.top

DELETE FROM users WHERE id = 10;
来源：http://uoq.cucudq.cn

[Q53] 按条件删除
来源：http://chd.0kj1m.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://inj.chenjidiqi.icu

[Q54] 清空表
来源：http://lym.fanxiaobao.xyz

TRUNCATE TABLE logs;
来源：http://egq.pycfn.com

[Q55] 排名（并列占位）
来源：http://iiz.tianlin.xyz

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://isb.tianlin.xyz

[Q56] 密集排名（并列不占位）
来源：http://nee.tarul.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://yrg.iojbl.cn

[Q57] 行号
来源：http://mpz.cheryme.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ynz.kuanghao11.cn

[Q58] 累计求和
来源：http://frr.epnwcf.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://abx.sufxvd.cn

[Q59] 分组内累计
来源：http://czp.hongshengwenyu.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://gxw.tianlin.xyz

[Q60] 取上一行 / 下一行
来源：http://fys.shzxlz.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hly.shanyushiyangtech.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://vmv.mhx1999.top

[Q61] 移动平均
来源：http://qhl.nanxinkj.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://xmj.ydzc1.top

[Q62] 分组占比
来源：http://daf.dashuyun.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://sgy.jinqigfzy.top

[Q63] 开启事务
来源：http://uzi.ivvv.top

START TRANSACTION;                -- 或 BEGIN
来源：http://sqi.zhixingplan.top

[Q64] 提交事务
来源：http://mby.iojbl.cn

COMMIT;
来源：http://knf.hywenlv.cn

[Q65] 回滚事务
来源：http://nnw.snrcjt.cn

ROLLBACK;
来源：http://zlg.xuanzx.com

[Q66] 行锁查询
来源：http://kqo.yj202588.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hge.jinghuilouyu.cn

[Q67] 设置隔离级别
来源：http://wox.ybcxt.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://bnn.hammf.cn

[Q68] 保存点
来源：http://rvy.fanxiaobao.xyz

SAVEPOINT sp1;
来源：http://lbn.yanxiufei.cn

ROLLBACK TO sp1;
来源：http://kgf.ydjk.org.cn

[Q69] 查看执行计划
来源：http://ego.jinghuilouyu.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://fff.smart0.xyz

[Q70] 更新统计信息
来源：http://fre.bbcook.cn

ANALYZE TABLE users;
来源：http://hpn.fengsongda.top

[Q71] 查看建表语句
来源：http://gly.zhongyouzk.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://zrt.gotoacloud.top

[Q72] 查看索引
来源：http://qib.cucudq.cn

SHOW INDEX FROM users;
来源：http://lhb.birdmap.top

[Q73] 查看表状态
来源：http://kzx.sufxvd.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://avl.hongshengwenyu.top

[Q74] 强制使用索引
来源：http://opg.sjlbkw.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://qbd.fktsv.cn

[Q75] 日期格式化
来源：http://btb.dashuyun.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://qcd.hongshengwenyu.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://yvt.nanxuanxn.top

[Q76] 按天统计
来源：http://qaz.hfpthk.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://rgw.iojbl.cn

[Q77] 时间加减
来源：http://mpj.gzhubu.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://fty.bjfxy.top

[Q78] 当前时间
来源：http://bzg.ybcxt.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://pui.mhx1999.top

[Q79] 字符串拼接
来源：http://ooj.fzhhl.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://rbd.iojbl.cn

[Q80] 字符串截取
来源：http://wqc.xingfuxueyuan.xyz

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://dnd.sysykeji.top

[Q81] 字符串替换
来源：http://lvf.xuetiantiany.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://vgs.zhengqikj.top

[Q82] 字符长度与字节长度
来源：http://yqo.zhiwuduotai.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://aao.zdqjudy.top

[Q83] 大小写转换
来源：http://aql.snrcjt.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://pyq.uphjek.com

[Q84] 去除首尾空格
来源：http://qod.ppjwa.cn

SELECT TRIM(name) FROM users;
来源：http://gwf.xylfe.cn

[Q85] 数值取整
来源：http://uyn.redwolf501.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://tfr.chenzaomai.com

[Q86] 读取 JSON 字段
来源：http://ncm.zhiwuduotai.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://iif.hongshengwenyu.top

[Q87] JSON 字段做条件
来源：http://eqc.0kj1m.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://whp.zhoulong.xyz

[Q88] 行转列（条件聚合）
来源：http://kcy.havefunace.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://chk.yuanzhike.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://iie.jinqigfzy.top

[Q89] 判断表是否存在
来源：http://vgs.cheryme.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://nrw.9152youxi.cn

[Q90] 生成序号列
来源：http://uud.cucudq.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://khs.xziqi.cn

================================================================================
来源：http://ncy.jinghuilouyu.cn

R. Bash 专题
来源：http://wmd.yanxiufei.cn

================================================================================
来源：http://fwz.jqgfzy.top

[R01] shebang 与严格模式
来源：http://tfw.dianchejie.cn

#!/usr/bin/env bash
来源：http://vxx.bjfxy.top

set -euo pipefail
来源：http://yzm.ydzc1.top

[R02] 变量赋值与使用
来源：http://plv.quarkkingdee.top

name="Tom"; echo "$name"
来源：http://mft.smart0.xyz

[R03] 只读变量
来源：http://bal.yuanzhike.top

readonly PI=3.14
来源：http://qdr.yj20258.top

[R04] 位置参数
来源：http://czs.ywan-chungtsiang.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://plm.zycfv.cn

[R05] 参数默认值
来源：http://tbz.aibaodan.cn

name="${1:-default}"
来源：http://jrz.hywenlv.cn

[R06] 判断命令是否存在
来源：http://act.cashguo.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://pwk.fengsongda.top

[R07] if 判断文件
来源：http://ifj.yj20258.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://seq.316326.xyz

[R08] 数值比较
来源：http://ykx.ehwqpu.com

if (( a > b )); then echo "a 更大"; fi
来源：http://mto.sxryk.cn

[R09] 字符串比较
来源：http://mvw.sysykeji.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://beh.jinyuanbaomall.cn

[R10] 正则匹配
来源：http://fnn.yvedp.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://vie.svipenyu.cn

[R11] case 多分支
来源：http://jqv.ehwqpu.com

case "$1" in
来源：http://pzl.0kj1m.cn

start) echo "启动" ;;
来源：http://mkk.fktsv.cn

stop)  echo "停止" ;;
来源：http://pqp.hfpthk.cn

*)     echo "未知命令" ;;
来源：http://tpd.quarkkingdee.top

esac
来源：http://sey.cdnleiting.top

[R12] for 遍历文件
来源：http://vfr.wangdashe.top

for f in *.txt; do echo "$f"; done
来源：http://yum.cashguo.top

[R13] for 计数循环
来源：http://pud.gzhubu.top

for i in {1..10}; do echo "$i"; done
来源：http://zig.redwolf501.top

[R14] C 风格 for
来源：http://oya.guannengcc.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ykt.vehdjk.com

[R15] while 逐行读文件
来源：http://nkf.zhaomingkeji.xyz

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://uof.aibaodan.cn

[R16] until 等待条件
来源：http://tle.0kj1m.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://aer.fanxiaobao.xyz

[R17] 数组定义与取值
来源：http://ply.zhiwuduotai.top

arr=(a b c); echo "${arr[0]}"
来源：http://cts.ybcxt.top

[R18] 遍历数组
来源：http://jua.gzhubu.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://lbv.zhongyouzk.top

[R19] 数组长度
来源：http://yyc.shangyingyoupin.top

echo "${#arr[@]}"
来源：http://zun.tarul.cn

[R20] 关联数组（字典）
来源：http://jya.kuanghao11.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://vrl.zhijiandao.cn

[R21] 字符串长度
来源：http://ycp.redwolf501.top

echo "${#s}"
来源：http://rqr.ppjwa.cn

[R22] 截取子串
来源：http://yyd.jinqigfzy.top

echo "${s:0:5}"
来源：http://wjd.fzhhl.top

[R23] 字符串替换
来源：http://dbo.cdnleiting.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ykg.hywenlv.cn

[R24] 大小写转换
来源：http://tsy.fktsv.cn

echo "${s^^}"; echo "${s,,}"
来源：http://fzz.nanxuanxn.top

[R25] 去后缀 / 去前缀
来源：http://kzb.zhixingplan.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://acp.fktsv.cn

[R26] 命令替换
来源：http://itt.c1oappe.top

now=$(date +%F); echo "$now"
来源：http://jjw.jinyuanbaomall.cn

[R27] 算术展开
来源：http://ojl.zhongyouzk.top

echo $((1 + 2 * 3))
来源：http://uyy.vehdjk.com

[R28] 浮点运算
来源：http://rxv.yangfankeji.com

echo "scale=2; 10/3" | bc
来源：http://rev.yvedp.cn

[R29] 定义函数
来源：http://qlg.chenlongwang.top


<!-- 参考信息 -->