代发 wailian999

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://dxp.chenlongwang.top

TS:   if (x == null) {}
来源：http://mtp.shanyushiyangkeji.top

Java: if (x == null || x.isEmpty()) {}
来源：http://omx.daria6918.cn

Go:   if x == nil {}
来源：http://ggc.zycfv.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://laj.guannengcc.top

C#:   if (x is null) {}
来源：http://gxw.tanke756.top

[P07] 防抖与节流
来源：http://nrn.ywan-chungtsiang.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://jmn.fengsongda.top

PHP:  // 手写时间戳比较
来源：http://lwl.nanxinkj.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hno.fehbvm.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://oxp.shanyushiyangtech.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://dig.ppjwa.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://boj.jqgfzy.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://idc.chenjidiqi.icu

C#:   // 用 System.Timers.Timer 重置实现
来源：http://pzh.xziqi.cn

[P08] 处理浮点精度问题
来源：http://ppp.jinyuanbaomall.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://efo.zhiwuduotai.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wke.yongpay.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://tpz.zhaomingkeji.xyz

TS:   (0.1 + 0.2).toFixed(2)
来源：http://fam.cucudq.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://afy.jianghu66.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://jvh.jinyuanbaomall.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://prg.fengsongda.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://pjm.fktsv.cn

================================================================================
来源：http://veh.316326.xyz

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://irq.zhoulong.xyz

================================================================================
来源：http://npi.hesvh.cn

[Q01] 创建表
来源：http://jcl.dianchejie.cn

CREATE TABLE users (
来源：http://ibw.fengsongda.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://knz.vehdjk.com

name VARCHAR(50) NOT NULL,
来源：http://ayx.tarul.cn

email VARCHAR(100) UNIQUE,
来源：http://sna.vehdjk.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ezc.shanyushiyangkeji.top

);
来源：http://xej.fktsv.cn

[Q02] 创建带外键的表
来源：http://nol.bbcook.cn

CREATE TABLE orders (
来源：http://sbs.jinghuilouyu.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://xsk.hcnkem.com

user_id INT NOT NULL,
来源：http://qfd.tarul.cn

amount DECIMAL(10, 2),
来源：http://nvl.bbcook.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ixy.dianchejie.cn

);
来源：http://aet.redwolf501.top

[Q03] 增加列
来源：http://cmw.shanyushiyangtech.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://alt.shanyushiyangkeji.top

[Q04] 修改列类型
来源：http://lwj.nanxuanxn.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://lnj.tanke756.top

[Q05] 重命名列
来源：http://zde.yanxiufei.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://xzq.jqgfzy.top

[Q06] 删除列
来源：http://nnx.ydjk.org.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ust.zhixingplan.top

[Q07] 删除表
来源：http://viu.snrcjt.cn

DROP TABLE IF EXISTS orders;
来源：http://swm.hnxiangtu.top

[Q08] 创建普通索引
来源：http://zga.shanyushiyangkeji.top

CREATE INDEX idx_users_email ON users(email);
来源：http://yej.gzhubu.top

[Q09] 创建唯一索引
来源：http://eam.xingfuxueyuan.xyz

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mlk.yongpay.top

[Q10] 插入单行
来源：http://twh.fzhhl.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://tvu.ctjpmb.com

[Q11] 一次插入多行
来源：http://ghe.smart0.xyz

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://aoy.hcnkem.com

[Q12] 插入后取自增 ID
来源：http://ybc.svipenyu.cn

INSERT INTO users (name) VALUES ('C');
来源：http://hkp.wangdashe.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://dwd.jqgfzy.top

[Q13] 忽略重复插入
来源：http://lmv.ppjwa.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://nvo.jinqigfzy.top

[Q14] 存在则更新（upsert）
来源：http://rii.jyoumei.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://agq.hammf.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://uac.gaohongyu789.top

[Q15] 查询全部
来源：http://zil.xinyue.icu

SELECT * FROM users;
来源：http://shh.hnqzz.top

[Q16] 查询指定列
来源：http://eer.jinyuanbaomall.cn

SELECT id, name FROM users;
来源：http://kee.hammf.cn

[Q17] 条件查询
来源：http://iju.jinqigfzy.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://cmt.52xcode.cn

[Q18] 模糊匹配
来源：http://nwf.yj202588.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://zog.xziqi.cn

[Q19] 范围查询
来源：http://jhd.jqgfzy.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://yzr.tian-w.cn

[Q20] IN 列表
来源：http://fmo.shangyingyoupin.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://xtb.jyoumei.cn

[Q21] 空值判断
来源：http://guu.bjfxy.top

SELECT * FROM users WHERE email IS NULL;
来源：http://yje.smart0.xyz

[Q22] 排序
来源：http://lhu.redwolf501.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://nvu.smart0.xyz

[Q23] 分页
来源：http://ldn.daria6918.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://flm.nanxinkj.top

[Q24] 去重
来源：http://ipu.quarkkingdee.top

SELECT DISTINCT city FROM users;
来源：http://msn.yj20258.top

[Q25] 只取前 N 条
来源：http://cos.fanxiaobao.xyz

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wqg.dianchejie.cn

[Q26] 计数
来源：http://uct.guannengcc.top

SELECT COUNT(*) FROM users;
来源：http://fwb.daria6918.cn

[Q27] 条件计数
来源：http://hlh.yj202588.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://pvk.hcnkem.com

[Q28] 求和与平均
来源：http://cfm.fanxiaobao.xyz

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://imd.shangyingyoupin.top

[Q29] 最大最小值
来源：http://iak.cashguo.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://typ.wangdashe.top

[Q30] 分组统计
来源：http://fup.shanyushiyangtech.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://sdu.fengsongda.top

[Q31] 分组后过滤
来源：http://zmm.guannengcc.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://omw.cqqwz.cn

[Q32] 分组拼接字符串
来源：http://hmk.fehbvm.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://pno.gzhubu.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://oow.gaohongyu789.top

[Q33] 多列分组
来源：http://zfw.hcnkem.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://jpe.zhengqikj.top

[Q34] 每组取第一条
来源：http://dfh.jqgfzy.top

SELECT * FROM (
来源：http://jmr.epnwcf.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://uvc.gotoacloud.top

) t WHERE rn = 1;
来源：http://szp.jinyuanbaomall.cn

[Q35] 内连接
来源：http://tmx.zdqjudy.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://fyw.zdqjudy.top

[Q36] 左连接
来源：http://sux.zdbjq.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://jnx.shanyushiyangtech.top

[Q37] 右连接
来源：http://lkh.yueranfly.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://gmh.ywan-chungtsiang.top

[Q38] 全外连接（PostgreSQL）
来源：http://qic.aibaodan.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://dcu.fanxiaobao.xyz

[Q39] 自连接（查上下级）
来源：http://uhg.zhoulong.xyz

SELECT e.name, m.name AS manager FROM employees e
来源：http://pzd.hesvh.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ftc.ydjk.org.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://nef.dianchejie.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://dil.pengpengdd.cyou

[Q41] 多表连接
来源：http://tnj.aibaodan.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ezm.tanke756.top

JOIN users u ON u.id = o.user_id
来源：http://ady.yuxming.cn

JOIN products p ON p.id = o.product_id;
来源：http://udh.bjfxy.top

[Q42] 连接条件附加过滤
来源：http://dtx.316326.xyz

SELECT u.name, o.amount FROM users u
来源：http://wji.yangfankeji.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://qme.yj20258888.top

[Q43] 标量子查询
来源：http://fcc.shuidangran.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://iuw.jinghuilouyu.cn

[Q44] IN 子查询
来源：http://jcd.epnwcf.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://okp.ydzc1.top

[Q45] EXISTS 判断存在
来源：http://zbl.epnwcf.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fjb.meibo888.top

[Q46] NOT EXISTS 判断不存在
来源：http://vgo.fanxiaobao.xyz

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://huy.tarul.cn

[Q47] 与平均值比较
来源：http://raw.dianchejie.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://vez.yangfankeji.com

[Q48] CTE 公用表表达式
来源：http://glv.zdqjudy.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://udg.tanke756.top

SELECT * FROM t WHERE c > 5;
来源：http://iyf.cdnleiting.top

[Q49] 更新单行
来源：http://qew.nanxinkj.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://bsg.uphjek.com

[Q50] 批量更新
来源：http://xqb.ydjk.org.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://zmr.mhx1999.top

[Q51] 用子查询更新
来源：http://ssn.xuetiantiany.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://rtb.sjlbkw.cn

[Q52] 删除指定行
来源：http://jbh.yvedp.cn

DELETE FROM users WHERE id = 10;
来源：http://iir.sweek.top

[Q53] 按条件删除
来源：http://jmd.ppjwa.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://pzd.chenzaomai.com

[Q54] 清空表
来源：http://sok.9152youxi.cn

TRUNCATE TABLE logs;
来源：http://ezm.yfazqb.com

[Q55] 排名（并列占位）
来源：http://xqb.gaohongyu789.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://vtc.nanxuanxn.top

[Q56] 密集排名（并列不占位）
来源：http://qgm.shangyingyoupin.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ysx.fehbvm.com

[Q57] 行号
来源：http://mmg.birdmap.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://jlw.haohaochexian.top

[Q58] 累计求和
来源：http://xzo.gzhubu.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hwz.xziqi.cn

[Q59] 分组内累计
来源：http://jie.zdqjudy.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://swx.zhoulong.xyz

[Q60] 取上一行 / 下一行
来源：http://xhd.sjlbkw.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://yst.xylfe.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://fcx.fengsongda.top

[Q61] 移动平均
来源：http://mot.dashuyun.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ysb.zhongyouzk.top

[Q62] 分组占比
来源：http://tna.vqdsnc.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://cua.c1oappe.top

[Q63] 开启事务
来源：http://zim.yongpay.top

START TRANSACTION;                -- 或 BEGIN
来源：http://xvg.kuanghao11.cn

[Q64] 提交事务
来源：http://fzr.chenlongwang.top

COMMIT;
来源：http://zbg.ywan-chungtsiang.top

[Q65] 回滚事务
来源：http://lrg.dianchejie.cn

ROLLBACK;
来源：http://ogz.jinyuanbaomall.cn

[Q66] 行锁查询
来源：http://hyb.yvedp.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://sro.jqgufenzy.top

[Q67] 设置隔离级别
来源：http://gvi.yfazqb.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://thl.xingfuxueyuan.xyz

[Q68] 保存点
来源：http://lnm.shzxlz.cn

SAVEPOINT sp1;
来源：http://cte.cheryme.top

ROLLBACK TO sp1;
来源：http://qem.cdnleiting.top

[Q69] 查看执行计划
来源：http://ykd.birdmap.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://rvs.dianchejie.cn

[Q70] 更新统计信息
来源：http://yoc.9152youxi.cn

ANALYZE TABLE users;
来源：http://uok.shanyushiyangtech.top

[Q71] 查看建表语句
来源：http://cwq.nanxinkj.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://bya.daxiang520.top

[Q72] 查看索引
来源：http://efb.bbcook.cn

SHOW INDEX FROM users;
来源：http://cln.shangyingyoupin.top

[Q73] 查看表状态
来源：http://vfq.yuanzhike.top

SHOW TABLE STATUS LIKE 'users';
来源：http://ocy.smart0.xyz

[Q74] 强制使用索引
来源：http://znh.ywan-chungtsiang.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://cmg.52xcode.cn

[Q75] 日期格式化
来源：http://gcc.fehbvm.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://bms.ydzc1.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://qxx.pengpengdd.cyou

[Q76] 按天统计
来源：http://jta.zhaomingkeji.xyz

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://jwx.meibo888.top

[Q77] 时间加减
来源：http://qkx.nwbrower.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://rim.snrcjt.cn

[Q78] 当前时间
来源：http://ijz.cdnleiting.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ett.zhijiandao.cn

[Q79] 字符串拼接
来源：http://ugj.quarkkingdee.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://abf.yangfankeji.com

[Q80] 字符串截取
来源：http://xjr.hywenlv.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://src.cucudq.cn

[Q81] 字符串替换
来源：http://euu.feifeiyinyue.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://qdy.zhaomingkeji.xyz

[Q82] 字符长度与字节长度
来源：http://czv.snrcjt.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hfi.fehbvm.com

[Q83] 大小写转换
来源：http://jza.hongshengwenyu.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://szh.ehwqpu.com

[Q84] 去除首尾空格
来源：http://kzn.zycfv.cn

SELECT TRIM(name) FROM users;
来源：http://hvq.jinqigufen.top

[Q85] 数值取整
来源：http://mrn.svipenyu.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://vgr.xinyue.icu

[Q86] 读取 JSON 字段
来源：http://wwz.yj20258.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://kwh.0kj1m.cn

[Q87] JSON 字段做条件
来源：http://hme.xylfe.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://eii.cdnleiting.top

[Q88] 行转列（条件聚合）
来源：http://qek.jlsjyb.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://kco.epnwcf.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://oqo.ctjpmb.com

[Q89] 判断表是否存在
来源：http://xod.cdnleiting.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://iga.yfazqb.com

[Q90] 生成序号列
来源：http://eed.zhiwuduotai.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://snj.guowangkeji.top

================================================================================
来源：http://ifk.cdnleiting.top

R. Bash 专题
来源：http://izl.fktsv.cn

================================================================================
来源：http://lmd.gotoacloud.top

[R01] shebang 与严格模式
来源：http://vzh.hesvh.cn

#!/usr/bin/env bash
来源：http://ivn.sysykeji.top

set -euo pipefail
来源：http://ujj.hcnkem.com

[R02] 变量赋值与使用
来源：http://ald.yangfankeji.com

name="Tom"; echo "$name"
来源：http://pdq.wangdashe.top

[R03] 只读变量
来源：http://nwd.jyoumei.cn

readonly PI=3.14
来源：http://tla.0kj1m.cn

[R04] 位置参数
来源：http://jfe.snrcjt.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://zdx.vqdsnc.cn

[R05] 参数默认值
来源：http://xuu.ehwqpu.com

name="${1:-default}"
来源：http://qbk.mhx1999.top

[R06] 判断命令是否存在
来源：http://flg.sysykeji.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://tto.zhijiandao.cn

[R07] if 判断文件
来源：http://yom.jiagoushi.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://gfa.pengpengdd.cyou

[R08] 数值比较
来源：http://gbq.52xcode.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://yna.bjfxy.top

[R09] 字符串比较
来源：http://pwj.cqqwz.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://swm.wangdashe.top

[R10] 正则匹配
来源：http://ysb.9152youxi.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://zkt.hammf.cn

[R11] case 多分支
来源：http://gui.sjlbkw.cn

case "$1" in
来源：http://ris.sweek.top

start) echo "启动" ;;
来源：http://ehj.zhaomingkeji.xyz

stop)  echo "停止" ;;
来源：http://tae.hysaishi.cn

*)     echo "未知命令" ;;
来源：http://jkm.cdnleiting.top

esac
来源：http://iqi.chenzaomai.com

[R12] for 遍历文件
来源：http://lgn.sxryk.cn

for f in *.txt; do echo "$f"; done
来源：http://vcl.yonumen.top

[R13] for 计数循环
来源：http://rjb.ctjpmb.com

for i in {1..10}; do echo "$i"; done
来源：http://iwv.sufxvd.cn

[R14] C 风格 for
来源：http://lwy.nanxinkj.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://lxm.cheryme.top

[R15] while 逐行读文件
来源：http://qto.ctjpmb.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hco.bjfxy.top

[R16] until 等待条件
来源：http://iab.sufxvd.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mde.cucudq.cn

[R17] 数组定义与取值
来源：http://ehm.meibo888.top

arr=(a b c); echo "${arr[0]}"
来源：http://dtf.quarkkingdee.top

[R18] 遍历数组
来源：http://dwh.cheryme.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://vet.jinqigfzy.top

[R19] 数组长度
来源：http://wfn.cashguo.top

echo "${#arr[@]}"
来源：http://uvq.sweek.top

[R20] 关联数组（字典）
来源：http://fdt.xuetiantiany.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://pux.cucudq.cn

[R21] 字符串长度
来源：http://lcu.svipenyu.cn

echo "${#s}"
来源：http://cwy.mhx1999.top

[R22] 截取子串
来源：http://ppi.dianchejie.cn

echo "${s:0:5}"
来源：http://qui.yongpay.top

[R23] 字符串替换
来源：http://bop.fanxiaobao.xyz

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://kce.shangyingyoupin.top

[R24] 大小写转换
来源：http://wzs.haohaochexian.top

echo "${s^^}"; echo "${s,,}"
来源：http://cgj.fehbvm.com

[R25] 去后缀 / 去前缀
来源：http://dqy.yonumen.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://okz.birdmap.top

[R26] 命令替换
来源：http://qhq.tian-w.cn

now=$(date +%F); echo "$now"
来源：http://ejr.ctjpmb.com

[R27] 算术展开
来源：http://psw.wangshuangyany.cn

echo $((1 + 2 * 3))
来源：http://njl.chenzaomai.com

[R28] 浮点运算
来源：http://plo.sxryk.cn

echo "scale=2; 10/3" | bc
来源：http://dty.feifeiyinyue.top

[R29] 定义函数
来源：http://huq.vqdsnc.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://zpq.jinqigfzy.top

[R30] 函数返回状态码
来源：http://xez.wangdashe.top

f() { return 0; }; f || echo "失败了"
来源：http://ahy.xuetiantiany.cn

[R31] 局部变量
来源：http://hnk.tianlin.xyz


<!-- 参考信息 -->