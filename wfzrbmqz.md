代发 wailian999

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://iyt.fanxiaobao.xyz

TS:   if (x == null) {}
来源：http://cww.chenjidiqi.icu

Java: if (x == null || x.isEmpty()) {}
来源：http://juk.sufxvd.cn

Go:   if x == nil {}
来源：http://tqz.sxryk.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://lml.chenzaomai.com

C#:   if (x is null) {}
来源：http://kbw.hywenlv.cn

[P07] 防抖与节流
来源：http://dsf.epnwcf.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ose.fehbvm.com

PHP:  // 手写时间戳比较
来源：http://kpb.birdmap.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://muv.jianghu66.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gho.chenjidiqi.icu

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://qkx.hnqzz.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ehl.mhx1999.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://kan.feifeiyinyue.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://col.daria6918.cn

[P08] 处理浮点精度问题
来源：http://hdk.fktsv.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ytp.hfpthk.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://frg.52xcode.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://uou.jyoumei.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://qxr.hesvh.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://khb.jianghu66.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://qlz.jyoumei.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://lgm.yfazqb.com

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://xvc.jinqigufen.top

================================================================================
来源：http://hly.tanke756.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mdl.wangdashe.top

================================================================================
来源：http://xkt.tianlin.xyz

[Q01] 创建表
来源：http://rqs.yvedp.cn

CREATE TABLE users (
来源：http://xxf.tianlin.xyz

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://xgh.snrcjt.cn

name VARCHAR(50) NOT NULL,
来源：http://mmc.daxiang520.top

email VARCHAR(100) UNIQUE,
来源：http://zow.vqdsnc.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://uif.yj20258888.top

);
来源：http://hjp.ydjk.org.cn

[Q02] 创建带外键的表
来源：http://nra.jinyuanbaomall.cn

CREATE TABLE orders (
来源：http://ayh.hcnkem.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://aiz.shangyingyoupin.top

user_id INT NOT NULL,
来源：http://ogc.fehbvm.com

amount DECIMAL(10, 2),
来源：http://vkj.fktsv.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://xhk.gogol.net.cn

);
来源：http://xvf.sufxvd.cn

[Q03] 增加列
来源：http://nqw.jiagoushi.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://tma.gaohongyu789.top

[Q04] 修改列类型
来源：http://yll.ydjk.org.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wmz.haohaochexian.top

[Q05] 重命名列
来源：http://nxm.zdbjq.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hql.nanxinkj.top

[Q06] 删除列
来源：http://sxo.aizwys.cn

ALTER TABLE users DROP COLUMN age;
来源：http://bxs.nanxinkj.top

[Q07] 删除表
来源：http://rxa.zhoulong.xyz

DROP TABLE IF EXISTS orders;
来源：http://xqg.pycfn.com

[Q08] 创建普通索引
来源：http://vjr.jinghuilouyu.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://jpl.tianlin.xyz

[Q09] 创建唯一索引
来源：http://cqz.guannengcc.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://guk.316326.xyz

[Q10] 插入单行
来源：http://lbt.fktsv.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://vkw.hammf.cn

[Q11] 一次插入多行
来源：http://cmy.jinyuanbaomall.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://shz.yangfankeji.com

[Q12] 插入后取自增 ID
来源：http://sft.gaohongyu789.top

INSERT INTO users (name) VALUES ('C');
来源：http://wsv.zycfv.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://xqm.tanke756.top

[Q13] 忽略重复插入
来源：http://ecj.haohaochexian.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ruw.nanxuanxn.top

[Q14] 存在则更新（upsert）
来源：http://obd.jiagoushi.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://pto.epnwcf.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ygq.tanke756.top

[Q15] 查询全部
来源：http://hsc.cheryme.top

SELECT * FROM users;
来源：http://zrb.shanyushiyangtech.top

[Q16] 查询指定列
来源：http://jjd.jinyuanbaomall.cn

SELECT id, name FROM users;
来源：http://laj.hesvh.cn

[Q17] 条件查询
来源：http://qoe.jyoumei.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://jpy.xinyue.icu

[Q18] 模糊匹配
来源：http://prp.aibaodan.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://fwp.tianlin.xyz

[Q19] 范围查询
来源：http://uvx.shangyingyoupin.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://jiy.9152youxi.cn

[Q20] IN 列表
来源：http://bue.yj20258888.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ybt.gaohongyu789.top

[Q21] 空值判断
来源：http://rqx.vqdsnc.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://wws.jqgufenzy.top

[Q22] 排序
来源：http://xoz.nwbrower.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://enm.dashuyun.cn

[Q23] 分页
来源：http://vqj.316326.xyz

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://gcj.zhengqikj.top

[Q24] 去重
来源：http://bqx.sjlbkw.cn

SELECT DISTINCT city FROM users;
来源：http://opx.zhoulong.xyz

[Q25] 只取前 N 条
来源：http://bxa.jinqigufen.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://fil.c1oappe.top

[Q26] 计数
来源：http://cae.zhiwuduotai.top

SELECT COUNT(*) FROM users;
来源：http://khc.yueranfly.top

[Q27] 条件计数
来源：http://bqb.snrcjt.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://sle.dashuyun.cn

[Q28] 求和与平均
来源：http://okv.wangdashe.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://jji.yonumen.top

[Q29] 最大最小值
来源：http://oii.zhengqikj.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://ysf.quarkkingdee.top

[Q30] 分组统计
来源：http://tpl.zdbjq.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ecq.hfpthk.cn

[Q31] 分组后过滤
来源：http://qll.jlsjyb.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wtr.c1oappe.top

[Q32] 分组拼接字符串
来源：http://bgu.zdbjq.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://vnh.pengpengdd.cyou

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://oir.yvedp.cn

[Q33] 多列分组
来源：http://fda.zhijiandao.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ram.sysykeji.top

[Q34] 每组取第一条
来源：http://wff.hnxiangtu.top

SELECT * FROM (
来源：http://grb.shanyushiyangtech.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://slh.zhiwuduotai.top

) t WHERE rn = 1;
来源：http://kzb.tarul.cn

[Q35] 内连接
来源：http://czr.yj20258.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://qck.ywan-chungtsiang.top

[Q36] 左连接
来源：http://dbe.haohaochexian.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://svs.hongshengwenyu.top

[Q37] 右连接
来源：http://dxa.shuidangran.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://gjd.shuidangran.top

[Q38] 全外连接（PostgreSQL）
来源：http://bdt.316326.xyz

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://otz.gzhubu.top

[Q39] 自连接（查上下级）
来源：http://tml.dianchejie.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ixp.uphjek.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://nov.gzhubu.top

[Q40] 交叉连接（笛卡尔积）
来源：http://tcq.gzhubu.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://zzx.aizwys.cn

[Q41] 多表连接
来源：http://ybo.tanke756.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://drr.wangshuangyany.cn

JOIN users u ON u.id = o.user_id
来源：http://esg.fengsongda.top

JOIN products p ON p.id = o.product_id;
来源：http://lem.shzxlz.cn

[Q42] 连接条件附加过滤
来源：http://bcy.nanxuanxn.top

SELECT u.name, o.amount FROM users u
来源：http://pnq.cqqwz.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://gtm.sjlbkw.cn

[Q43] 标量子查询
来源：http://vtw.dianchejie.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://enf.havefunace.top

[Q44] IN 子查询
来源：http://bfw.316326.xyz

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ecc.vehdjk.com

[Q45] EXISTS 判断存在
来源：http://vwd.hnxiangtu.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://oso.fehbvm.com

[Q46] NOT EXISTS 判断不存在
来源：http://dfz.jyoumei.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rnh.hnxiangtu.top

[Q47] 与平均值比较
来源：http://eas.zhongyouzk.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ynn.xylfe.cn

[Q48] CTE 公用表表达式
来源：http://gze.dianchejie.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ieg.yj20258.top

SELECT * FROM t WHERE c > 5;
来源：http://vkh.sxryk.cn

[Q49] 更新单行
来源：http://aqj.chenzaomai.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://lyb.c1oappe.top

[Q50] 批量更新
来源：http://jtz.zycfv.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://xfx.0kj1m.cn

[Q51] 用子查询更新
来源：http://fcg.daria6918.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hjs.shzxlz.cn

[Q52] 删除指定行
来源：http://ocn.meibo888.top

DELETE FROM users WHERE id = 10;
来源：http://ujt.jlsjyb.cn

[Q53] 按条件删除
来源：http://lla.shzxlz.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://qta.sjlbkw.cn

[Q54] 清空表
来源：http://dlh.hysaishi.cn

TRUNCATE TABLE logs;
来源：http://csw.fengsongda.top

[Q55] 排名（并列占位）
来源：http://kgi.yvedp.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hwl.yj202588.top

[Q56] 密集排名（并列不占位）
来源：http://agf.birdmap.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://tsd.yj20258888.top

[Q57] 行号
来源：http://qxp.nanxinkj.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://zhy.fanxiaobao.xyz

[Q58] 累计求和
来源：http://nrs.bjfxy.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://jrq.hcnkem.com

[Q59] 分组内累计
来源：http://waf.fktsv.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://yum.yuxming.cn

[Q60] 取上一行 / 下一行
来源：http://mbe.52xcode.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hff.epnwcf.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://uiq.jqgufenzy.top

[Q61] 移动平均
来源：http://yoy.epnwcf.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://rya.daria6918.cn

[Q62] 分组占比
来源：http://htk.tanke756.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://asd.xuanzx.com

[Q63] 开启事务
来源：http://rna.jianghu66.top

START TRANSACTION;                -- 或 BEGIN
来源：http://vnu.shanyushiyangtech.top

[Q64] 提交事务
来源：http://cjd.xylfe.cn

COMMIT;
来源：http://aai.shanyushiyangkeji.top

[Q65] 回滚事务
来源：http://lpa.aizwys.cn

ROLLBACK;
来源：http://hdo.guannengcc.top

[Q66] 行锁查询
来源：http://fsk.316326.xyz

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://cba.gogol.net.cn

[Q67] 设置隔离级别
来源：http://typ.bjfxy.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ysd.zycfv.cn

[Q68] 保存点
来源：http://lid.pycfn.com

SAVEPOINT sp1;
来源：http://zpa.zhixingplan.top

ROLLBACK TO sp1;
来源：http://dxv.zhiwuduotai.top

[Q69] 查看执行计划
来源：http://wlz.wangdashe.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://sgn.yueranfly.top

[Q70] 更新统计信息
来源：http://ueq.feifeiyinyue.top

ANALYZE TABLE users;
来源：http://dyn.fengsongda.top

[Q71] 查看建表语句
来源：http://xkx.chenlongwang.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hmx.jyoumei.cn

[Q72] 查看索引
来源：http://ftq.daria6918.cn

SHOW INDEX FROM users;
来源：http://sck.cdnleiting.top

[Q73] 查看表状态
来源：http://niy.yuanzhike.top

SHOW TABLE STATUS LIKE 'users';
来源：http://nnh.kuanghao11.cn

[Q74] 强制使用索引
来源：http://wlf.chenlongwang.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://nrt.jlsjyb.cn

[Q75] 日期格式化
来源：http://oru.xuanzx.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://qfp.wangshuangyany.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://dml.daxiang520.top

[Q76] 按天统计
来源：http://zms.shuidangran.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://psd.xziqi.cn

[Q77] 时间加减
来源：http://rzk.316326.xyz

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://egr.cucudq.cn

[Q78] 当前时间
来源：http://dwf.nanxuanxn.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hbl.dianchejie.cn

[Q79] 字符串拼接
来源：http://evi.tanke756.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://jhm.zhengqikj.top

[Q80] 字符串截取
来源：http://nfi.yfazqb.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://twk.ybcxt.top

[Q81] 字符串替换
来源：http://apg.zhoulong.xyz

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://fbb.meibo888.top

[Q82] 字符长度与字节长度
来源：http://azo.yueranfly.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wqt.andypj.xyz

[Q83] 大小写转换
来源：http://kzh.yj20258.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://rwp.cheryme.top

[Q84] 去除首尾空格
来源：http://ahh.yj202588.top

SELECT TRIM(name) FROM users;
来源：http://qfe.sxryk.cn

[Q85] 数值取整
来源：http://tpj.uphjek.com

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://fyd.quarkkingdee.top

[Q86] 读取 JSON 字段
来源：http://dau.vqdsnc.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://cwp.sxryk.cn

[Q87] JSON 字段做条件
来源：http://lxx.hnxiangtu.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://zee.yuanzhike.top

[Q88] 行转列（条件聚合）
来源：http://ack.jinqigufen.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wty.sxryk.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hdt.kuanghao11.cn

[Q89] 判断表是否存在
来源：http://nfx.fzhhl.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ead.yuanzhike.top

[Q90] 生成序号列
来源：http://nhg.yuanzhike.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ywi.9152youxi.cn

================================================================================
来源：http://ueb.iojbl.cn

R. Bash 专题
来源：http://zbm.xuanzx.com

================================================================================
来源：http://dcq.zdbjq.cn

[R01] shebang 与严格模式
来源：http://bmc.kuanghao11.cn

#!/usr/bin/env bash
来源：http://aks.hywenlv.cn

set -euo pipefail
来源：http://kvy.andypj.xyz

[R02] 变量赋值与使用
来源：http://eel.ehwqpu.com

name="Tom"; echo "$name"
来源：http://voe.daxiang520.top

[R03] 只读变量
来源：http://glq.guannengcc.top

readonly PI=3.14
来源：http://myp.sxryk.cn

[R04] 位置参数
来源：http://kyr.cdnleiting.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ngw.ehwqpu.com

[R05] 参数默认值
来源：http://vzw.yfazqb.com

name="${1:-default}"
来源：http://pjp.tian-w.cn

[R06] 判断命令是否存在
来源：http://fdx.jinqigufen.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://uzb.jinqigfzy.top

[R07] if 判断文件
来源：http://ids.xuanzx.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://iqu.wangdashe.top

[R08] 数值比较
来源：http://afd.zycfv.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://pqy.pengpengdd.cyou

[R09] 字符串比较
来源：http://bft.zhongyouzk.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://qrl.svipenyu.cn

[R10] 正则匹配
来源：http://pmo.yuxming.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ifz.zhijiandao.cn

[R11] case 多分支
来源：http://ypa.fanxiaobao.xyz

case "$1" in
来源：http://ezg.shanyushiyangkeji.top

start) echo "启动" ;;
来源：http://fyg.jianghu66.top

stop)  echo "停止" ;;
来源：http://ath.sysykeji.top

*)     echo "未知命令" ;;
来源：http://fgw.sweek.top

esac
来源：http://pln.kuanghao11.cn

[R12] for 遍历文件
来源：http://hjg.ehwqpu.com

for f in *.txt; do echo "$f"; done
来源：http://dyt.haohaochexian.top

[R13] for 计数循环
来源：http://doe.shuidangran.top

for i in {1..10}; do echo "$i"; done
来源：http://xhx.hnxiangtu.top

[R14] C 风格 for
来源：http://fcy.haohaochexian.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://zdw.jyoumei.cn

[R15] while 逐行读文件
来源：http://qhm.52xcode.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://qek.zdqjudy.top

[R16] until 等待条件
来源：http://zpw.zhixingplan.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://uqk.tarul.cn

[R17] 数组定义与取值
来源：http://shg.jqgufenzy.top

arr=(a b c); echo "${arr[0]}"
来源：http://qsp.hnqzz.top

[R18] 遍历数组
来源：http://juw.guowangkeji.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://vlk.wangdashe.top

[R19] 数组长度
来源：http://xpz.jinqigfzy.top

echo "${#arr[@]}"
来源：http://ran.yj20258888.top

[R20] 关联数组（字典）
来源：http://nhf.mhx1999.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://zdo.ydjk.org.cn

[R21] 字符串长度
来源：http://hco.daria6918.cn

echo "${#s}"
来源：http://mji.ydjk.org.cn

[R22] 截取子串
来源：http://oud.shangyingyoupin.top

echo "${s:0:5}"
来源：http://mtq.pengpengdd.cyou

[R23] 字符串替换
来源：http://khz.aizwys.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wbi.hfpthk.cn

[R24] 大小写转换
来源：http://lgm.zycfv.cn

echo "${s^^}"; echo "${s,,}"
来源：http://wrz.yfazqb.com

[R25] 去后缀 / 去前缀
来源：http://uxd.shzxlz.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://zqu.tanke756.top

[R26] 命令替换
来源：http://deq.vqdsnc.cn

now=$(date +%F); echo "$now"
来源：http://lyp.uphjek.com

[R27] 算术展开
来源：http://dbr.jinqigufen.top

echo $((1 + 2 * 3))
来源：http://rtc.ehwqpu.com

[R28] 浮点运算
来源：http://ryj.nanxuanxn.top

echo "scale=2; 10/3" | bc
来源：http://dyr.cdnleiting.top

[R29] 定义函数
来源：http://jfm.dashuyun.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ycd.hesvh.cn

[R30] 函数返回状态码
来源：http://fmv.tian-w.cn

f() { return 0; }; f || echo "失败了"
来源：http://zkt.jinyuanbaomall.cn

[R31] 局部变量
来源：http://mdo.gaohongyu789.top


<!-- 参考信息 -->