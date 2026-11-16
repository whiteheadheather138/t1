代发 wailian999

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://qgj.quarkkingdee.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://kmn.zdqjudy.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://nal.jinghuilouyu.cn

PHP:  if (empty($x)) {}
来源：http://tsr.fanxiaobao.xyz

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://dnz.andypj.xyz

TS:   if (x == null) {}
来源：http://hbp.hysaishi.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://pdi.iojbl.cn

Go:   if x == nil {}
来源：http://pzq.aizwys.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://uti.zhoulong.xyz

C#:   if (x is null) {}
来源：http://vmx.guannengcc.top

[P07] 防抖与节流
来源：http://xsu.yuanzhike.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://rbn.jianghu66.top

PHP:  // 手写时间戳比较
来源：http://fjt.fzhhl.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xhn.jinyuanbaomall.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://shc.zhongyouzk.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://cpb.ywan-chungtsiang.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://qnf.jinyuanbaomall.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://puv.aizwys.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://kht.ppjwa.cn

[P08] 处理浮点精度问题
来源：http://atg.ivvv.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mmv.fzhhl.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://dbw.fanxiaobao.xyz

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://jqx.jyoumei.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://qjf.yuxming.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ioc.ybcxt.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ggv.9152youxi.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://zlu.pycfn.com

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://lmk.xinyue.icu

================================================================================
来源：http://ulr.9152youxi.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://sue.guowangkeji.top

================================================================================
来源：http://jda.nanxuanxn.top

[Q01] 创建表
来源：http://ekr.epnwcf.com

CREATE TABLE users (
来源：http://jij.snrcjt.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://zqd.nanxuanxn.top

name VARCHAR(50) NOT NULL,
来源：http://lwp.gzhubu.top

email VARCHAR(100) UNIQUE,
来源：http://cfk.haohaochexian.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://jmv.zdqjudy.top

);
来源：http://ecb.feifeiyinyue.top

[Q02] 创建带外键的表
来源：http://egn.zhongyouzk.top

CREATE TABLE orders (
来源：http://vjy.cucudq.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://edm.snrcjt.cn

user_id INT NOT NULL,
来源：http://zio.chenzaomai.com

amount DECIMAL(10, 2),
来源：http://tus.xylfe.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ywp.dashuyun.cn

);
来源：http://zmd.cucudq.cn

[Q03] 增加列
来源：http://txc.zhixingplan.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://tkd.yuxming.cn

[Q04] 修改列类型
来源：http://uah.redwolf501.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://seu.jqgufenzy.top

[Q05] 重命名列
来源：http://lqx.tian-w.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hke.shuidangran.top

[Q06] 删除列
来源：http://amx.xziqi.cn

ALTER TABLE users DROP COLUMN age;
来源：http://bot.bbcook.cn

[Q07] 删除表
来源：http://byu.shuidangran.top

DROP TABLE IF EXISTS orders;
来源：http://bds.xziqi.cn

[Q08] 创建普通索引
来源：http://xyn.jyoumei.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ssp.zdqjudy.top

[Q09] 创建唯一索引
来源：http://ebb.smart0.xyz

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://kua.gogol.net.cn

[Q10] 插入单行
来源：http://nes.birdmap.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://qek.feifeiyinyue.top

[Q11] 一次插入多行
来源：http://ykn.dianchejie.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://jyq.sjlbkw.cn

[Q12] 插入后取自增 ID
来源：http://tgt.dianchejie.cn

INSERT INTO users (name) VALUES ('C');
来源：http://zqf.ppjwa.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://bsq.bjfxy.top

[Q13] 忽略重复插入
来源：http://gun.aizwys.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://gyj.fengsongda.top

[Q14] 存在则更新（upsert）
来源：http://mch.redwolf501.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://gkx.yuanzhike.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ztp.yfazqb.com

[Q15] 查询全部
来源：http://dvg.jlsjyb.cn

SELECT * FROM users;
来源：http://wui.hfpthk.cn

[Q16] 查询指定列
来源：http://ngf.feifeiyinyue.top

SELECT id, name FROM users;
来源：http://ffn.zhengqikj.top

[Q17] 条件查询
来源：http://qpy.jqgfzy.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://rwp.zhaomingkeji.xyz

[Q18] 模糊匹配
来源：http://uou.fzhhl.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://qst.yanxiufei.cn

[Q19] 范围查询
来源：http://qzm.havefunace.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://oiw.tian-w.cn

[Q20] IN 列表
来源：http://wpk.yuanzhike.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ywr.jyoumei.cn

[Q21] 空值判断
来源：http://zxh.fanxiaobao.xyz

SELECT * FROM users WHERE email IS NULL;
来源：http://uni.jinghuilouyu.cn

[Q22] 排序
来源：http://eaw.zhoulong.xyz

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mbr.jyoumei.cn

[Q23] 分页
来源：http://ijy.hnqzz.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://whw.mhx1999.top

[Q24] 去重
来源：http://twk.wangshuangyany.cn

SELECT DISTINCT city FROM users;
来源：http://zji.mhx1999.top

[Q25] 只取前 N 条
来源：http://byq.jyoumei.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://gbi.yuanzhike.top

[Q26] 计数
来源：http://pgs.quarkkingdee.top

SELECT COUNT(*) FROM users;
来源：http://cge.cashguo.top

[Q27] 条件计数
来源：http://fez.birdmap.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ogd.yj20258.top

[Q28] 求和与平均
来源：http://uwu.fktsv.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://pit.shanyushiyangkeji.top

[Q29] 最大最小值
来源：http://qyr.yonumen.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://avf.ydzc1.top

[Q30] 分组统计
来源：http://lgd.0kj1m.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://eem.zhijiandao.cn

[Q31] 分组后过滤
来源：http://tyx.sufxvd.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://yua.yj20258888.top

[Q32] 分组拼接字符串
来源：http://fic.52xcode.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ekj.dashuyun.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ssv.jqgfzy.top

[Q33] 多列分组
来源：http://xfl.vqdsnc.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://xfg.hfpthk.cn

[Q34] 每组取第一条
来源：http://fxv.xuetiantiany.cn

SELECT * FROM (
来源：http://ufx.jqgfzy.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://brd.yanxiufei.cn

) t WHERE rn = 1;
来源：http://xvz.0kj1m.cn

[Q35] 内连接
来源：http://odc.xuetiantiany.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hmx.tianlin.xyz

[Q36] 左连接
来源：http://lqs.ctjpmb.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://fhq.chenlongwang.top

[Q37] 右连接
来源：http://qqt.sjlbkw.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://rxq.zhijiandao.cn

[Q38] 全外连接（PostgreSQL）
来源：http://zns.hcnkem.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://zhf.ppjwa.cn

[Q39] 自连接（查上下级）
来源：http://bxu.wangdashe.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://usp.cqqwz.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://jns.hywenlv.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://iui.feifeiyinyue.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://zhq.ehwqpu.com

[Q41] 多表连接
来源：http://ovg.sweek.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://hsv.svipenyu.cn

JOIN users u ON u.id = o.user_id
来源：http://ywq.yongpay.top

JOIN products p ON p.id = o.product_id;
来源：http://smy.fzhhl.top

[Q42] 连接条件附加过滤
来源：http://vsx.jiagoushi.top

SELECT u.name, o.amount FROM users u
来源：http://jif.bbcook.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://zua.jinyuanbaomall.cn

[Q43] 标量子查询
来源：http://hfb.316326.xyz

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ida.fktsv.cn

[Q44] IN 子查询
来源：http://ypg.nanxinkj.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ngx.cashguo.top

[Q45] EXISTS 判断存在
来源：http://fac.shanyushiyangkeji.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://uhd.tarul.cn

[Q46] NOT EXISTS 判断不存在
来源：http://sey.iojbl.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://nmx.mhx1999.top

[Q47] 与平均值比较
来源：http://bbd.snrcjt.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ctg.hcnkem.com

[Q48] CTE 公用表表达式
来源：http://rzn.mhx1999.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://csf.redwolf501.top

SELECT * FROM t WHERE c > 5;
来源：http://ucq.zhixingplan.top

[Q49] 更新单行
来源：http://qcu.daxiang520.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://fge.ctjpmb.com

[Q50] 批量更新
来源：http://mkg.tanke756.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hfa.jinyuanbaomall.cn

[Q51] 用子查询更新
来源：http://ted.haohaochexian.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://pwl.cqqwz.cn

[Q52] 删除指定行
来源：http://oag.chenjidiqi.icu

DELETE FROM users WHERE id = 10;
来源：http://rqk.yvedp.cn

[Q53] 按条件删除
来源：http://sit.xinyue.icu

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://fwb.aibaodan.cn

[Q54] 清空表
来源：http://sdm.nwbrower.top

TRUNCATE TABLE logs;
来源：http://gpj.shzxlz.cn

[Q55] 排名（并列占位）
来源：http://xwi.9152youxi.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wpz.guowangkeji.top

[Q56] 密集排名（并列不占位）
来源：http://php.fanxiaobao.xyz

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://out.cheryme.top

[Q57] 行号
来源：http://gcy.haohaochexian.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://jfu.hammf.cn

[Q58] 累计求和
来源：http://dfg.zhiwuduotai.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://psb.sweek.top

[Q59] 分组内累计
来源：http://imj.sjlbkw.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://yae.wangdashe.top

[Q60] 取上一行 / 下一行
来源：http://fws.yongpay.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://sfg.chenjidiqi.icu

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://lkw.guannengcc.top

[Q61] 移动平均
来源：http://cwi.gaohongyu789.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://nhr.nwbrower.top

[Q62] 分组占比
来源：http://hbn.tarul.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://pki.wangdashe.top

[Q63] 开启事务
来源：http://yop.cucudq.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://oek.tanke756.top

[Q64] 提交事务
来源：http://buw.tian-w.cn

COMMIT;
来源：http://otj.pycfn.com

[Q65] 回滚事务
来源：http://pha.meibo888.top

ROLLBACK;
来源：http://uaj.cqqwz.cn

[Q66] 行锁查询
来源：http://rhk.nwbrower.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ilo.jyoumei.cn

[Q67] 设置隔离级别
来源：http://quv.yfazqb.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hns.52xcode.cn

[Q68] 保存点
来源：http://hxy.cashguo.top

SAVEPOINT sp1;
来源：http://zvz.ivvv.top

ROLLBACK TO sp1;
来源：http://mxv.gaohongyu789.top

[Q69] 查看执行计划
来源：http://ake.jinqigufen.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mad.fehbvm.com

[Q70] 更新统计信息
来源：http://omo.aizwys.cn

ANALYZE TABLE users;
来源：http://cfi.0kj1m.cn

[Q71] 查看建表语句
来源：http://xzj.wangshuangyany.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://gwf.guowangkeji.top

[Q72] 查看索引
来源：http://xex.shanyushiyangtech.top

SHOW INDEX FROM users;
来源：http://iqx.yj202588.top

[Q73] 查看表状态
来源：http://nlr.xingfuxueyuan.xyz

SHOW TABLE STATUS LIKE 'users';
来源：http://rhn.zhoulong.xyz

[Q74] 强制使用索引
来源：http://fgj.shanyushiyangtech.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://rju.yongpay.top

[Q75] 日期格式化
来源：http://aqo.daria6918.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://shy.ybcxt.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://azr.pycfn.com

[Q76] 按天统计
来源：http://ykk.aibaodan.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://yml.jlsjyb.cn

[Q77] 时间加减
来源：http://kue.zhongyouzk.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://iel.guowangkeji.top

[Q78] 当前时间
来源：http://aze.snrcjt.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://gct.haohaochexian.top

[Q79] 字符串拼接
来源：http://qrb.ywan-chungtsiang.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://fup.yongpay.top

[Q80] 字符串截取
来源：http://ute.nanxinkj.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://idv.hongshengwenyu.top

[Q81] 字符串替换
来源：http://ayg.chenjidiqi.icu

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://dwp.52xcode.cn

[Q82] 字符长度与字节长度
来源：http://wsh.gotoacloud.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ezl.yuxming.cn

[Q83] 大小写转换
来源：http://jqs.shangyingyoupin.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://gbo.daxiang520.top

[Q84] 去除首尾空格
来源：http://scw.tian-w.cn

SELECT TRIM(name) FROM users;
来源：http://zov.zhoulong.xyz

[Q85] 数值取整
来源：http://ota.yj202588.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://qaj.dashuyun.cn

[Q86] 读取 JSON 字段
来源：http://zxe.zhongyouzk.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://cbd.ivvv.top

[Q87] JSON 字段做条件
来源：http://mcs.xinyue.icu

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wcj.hywenlv.cn

[Q88] 行转列（条件聚合）
来源：http://swt.bbcook.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://nhd.chenlongwang.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wog.nanxuanxn.top

[Q89] 判断表是否存在
来源：http://gra.uphjek.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://rqv.sysykeji.top

[Q90] 生成序号列
来源：http://upx.tian-w.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://gdj.xinyue.icu

================================================================================
来源：http://bic.ehwqpu.com

R. Bash 专题
来源：http://fmc.shanyushiyangtech.top

================================================================================
来源：http://ntm.xinyue.icu

[R01] shebang 与严格模式
来源：http://qvi.316326.xyz

#!/usr/bin/env bash
来源：http://ygx.yj20258.top

set -euo pipefail
来源：http://qpz.vehdjk.com

[R02] 变量赋值与使用
来源：http://lqs.shangyingyoupin.top

name="Tom"; echo "$name"
来源：http://kwj.ctjpmb.com

[R03] 只读变量
来源：http://hxt.xziqi.cn

readonly PI=3.14
来源：http://zwv.tarul.cn

[R04] 位置参数
来源：http://ppe.cashguo.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://glv.yvedp.cn

[R05] 参数默认值
来源：http://zeo.52xcode.cn

name="${1:-default}"
来源：http://wbc.vqdsnc.cn

[R06] 判断命令是否存在
来源：http://ucr.yongpay.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://vdh.pengpengdd.cyou

[R07] if 判断文件
来源：http://ezh.nwbrower.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://qun.quarkkingdee.top

[R08] 数值比较
来源：http://nan.hongshengwenyu.top

if (( a > b )); then echo "a 更大"; fi
来源：http://jck.fengsongda.top

[R09] 字符串比较
来源：http://abb.shuidangran.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://thl.yuxming.cn

[R10] 正则匹配
来源：http://ucd.zhiwuduotai.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://zao.ydzc1.top

[R11] case 多分支
来源：http://sbh.cheryme.top

case "$1" in
来源：http://sox.meibo888.top

start) echo "启动" ;;
来源：http://lyl.sxryk.cn

stop)  echo "停止" ;;
来源：http://nbc.bbcook.cn

*)     echo "未知命令" ;;
来源：http://fwi.tanke756.top

esac
来源：http://geb.yueranfly.top

[R12] for 遍历文件
来源：http://hnc.xingfuxueyuan.xyz

for f in *.txt; do echo "$f"; done
来源：http://vhs.epnwcf.com

[R13] for 计数循环
来源：http://rik.jinqigufen.top

for i in {1..10}; do echo "$i"; done
来源：http://fvn.vehdjk.com

[R14] C 风格 for
来源：http://oem.yj20258888.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://dgq.fzhhl.top

[R15] while 逐行读文件
来源：http://zoh.jinqigufen.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://diz.tarul.cn

[R16] until 等待条件
来源：http://nik.zhixingplan.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://omw.hammf.cn

[R17] 数组定义与取值
来源：http://lpi.iojbl.cn

arr=(a b c); echo "${arr[0]}"
来源：http://zgs.wangdashe.top

[R18] 遍历数组
来源：http://reb.gotoacloud.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hql.ctjpmb.com

[R19] 数组长度
来源：http://azq.yuanzhike.top

echo "${#arr[@]}"
来源：http://xjx.cdnleiting.top

[R20] 关联数组（字典）
来源：http://jxf.smart0.xyz

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://jxe.jinqigfzy.top

[R21] 字符串长度
来源：http://ndf.guowangkeji.top

echo "${#s}"
来源：http://dhd.jqgfzy.top

[R22] 截取子串
来源：http://ihn.52xcode.cn

echo "${s:0:5}"
来源：http://hwb.chenjidiqi.icu

[R23] 字符串替换
来源：http://fxc.svipenyu.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://fss.nanxuanxn.top

[R24] 大小写转换
来源：http://fdn.birdmap.top

echo "${s^^}"; echo "${s,,}"
来源：http://orm.yueranfly.top

[R25] 去后缀 / 去前缀
来源：http://cvz.jinqigfzy.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://giv.xingfuxueyuan.xyz

[R26] 命令替换
来源：http://xbv.jinqigufen.top

now=$(date +%F); echo "$now"
来源：http://ash.jqgufenzy.top

[R27] 算术展开
来源：http://zhy.epnwcf.com

echo $((1 + 2 * 3))
来源：http://toe.ivvv.top

[R28] 浮点运算
来源：http://zle.aibaodan.cn

echo "scale=2; 10/3" | bc
来源：http://qjr.yj20258.top

[R29] 定义函数
来源：http://xmd.xuanzx.com


<!-- 参考信息 -->