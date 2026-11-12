代发 wailian999

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://rsk.cdnleiting.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://txs.gzhubu.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://gbf.yuanzhike.top

PHP:  if (empty($x)) {}
来源：http://dvx.guowangkeji.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://rgz.tianlin.xyz

TS:   if (x == null) {}
来源：http://krq.jinghuilouyu.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://tmf.chenzaomai.com

Go:   if x == nil {}
来源：http://xzz.shuidangran.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hkj.fengsongda.top

C#:   if (x is null) {}
来源：http://paf.hongshengwenyu.top

[P07] 防抖与节流
来源：http://bms.bjfxy.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hvo.dashuyun.cn

PHP:  // 手写时间戳比较
来源：http://hqq.0kj1m.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mfh.cheryme.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ztr.cqqwz.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://uus.hywenlv.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://drd.jinghuilouyu.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ncy.havefunace.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://xgn.hywenlv.cn

[P08] 处理浮点精度问题
来源：http://xbs.jqgfzy.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://auv.xinyue.icu

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ski.nanxuanxn.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ywt.fehbvm.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://zwj.aibaodan.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://yat.meibo888.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://oew.zhoulong.xyz

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://zgh.xuetiantiany.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ryq.bjfxy.top

================================================================================
来源：http://qch.0kj1m.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ljm.bbcook.cn

================================================================================
来源：http://jfm.jqgfzy.top

[Q01] 创建表
来源：http://pri.fktsv.cn

CREATE TABLE users (
来源：http://maj.zhaomingkeji.xyz

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://jjo.svipenyu.cn

name VARCHAR(50) NOT NULL,
来源：http://yoz.svipenyu.cn

email VARCHAR(100) UNIQUE,
来源：http://aem.birdmap.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://kpg.ydjk.org.cn

);
来源：http://hfm.guannengcc.top

[Q02] 创建带外键的表
来源：http://vff.zhijiandao.cn

CREATE TABLE orders (
来源：http://bzp.xuetiantiany.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://jky.zhoulong.xyz

user_id INT NOT NULL,
来源：http://ouq.snrcjt.cn

amount DECIMAL(10, 2),
来源：http://yic.yangfankeji.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://kfe.hysaishi.cn

);
来源：http://jpy.shanyushiyangtech.top

[Q03] 增加列
来源：http://jnb.jinyuanbaomall.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://zul.chenzaomai.com

[Q04] 修改列类型
来源：http://ntm.zhiwuduotai.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://kae.zdqjudy.top

[Q05] 重命名列
来源：http://mda.zycfv.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://qeh.jinyuanbaomall.cn

[Q06] 删除列
来源：http://uyo.jinqigfzy.top

ALTER TABLE users DROP COLUMN age;
来源：http://jlc.jinghuilouyu.cn

[Q07] 删除表
来源：http://jae.zdbjq.cn

DROP TABLE IF EXISTS orders;
来源：http://rol.fktsv.cn

[Q08] 创建普通索引
来源：http://ywm.fzhhl.top

CREATE INDEX idx_users_email ON users(email);
来源：http://ogb.shzxlz.cn

[Q09] 创建唯一索引
来源：http://fes.xylfe.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ujk.hammf.cn

[Q10] 插入单行
来源：http://hnr.ctjpmb.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mpv.smart0.xyz

[Q11] 一次插入多行
来源：http://uas.gzhubu.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://upx.9152youxi.cn

[Q12] 插入后取自增 ID
来源：http://ovh.xziqi.cn

INSERT INTO users (name) VALUES ('C');
来源：http://pdx.bbcook.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://cpg.hnxiangtu.top

[Q13] 忽略重复插入
来源：http://mzh.hesvh.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ksz.xinyue.icu

[Q14] 存在则更新（upsert）
来源：http://okd.ppjwa.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://cpi.xuanzx.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://slp.shanyushiyangtech.top

[Q15] 查询全部
来源：http://vhx.aibaodan.cn

SELECT * FROM users;
来源：http://hva.kuanghao11.cn

[Q16] 查询指定列
来源：http://hjh.ctjpmb.com

SELECT id, name FROM users;
来源：http://sim.yvedp.cn

[Q17] 条件查询
来源：http://ati.tianlin.xyz

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://orf.vqdsnc.cn

[Q18] 模糊匹配
来源：http://jxp.zhongyouzk.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://eqw.0kj1m.cn

[Q19] 范围查询
来源：http://xuj.yongpay.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://yvy.gotoacloud.top

[Q20] IN 列表
来源：http://wbk.yueranfly.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://toe.c1oappe.top

[Q21] 空值判断
来源：http://thb.fzhhl.top

SELECT * FROM users WHERE email IS NULL;
来源：http://slm.zhijiandao.cn

[Q22] 排序
来源：http://ruc.tianlin.xyz

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://jad.epnwcf.com

[Q23] 分页
来源：http://wpd.pycfn.com

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://cco.tanke756.top

[Q24] 去重
来源：http://rry.wangdashe.top

SELECT DISTINCT city FROM users;
来源：http://duo.gzhubu.top

[Q25] 只取前 N 条
来源：http://yte.jlsjyb.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blw.ppjwa.cn

[Q26] 计数
来源：http://sty.shanyushiyangtech.top

SELECT COUNT(*) FROM users;
来源：http://xbl.cdnleiting.top

[Q27] 条件计数
来源：http://yjc.cheryme.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hoj.jinyuanbaomall.cn

[Q28] 求和与平均
来源：http://bua.shzxlz.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ile.svipenyu.cn

[Q29] 最大最小值
来源：http://kia.zhongyouzk.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://ujo.daria6918.cn

[Q30] 分组统计
来源：http://zxd.ppjwa.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://lla.xuetiantiany.cn

[Q31] 分组后过滤
来源：http://dgu.jqgufenzy.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://gis.nanxinkj.top

[Q32] 分组拼接字符串
来源：http://tzm.shangyingyoupin.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://dwx.52xcode.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://yjq.vehdjk.com

[Q33] 多列分组
来源：http://xai.zhaomingkeji.xyz

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://rrf.ydzc1.top

[Q34] 每组取第一条
来源：http://vfd.zhijiandao.cn

SELECT * FROM (
来源：http://upr.tarul.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://lwm.cucudq.cn

) t WHERE rn = 1;
来源：http://frc.guowangkeji.top

[Q35] 内连接
来源：http://vuy.xuanzx.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hgm.hnxiangtu.top

[Q36] 左连接
来源：http://pjt.fanxiaobao.xyz

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://pxp.bjfxy.top

[Q37] 右连接
来源：http://cve.havefunace.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://vqn.redwolf501.top

[Q38] 全外连接（PostgreSQL）
来源：http://hky.hammf.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://yyw.ppjwa.cn

[Q39] 自连接（查上下级）
来源：http://swn.shanyushiyangtech.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://gbr.meibo888.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://oag.jqgfzy.top

[Q40] 交叉连接（笛卡尔积）
来源：http://eww.zhijiandao.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://kto.c1oappe.top

[Q41] 多表连接
来源：http://ppw.cdnleiting.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://ngv.yueranfly.top

JOIN users u ON u.id = o.user_id
来源：http://bpy.tarul.cn

JOIN products p ON p.id = o.product_id;
来源：http://nrz.chenzaomai.com

[Q42] 连接条件附加过滤
来源：http://izl.tarul.cn

SELECT u.name, o.amount FROM users u
来源：http://fkd.redwolf501.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://rii.yj202588.top

[Q43] 标量子查询
来源：http://ppn.dashuyun.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://zmn.shanyushiyangkeji.top

[Q44] IN 子查询
来源：http://jtd.gotoacloud.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://inu.yfazqb.com

[Q45] EXISTS 判断存在
来源：http://eto.cashguo.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mgz.dianchejie.cn

[Q46] NOT EXISTS 判断不存在
来源：http://xgn.yongpay.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kdw.gogol.net.cn

[Q47] 与平均值比较
来源：http://euw.zhengqikj.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://xsu.yvedp.cn

[Q48] CTE 公用表表达式
来源：http://hks.yj20258.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://qbr.c1oappe.top

SELECT * FROM t WHERE c > 5;
来源：http://rwv.cdnleiting.top

[Q49] 更新单行
来源：http://inq.uphjek.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://tnj.meibo888.top

[Q50] 批量更新
来源：http://pwx.shanyushiyangkeji.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wyo.jinqigufen.top

[Q51] 用子查询更新
来源：http://ade.yj20258888.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://njo.birdmap.top

[Q52] 删除指定行
来源：http://oho.chenlongwang.top

DELETE FROM users WHERE id = 10;
来源：http://hng.yj202588.top

[Q53] 按条件删除
来源：http://upq.kuanghao11.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://eqj.fehbvm.com

[Q54] 清空表
来源：http://hab.sufxvd.cn

TRUNCATE TABLE logs;
来源：http://fku.yangfankeji.com

[Q55] 排名（并列占位）
来源：http://cap.yueranfly.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://zfd.guannengcc.top

[Q56] 密集排名（并列不占位）
来源：http://stw.jqgufenzy.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://vqu.sjlbkw.cn

[Q57] 行号
来源：http://czb.ybcxt.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://khg.zhengqikj.top

[Q58] 累计求和
来源：http://bke.zhengqikj.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://llw.yj202588.top

[Q59] 分组内累计
来源：http://oef.smart0.xyz

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://yus.jlsjyb.cn

[Q60] 取上一行 / 下一行
来源：http://dbc.xziqi.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://uaj.tian-w.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://duv.uphjek.com

[Q61] 移动平均
来源：http://nhs.aizwys.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://zxm.hnqzz.top

[Q62] 分组占比
来源：http://oez.zhiwuduotai.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wdh.vehdjk.com

[Q63] 开启事务
来源：http://rln.jianghu66.top

START TRANSACTION;                -- 或 BEGIN
来源：http://psw.hammf.cn

[Q64] 提交事务
来源：http://rqj.shangyingyoupin.top

COMMIT;
来源：http://vpn.jiagoushi.top

[Q65] 回滚事务
来源：http://aqg.xingfuxueyuan.xyz

ROLLBACK;
来源：http://ijz.xuanzx.com

[Q66] 行锁查询
来源：http://mqf.yuxming.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ghk.52xcode.cn

[Q67] 设置隔离级别
来源：http://asm.bbcook.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://tfy.jqgufenzy.top

[Q68] 保存点
来源：http://met.nwbrower.top

SAVEPOINT sp1;
来源：http://snp.jinghuilouyu.cn

ROLLBACK TO sp1;
来源：http://pog.52xcode.cn

[Q69] 查看执行计划
来源：http://rfp.yongpay.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ybr.xinyue.icu

[Q70] 更新统计信息
来源：http://rxd.havefunace.top

ANALYZE TABLE users;
来源：http://kqw.xuanzx.com

[Q71] 查看建表语句
来源：http://wnk.zhongyouzk.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://cms.hfpthk.cn

[Q72] 查看索引
来源：http://jjb.yongpay.top

SHOW INDEX FROM users;
来源：http://lac.hcnkem.com

[Q73] 查看表状态
来源：http://dzv.fengsongda.top

SHOW TABLE STATUS LIKE 'users';
来源：http://jiz.cucudq.cn

[Q74] 强制使用索引
来源：http://yur.nanxuanxn.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://xjk.ppjwa.cn

[Q75] 日期格式化
来源：http://kuf.sweek.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://jop.hesvh.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://new.tarul.cn

[Q76] 按天统计
来源：http://ldf.ydzc1.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wab.gaohongyu789.top

[Q77] 时间加减
来源：http://woq.zhaomingkeji.xyz

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://rub.birdmap.top

[Q78] 当前时间
来源：http://uyy.jqgfzy.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ioq.ybcxt.top

[Q79] 字符串拼接
来源：http://bni.yangfankeji.com

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ftk.52xcode.cn

[Q80] 字符串截取
来源：http://fiw.yanxiufei.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://aht.guowangkeji.top

[Q81] 字符串替换
来源：http://avf.svipenyu.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://eci.hcnkem.com

[Q82] 字符长度与字节长度
来源：http://eei.svipenyu.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://isf.bjfxy.top

[Q83] 大小写转换
来源：http://xdh.wangdashe.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mcf.sxryk.cn

[Q84] 去除首尾空格
来源：http://kdn.hnxiangtu.top

SELECT TRIM(name) FROM users;
来源：http://cse.hfpthk.cn

[Q85] 数值取整
来源：http://ars.sweek.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://avm.chenjidiqi.icu

[Q86] 读取 JSON 字段
来源：http://hbe.shuidangran.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://kuk.zycfv.cn

[Q87] JSON 字段做条件
来源：http://vym.shzxlz.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://pll.sjlbkw.cn

[Q88] 行转列（条件聚合）
来源：http://eep.fehbvm.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://miz.yongpay.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://khe.wangshuangyany.cn

[Q89] 判断表是否存在
来源：http://kfw.xylfe.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://bfd.svipenyu.cn

[Q90] 生成序号列
来源：http://bgo.hcnkem.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://dmt.9152youxi.cn

================================================================================
来源：http://nxs.yj202588.top

R. Bash 专题
来源：http://dlp.kuanghao11.cn

================================================================================
来源：http://ggf.iojbl.cn

[R01] shebang 与严格模式
来源：http://ayh.zhiwuduotai.top

#!/usr/bin/env bash
来源：http://wkj.jqgfzy.top

set -euo pipefail
来源：http://xxt.havefunace.top

[R02] 变量赋值与使用
来源：http://eej.ehwqpu.com

name="Tom"; echo "$name"
来源：http://igy.chenjidiqi.icu

[R03] 只读变量
来源：http://ssu.andypj.xyz

readonly PI=3.14
来源：http://rju.dashuyun.cn

[R04] 位置参数
来源：http://ods.uphjek.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://cqf.zdbjq.cn

[R05] 参数默认值
来源：http://gka.yuanzhike.top

name="${1:-default}"
来源：http://mte.yuxming.cn

[R06] 判断命令是否存在
来源：http://hws.jyoumei.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://gjb.sweek.top

[R07] if 判断文件
来源：http://yeq.hesvh.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ibm.sxryk.cn

[R08] 数值比较
来源：http://njc.hongshengwenyu.top

if (( a > b )); then echo "a 更大"; fi
来源：http://bxy.shzxlz.cn

[R09] 字符串比较
来源：http://thc.xuetiantiany.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ega.xingfuxueyuan.xyz

[R10] 正则匹配
来源：http://raa.zdqjudy.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://xrf.tian-w.cn

[R11] case 多分支
来源：http://tpi.tianlin.xyz

case "$1" in
来源：http://jfv.hcnkem.com

start) echo "启动" ;;
来源：http://tob.gzhubu.top

stop)  echo "停止" ;;
来源：http://sfa.havefunace.top

*)     echo "未知命令" ;;
来源：http://rpx.havefunace.top

esac
来源：http://shr.chenjidiqi.icu

[R12] for 遍历文件
来源：http://zal.xingfuxueyuan.xyz

for f in *.txt; do echo "$f"; done
来源：http://jaz.jyoumei.cn

[R13] for 计数循环
来源：http://gay.xinyue.icu

for i in {1..10}; do echo "$i"; done
来源：http://mrd.ivvv.top

[R14] C 风格 for
来源：http://tqy.iojbl.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://yft.c1oappe.top

[R15] while 逐行读文件
来源：http://spb.fktsv.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mqt.sufxvd.cn

[R16] until 等待条件
来源：http://dqm.hammf.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://vgk.xuetiantiany.cn

[R17] 数组定义与取值
来源：http://ksz.jqgufenzy.top

arr=(a b c); echo "${arr[0]}"
来源：http://hcb.pengpengdd.cyou

[R18] 遍历数组
来源：http://jos.chenjidiqi.icu

for x in "${arr[@]}"; do echo "$x"; done
来源：http://zvv.hysaishi.cn

[R19] 数组长度
来源：http://onq.vqdsnc.cn

echo "${#arr[@]}"
来源：http://huy.sxryk.cn

[R20] 关联数组（字典）
来源：http://ant.tian-w.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ate.xingfuxueyuan.xyz

[R21] 字符串长度
来源：http://vof.xuanzx.com

echo "${#s}"
来源：http://uun.gzhubu.top

[R22] 截取子串
来源：http://lfo.yanxiufei.cn

echo "${s:0:5}"
来源：http://fcv.ywan-chungtsiang.top

[R23] 字符串替换
来源：http://yxc.jqgfzy.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://abk.fktsv.cn

[R24] 大小写转换
来源：http://pck.meibo888.top

echo "${s^^}"; echo "${s,,}"
来源：http://yxy.c1oappe.top

[R25] 去后缀 / 去前缀
来源：http://tjr.mhx1999.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://hrf.jqgfzy.top

[R26] 命令替换
来源：http://nsa.tianlin.xyz

now=$(date +%F); echo "$now"
来源：http://hld.aizwys.cn

[R27] 算术展开
来源：http://lzh.nwbrower.top

echo $((1 + 2 * 3))
来源：http://fzw.xuetiantiany.cn

[R28] 浮点运算
来源：http://afq.ctjpmb.com

echo "scale=2; 10/3" | bc
来源：http://oer.yanxiufei.cn

[R29] 定义函数
来源：http://zfz.cdnleiting.top


<!-- 参考信息 -->