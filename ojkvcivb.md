代发 wailian999

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://rus.tanke756.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://lao.cdnleiting.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://tpd.sjlbkw.cn

PHP:  if (empty($x)) {}
来源：http://scv.jinyuanbaomall.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://csu.cashguo.top

TS:   if (x == null) {}
来源：http://ltk.cqqwz.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://zta.cucudq.cn

Go:   if x == nil {}
来源：http://qjc.yuxming.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://smr.mhx1999.top

C#:   if (x is null) {}
来源：http://uoi.fktsv.cn

[P07] 防抖与节流
来源：http://oir.hfpthk.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hfm.jinqigfzy.top

PHP:  // 手写时间戳比较
来源：http://jyq.chenjidiqi.icu

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xqa.daria6918.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yxf.jinqigfzy.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://bet.gotoacloud.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://psu.hywenlv.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://mem.ppjwa.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://fqv.cashguo.top

[P08] 处理浮点精度问题
来源：http://wut.ydzc1.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://see.kuanghao11.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://eba.yj202588.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://qgr.nwbrower.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hse.hysaishi.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://qgx.ywan-chungtsiang.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ahk.xylfe.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://jfm.sysykeji.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://zpj.gzhubu.top

================================================================================
来源：http://owm.fehbvm.com

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wco.guannengcc.top

================================================================================
来源：http://vjx.chenlongwang.top

[Q01] 创建表
来源：http://gcs.jinqigufen.top

CREATE TABLE users (
来源：http://pcf.jinqigufen.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wha.xziqi.cn

name VARCHAR(50) NOT NULL,
来源：http://pmu.316326.xyz

email VARCHAR(100) UNIQUE,
来源：http://ktg.0kj1m.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ghh.fengsongda.top

);
来源：http://apl.ydzc1.top

[Q02] 创建带外键的表
来源：http://mlq.fengsongda.top

CREATE TABLE orders (
来源：http://dwr.xuanzx.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://iqq.cucudq.cn

user_id INT NOT NULL,
来源：http://wcb.havefunace.top

amount DECIMAL(10, 2),
来源：http://tgw.hywenlv.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://gfx.jqgufenzy.top

);
来源：http://gjh.jinghuilouyu.cn

[Q03] 增加列
来源：http://ita.redwolf501.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://yjl.smart0.xyz

[Q04] 修改列类型
来源：http://jqs.ctjpmb.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ntw.fengsongda.top

[Q05] 重命名列
来源：http://zhw.hongshengwenyu.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hgo.ywan-chungtsiang.top

[Q06] 删除列
来源：http://qaz.nanxinkj.top

ALTER TABLE users DROP COLUMN age;
来源：http://hjr.jianghu66.top

[Q07] 删除表
来源：http://vig.chenzaomai.com

DROP TABLE IF EXISTS orders;
来源：http://dmt.daxiang520.top

[Q08] 创建普通索引
来源：http://mbz.gotoacloud.top

CREATE INDEX idx_users_email ON users(email);
来源：http://sik.haohaochexian.top

[Q09] 创建唯一索引
来源：http://diq.shzxlz.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://non.ywan-chungtsiang.top

[Q10] 插入单行
来源：http://obm.gotoacloud.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://uym.hongshengwenyu.top

[Q11] 一次插入多行
来源：http://yvf.fktsv.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://unp.ybcxt.top

[Q12] 插入后取自增 ID
来源：http://lnm.yuanzhike.top

INSERT INTO users (name) VALUES ('C');
来源：http://gmq.0kj1m.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://jtc.yanxiufei.cn

[Q13] 忽略重复插入
来源：http://njo.cheryme.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://yax.daxiang520.top

[Q14] 存在则更新（upsert）
来源：http://ffl.nanxinkj.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://bee.jinqigufen.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hqt.yangfankeji.com

[Q15] 查询全部
来源：http://clx.fengsongda.top

SELECT * FROM users;
来源：http://ujk.gogol.net.cn

[Q16] 查询指定列
来源：http://oln.nwbrower.top

SELECT id, name FROM users;
来源：http://yum.dashuyun.cn

[Q17] 条件查询
来源：http://hab.epnwcf.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://rao.mhx1999.top

[Q18] 模糊匹配
来源：http://vik.nwbrower.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ebe.uphjek.com

[Q19] 范围查询
来源：http://ajo.cheryme.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ywu.shanyushiyangtech.top

[Q20] IN 列表
来源：http://fro.quarkkingdee.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ifz.xziqi.cn

[Q21] 空值判断
来源：http://jri.chenlongwang.top

SELECT * FROM users WHERE email IS NULL;
来源：http://ndl.svipenyu.cn

[Q22] 排序
来源：http://auf.tarul.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ijy.52xcode.cn

[Q23] 分页
来源：http://crl.zhiwuduotai.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://kcj.ywan-chungtsiang.top

[Q24] 去重
来源：http://sli.zhaomingkeji.xyz

SELECT DISTINCT city FROM users;
来源：http://usg.zhengqikj.top

[Q25] 只取前 N 条
来源：http://wss.redwolf501.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://nbn.yanxiufei.cn

[Q26] 计数
来源：http://its.tanke756.top

SELECT COUNT(*) FROM users;
来源：http://hof.havefunace.top

[Q27] 条件计数
来源：http://tcm.zhiwuduotai.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://xcs.jqgufenzy.top

[Q28] 求和与平均
来源：http://mpa.fktsv.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://zth.yvedp.cn

[Q29] 最大最小值
来源：http://vrd.hnqzz.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://szy.fengsongda.top

[Q30] 分组统计
来源：http://xmr.hnqzz.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wzc.xylfe.cn

[Q31] 分组后过滤
来源：http://oct.jiagoushi.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://fph.jinyuanbaomall.cn

[Q32] 分组拼接字符串
来源：http://eyv.ppjwa.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mqr.meibo888.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mxi.hcnkem.com

[Q33] 多列分组
来源：http://hva.cqqwz.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://sdg.smart0.xyz

[Q34] 每组取第一条
来源：http://dos.nanxinkj.top

SELECT * FROM (
来源：http://gyk.c1oappe.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://lss.sweek.top

) t WHERE rn = 1;
来源：http://xtz.cashguo.top

[Q35] 内连接
来源：http://jrf.52xcode.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://jzy.quarkkingdee.top

[Q36] 左连接
来源：http://sly.zhiwuduotai.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://kso.hcnkem.com

[Q37] 右连接
来源：http://ykx.smart0.xyz

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://xxa.nwbrower.top

[Q38] 全外连接（PostgreSQL）
来源：http://rrg.yuanzhike.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ysr.ydzc1.top

[Q39] 自连接（查上下级）
来源：http://rqd.sweek.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://wez.nanxuanxn.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://xxm.vehdjk.com

[Q40] 交叉连接（笛卡尔积）
来源：http://rji.shangyingyoupin.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://diz.gogol.net.cn

[Q41] 多表连接
来源：http://ipg.zhaomingkeji.xyz

SELECT o.id, u.name, p.title FROM orders o
来源：http://wyt.feifeiyinyue.top

JOIN users u ON u.id = o.user_id
来源：http://yeq.yj202588.top

JOIN products p ON p.id = o.product_id;
来源：http://cyu.ctjpmb.com

[Q42] 连接条件附加过滤
来源：http://quw.guowangkeji.top

SELECT u.name, o.amount FROM users u
来源：http://rjo.shangyingyoupin.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ahe.yuxming.cn

[Q43] 标量子查询
来源：http://qwg.guowangkeji.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://iwq.zhixingplan.top

[Q44] IN 子查询
来源：http://cxp.tarul.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wuc.zdbjq.cn

[Q45] EXISTS 判断存在
来源：http://kyb.shangyingyoupin.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mdb.xziqi.cn

[Q46] NOT EXISTS 判断不存在
来源：http://zyw.havefunace.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://msx.aizwys.cn

[Q47] 与平均值比较
来源：http://kbd.zhixingplan.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://qye.hammf.cn

[Q48] CTE 公用表表达式
来源：http://nxi.hnqzz.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://qpi.hnqzz.top

SELECT * FROM t WHERE c > 5;
来源：http://dwg.tarul.cn

[Q49] 更新单行
来源：http://gjo.zycfv.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://uqn.zhixingplan.top

[Q50] 批量更新
来源：http://vyx.yuanzhike.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://xky.uphjek.com

[Q51] 用子查询更新
来源：http://dld.hywenlv.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://trk.kuanghao11.cn

[Q52] 删除指定行
来源：http://ayc.ppjwa.cn

DELETE FROM users WHERE id = 10;
来源：http://pes.hnqzz.top

[Q53] 按条件删除
来源：http://bfq.yangfankeji.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://roa.ywan-chungtsiang.top

[Q54] 清空表
来源：http://hfz.cheryme.top

TRUNCATE TABLE logs;
来源：http://grv.yj20258888.top

[Q55] 排名（并列占位）
来源：http://irz.epnwcf.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://kmq.zdbjq.cn

[Q56] 密集排名（并列不占位）
来源：http://bgm.epnwcf.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://vgv.jqgufenzy.top

[Q57] 行号
来源：http://xoo.pycfn.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hxt.hesvh.cn

[Q58] 累计求和
来源：http://ouf.jinghuilouyu.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://twr.xziqi.cn

[Q59] 分组内累计
来源：http://ymm.chenlongwang.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://sjg.9152youxi.cn

[Q60] 取上一行 / 下一行
来源：http://iul.jinqigufen.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://rph.ydzc1.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://vif.zdbjq.cn

[Q61] 移动平均
来源：http://ukp.xuetiantiany.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://foz.pycfn.com

[Q62] 分组占比
来源：http://glv.yangfankeji.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wdq.dianchejie.cn

[Q63] 开启事务
来源：http://sxh.gotoacloud.top

START TRANSACTION;                -- 或 BEGIN
来源：http://rsa.zhaomingkeji.xyz

[Q64] 提交事务
来源：http://jcm.jyoumei.cn

COMMIT;
来源：http://htj.xylfe.cn

[Q65] 回滚事务
来源：http://gub.iojbl.cn

ROLLBACK;
来源：http://iwy.jinghuilouyu.cn

[Q66] 行锁查询
来源：http://cuo.shuidangran.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://jnc.sxryk.cn

[Q67] 设置隔离级别
来源：http://huj.hammf.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://gty.tarul.cn

[Q68] 保存点
来源：http://tis.sufxvd.cn

SAVEPOINT sp1;
来源：http://ggu.tianlin.xyz

ROLLBACK TO sp1;
来源：http://snx.zhoulong.xyz

[Q69] 查看执行计划
来源：http://ofh.sjlbkw.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ggt.havefunace.top

[Q70] 更新统计信息
来源：http://fkj.zhengqikj.top

ANALYZE TABLE users;
来源：http://bzi.jlsjyb.cn

[Q71] 查看建表语句
来源：http://qhx.zhoulong.xyz

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://kwn.guannengcc.top

[Q72] 查看索引
来源：http://pkp.guannengcc.top

SHOW INDEX FROM users;
来源：http://fpj.ppjwa.cn

[Q73] 查看表状态
来源：http://duy.jinyuanbaomall.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://fpz.ctjpmb.com

[Q74] 强制使用索引
来源：http://nuv.wangshuangyany.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mgj.hongshengwenyu.top

[Q75] 日期格式化
来源：http://xvh.xinyue.icu

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://arn.xuetiantiany.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://uvt.zdbjq.cn

[Q76] 按天统计
来源：http://eyb.yonumen.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://twf.dianchejie.cn

[Q77] 时间加减
来源：http://dan.aibaodan.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://xig.aizwys.cn

[Q78] 当前时间
来源：http://qcs.hnxiangtu.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hjg.aibaodan.cn

[Q79] 字符串拼接
来源：http://hwb.zdqjudy.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wzg.jiagoushi.top

[Q80] 字符串截取
来源：http://wzi.52xcode.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://iiv.tian-w.cn

[Q81] 字符串替换
来源：http://opu.sysykeji.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ahf.hnxiangtu.top

[Q82] 字符长度与字节长度
来源：http://bkv.zhijiandao.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://xiw.svipenyu.cn

[Q83] 大小写转换
来源：http://mxw.fzhhl.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://eyx.andypj.xyz

[Q84] 去除首尾空格
来源：http://nuc.c1oappe.top

SELECT TRIM(name) FROM users;
来源：http://rwo.yuxming.cn

[Q85] 数值取整
来源：http://wix.feifeiyinyue.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://oqo.uphjek.com

[Q86] 读取 JSON 字段
来源：http://fvq.gotoacloud.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://dnx.fengsongda.top

[Q87] JSON 字段做条件
来源：http://jqz.fengsongda.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ffp.gaohongyu789.top

[Q88] 行转列（条件聚合）
来源：http://lec.0kj1m.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://azu.fanxiaobao.xyz

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://dtu.sysykeji.top

[Q89] 判断表是否存在
来源：http://shc.xziqi.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://bnq.svipenyu.cn

[Q90] 生成序号列
来源：http://rhz.wangshuangyany.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://sni.xylfe.cn

================================================================================
来源：http://gnl.gotoacloud.top

R. Bash 专题
来源：http://iep.svipenyu.cn

================================================================================
来源：http://lpu.ehwqpu.com

[R01] shebang 与严格模式
来源：http://nmc.yongpay.top

#!/usr/bin/env bash
来源：http://fra.jiagoushi.top

set -euo pipefail
来源：http://zgs.sysykeji.top

[R02] 变量赋值与使用
来源：http://zlg.yongpay.top

name="Tom"; echo "$name"
来源：http://iaz.pengpengdd.cyou

[R03] 只读变量
来源：http://wcp.wangdashe.top

readonly PI=3.14
来源：http://bjh.bjfxy.top

[R04] 位置参数
来源：http://eaz.ctjpmb.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://dey.ivvv.top

[R05] 参数默认值
来源：http://len.jqgufenzy.top

name="${1:-default}"
来源：http://uwu.daxiang520.top

[R06] 判断命令是否存在
来源：http://lmf.hnqzz.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://tbo.c1oappe.top

[R07] if 判断文件
来源：http://bne.fktsv.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wpm.daxiang520.top

[R08] 数值比较
来源：http://wws.ydjk.org.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://yvp.vqdsnc.cn

[R09] 字符串比较
来源：http://pps.gzhubu.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mpy.feifeiyinyue.top

[R10] 正则匹配
来源：http://gaa.zhengqikj.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wjt.xuanzx.com

[R11] case 多分支
来源：http://xip.guannengcc.top

case "$1" in
来源：http://rlt.yvedp.cn

start) echo "启动" ;;
来源：http://njk.aizwys.cn

stop)  echo "停止" ;;
来源：http://ceq.ydjk.org.cn

*)     echo "未知命令" ;;
来源：http://nxa.zhijiandao.cn

esac
来源：http://djt.jinqigfzy.top

[R12] for 遍历文件
来源：http://pgo.jinqigfzy.top

for f in *.txt; do echo "$f"; done
来源：http://vme.fehbvm.com

[R13] for 计数循环
来源：http://wgz.vqdsnc.cn

for i in {1..10}; do echo "$i"; done
来源：http://uft.jinqigufen.top

[R14] C 风格 for
来源：http://bjx.hongshengwenyu.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://nkf.nwbrower.top

[R15] while 逐行读文件
来源：http://yxj.jqgufenzy.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://iin.tanke756.top

[R16] until 等待条件
来源：http://flt.yanxiufei.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mba.yvedp.cn

[R17] 数组定义与取值
来源：http://xdm.uphjek.com

arr=(a b c); echo "${arr[0]}"
来源：http://jcq.yanxiufei.cn

[R18] 遍历数组
来源：http://bcx.birdmap.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://grl.cheryme.top

[R19] 数组长度
来源：http://til.cqqwz.cn

echo "${#arr[@]}"
来源：http://qog.jinyuanbaomall.cn

[R20] 关联数组（字典）
来源：http://toq.pycfn.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://nxs.dashuyun.cn

[R21] 字符串长度
来源：http://kev.daria6918.cn

echo "${#s}"
来源：http://ijo.hnxiangtu.top

[R22] 截取子串
来源：http://qxw.shangyingyoupin.top

echo "${s:0:5}"
来源：http://tsc.ctjpmb.com

[R23] 字符串替换
来源：http://dqp.yueranfly.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://jus.jinqigufen.top

[R24] 大小写转换
来源：http://vwr.ybcxt.top

echo "${s^^}"; echo "${s,,}"
来源：http://ned.zhongyouzk.top

[R25] 去后缀 / 去前缀
来源：http://ogr.gzhubu.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://epk.daria6918.cn

[R26] 命令替换
来源：http://def.ivvv.top

now=$(date +%F); echo "$now"
来源：http://ary.0kj1m.cn

[R27] 算术展开
来源：http://dky.zhongyouzk.top

echo $((1 + 2 * 3))
来源：http://fie.chenzaomai.com

[R28] 浮点运算
来源：http://sna.ctjpmb.com

echo "scale=2; 10/3" | bc
来源：http://szq.feifeiyinyue.top

[R29] 定义函数
来源：http://cth.epnwcf.com


<!-- 参考信息 -->