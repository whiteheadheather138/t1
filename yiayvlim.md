代发 wailian999

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://vpd.iojbl.cn

TS:   if (x == null) {}
来源：http://ies.gzhubu.top

Java: if (x == null || x.isEmpty()) {}
来源：http://eyb.gotoacloud.top

Go:   if x == nil {}
来源：http://uzm.hfpthk.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://bbd.chenzaomai.com

C#:   if (x is null) {}
来源：http://vde.chenlongwang.top

[P07] 防抖与节流
来源：http://qtq.smart0.xyz

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://lib.tian-w.cn

PHP:  // 手写时间戳比较
来源：http://sju.svipenyu.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ujk.xinyue.icu

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xuv.zhaomingkeji.xyz

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://kne.jinqigfzy.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hzm.tarul.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://fti.zhiwuduotai.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://tlk.ctjpmb.com

[P08] 处理浮点精度问题
来源：http://ivr.cashguo.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://duj.haohaochexian.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://bnm.nanxinkj.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wua.jianghu66.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://yds.zhoulong.xyz

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://xyj.shuidangran.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wia.yueranfly.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ruq.aizwys.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://xsp.jlsjyb.cn

================================================================================
来源：http://krf.hongshengwenyu.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://bpn.snrcjt.cn

================================================================================
来源：http://swn.bbcook.cn

[Q01] 创建表
来源：http://dfe.zycfv.cn

CREATE TABLE users (
来源：http://xmb.shanyushiyangtech.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://uao.jqgfzy.top

name VARCHAR(50) NOT NULL,
来源：http://rab.haohaochexian.top

email VARCHAR(100) UNIQUE,
来源：http://mvb.zdbjq.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ltk.jqgfzy.top

);
来源：http://xnx.yangfankeji.com

[Q02] 创建带外键的表
来源：http://fpe.ctjpmb.com

CREATE TABLE orders (
来源：http://wet.fktsv.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://xog.yueranfly.top

user_id INT NOT NULL,
来源：http://wvp.zhaomingkeji.xyz

amount DECIMAL(10, 2),
来源：http://nis.nanxinkj.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://bpz.sxryk.cn

);
来源：http://txx.yj20258888.top

[Q03] 增加列
来源：http://neo.sweek.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ezc.fehbvm.com

[Q04] 修改列类型
来源：http://cir.uphjek.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://iss.yvedp.cn

[Q05] 重命名列
来源：http://ood.havefunace.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ocz.jinyuanbaomall.cn

[Q06] 删除列
来源：http://odk.52xcode.cn

ALTER TABLE users DROP COLUMN age;
来源：http://eho.sufxvd.cn

[Q07] 删除表
来源：http://zrz.vehdjk.com

DROP TABLE IF EXISTS orders;
来源：http://iyo.hfpthk.cn

[Q08] 创建普通索引
来源：http://dme.52xcode.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://azk.gotoacloud.top

[Q09] 创建唯一索引
来源：http://abz.sweek.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://yvu.guannengcc.top

[Q10] 插入单行
来源：http://ebr.zhoulong.xyz

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://evv.ydzc1.top

[Q11] 一次插入多行
来源：http://pop.yj202588.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://lbn.bbcook.cn

[Q12] 插入后取自增 ID
来源：http://xmd.yj20258.top

INSERT INTO users (name) VALUES ('C');
来源：http://ztz.zdbjq.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://euh.sysykeji.top

[Q13] 忽略重复插入
来源：http://gbt.shzxlz.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://yug.redwolf501.top

[Q14] 存在则更新（upsert）
来源：http://gkv.aizwys.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://uwo.chenlongwang.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://skr.yanxiufei.cn

[Q15] 查询全部
来源：http://fyz.haohaochexian.top

SELECT * FROM users;
来源：http://mqf.yangfankeji.com

[Q16] 查询指定列
来源：http://zgq.jqgufenzy.top

SELECT id, name FROM users;
来源：http://xfz.shuidangran.top

[Q17] 条件查询
来源：http://bkt.bbcook.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://xfk.shangyingyoupin.top

[Q18] 模糊匹配
来源：http://knt.fktsv.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://dhd.shanyushiyangkeji.top

[Q19] 范围查询
来源：http://gym.wangshuangyany.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://pow.xingfuxueyuan.xyz

[Q20] IN 列表
来源：http://fcv.shanyushiyangkeji.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://yht.jiagoushi.top

[Q21] 空值判断
来源：http://gzo.yanxiufei.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://xqs.xuanzx.com

[Q22] 排序
来源：http://ljd.sufxvd.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mam.gzhubu.top

[Q23] 分页
来源：http://pgk.jyoumei.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://kaa.shzxlz.cn

[Q24] 去重
来源：http://xsd.jqgufenzy.top

SELECT DISTINCT city FROM users;
来源：http://awl.vehdjk.com

[Q25] 只取前 N 条
来源：http://asc.bjfxy.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://uoi.zdbjq.cn

[Q26] 计数
来源：http://xbb.wangdashe.top

SELECT COUNT(*) FROM users;
来源：http://vvw.cheryme.top

[Q27] 条件计数
来源：http://zjd.fzhhl.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://rxw.fzhhl.top

[Q28] 求和与平均
来源：http://pds.ivvv.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://csz.zhiwuduotai.top

[Q29] 最大最小值
来源：http://vkb.quarkkingdee.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://ebl.ywan-chungtsiang.top

[Q30] 分组统计
来源：http://ffn.ydjk.org.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://yyd.ctjpmb.com

[Q31] 分组后过滤
来源：http://bun.zhengqikj.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://eay.aibaodan.cn

[Q32] 分组拼接字符串
来源：http://msi.chenlongwang.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://nfh.gogol.net.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://fko.ydzc1.top

[Q33] 多列分组
来源：http://ytk.zhiwuduotai.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://niz.feifeiyinyue.top

[Q34] 每组取第一条
来源：http://fev.fengsongda.top

SELECT * FROM (
来源：http://blu.sysykeji.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://tdi.yongpay.top

) t WHERE rn = 1;
来源：http://mua.havefunace.top

[Q35] 内连接
来源：http://ozh.yuanzhike.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://lji.jinyuanbaomall.cn

[Q36] 左连接
来源：http://dds.jianghu66.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://zjh.ydzc1.top

[Q37] 右连接
来源：http://qhk.zhixingplan.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wjq.svipenyu.cn

[Q38] 全外连接（PostgreSQL）
来源：http://hsa.jinqigufen.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mji.haohaochexian.top

[Q39] 自连接（查上下级）
来源：http://esf.xuanzx.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://rec.jiagoushi.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://kho.zhixingplan.top

[Q40] 交叉连接（笛卡尔积）
来源：http://dhd.yfazqb.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://rqo.daria6918.cn

[Q41] 多表连接
来源：http://lgx.iojbl.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://iwy.shangyingyoupin.top

JOIN users u ON u.id = o.user_id
来源：http://jmy.snrcjt.cn

JOIN products p ON p.id = o.product_id;
来源：http://wqq.yuanzhike.top

[Q42] 连接条件附加过滤
来源：http://duj.jyoumei.cn

SELECT u.name, o.amount FROM users u
来源：http://tvs.9152youxi.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://xzs.c1oappe.top

[Q43] 标量子查询
来源：http://gbx.ydjk.org.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://yho.andypj.xyz

[Q44] IN 子查询
来源：http://uez.cucudq.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://uaw.zhaomingkeji.xyz

[Q45] EXISTS 判断存在
来源：http://zmw.yj20258.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mpy.guowangkeji.top

[Q46] NOT EXISTS 判断不存在
来源：http://wuh.chenlongwang.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ctp.feifeiyinyue.top

[Q47] 与平均值比较
来源：http://xxm.ehwqpu.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://lhw.0kj1m.cn

[Q48] CTE 公用表表达式
来源：http://erq.havefunace.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://svq.nwbrower.top

SELECT * FROM t WHERE c > 5;
来源：http://nrw.yj202588.top

[Q49] 更新单行
来源：http://yio.epnwcf.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://gqj.jiagoushi.top

[Q50] 批量更新
来源：http://pnn.tarul.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://egs.yuxming.cn

[Q51] 用子查询更新
来源：http://smg.yvedp.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mcv.fzhhl.top

[Q52] 删除指定行
来源：http://ofs.bjfxy.top

DELETE FROM users WHERE id = 10;
来源：http://wft.bbcook.cn

[Q53] 按条件删除
来源：http://acg.jianghu66.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://rch.sysykeji.top

[Q54] 清空表
来源：http://uao.andypj.xyz

TRUNCATE TABLE logs;
来源：http://brh.guowangkeji.top

[Q55] 排名（并列占位）
来源：http://fit.jyoumei.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ieg.shuidangran.top

[Q56] 密集排名（并列不占位）
来源：http://otk.hfpthk.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://zzr.jqgufenzy.top

[Q57] 行号
来源：http://pav.jyoumei.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mcg.shangyingyoupin.top

[Q58] 累计求和
来源：http://kzu.bbcook.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://qpt.redwolf501.top

[Q59] 分组内累计
来源：http://tvz.316326.xyz

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://uzc.nwbrower.top

[Q60] 取上一行 / 下一行
来源：http://qan.yongpay.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://nzb.snrcjt.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://lob.gaohongyu789.top

[Q61] 移动平均
来源：http://hma.zhengqikj.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wuh.hcnkem.com

[Q62] 分组占比
来源：http://vjb.ydzc1.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://rso.pengpengdd.cyou

[Q63] 开启事务
来源：http://ayg.xinyue.icu

START TRANSACTION;                -- 或 BEGIN
来源：http://qmv.xinyue.icu

[Q64] 提交事务
来源：http://fwd.iojbl.cn

COMMIT;
来源：http://gqm.tarul.cn

[Q65] 回滚事务
来源：http://hdf.bjfxy.top

ROLLBACK;
来源：http://uap.shangyingyoupin.top

[Q66] 行锁查询
来源：http://jse.yanxiufei.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://kmt.tarul.cn

[Q67] 设置隔离级别
来源：http://moy.316326.xyz

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://xka.jinyuanbaomall.cn

[Q68] 保存点
来源：http://nzf.9152youxi.cn

SAVEPOINT sp1;
来源：http://cww.jiagoushi.top

ROLLBACK TO sp1;
来源：http://qng.zdbjq.cn

[Q69] 查看执行计划
来源：http://odd.chenlongwang.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://iys.hesvh.cn

[Q70] 更新统计信息
来源：http://wpa.cdnleiting.top

ANALYZE TABLE users;
来源：http://dsx.jinghuilouyu.cn

[Q71] 查看建表语句
来源：http://aqc.gaohongyu789.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://syc.jiagoushi.top

[Q72] 查看索引
来源：http://frj.yongpay.top

SHOW INDEX FROM users;
来源：http://csn.snrcjt.cn

[Q73] 查看表状态
来源：http://vrc.xuanzx.com

SHOW TABLE STATUS LIKE 'users';
来源：http://gwv.9152youxi.cn

[Q74] 强制使用索引
来源：http://pqw.gaohongyu789.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://bcg.jqgufenzy.top

[Q75] 日期格式化
来源：http://lnl.yj202588.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://psi.zdbjq.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://req.jinyuanbaomall.cn

[Q76] 按天统计
来源：http://tqa.52xcode.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://sag.tanke756.top

[Q77] 时间加减
来源：http://pac.svipenyu.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://vnt.pengpengdd.cyou

[Q78] 当前时间
来源：http://cnv.yuanzhike.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://tnb.smart0.xyz

[Q79] 字符串拼接
来源：http://uxu.hysaishi.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://kfg.fehbvm.com

[Q80] 字符串截取
来源：http://bdj.haohaochexian.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://rzx.jinqigufen.top

[Q81] 字符串替换
来源：http://sug.aizwys.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://pjb.snrcjt.cn

[Q82] 字符长度与字节长度
来源：http://wcx.xziqi.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://byy.aizwys.cn

[Q83] 大小写转换
来源：http://hne.bbcook.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://llv.zhongyouzk.top

[Q84] 去除首尾空格
来源：http://pbo.c1oappe.top

SELECT TRIM(name) FROM users;
来源：http://cah.yanxiufei.cn

[Q85] 数值取整
来源：http://wsi.tian-w.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://upd.wangdashe.top

[Q86] 读取 JSON 字段
来源：http://krk.jianghu66.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://gqn.meibo888.top

[Q87] JSON 字段做条件
来源：http://ifw.hesvh.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://lpm.cashguo.top

[Q88] 行转列（条件聚合）
来源：http://gkt.shzxlz.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://jry.jinghuilouyu.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://llb.9152youxi.cn

[Q89] 判断表是否存在
来源：http://qak.zycfv.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://gtm.yonumen.top

[Q90] 生成序号列
来源：http://vev.haohaochexian.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://lhd.smart0.xyz

================================================================================
来源：http://xzr.nwbrower.top

R. Bash 专题
来源：http://oyh.havefunace.top

================================================================================
来源：http://xni.daria6918.cn

[R01] shebang 与严格模式
来源：http://xvv.ctjpmb.com

#!/usr/bin/env bash
来源：http://mzs.bbcook.cn

set -euo pipefail
来源：http://ufa.gaohongyu789.top

[R02] 变量赋值与使用
来源：http://oxq.ehwqpu.com

name="Tom"; echo "$name"
来源：http://uhd.ydzc1.top

[R03] 只读变量
来源：http://cgn.svipenyu.cn

readonly PI=3.14
来源：http://xuv.wangdashe.top

[R04] 位置参数
来源：http://ovl.jiagoushi.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://gyb.jlsjyb.cn

[R05] 参数默认值
来源：http://xwp.nanxinkj.top

name="${1:-default}"
来源：http://znb.ydzc1.top

[R06] 判断命令是否存在
来源：http://oku.sxryk.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wgf.fktsv.cn

[R07] if 判断文件
来源：http://hvt.hongshengwenyu.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://sjw.jinqigfzy.top

[R08] 数值比较
来源：http://aoj.xinyue.icu

if (( a > b )); then echo "a 更大"; fi
来源：http://gsa.ivvv.top

[R09] 字符串比较
来源：http://iyk.9152youxi.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wqx.gzhubu.top

[R10] 正则匹配
来源：http://wfp.sjlbkw.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://owv.quarkkingdee.top

[R11] case 多分支
来源：http://pjo.tianlin.xyz

case "$1" in
来源：http://fcw.zdbjq.cn

start) echo "启动" ;;
来源：http://uos.hammf.cn

stop)  echo "停止" ;;
来源：http://qcy.daria6918.cn

*)     echo "未知命令" ;;
来源：http://htn.shanyushiyangkeji.top

esac
来源：http://lqh.fanxiaobao.xyz

[R12] for 遍历文件
来源：http://mpy.tianlin.xyz

for f in *.txt; do echo "$f"; done
来源：http://vnu.c1oappe.top

[R13] for 计数循环
来源：http://ryh.yvedp.cn

for i in {1..10}; do echo "$i"; done
来源：http://xtc.xuanzx.com

[R14] C 风格 for
来源：http://ypg.ydzc1.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://tyr.tianlin.xyz

[R15] while 逐行读文件
来源：http://ooy.jqgfzy.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hjx.vqdsnc.cn

[R16] until 等待条件
来源：http://dni.fktsv.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://slh.jqgufenzy.top

[R17] 数组定义与取值
来源：http://ime.epnwcf.com

arr=(a b c); echo "${arr[0]}"
来源：http://srs.ehwqpu.com

[R18] 遍历数组
来源：http://wtg.yj202588.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://tux.jiagoushi.top

[R19] 数组长度
来源：http://pte.bjfxy.top

echo "${#arr[@]}"
来源：http://caw.redwolf501.top

[R20] 关联数组（字典）
来源：http://nsd.iojbl.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mjw.hongshengwenyu.top

[R21] 字符串长度
来源：http://imh.zhixingplan.top

echo "${#s}"
来源：http://xgy.yj20258888.top

[R22] 截取子串
来源：http://vcj.zycfv.cn

echo "${s:0:5}"
来源：http://cqu.xylfe.cn

[R23] 字符串替换
来源：http://thz.feifeiyinyue.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://pfk.daxiang520.top

[R24] 大小写转换
来源：http://ept.daxiang520.top

echo "${s^^}"; echo "${s,,}"
来源：http://adj.gotoacloud.top

[R25] 去后缀 / 去前缀
来源：http://yrl.cashguo.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://hja.yanxiufei.cn

[R26] 命令替换
来源：http://quc.shuidangran.top

now=$(date +%F); echo "$now"
来源：http://lwx.zycfv.cn

[R27] 算术展开
来源：http://eld.ydzc1.top

echo $((1 + 2 * 3))
来源：http://vyc.yueranfly.top

[R28] 浮点运算
来源：http://lbc.quarkkingdee.top

echo "scale=2; 10/3" | bc
来源：http://vtw.mhx1999.top

[R29] 定义函数
来源：http://jfb.chenzaomai.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://raw.hnqzz.top

[R30] 函数返回状态码
来源：http://sqy.yonumen.top

f() { return 0; }; f || echo "失败了"
来源：http://xza.ydjk.org.cn

[R31] 局部变量
来源：http://gqr.yfazqb.com


<!-- 参考信息 -->