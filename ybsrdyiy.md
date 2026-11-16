代发 wailian999

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://osi.sxryk.cn

TS:   if (x == null) {}
来源：http://ppo.hywenlv.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://rdc.aibaodan.cn

Go:   if x == nil {}
来源：http://cqj.sufxvd.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://rpv.sxryk.cn

C#:   if (x is null) {}
来源：http://agd.yuxming.cn

[P07] 防抖与节流
来源：http://vhv.shzxlz.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://bnm.zhijiandao.cn

PHP:  // 手写时间戳比较
来源：http://apm.sufxvd.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vbj.redwolf501.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nle.havefunace.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://uft.bbcook.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://xxh.xingfuxueyuan.xyz

Ruby: // 手写闭包 + Time.now 判断
来源：http://yff.tanke756.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://cyu.yangfankeji.com

[P08] 处理浮点精度问题
来源：http://qxg.dianchejie.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://arf.jinghuilouyu.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://obu.cqqwz.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://rrp.fktsv.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://stz.zhengqikj.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://lgo.zhijiandao.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://fja.ctjpmb.com

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://sub.fengsongda.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://xdj.shanyushiyangkeji.top

================================================================================
来源：http://xfw.bbcook.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://kwh.hfpthk.cn

================================================================================
来源：http://vqw.nanxuanxn.top

[Q01] 创建表
来源：http://tko.gzhubu.top

CREATE TABLE users (
来源：http://dfq.sysykeji.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://nnf.9152youxi.cn

name VARCHAR(50) NOT NULL,
来源：http://ozg.gaohongyu789.top

email VARCHAR(100) UNIQUE,
来源：http://luy.0kj1m.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://kjx.pycfn.com

);
来源：http://ieo.ehwqpu.com

[Q02] 创建带外键的表
来源：http://iry.epnwcf.com

CREATE TABLE orders (
来源：http://mal.gzhubu.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://jej.shuidangran.top

user_id INT NOT NULL,
来源：http://ufm.jqgfzy.top

amount DECIMAL(10, 2),
来源：http://inm.cashguo.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ylf.c1oappe.top

);
来源：http://yle.jiagoushi.top

[Q03] 增加列
来源：http://fzw.c1oappe.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://jfu.52xcode.cn

[Q04] 修改列类型
来源：http://utu.iojbl.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wrz.andypj.xyz

[Q05] 重命名列
来源：http://yik.0kj1m.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mtv.jinqigufen.top

[Q06] 删除列
来源：http://vfh.shangyingyoupin.top

ALTER TABLE users DROP COLUMN age;
来源：http://hue.jinyuanbaomall.cn

[Q07] 删除表
来源：http://qvu.zhiwuduotai.top

DROP TABLE IF EXISTS orders;
来源：http://qac.jianghu66.top

[Q08] 创建普通索引
来源：http://gfh.nwbrower.top

CREATE INDEX idx_users_email ON users(email);
来源：http://xol.yueranfly.top

[Q09] 创建唯一索引
来源：http://uzv.guannengcc.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ikp.guowangkeji.top

[Q10] 插入单行
来源：http://pyx.hnqzz.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://idl.daxiang520.top

[Q11] 一次插入多行
来源：http://ezo.chenjidiqi.icu

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://odv.dashuyun.cn

[Q12] 插入后取自增 ID
来源：http://efs.hnqzz.top

INSERT INTO users (name) VALUES ('C');
来源：http://zxy.zhixingplan.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hsp.yuanzhike.top

[Q13] 忽略重复插入
来源：http://iqm.hcnkem.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://sys.zhiwuduotai.top

[Q14] 存在则更新（upsert）
来源：http://tlw.fehbvm.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://rkc.cdnleiting.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ncw.ydzc1.top

[Q15] 查询全部
来源：http://ycr.xinyue.icu

SELECT * FROM users;
来源：http://hyy.0kj1m.cn

[Q16] 查询指定列
来源：http://gsr.fehbvm.com

SELECT id, name FROM users;
来源：http://tzh.havefunace.top

[Q17] 条件查询
来源：http://vqx.guannengcc.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wlt.gogol.net.cn

[Q18] 模糊匹配
来源：http://tug.jinyuanbaomall.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://gkc.yanxiufei.cn

[Q19] 范围查询
来源：http://ghe.0kj1m.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://yxn.fehbvm.com

[Q20] IN 列表
来源：http://bhc.hongshengwenyu.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://zae.gogol.net.cn

[Q21] 空值判断
来源：http://fml.cashguo.top

SELECT * FROM users WHERE email IS NULL;
来源：http://wxd.yongpay.top

[Q22] 排序
来源：http://cva.hfpthk.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mkz.vehdjk.com

[Q23] 分页
来源：http://wct.chenzaomai.com

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://fvm.meibo888.top

[Q24] 去重
来源：http://dxh.0kj1m.cn

SELECT DISTINCT city FROM users;
来源：http://epf.yj202588.top

[Q25] 只取前 N 条
来源：http://lol.sxryk.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://lxf.ywan-chungtsiang.top

[Q26] 计数
来源：http://vhm.shanyushiyangkeji.top

SELECT COUNT(*) FROM users;
来源：http://nyn.jqgfzy.top

[Q27] 条件计数
来源：http://suu.fzhhl.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ebk.ivvv.top

[Q28] 求和与平均
来源：http://evq.feifeiyinyue.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ibc.zhijiandao.cn

[Q29] 最大最小值
来源：http://ewq.fengsongda.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://uru.zdqjudy.top

[Q30] 分组统计
来源：http://tdk.birdmap.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://gdw.pycfn.com

[Q31] 分组后过滤
来源：http://jde.ivvv.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://dih.guannengcc.top

[Q32] 分组拼接字符串
来源：http://onv.hnqzz.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://trp.jianghu66.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hcb.meibo888.top

[Q33] 多列分组
来源：http://got.yuxming.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://lau.kuanghao11.cn

[Q34] 每组取第一条
来源：http://kdc.zhijiandao.cn

SELECT * FROM (
来源：http://vfj.yj20258888.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://khs.tanke756.top

) t WHERE rn = 1;
来源：http://mpp.nanxuanxn.top

[Q35] 内连接
来源：http://mgp.bjfxy.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://zhk.shuidangran.top

[Q36] 左连接
来源：http://vin.jlsjyb.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://uhq.aibaodan.cn

[Q37] 右连接
来源：http://pwr.redwolf501.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://dzo.52xcode.cn

[Q38] 全外连接（PostgreSQL）
来源：http://lzt.xylfe.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://vzv.yueranfly.top

[Q39] 自连接（查上下级）
来源：http://ziw.zhiwuduotai.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://sea.pycfn.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://aga.jyoumei.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://jft.xuanzx.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ywx.chenzaomai.com

[Q41] 多表连接
来源：http://lzs.zdbjq.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ihh.daxiang520.top

JOIN users u ON u.id = o.user_id
来源：http://xbu.ydjk.org.cn

JOIN products p ON p.id = o.product_id;
来源：http://qbf.c1oappe.top

[Q42] 连接条件附加过滤
来源：http://dve.fehbvm.com

SELECT u.name, o.amount FROM users u
来源：http://qyt.zdbjq.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mgq.c1oappe.top

[Q43] 标量子查询
来源：http://tlg.xuetiantiany.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://xcn.zhaomingkeji.xyz

[Q44] IN 子查询
来源：http://mdo.haohaochexian.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wiy.havefunace.top

[Q45] EXISTS 判断存在
来源：http://jtf.hammf.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://srr.dashuyun.cn

[Q46] NOT EXISTS 判断不存在
来源：http://mdi.hywenlv.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ikm.ppjwa.cn

[Q47] 与平均值比较
来源：http://qcf.sufxvd.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://elk.havefunace.top

[Q48] CTE 公用表表达式
来源：http://qnp.jqgufenzy.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://vkq.hnxiangtu.top

SELECT * FROM t WHERE c > 5;
来源：http://hwg.ctjpmb.com

[Q49] 更新单行
来源：http://ddt.sufxvd.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hwn.ppjwa.cn

[Q50] 批量更新
来源：http://jye.zhiwuduotai.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://sjq.aibaodan.cn

[Q51] 用子查询更新
来源：http://gmh.yongpay.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://kjo.birdmap.top

[Q52] 删除指定行
来源：http://hoj.kuanghao11.cn

DELETE FROM users WHERE id = 10;
来源：http://jbc.gaohongyu789.top

[Q53] 按条件删除
来源：http://gpt.mhx1999.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://qcf.svipenyu.cn

[Q54] 清空表
来源：http://lqx.feifeiyinyue.top

TRUNCATE TABLE logs;
来源：http://jgb.hesvh.cn

[Q55] 排名（并列占位）
来源：http://mcd.zhijiandao.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://lhz.quarkkingdee.top

[Q56] 密集排名（并列不占位）
来源：http://jpo.wangdashe.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://xyl.yj20258.top

[Q57] 行号
来源：http://geq.aizwys.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://lcz.snrcjt.cn

[Q58] 累计求和
来源：http://pcv.bbcook.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wig.shanyushiyangkeji.top

[Q59] 分组内累计
来源：http://vij.xinyue.icu

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mbw.gogol.net.cn

[Q60] 取上一行 / 下一行
来源：http://scd.ydjk.org.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://sua.hammf.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wmr.hnxiangtu.top

[Q61] 移动平均
来源：http://ywg.hesvh.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://dan.haohaochexian.top

[Q62] 分组占比
来源：http://cmg.iojbl.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://lwe.yuanzhike.top

[Q63] 开启事务
来源：http://wvv.ctjpmb.com

START TRANSACTION;                -- 或 BEGIN
来源：http://ylm.c1oappe.top

[Q64] 提交事务
来源：http://bgh.nwbrower.top

COMMIT;
来源：http://bap.jiagoushi.top

[Q65] 回滚事务
来源：http://meo.gzhubu.top

ROLLBACK;
来源：http://xso.hnxiangtu.top

[Q66] 行锁查询
来源：http://dvx.dianchejie.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://nil.dianchejie.cn

[Q67] 设置隔离级别
来源：http://hvb.mhx1999.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://vaa.xylfe.cn

[Q68] 保存点
来源：http://fgo.bjfxy.top

SAVEPOINT sp1;
来源：http://myh.iojbl.cn

ROLLBACK TO sp1;
来源：http://kxj.fehbvm.com

[Q69] 查看执行计划
来源：http://azs.zdbjq.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://dgh.hongshengwenyu.top

[Q70] 更新统计信息
来源：http://wje.0kj1m.cn

ANALYZE TABLE users;
来源：http://rbk.zhixingplan.top

[Q71] 查看建表语句
来源：http://uvs.daxiang520.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://qvr.cashguo.top

[Q72] 查看索引
来源：http://ilr.quarkkingdee.top

SHOW INDEX FROM users;
来源：http://xcv.daria6918.cn

[Q73] 查看表状态
来源：http://kxt.mhx1999.top

SHOW TABLE STATUS LIKE 'users';
来源：http://ilz.jlsjyb.cn

[Q74] 强制使用索引
来源：http://jjf.zhijiandao.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wqw.birdmap.top

[Q75] 日期格式化
来源：http://wzi.sxryk.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://qck.tian-w.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://evd.daria6918.cn

[Q76] 按天统计
来源：http://odb.bbcook.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://aik.hongshengwenyu.top

[Q77] 时间加减
来源：http://tlp.pycfn.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://uix.snrcjt.cn

[Q78] 当前时间
来源：http://sog.fzhhl.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ivt.xingfuxueyuan.xyz

[Q79] 字符串拼接
来源：http://gsl.aibaodan.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://gig.ydzc1.top

[Q80] 字符串截取
来源：http://uex.jinyuanbaomall.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://oon.ydjk.org.cn

[Q81] 字符串替换
来源：http://wqx.chenlongwang.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mmq.hongshengwenyu.top

[Q82] 字符长度与字节长度
来源：http://wzu.sufxvd.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://veh.jlsjyb.cn

[Q83] 大小写转换
来源：http://uev.shuidangran.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://lun.ywan-chungtsiang.top

[Q84] 去除首尾空格
来源：http://hyf.0kj1m.cn

SELECT TRIM(name) FROM users;
来源：http://mgg.fzhhl.top

[Q85] 数值取整
来源：http://imy.birdmap.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ekm.gzhubu.top

[Q86] 读取 JSON 字段
来源：http://dos.ywan-chungtsiang.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://cpr.tarul.cn

[Q87] JSON 字段做条件
来源：http://xyu.gogol.net.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://utl.xuetiantiany.cn

[Q88] 行转列（条件聚合）
来源：http://tzd.fengsongda.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://cgl.daxiang520.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://pop.chenlongwang.top

[Q89] 判断表是否存在
来源：http://ybm.sysykeji.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ors.wangshuangyany.cn

[Q90] 生成序号列
来源：http://ira.ctjpmb.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://vhe.iojbl.cn

================================================================================
来源：http://ddg.hammf.cn

R. Bash 专题
来源：http://rzw.sweek.top

================================================================================
来源：http://pha.jyoumei.cn

[R01] shebang 与严格模式
来源：http://loq.tanke756.top

#!/usr/bin/env bash
来源：http://ima.hcnkem.com

set -euo pipefail
来源：http://mbe.xuetiantiany.cn

[R02] 变量赋值与使用
来源：http://fwh.jinqigfzy.top

name="Tom"; echo "$name"
来源：http://lkb.mhx1999.top

[R03] 只读变量
来源：http://for.gotoacloud.top

readonly PI=3.14
来源：http://qea.pycfn.com

[R04] 位置参数
来源：http://oqr.quarkkingdee.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://uws.yonumen.top

[R05] 参数默认值
来源：http://als.yuanzhike.top

name="${1:-default}"
来源：http://fwx.yonumen.top

[R06] 判断命令是否存在
来源：http://cmm.dianchejie.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://rhh.dianchejie.cn

[R07] if 判断文件
来源：http://tsn.tarul.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://dnh.chenzaomai.com

[R08] 数值比较
来源：http://cke.cdnleiting.top

if (( a > b )); then echo "a 更大"; fi
来源：http://llz.wangdashe.top

[R09] 字符串比较
来源：http://mgx.epnwcf.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ygf.xuetiantiany.cn

[R10] 正则匹配
来源：http://yug.jlsjyb.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://rsi.sjlbkw.cn

[R11] case 多分支
来源：http://oko.hesvh.cn

case "$1" in
来源：http://ner.bjfxy.top

start) echo "启动" ;;
来源：http://ehm.shanyushiyangkeji.top

stop)  echo "停止" ;;
来源：http://czv.jinyuanbaomall.cn

*)     echo "未知命令" ;;
来源：http://dqc.andypj.xyz

esac
来源：http://zuz.daxiang520.top

[R12] for 遍历文件
来源：http://asf.zdqjudy.top

for f in *.txt; do echo "$f"; done
来源：http://dmk.wangshuangyany.cn

[R13] for 计数循环
来源：http://ehz.ctjpmb.com

for i in {1..10}; do echo "$i"; done
来源：http://qvi.ivvv.top

[R14] C 风格 for
来源：http://glu.svipenyu.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://rrl.gogol.net.cn

[R15] while 逐行读文件
来源：http://hzv.shangyingyoupin.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mra.cashguo.top

[R16] until 等待条件
来源：http://juf.gzhubu.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://aor.zhongyouzk.top

[R17] 数组定义与取值
来源：http://bxc.gzhubu.top

arr=(a b c); echo "${arr[0]}"
来源：http://kpy.fzhhl.top

[R18] 遍历数组
来源：http://cub.havefunace.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://kai.havefunace.top

[R19] 数组长度
来源：http://lql.ctjpmb.com

echo "${#arr[@]}"
来源：http://bql.zhoulong.xyz

[R20] 关联数组（字典）
来源：http://fnj.shzxlz.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://pxu.tarul.cn

[R21] 字符串长度
来源：http://cie.shuidangran.top

echo "${#s}"
来源：http://lrz.xziqi.cn

[R22] 截取子串
来源：http://dzx.9152youxi.cn

echo "${s:0:5}"
来源：http://kbr.zhaomingkeji.xyz

[R23] 字符串替换
来源：http://mit.nanxuanxn.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://jsw.daxiang520.top

[R24] 大小写转换
来源：http://jrj.zhongyouzk.top

echo "${s^^}"; echo "${s,,}"
来源：http://jrd.tanke756.top

[R25] 去后缀 / 去前缀
来源：http://ybu.gzhubu.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://xdl.0kj1m.cn

[R26] 命令替换
来源：http://rhh.nanxinkj.top

now=$(date +%F); echo "$now"
来源：http://ouq.fktsv.cn

[R27] 算术展开
来源：http://iah.cucudq.cn

echo $((1 + 2 * 3))
来源：http://soh.fktsv.cn

[R28] 浮点运算
来源：http://cjy.shanyushiyangtech.top

echo "scale=2; 10/3" | bc
来源：http://zax.sufxvd.cn

[R29] 定义函数
来源：http://moi.tanke756.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://vxu.birdmap.top

[R30] 函数返回状态码
来源：http://yti.quarkkingdee.top

f() { return 0; }; f || echo "失败了"
来源：http://ksr.ppjwa.cn

[R31] 局部变量
来源：http://xec.shangyingyoupin.top


<!-- 参考信息 -->