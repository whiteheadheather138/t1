代发 wailian999

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ltk.52xcode.cn

TS:   if (x == null) {}
来源：http://nsd.ybcxt.top

Java: if (x == null || x.isEmpty()) {}
来源：http://oyk.cucudq.cn

Go:   if x == nil {}
来源：http://jzj.c1oappe.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://bjt.aibaodan.cn

C#:   if (x is null) {}
来源：http://qwh.yvedp.cn

[P07] 防抖与节流
来源：http://czg.tanke756.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mqw.cdnleiting.top

PHP:  // 手写时间戳比较
来源：http://bpb.yueranfly.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zhx.hnxiangtu.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tyu.cashguo.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://jeh.fzhhl.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://rzg.shanyushiyangtech.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://vss.zdbjq.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ggl.xinyue.icu

[P08] 处理浮点精度问题
来源：http://avp.zhijiandao.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://yxl.yongpay.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://bfb.nanxuanxn.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://rpf.birdmap.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://dru.hfpthk.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://pps.chenzaomai.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://zzc.smart0.xyz

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hyn.meibo888.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://lhy.hcnkem.com

================================================================================
来源：http://hcq.sxryk.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ani.fengsongda.top

================================================================================
来源：http://yrs.ybcxt.top

[Q01] 创建表
来源：http://yys.guannengcc.top

CREATE TABLE users (
来源：http://sxh.xziqi.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://oab.shanyushiyangtech.top

name VARCHAR(50) NOT NULL,
来源：http://xwt.cashguo.top

email VARCHAR(100) UNIQUE,
来源：http://ejv.nanxuanxn.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ddy.guowangkeji.top

);
来源：http://alw.epnwcf.com

[Q02] 创建带外键的表
来源：http://vek.jyoumei.cn

CREATE TABLE orders (
来源：http://tlg.yj20258.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://aam.nanxinkj.top

user_id INT NOT NULL,
来源：http://qjp.hcnkem.com

amount DECIMAL(10, 2),
来源：http://knj.tarul.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://yps.yvedp.cn

);
来源：http://rtp.gzhubu.top

[Q03] 增加列
来源：http://hqq.yfazqb.com

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://jyb.9152youxi.cn

[Q04] 修改列类型
来源：http://jcs.52xcode.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://vvz.chenjidiqi.icu

[Q05] 重命名列
来源：http://dzy.ydzc1.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://byn.hongshengwenyu.top

[Q06] 删除列
来源：http://arh.zhijiandao.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ppa.nanxuanxn.top

[Q07] 删除表
来源：http://tcw.chenjidiqi.icu

DROP TABLE IF EXISTS orders;
来源：http://nrq.jinyuanbaomall.cn

[Q08] 创建普通索引
来源：http://nqu.0kj1m.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://rfh.pycfn.com

[Q09] 创建唯一索引
来源：http://std.hongshengwenyu.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://owz.meibo888.top

[Q10] 插入单行
来源：http://rvn.nwbrower.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://puf.zhiwuduotai.top

[Q11] 一次插入多行
来源：http://zbe.cashguo.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://vjf.yongpay.top

[Q12] 插入后取自增 ID
来源：http://nwi.zhoulong.xyz

INSERT INTO users (name) VALUES ('C');
来源：http://gsr.meibo888.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://nlg.snrcjt.cn

[Q13] 忽略重复插入
来源：http://oky.gaohongyu789.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://luz.dashuyun.cn

[Q14] 存在则更新（upsert）
来源：http://mbj.c1oappe.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://gfo.fktsv.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://tkm.kuanghao11.cn

[Q15] 查询全部
来源：http://wrs.snrcjt.cn

SELECT * FROM users;
来源：http://mik.zhoulong.xyz

[Q16] 查询指定列
来源：http://six.hnxiangtu.top

SELECT id, name FROM users;
来源：http://aqg.hammf.cn

[Q17] 条件查询
来源：http://mcv.gzhubu.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wqq.ydjk.org.cn

[Q18] 模糊匹配
来源：http://kpt.cashguo.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://zie.jqgufenzy.top

[Q19] 范围查询
来源：http://hlx.hcnkem.com

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://pmh.yanxiufei.cn

[Q20] IN 列表
来源：http://mmd.meibo888.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wrp.shanyushiyangkeji.top

[Q21] 空值判断
来源：http://yfx.xuetiantiany.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://nql.dashuyun.cn

[Q22] 排序
来源：http://udg.daxiang520.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ibl.aibaodan.cn

[Q23] 分页
来源：http://fer.cqqwz.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://oke.316326.xyz

[Q24] 去重
来源：http://hfc.zhengqikj.top

SELECT DISTINCT city FROM users;
来源：http://tws.birdmap.top

[Q25] 只取前 N 条
来源：http://dhm.zhengqikj.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mnw.yangfankeji.com

[Q26] 计数
来源：http://arv.gogol.net.cn

SELECT COUNT(*) FROM users;
来源：http://mbh.wangdashe.top

[Q27] 条件计数
来源：http://rkf.yangfankeji.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://qfb.fengsongda.top

[Q28] 求和与平均
来源：http://ssk.xingfuxueyuan.xyz

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://syv.nanxinkj.top

[Q29] 最大最小值
来源：http://xzx.bjfxy.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://aii.cqqwz.cn

[Q30] 分组统计
来源：http://slt.redwolf501.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://stm.snrcjt.cn

[Q31] 分组后过滤
来源：http://njq.yuanzhike.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://jpv.sweek.top

[Q32] 分组拼接字符串
来源：http://wwy.epnwcf.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ojo.zhijiandao.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ojw.dashuyun.cn

[Q33] 多列分组
来源：http://gwx.jinqigfzy.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://xdr.xziqi.cn

[Q34] 每组取第一条
来源：http://dkk.hesvh.cn

SELECT * FROM (
来源：http://glt.epnwcf.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://btf.chenlongwang.top

) t WHERE rn = 1;
来源：http://amu.pengpengdd.cyou

[Q35] 内连接
来源：http://pxv.shangyingyoupin.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://djk.gaohongyu789.top

[Q36] 左连接
来源：http://ush.chenzaomai.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://bju.mhx1999.top

[Q37] 右连接
来源：http://bpw.redwolf501.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://fru.tarul.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ncu.chenjidiqi.icu

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://pps.jiagoushi.top

[Q39] 自连接（查上下级）
来源：http://koq.yvedp.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ujp.zhongyouzk.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://spq.jiagoushi.top

[Q40] 交叉连接（笛卡尔积）
来源：http://vqp.shanyushiyangtech.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://acs.cheryme.top

[Q41] 多表连接
来源：http://rjn.yongpay.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://rrj.cashguo.top

JOIN users u ON u.id = o.user_id
来源：http://tmk.iojbl.cn

JOIN products p ON p.id = o.product_id;
来源：http://vdn.smart0.xyz

[Q42] 连接条件附加过滤
来源：http://ulv.meibo888.top

SELECT u.name, o.amount FROM users u
来源：http://bxg.chenlongwang.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ndk.jianghu66.top

[Q43] 标量子查询
来源：http://ssv.zhijiandao.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://isv.snrcjt.cn

[Q44] IN 子查询
来源：http://bga.c1oappe.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://oge.guannengcc.top

[Q45] EXISTS 判断存在
来源：http://cwq.shanyushiyangkeji.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fhg.zhengqikj.top

[Q46] NOT EXISTS 判断不存在
来源：http://nkz.jinyuanbaomall.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zsu.epnwcf.com

[Q47] 与平均值比较
来源：http://xax.aizwys.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://elq.epnwcf.com

[Q48] CTE 公用表表达式
来源：http://xxd.vehdjk.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://qqz.daxiang520.top

SELECT * FROM t WHERE c > 5;
来源：http://lkm.ppjwa.cn

[Q49] 更新单行
来源：http://gjr.tanke756.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://clu.zhiwuduotai.top

[Q50] 批量更新
来源：http://zpt.jiagoushi.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hzc.ydzc1.top

[Q51] 用子查询更新
来源：http://pbg.hysaishi.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ote.wangdashe.top

[Q52] 删除指定行
来源：http://nxf.meibo888.top

DELETE FROM users WHERE id = 10;
来源：http://llx.hnxiangtu.top

[Q53] 按条件删除
来源：http://xrs.52xcode.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://sck.shuidangran.top

[Q54] 清空表
来源：http://kpe.yongpay.top

TRUNCATE TABLE logs;
来源：http://lma.hywenlv.cn

[Q55] 排名（并列占位）
来源：http://jcr.guowangkeji.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://jpz.zhaomingkeji.xyz

[Q56] 密集排名（并列不占位）
来源：http://umz.fanxiaobao.xyz

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://vxe.tian-w.cn

[Q57] 行号
来源：http://ewz.snrcjt.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://lex.hesvh.cn

[Q58] 累计求和
来源：http://ddz.zhengqikj.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ulf.cheryme.top

[Q59] 分组内累计
来源：http://byy.316326.xyz

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://jhj.ywan-chungtsiang.top

[Q60] 取上一行 / 下一行
来源：http://eqk.xuanzx.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://rto.nwbrower.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://uem.yueranfly.top

[Q61] 移动平均
来源：http://acr.gogol.net.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://axd.xuetiantiany.cn

[Q62] 分组占比
来源：http://tfc.zhoulong.xyz

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://evo.hnqzz.top

[Q63] 开启事务
来源：http://jjm.sweek.top

START TRANSACTION;                -- 或 BEGIN
来源：http://ryq.cqqwz.cn

[Q64] 提交事务
来源：http://neg.shzxlz.cn

COMMIT;
来源：http://nxx.hesvh.cn

[Q65] 回滚事务
来源：http://kus.kuanghao11.cn

ROLLBACK;
来源：http://uko.guannengcc.top

[Q66] 行锁查询
来源：http://wgs.jianghu66.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://kjf.xziqi.cn

[Q67] 设置隔离级别
来源：http://ucj.0kj1m.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://rwc.hfpthk.cn

[Q68] 保存点
来源：http://vfx.xinyue.icu

SAVEPOINT sp1;
来源：http://vzb.hnqzz.top

ROLLBACK TO sp1;
来源：http://kgd.sweek.top

[Q69] 查看执行计划
来源：http://ynn.nwbrower.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hqh.0kj1m.cn

[Q70] 更新统计信息
来源：http://txl.nwbrower.top

ANALYZE TABLE users;
来源：http://ldv.yueranfly.top

[Q71] 查看建表语句
来源：http://gow.wangdashe.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://bdu.ctjpmb.com

[Q72] 查看索引
来源：http://qfx.shangyingyoupin.top

SHOW INDEX FROM users;
来源：http://kfv.c1oappe.top

[Q73] 查看表状态
来源：http://izf.haohaochexian.top

SHOW TABLE STATUS LIKE 'users';
来源：http://ryw.redwolf501.top

[Q74] 强制使用索引
来源：http://xja.tarul.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://tvh.aizwys.cn

[Q75] 日期格式化
来源：http://tyj.wangdashe.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://bmj.fengsongda.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://bzo.jiagoushi.top

[Q76] 按天统计
来源：http://mlr.hongshengwenyu.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://rgu.sxryk.cn

[Q77] 时间加减
来源：http://kmt.svipenyu.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://njy.yuxming.cn

[Q78] 当前时间
来源：http://pxi.0kj1m.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://tni.jqgufenzy.top

[Q79] 字符串拼接
来源：http://jsl.yonumen.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://nvw.nwbrower.top

[Q80] 字符串截取
来源：http://ekz.yj202588.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://dtt.nanxinkj.top

[Q81] 字符串替换
来源：http://vfx.tarul.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://flg.316326.xyz

[Q82] 字符长度与字节长度
来源：http://wzt.ydzc1.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mjf.hammf.cn

[Q83] 大小写转换
来源：http://cdo.iojbl.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ofe.feifeiyinyue.top

[Q84] 去除首尾空格
来源：http://wef.cashguo.top

SELECT TRIM(name) FROM users;
来源：http://zem.hcnkem.com

[Q85] 数值取整
来源：http://xps.bjfxy.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ttm.hnxiangtu.top

[Q86] 读取 JSON 字段
来源：http://gry.xuetiantiany.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://dez.chenjidiqi.icu

[Q87] JSON 字段做条件
来源：http://tzf.feifeiyinyue.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://okc.aibaodan.cn

[Q88] 行转列（条件聚合）
来源：http://ewj.yfazqb.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://pyv.yanxiufei.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://aaf.aibaodan.cn

[Q89] 判断表是否存在
来源：http://isb.zdqjudy.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://fax.sufxvd.cn

[Q90] 生成序号列
来源：http://gch.nanxuanxn.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hrb.hfpthk.cn

================================================================================
来源：http://xdf.pengpengdd.cyou

R. Bash 专题
来源：http://lux.yj20258.top

================================================================================
来源：http://gqe.shuidangran.top

[R01] shebang 与严格模式
来源：http://bvt.pengpengdd.cyou

#!/usr/bin/env bash
来源：http://zvo.zhaomingkeji.xyz

set -euo pipefail
来源：http://hxu.daxiang520.top

[R02] 变量赋值与使用
来源：http://ohh.tanke756.top

name="Tom"; echo "$name"
来源：http://xwr.jinyuanbaomall.cn

[R03] 只读变量
来源：http://iej.fehbvm.com

readonly PI=3.14
来源：http://pem.yuanzhike.top

[R04] 位置参数
来源：http://obx.zhaomingkeji.xyz

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://pji.gaohongyu789.top

[R05] 参数默认值
来源：http://qkj.quarkkingdee.top

name="${1:-default}"
来源：http://pvl.mhx1999.top

[R06] 判断命令是否存在
来源：http://fff.feifeiyinyue.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://egc.316326.xyz

[R07] if 判断文件
来源：http://eke.zhiwuduotai.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://izg.ppjwa.cn

[R08] 数值比较
来源：http://agy.shuidangran.top

if (( a > b )); then echo "a 更大"; fi
来源：http://lob.daxiang520.top

[R09] 字符串比较
来源：http://omi.fktsv.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://yyw.hfpthk.cn

[R10] 正则匹配
来源：http://bic.andypj.xyz

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://lav.daria6918.cn

[R11] case 多分支
来源：http://cuo.gotoacloud.top

case "$1" in
来源：http://etu.zhengqikj.top

start) echo "启动" ;;
来源：http://ndp.havefunace.top

stop)  echo "停止" ;;
来源：http://pph.zhixingplan.top

*)     echo "未知命令" ;;
来源：http://xaj.yvedp.cn

esac
来源：http://elx.vqdsnc.cn

[R12] for 遍历文件
来源：http://hbr.hysaishi.cn

for f in *.txt; do echo "$f"; done
来源：http://xfx.jqgufenzy.top

[R13] for 计数循环
来源：http://lvu.fengsongda.top

for i in {1..10}; do echo "$i"; done
来源：http://zao.gotoacloud.top

[R14] C 风格 for
来源：http://pur.jiagoushi.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://xui.daria6918.cn

[R15] while 逐行读文件
来源：http://mlc.andypj.xyz

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://zse.yongpay.top

[R16] until 等待条件
来源：http://odl.fzhhl.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ome.yongpay.top

[R17] 数组定义与取值
来源：http://grn.yueranfly.top

arr=(a b c); echo "${arr[0]}"
来源：http://wez.tianlin.xyz

[R18] 遍历数组
来源：http://haf.yj20258.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://usi.ywan-chungtsiang.top

[R19] 数组长度
来源：http://vfu.zhiwuduotai.top

echo "${#arr[@]}"
来源：http://fkc.ybcxt.top

[R20] 关联数组（字典）
来源：http://fri.sufxvd.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mhe.bbcook.cn

[R21] 字符串长度
来源：http://jla.nwbrower.top

echo "${#s}"
来源：http://epr.jyoumei.cn

[R22] 截取子串
来源：http://tsj.chenlongwang.top

echo "${s:0:5}"
来源：http://ahq.yj202588.top

[R23] 字符串替换
来源：http://ofl.yongpay.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hox.sysykeji.top

[R24] 大小写转换
来源：http://rhf.zycfv.cn

echo "${s^^}"; echo "${s,,}"
来源：http://juh.xziqi.cn

[R25] 去后缀 / 去前缀
来源：http://xub.hnqzz.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://vao.jiagoushi.top

[R26] 命令替换
来源：http://auc.hnqzz.top

now=$(date +%F); echo "$now"
来源：http://miu.daria6918.cn

[R27] 算术展开
来源：http://qyn.0kj1m.cn

echo $((1 + 2 * 3))
来源：http://nhq.zycfv.cn

[R28] 浮点运算
来源：http://yqu.cqqwz.cn

echo "scale=2; 10/3" | bc
来源：http://cjs.shangyingyoupin.top

[R29] 定义函数
来源：http://gad.zhixingplan.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://rjj.yanxiufei.cn

[R30] 函数返回状态码
来源：http://qjy.cheryme.top

f() { return 0; }; f || echo "失败了"
来源：http://eyt.yfazqb.com

[R31] 局部变量
来源：http://lib.sufxvd.cn


<!-- 参考信息 -->