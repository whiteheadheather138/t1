代发 wailian999

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ibs.shanyushiyangkeji.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://srv.sjlbkw.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://rxg.gaohongyu789.top

PHP:  if (empty($x)) {}
来源：http://ppt.aibaodan.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://uhm.pengpengdd.cyou

TS:   if (x == null) {}
来源：http://jyz.0kj1m.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://cvz.xylfe.cn

Go:   if x == nil {}
来源：http://yvc.guannengcc.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ezv.wangdashe.top

C#:   if (x is null) {}
来源：http://wfu.yuxming.cn

[P07] 防抖与节流
来源：http://oin.yueranfly.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://oms.hammf.cn

PHP:  // 手写时间戳比较
来源：http://zid.fengsongda.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dma.vqdsnc.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mbw.jinyuanbaomall.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://sxx.hammf.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://dpm.hywenlv.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://bvr.jqgufenzy.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://arp.fengsongda.top

[P08] 处理浮点精度问题
来源：http://nth.daria6918.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://gfb.daxiang520.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://qvi.tianlin.xyz

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://eqj.shangyingyoupin.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ywf.aibaodan.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://kpc.gotoacloud.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ftw.epnwcf.com

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://osq.sxryk.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ayy.hammf.cn

================================================================================
来源：http://lgz.zdbjq.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://rfc.shanyushiyangkeji.top

================================================================================
来源：http://fne.ydjk.org.cn

[Q01] 创建表
来源：http://rai.vqdsnc.cn

CREATE TABLE users (
来源：http://rnt.hnqzz.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://dtk.yj202588.top

name VARCHAR(50) NOT NULL,
来源：http://hfv.zhongyouzk.top

email VARCHAR(100) UNIQUE,
来源：http://euk.bbcook.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://pvj.zhiwuduotai.top

);
来源：http://kov.yj20258.top

[Q02] 创建带外键的表
来源：http://txm.tanke756.top

CREATE TABLE orders (
来源：http://jdb.nanxinkj.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://pdo.nanxuanxn.top

user_id INT NOT NULL,
来源：http://elm.sjlbkw.cn

amount DECIMAL(10, 2),
来源：http://ngs.nanxinkj.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://jah.gotoacloud.top

);
来源：http://egf.ctjpmb.com

[Q03] 增加列
来源：http://dov.vqdsnc.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://kcy.xziqi.cn

[Q04] 修改列类型
来源：http://cti.yuanzhike.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://aet.meibo888.top

[Q05] 重命名列
来源：http://tgn.xylfe.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://lej.yuxming.cn

[Q06] 删除列
来源：http://cae.tarul.cn

ALTER TABLE users DROP COLUMN age;
来源：http://bsp.feifeiyinyue.top

[Q07] 删除表
来源：http://jqf.dashuyun.cn

DROP TABLE IF EXISTS orders;
来源：http://lpj.aibaodan.cn

[Q08] 创建普通索引
来源：http://neu.fktsv.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://eik.yj20258888.top

[Q09] 创建唯一索引
来源：http://eqx.xuanzx.com

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://asf.meibo888.top

[Q10] 插入单行
来源：http://hla.gzhubu.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ogg.hnqzz.top

[Q11] 一次插入多行
来源：http://cml.yonumen.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ckc.bjfxy.top

[Q12] 插入后取自增 ID
来源：http://bnb.dashuyun.cn

INSERT INTO users (name) VALUES ('C');
来源：http://rav.xuetiantiany.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://yli.pycfn.com

[Q13] 忽略重复插入
来源：http://epk.tarul.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ivg.cucudq.cn

[Q14] 存在则更新（upsert）
来源：http://bnu.hammf.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://bye.gzhubu.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://dak.ybcxt.top

[Q15] 查询全部
来源：http://gst.dashuyun.cn

SELECT * FROM users;
来源：http://hwn.zhiwuduotai.top

[Q16] 查询指定列
来源：http://ghn.9152youxi.cn

SELECT id, name FROM users;
来源：http://agh.yuxming.cn

[Q17] 条件查询
来源：http://mlw.svipenyu.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ups.zhengqikj.top

[Q18] 模糊匹配
来源：http://mis.haohaochexian.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://kqk.yueranfly.top

[Q19] 范围查询
来源：http://cjb.kuanghao11.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ybl.zycfv.cn

[Q20] IN 列表
来源：http://nxj.hammf.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://kzt.jinqigfzy.top

[Q21] 空值判断
来源：http://rav.gaohongyu789.top

SELECT * FROM users WHERE email IS NULL;
来源：http://dnu.sweek.top

[Q22] 排序
来源：http://xrx.zhaomingkeji.xyz

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ryl.wangdashe.top

[Q23] 分页
来源：http://hbk.snrcjt.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://gwa.hnxiangtu.top

[Q24] 去重
来源：http://mlv.dashuyun.cn

SELECT DISTINCT city FROM users;
来源：http://len.zhengqikj.top

[Q25] 只取前 N 条
来源：http://ekt.havefunace.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mcj.jiagoushi.top

[Q26] 计数
来源：http://dml.fktsv.cn

SELECT COUNT(*) FROM users;
来源：http://efr.jianghu66.top

[Q27] 条件计数
来源：http://wtz.nanxinkj.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://oql.hesvh.cn

[Q28] 求和与平均
来源：http://uze.hywenlv.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://erh.wangdashe.top

[Q29] 最大最小值
来源：http://ysl.pengpengdd.cyou

SELECT MAX(age), MIN(age) FROM users;
来源：http://hlb.guowangkeji.top

[Q30] 分组统计
来源：http://vgh.cashguo.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://asg.ydzc1.top

[Q31] 分组后过滤
来源：http://ovm.yj20258.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ijv.gogol.net.cn

[Q32] 分组拼接字符串
来源：http://vey.dashuyun.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://sdu.xylfe.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://dui.ivvv.top

[Q33] 多列分组
来源：http://vvs.shangyingyoupin.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://cxu.ybcxt.top

[Q34] 每组取第一条
来源：http://yfx.gzhubu.top

SELECT * FROM (
来源：http://aad.jqgufenzy.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://bkj.chenlongwang.top

) t WHERE rn = 1;
来源：http://oub.shzxlz.cn

[Q35] 内连接
来源：http://qvn.nwbrower.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://oev.vqdsnc.cn

[Q36] 左连接
来源：http://hvv.uphjek.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://bhp.uphjek.com

[Q37] 右连接
来源：http://zem.sysykeji.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://qjz.zycfv.cn

[Q38] 全外连接（PostgreSQL）
来源：http://rbl.sufxvd.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://lnj.fehbvm.com

[Q39] 自连接（查上下级）
来源：http://ylf.tanke756.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://ozh.chenzaomai.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://xoy.shanyushiyangkeji.top

[Q40] 交叉连接（笛卡尔积）
来源：http://kit.dianchejie.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mzv.nwbrower.top

[Q41] 多表连接
来源：http://gcx.jyoumei.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://lli.sysykeji.top

JOIN users u ON u.id = o.user_id
来源：http://uqa.shanyushiyangtech.top

JOIN products p ON p.id = o.product_id;
来源：http://xtn.shanyushiyangkeji.top

[Q42] 连接条件附加过滤
来源：http://cxe.aibaodan.cn

SELECT u.name, o.amount FROM users u
来源：http://bcs.yj202588.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ymh.yuanzhike.top

[Q43] 标量子查询
来源：http://uwn.gzhubu.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://tus.redwolf501.top

[Q44] IN 子查询
来源：http://fyn.zhongyouzk.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wxt.tianlin.xyz

[Q45] EXISTS 判断存在
来源：http://nnw.zhoulong.xyz

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bpp.shzxlz.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ywf.hnqzz.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://iqw.cheryme.top

[Q47] 与平均值比较
来源：http://vtr.fktsv.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://rxs.yangfankeji.com

[Q48] CTE 公用表表达式
来源：http://sie.hongshengwenyu.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://uin.jinyuanbaomall.cn

SELECT * FROM t WHERE c > 5;
来源：http://kwh.zhaomingkeji.xyz

[Q49] 更新单行
来源：http://oae.jiagoushi.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://nqa.jiagoushi.top

[Q50] 批量更新
来源：http://rpm.daxiang520.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wab.dashuyun.cn

[Q51] 用子查询更新
来源：http://aoi.sjlbkw.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://gse.nwbrower.top

[Q52] 删除指定行
来源：http://jvj.xylfe.cn

DELETE FROM users WHERE id = 10;
来源：http://kdp.yfazqb.com

[Q53] 按条件删除
来源：http://mgm.jqgufenzy.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://fqw.dashuyun.cn

[Q54] 清空表
来源：http://hyb.smart0.xyz

TRUNCATE TABLE logs;
来源：http://kyj.shzxlz.cn

[Q55] 排名（并列占位）
来源：http://pwv.zdqjudy.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://llh.yuanzhike.top

[Q56] 密集排名（并列不占位）
来源：http://ahb.jqgfzy.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://dwu.fzhhl.top

[Q57] 行号
来源：http://gkl.jinqigfzy.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mvk.quarkkingdee.top

[Q58] 累计求和
来源：http://rlg.aibaodan.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://tfq.ppjwa.cn

[Q59] 分组内累计
来源：http://wjq.yonumen.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://bdf.smart0.xyz

[Q60] 取上一行 / 下一行
来源：http://rrx.ydzc1.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://jyw.cheryme.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hyl.guannengcc.top

[Q61] 移动平均
来源：http://nps.zhixingplan.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://iuz.shuidangran.top

[Q62] 分组占比
来源：http://wco.ivvv.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hhg.wangdashe.top

[Q63] 开启事务
来源：http://msj.hnqzz.top

START TRANSACTION;                -- 或 BEGIN
来源：http://nny.fengsongda.top

[Q64] 提交事务
来源：http://tfn.hnqzz.top

COMMIT;
来源：http://rdm.52xcode.cn

[Q65] 回滚事务
来源：http://dun.gaohongyu789.top

ROLLBACK;
来源：http://fak.aizwys.cn

[Q66] 行锁查询
来源：http://dwd.52xcode.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ejk.fengsongda.top

[Q67] 设置隔离级别
来源：http://mtb.epnwcf.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wkq.gaohongyu789.top

[Q68] 保存点
来源：http://doe.nwbrower.top

SAVEPOINT sp1;
来源：http://zkf.gzhubu.top

ROLLBACK TO sp1;
来源：http://tll.jqgfzy.top

[Q69] 查看执行计划
来源：http://kaz.sweek.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://puf.ydjk.org.cn

[Q70] 更新统计信息
来源：http://zbl.9152youxi.cn

ANALYZE TABLE users;
来源：http://qpz.birdmap.top

[Q71] 查看建表语句
来源：http://jrn.tarul.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://yah.ybcxt.top

[Q72] 查看索引
来源：http://rxm.chenzaomai.com

SHOW INDEX FROM users;
来源：http://spe.gzhubu.top

[Q73] 查看表状态
来源：http://bqj.havefunace.top

SHOW TABLE STATUS LIKE 'users';
来源：http://ydl.jinghuilouyu.cn

[Q74] 强制使用索引
来源：http://mlf.chenlongwang.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://lei.jinqigfzy.top

[Q75] 日期格式化
来源：http://wqc.svipenyu.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://pex.guannengcc.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://fye.9152youxi.cn

[Q76] 按天统计
来源：http://gpw.zhongyouzk.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://cex.fktsv.cn

[Q77] 时间加减
来源：http://xbu.yj202588.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://bhj.yonumen.top

[Q78] 当前时间
来源：http://dzg.guowangkeji.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://yjj.316326.xyz

[Q79] 字符串拼接
来源：http://vsp.smart0.xyz

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://cye.jqgfzy.top

[Q80] 字符串截取
来源：http://edx.birdmap.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://eak.smart0.xyz

[Q81] 字符串替换
来源：http://qnk.yongpay.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://izk.pengpengdd.cyou

[Q82] 字符长度与字节长度
来源：http://scv.pengpengdd.cyou

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://yvf.cheryme.top

[Q83] 大小写转换
来源：http://nfa.xylfe.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wpm.nwbrower.top

[Q84] 去除首尾空格
来源：http://oca.snrcjt.cn

SELECT TRIM(name) FROM users;
来源：http://ecm.pengpengdd.cyou

[Q85] 数值取整
来源：http://hcn.tian-w.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://xdn.hammf.cn

[Q86] 读取 JSON 字段
来源：http://lpt.zdbjq.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ffv.gzhubu.top

[Q87] JSON 字段做条件
来源：http://ijk.gzhubu.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wlq.xuetiantiany.cn

[Q88] 行转列（条件聚合）
来源：http://iyj.hfpthk.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://qsl.fktsv.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://tmf.sweek.top

[Q89] 判断表是否存在
来源：http://znh.cdnleiting.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://dzz.ydzc1.top

[Q90] 生成序号列
来源：http://trm.andypj.xyz

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://bcn.snrcjt.cn

================================================================================
来源：http://uqv.guannengcc.top

R. Bash 专题
来源：http://tda.yj20258888.top

================================================================================
来源：http://oby.zhijiandao.cn

[R01] shebang 与严格模式
来源：http://tbb.tian-w.cn

#!/usr/bin/env bash
来源：http://tgq.jqgufenzy.top

set -euo pipefail
来源：http://yam.yj202588.top

[R02] 变量赋值与使用
来源：http://ahi.ywan-chungtsiang.top

name="Tom"; echo "$name"
来源：http://zrc.guowangkeji.top

[R03] 只读变量
来源：http://wjs.c1oappe.top

readonly PI=3.14
来源：http://hzf.sweek.top

[R04] 位置参数
来源：http://ybb.0kj1m.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://yjc.smart0.xyz

[R05] 参数默认值
来源：http://vvt.cashguo.top

name="${1:-default}"
来源：http://szd.52xcode.cn

[R06] 判断命令是否存在
来源：http://wrb.fanxiaobao.xyz

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://fmj.cashguo.top

[R07] if 判断文件
来源：http://izz.tianlin.xyz

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mph.epnwcf.com

[R08] 数值比较
来源：http://scc.ydzc1.top

if (( a > b )); then echo "a 更大"; fi
来源：http://ink.cdnleiting.top

[R09] 字符串比较
来源：http://qiz.andypj.xyz

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://rkp.guowangkeji.top

[R10] 正则匹配
来源：http://hbl.sxryk.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://vdq.xuetiantiany.cn

[R11] case 多分支
来源：http://pfo.52xcode.cn

case "$1" in
来源：http://tyl.shzxlz.cn

start) echo "启动" ;;
来源：http://ekk.shangyingyoupin.top

stop)  echo "停止" ;;
来源：http://pva.jqgufenzy.top

*)     echo "未知命令" ;;
来源：http://ihw.ydjk.org.cn

esac
来源：http://mbm.hywenlv.cn

[R12] for 遍历文件
来源：http://vpp.chenjidiqi.icu

for f in *.txt; do echo "$f"; done
来源：http://gjf.hywenlv.cn

[R13] for 计数循环
来源：http://guw.meibo888.top

for i in {1..10}; do echo "$i"; done
来源：http://ten.andypj.xyz

[R14] C 风格 for
来源：http://vpt.tanke756.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://jog.nanxinkj.top

[R15] while 逐行读文件
来源：http://onl.zdqjudy.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://aqd.mhx1999.top

[R16] until 等待条件
来源：http://mae.ivvv.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://znq.zhongyouzk.top

[R17] 数组定义与取值
来源：http://ssp.iojbl.cn

arr=(a b c); echo "${arr[0]}"
来源：http://auy.jqgufenzy.top

[R18] 遍历数组
来源：http://tpc.0kj1m.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://uoe.c1oappe.top

[R19] 数组长度
来源：http://dwk.nwbrower.top

echo "${#arr[@]}"
来源：http://aun.snrcjt.cn

[R20] 关联数组（字典）
来源：http://hyz.jlsjyb.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://yow.meibo888.top

[R21] 字符串长度
来源：http://xul.cucudq.cn

echo "${#s}"
来源：http://zgm.cucudq.cn

[R22] 截取子串
来源：http://aeu.tarul.cn

echo "${s:0:5}"
来源：http://bob.meibo888.top

[R23] 字符串替换
来源：http://mln.xuetiantiany.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://qdl.yueranfly.top

[R24] 大小写转换
来源：http://yyd.jiagoushi.top

echo "${s^^}"; echo "${s,,}"
来源：http://yzx.tanke756.top

[R25] 去后缀 / 去前缀
来源：http://fks.yueranfly.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://vpl.52xcode.cn

[R26] 命令替换
来源：http://jmf.yangfankeji.com

now=$(date +%F); echo "$now"
来源：http://ian.chenlongwang.top

[R27] 算术展开
来源：http://msr.iojbl.cn

echo $((1 + 2 * 3))
来源：http://hjn.birdmap.top

[R28] 浮点运算
来源：http://vre.fktsv.cn

echo "scale=2; 10/3" | bc
来源：http://vhz.zhijiandao.cn

[R29] 定义函数
来源：http://ozn.quarkkingdee.top


<!-- 参考信息 -->