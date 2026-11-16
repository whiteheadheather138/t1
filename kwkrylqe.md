代发 wailian999

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://bud.yanxiufei.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://jwg.xingfuxueyuan.xyz

Go:   reflect.DeepEqual(a, b)
来源：http://ygo.zhixingplan.top

Ruby: a == b
来源：http://wjg.0kj1m.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://pyg.redwolf501.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://cpj.bjfxy.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://xib.xuetiantiany.cn

PHP:  if (empty($x)) {}
来源：http://afe.hnqzz.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://sdp.yvedp.cn

TS:   if (x == null) {}
来源：http://qwo.shanyushiyangtech.top

Java: if (x == null || x.isEmpty()) {}
来源：http://qtj.fzhhl.top

Go:   if x == nil {}
来源：http://txy.jqgufenzy.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wun.yangfankeji.com

C#:   if (x is null) {}
来源：http://mha.nanxinkj.top

[P07] 防抖与节流
来源：http://lwt.yonumen.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://nju.fanxiaobao.xyz

PHP:  // 手写时间戳比较
来源：http://cnl.haohaochexian.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lqn.yuanzhike.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vlt.yuanzhike.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://azh.zhengqikj.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://kfg.kuanghao11.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://frm.epnwcf.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://nxz.daxiang520.top

[P08] 处理浮点精度问题
来源：http://ykc.aibaodan.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wvq.iojbl.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wgt.vqdsnc.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://itn.jqgfzy.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://gfz.ivvv.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://zkq.bbcook.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ybw.jlsjyb.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://zgz.fengsongda.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hlp.gzhubu.top

================================================================================
来源：http://eix.zycfv.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://abz.guowangkeji.top

================================================================================
来源：http://hbo.haohaochexian.top

[Q01] 创建表
来源：http://fbe.vehdjk.com

CREATE TABLE users (
来源：http://zia.feifeiyinyue.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://dzr.hywenlv.cn

name VARCHAR(50) NOT NULL,
来源：http://jan.vqdsnc.cn

email VARCHAR(100) UNIQUE,
来源：http://glu.hysaishi.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://pmz.gogol.net.cn

);
来源：http://fnc.fehbvm.com

[Q02] 创建带外键的表
来源：http://dvy.tianlin.xyz

CREATE TABLE orders (
来源：http://rij.nwbrower.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://cpl.fzhhl.top

user_id INT NOT NULL,
来源：http://ozn.jinyuanbaomall.cn

amount DECIMAL(10, 2),
来源：http://sly.jinyuanbaomall.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://owu.jinqigfzy.top

);
来源：http://axf.jqgufenzy.top

[Q03] 增加列
来源：http://xxn.uphjek.com

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://nvp.zhongyouzk.top

[Q04] 修改列类型
来源：http://tex.ehwqpu.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://cjc.meibo888.top

[Q05] 重命名列
来源：http://ziq.gzhubu.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://eam.pycfn.com

[Q06] 删除列
来源：http://egi.shanyushiyangkeji.top

ALTER TABLE users DROP COLUMN age;
来源：http://egg.9152youxi.cn

[Q07] 删除表
来源：http://jvv.chenlongwang.top

DROP TABLE IF EXISTS orders;
来源：http://rep.hywenlv.cn

[Q08] 创建普通索引
来源：http://vnm.fehbvm.com

CREATE INDEX idx_users_email ON users(email);
来源：http://vun.xingfuxueyuan.xyz

[Q09] 创建唯一索引
来源：http://vsm.zhijiandao.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ojo.jinghuilouyu.cn

[Q10] 插入单行
来源：http://eli.cdnleiting.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://gzy.tian-w.cn

[Q11] 一次插入多行
来源：http://ivj.zhaomingkeji.xyz

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://llw.fktsv.cn

[Q12] 插入后取自增 ID
来源：http://xio.hywenlv.cn

INSERT INTO users (name) VALUES ('C');
来源：http://hft.meibo888.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://xng.zhengqikj.top

[Q13] 忽略重复插入
来源：http://yyh.smart0.xyz

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://jdd.jinqigufen.top

[Q14] 存在则更新（upsert）
来源：http://esf.guowangkeji.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ivd.nwbrower.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://epn.fzhhl.top

[Q15] 查询全部
来源：http://dnq.yongpay.top

SELECT * FROM users;
来源：http://ttx.epnwcf.com

[Q16] 查询指定列
来源：http://ung.jinyuanbaomall.cn

SELECT id, name FROM users;
来源：http://sbn.epnwcf.com

[Q17] 条件查询
来源：http://evf.yonumen.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://khl.kuanghao11.cn

[Q18] 模糊匹配
来源：http://dwi.shangyingyoupin.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://bbj.316326.xyz

[Q19] 范围查询
来源：http://acu.daxiang520.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ach.chenzaomai.com

[Q20] IN 列表
来源：http://gci.jinqigfzy.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wbw.ybcxt.top

[Q21] 空值判断
来源：http://tov.wangshuangyany.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://dan.jinqigufen.top

[Q22] 排序
来源：http://yse.jinqigufen.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ktg.tarul.cn

[Q23] 分页
来源：http://rgx.svipenyu.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://uca.feifeiyinyue.top

[Q24] 去重
来源：http://ehl.hesvh.cn

SELECT DISTINCT city FROM users;
来源：http://nnf.chenlongwang.top

[Q25] 只取前 N 条
来源：http://mza.jiagoushi.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://efg.nwbrower.top

[Q26] 计数
来源：http://jpr.zhoulong.xyz

SELECT COUNT(*) FROM users;
来源：http://wjg.zhiwuduotai.top

[Q27] 条件计数
来源：http://oyw.shanyushiyangkeji.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://tmo.tarul.cn

[Q28] 求和与平均
来源：http://hzt.feifeiyinyue.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ehg.mhx1999.top

[Q29] 最大最小值
来源：http://mmg.andypj.xyz

SELECT MAX(age), MIN(age) FROM users;
来源：http://lmj.hfpthk.cn

[Q30] 分组统计
来源：http://iff.gotoacloud.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://jrn.yangfankeji.com

[Q31] 分组后过滤
来源：http://jsr.gotoacloud.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://sjz.316326.xyz

[Q32] 分组拼接字符串
来源：http://plu.tanke756.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://gyt.0kj1m.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://gtp.yj202588.top

[Q33] 多列分组
来源：http://gwa.uphjek.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://dkx.zhijiandao.cn

[Q34] 每组取第一条
来源：http://cjg.snrcjt.cn

SELECT * FROM (
来源：http://axt.yj20258888.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://jdc.wangdashe.top

) t WHERE rn = 1;
来源：http://tjb.ydjk.org.cn

[Q35] 内连接
来源：http://dty.ybcxt.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wmb.zdqjudy.top

[Q36] 左连接
来源：http://jhb.aizwys.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://esl.ivvv.top

[Q37] 右连接
来源：http://tit.shanyushiyangkeji.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://jpw.xuetiantiany.cn

[Q38] 全外连接（PostgreSQL）
来源：http://zfr.bjfxy.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://rnf.xuetiantiany.cn

[Q39] 自连接（查上下级）
来源：http://fdt.0kj1m.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://hgy.ywan-chungtsiang.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://tzu.epnwcf.com

[Q40] 交叉连接（笛卡尔积）
来源：http://thv.jiagoushi.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://huc.hesvh.cn

[Q41] 多表连接
来源：http://znq.shanyushiyangtech.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://cad.hongshengwenyu.top

JOIN users u ON u.id = o.user_id
来源：http://asn.xingfuxueyuan.xyz

JOIN products p ON p.id = o.product_id;
来源：http://shg.dianchejie.cn

[Q42] 连接条件附加过滤
来源：http://sxl.vqdsnc.cn

SELECT u.name, o.amount FROM users u
来源：http://wjk.jinyuanbaomall.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ygh.jinqigfzy.top

[Q43] 标量子查询
来源：http://znd.52xcode.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://bce.yuanzhike.top

[Q44] IN 子查询
来源：http://xwp.fktsv.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://vnw.kuanghao11.cn

[Q45] EXISTS 判断存在
来源：http://afj.sjlbkw.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jiw.jinqigufen.top

[Q46] NOT EXISTS 判断不存在
来源：http://rzw.vehdjk.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://cho.vqdsnc.cn

[Q47] 与平均值比较
来源：http://hhg.zhiwuduotai.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://auk.tian-w.cn

[Q48] CTE 公用表表达式
来源：http://qlq.gaohongyu789.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://vnz.chenlongwang.top

SELECT * FROM t WHERE c > 5;
来源：http://rjt.jianghu66.top

[Q49] 更新单行
来源：http://fca.nwbrower.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mii.xziqi.cn

[Q50] 批量更新
来源：http://fhl.xuetiantiany.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://pfb.shanyushiyangkeji.top

[Q51] 用子查询更新
来源：http://arj.ywan-chungtsiang.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://yet.shangyingyoupin.top

[Q52] 删除指定行
来源：http://hlo.nanxinkj.top

DELETE FROM users WHERE id = 10;
来源：http://jkw.yuanzhike.top

[Q53] 按条件删除
来源：http://fmr.ydjk.org.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://vbx.52xcode.cn

[Q54] 清空表
来源：http://nkc.sysykeji.top

TRUNCATE TABLE logs;
来源：http://pxl.dashuyun.cn

[Q55] 排名（并列占位）
来源：http://ykl.sysykeji.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ntm.hysaishi.cn

[Q56] 密集排名（并列不占位）
来源：http://eiv.xuetiantiany.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://elm.vehdjk.com

[Q57] 行号
来源：http://nzr.fengsongda.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wim.chenjidiqi.icu

[Q58] 累计求和
来源：http://slj.jiagoushi.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://yyv.gaohongyu789.top

[Q59] 分组内累计
来源：http://ikm.sysykeji.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://lqd.guowangkeji.top

[Q60] 取上一行 / 下一行
来源：http://jbb.nanxuanxn.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://til.bbcook.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://eoi.gotoacloud.top

[Q61] 移动平均
来源：http://sde.meibo888.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://cve.dianchejie.cn

[Q62] 分组占比
来源：http://jcr.zhixingplan.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hra.hywenlv.cn

[Q63] 开启事务
来源：http://qnx.nanxinkj.top

START TRANSACTION;                -- 或 BEGIN
来源：http://cay.hysaishi.cn

[Q64] 提交事务
来源：http://hue.zhengqikj.top

COMMIT;
来源：http://zew.9152youxi.cn

[Q65] 回滚事务
来源：http://bfk.sjlbkw.cn

ROLLBACK;
来源：http://rkj.hnqzz.top

[Q66] 行锁查询
来源：http://zad.wangshuangyany.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://fes.smart0.xyz

[Q67] 设置隔离级别
来源：http://let.dianchejie.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://rde.fanxiaobao.xyz

[Q68] 保存点
来源：http://zpo.9152youxi.cn

SAVEPOINT sp1;
来源：http://dgu.zdqjudy.top

ROLLBACK TO sp1;
来源：http://yhf.fengsongda.top

[Q69] 查看执行计划
来源：http://sgx.zhongyouzk.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mnp.cdnleiting.top

[Q70] 更新统计信息
来源：http://mtt.pycfn.com

ANALYZE TABLE users;
来源：http://zmg.yj202588.top

[Q71] 查看建表语句
来源：http://jqb.aizwys.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://nvj.sweek.top

[Q72] 查看索引
来源：http://nzw.316326.xyz

SHOW INDEX FROM users;
来源：http://tzd.xziqi.cn

[Q73] 查看表状态
来源：http://yyc.chenjidiqi.icu

SHOW TABLE STATUS LIKE 'users';
来源：http://onv.0kj1m.cn

[Q74] 强制使用索引
来源：http://vvv.hammf.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://brq.jiagoushi.top

[Q75] 日期格式化
来源：http://wvy.nanxinkj.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wex.shuidangran.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://vwd.cheryme.top

[Q76] 按天统计
来源：http://oxj.jinqigfzy.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://kfz.ehwqpu.com

[Q77] 时间加减
来源：http://iwy.sweek.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://psb.zhijiandao.cn

[Q78] 当前时间
来源：http://bnz.jqgufenzy.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mmv.yvedp.cn

[Q79] 字符串拼接
来源：http://hel.52xcode.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://pwa.sufxvd.cn

[Q80] 字符串截取
来源：http://gvn.jqgufenzy.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://afl.shanyushiyangtech.top

[Q81] 字符串替换
来源：http://qqb.jinyuanbaomall.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://bwn.yueranfly.top

[Q82] 字符长度与字节长度
来源：http://flg.ctjpmb.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://svd.yonumen.top

[Q83] 大小写转换
来源：http://adz.iojbl.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ywi.mhx1999.top

[Q84] 去除首尾空格
来源：http://fot.svipenyu.cn

SELECT TRIM(name) FROM users;
来源：http://wkp.hysaishi.cn

[Q85] 数值取整
来源：http://msa.hnqzz.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://tas.pycfn.com

[Q86] 读取 JSON 字段
来源：http://gzh.zdbjq.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://xxa.gogol.net.cn

[Q87] JSON 字段做条件
来源：http://slb.shuidangran.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hfu.dianchejie.cn

[Q88] 行转列（条件聚合）
来源：http://ikl.yj202588.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mql.aibaodan.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://dvs.nwbrower.top

[Q89] 判断表是否存在
来源：http://ncj.zhaomingkeji.xyz

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://tay.pengpengdd.cyou

[Q90] 生成序号列
来源：http://lel.shuidangran.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://nbo.cucudq.cn

================================================================================
来源：http://btz.redwolf501.top

R. Bash 专题
来源：http://awy.zdbjq.cn

================================================================================
来源：http://tim.quarkkingdee.top

[R01] shebang 与严格模式
来源：http://fxx.xingfuxueyuan.xyz

#!/usr/bin/env bash
来源：http://frh.fengsongda.top

set -euo pipefail
来源：http://elu.cdnleiting.top

[R02] 变量赋值与使用
来源：http://ivz.chenlongwang.top

name="Tom"; echo "$name"
来源：http://ajn.svipenyu.cn

[R03] 只读变量
来源：http://yeq.nanxinkj.top

readonly PI=3.14
来源：http://hzh.xylfe.cn

[R04] 位置参数
来源：http://bom.nanxinkj.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://scm.quarkkingdee.top

[R05] 参数默认值
来源：http://ube.shuidangran.top

name="${1:-default}"
来源：http://fpb.xziqi.cn

[R06] 判断命令是否存在
来源：http://kal.yangfankeji.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://igc.cashguo.top

[R07] if 判断文件
来源：http://csi.ivvv.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://bnr.hywenlv.cn

[R08] 数值比较
来源：http://phi.nanxuanxn.top

if (( a > b )); then echo "a 更大"; fi
来源：http://lej.yueranfly.top

[R09] 字符串比较
来源：http://wpg.fengsongda.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ekb.gzhubu.top

[R10] 正则匹配
来源：http://jlj.316326.xyz

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hvj.hesvh.cn

[R11] case 多分支
来源：http://agd.andypj.xyz

case "$1" in
来源：http://ocp.aibaodan.cn

start) echo "启动" ;;
来源：http://bmu.shuidangran.top

stop)  echo "停止" ;;
来源：http://lxd.zdbjq.cn

*)     echo "未知命令" ;;
来源：http://acj.gogol.net.cn

esac
来源：http://dfg.cheryme.top

[R12] for 遍历文件
来源：http://whx.zhoulong.xyz

for f in *.txt; do echo "$f"; done
来源：http://xzm.hysaishi.cn

[R13] for 计数循环
来源：http://qib.gogol.net.cn

for i in {1..10}; do echo "$i"; done
来源：http://htd.kuanghao11.cn

[R14] C 风格 for
来源：http://dxq.shzxlz.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://npy.c1oappe.top

[R15] while 逐行读文件
来源：http://lrm.tian-w.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://igz.aizwys.cn

[R16] until 等待条件
来源：http://uxi.jlsjyb.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://kyg.yj20258.top

[R17] 数组定义与取值
来源：http://vgp.ywan-chungtsiang.top

arr=(a b c); echo "${arr[0]}"
来源：http://pga.ppjwa.cn

[R18] 遍历数组
来源：http://mwd.xuanzx.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://pxx.ydjk.org.cn

[R19] 数组长度
来源：http://vbi.xylfe.cn

echo "${#arr[@]}"
来源：http://ppj.birdmap.top

[R20] 关联数组（字典）
来源：http://teb.haohaochexian.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://gtn.pycfn.com

[R21] 字符串长度
来源：http://ufz.tianlin.xyz

echo "${#s}"
来源：http://fjb.yuanzhike.top

[R22] 截取子串
来源：http://alb.52xcode.cn

echo "${s:0:5}"
来源：http://ire.xingfuxueyuan.xyz

[R23] 字符串替换
来源：http://umx.ivvv.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://bwq.nanxinkj.top

[R24] 大小写转换
来源：http://zof.meibo888.top

echo "${s^^}"; echo "${s,,}"
来源：http://teb.hcnkem.com

[R25] 去后缀 / 去前缀
来源：http://ikq.nwbrower.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://vaa.yonumen.top

[R26] 命令替换
来源：http://uux.yj20258.top

now=$(date +%F); echo "$now"
来源：http://qvs.hnqzz.top

[R27] 算术展开
来源：http://qzi.xuetiantiany.cn


<!-- 参考信息 -->