代发 wailian999

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://qop.fehbvm.com

TS:   if (x == null) {}
来源：http://sjt.redwolf501.top

Java: if (x == null || x.isEmpty()) {}
来源：http://ota.yueranfly.top

Go:   if x == nil {}
来源：http://xfo.meibo888.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://sib.yj20258888.top

C#:   if (x is null) {}
来源：http://bxo.yj20258888.top

[P07] 防抖与节流
来源：http://fts.birdmap.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://dmb.hcnkem.com

PHP:  // 手写时间戳比较
来源：http://kof.yj202588.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cey.sweek.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://oto.zhoulong.xyz

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hds.tian-w.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://gph.feifeiyinyue.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://ina.gogol.net.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://sqs.dianchejie.cn

[P08] 处理浮点精度问题
来源：http://qeg.ppjwa.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://rqs.daxiang520.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://uej.dianchejie.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://yjd.xuetiantiany.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hmr.xuetiantiany.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://vao.yanxiufei.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://vzi.ctjpmb.com

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://zsx.daria6918.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://rwq.ybcxt.top

================================================================================
来源：http://qip.shzxlz.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://xlb.shangyingyoupin.top

================================================================================
来源：http://act.guowangkeji.top

[Q01] 创建表
来源：http://zan.zhixingplan.top

CREATE TABLE users (
来源：http://yma.havefunace.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://cyk.bjfxy.top

name VARCHAR(50) NOT NULL,
来源：http://rsv.havefunace.top

email VARCHAR(100) UNIQUE,
来源：http://hss.mhx1999.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://dab.chenlongwang.top

);
来源：http://fny.jlsjyb.cn

[Q02] 创建带外键的表
来源：http://gxv.fzhhl.top

CREATE TABLE orders (
来源：http://atu.sxryk.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://bfx.yj202588.top

user_id INT NOT NULL,
来源：http://eer.daria6918.cn

amount DECIMAL(10, 2),
来源：http://afw.52xcode.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://rnr.tian-w.cn

);
来源：http://azo.cheryme.top

[Q03] 增加列
来源：http://tvf.yueranfly.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://isk.shangyingyoupin.top

[Q04] 修改列类型
来源：http://aou.sufxvd.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hyr.gogol.net.cn

[Q05] 重命名列
来源：http://dup.aizwys.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://qcb.zhiwuduotai.top

[Q06] 删除列
来源：http://xzd.gotoacloud.top

ALTER TABLE users DROP COLUMN age;
来源：http://rqm.yfazqb.com

[Q07] 删除表
来源：http://pxd.yangfankeji.com

DROP TABLE IF EXISTS orders;
来源：http://fxh.haohaochexian.top

[Q08] 创建普通索引
来源：http://znj.jinyuanbaomall.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://boo.aizwys.cn

[Q09] 创建唯一索引
来源：http://mxp.ppjwa.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://lgr.shanyushiyangkeji.top

[Q10] 插入单行
来源：http://crj.yj202588.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://rsh.shanyushiyangkeji.top

[Q11] 一次插入多行
来源：http://qkc.xylfe.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://cuh.zhengqikj.top

[Q12] 插入后取自增 ID
来源：http://nty.316326.xyz

INSERT INTO users (name) VALUES ('C');
来源：http://gjh.iojbl.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mtz.shzxlz.cn

[Q13] 忽略重复插入
来源：http://ghs.zhiwuduotai.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hyb.sysykeji.top

[Q14] 存在则更新（upsert）
来源：http://vmm.feifeiyinyue.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://upe.jlsjyb.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://bpa.daria6918.cn

[Q15] 查询全部
来源：http://kmj.cdnleiting.top

SELECT * FROM users;
来源：http://aaj.yj20258.top

[Q16] 查询指定列
来源：http://bvx.xuetiantiany.cn

SELECT id, name FROM users;
来源：http://sed.gotoacloud.top

[Q17] 条件查询
来源：http://lpi.havefunace.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://tis.yangfankeji.com

[Q18] 模糊匹配
来源：http://stc.xingfuxueyuan.xyz

SELECT * FROM users WHERE name LIKE '张%';
来源：http://gjk.ctjpmb.com

[Q19] 范围查询
来源：http://vgd.xuetiantiany.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://vaj.tian-w.cn

[Q20] IN 列表
来源：http://xtk.hammf.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://gzq.zhengqikj.top

[Q21] 空值判断
来源：http://oyn.tianlin.xyz

SELECT * FROM users WHERE email IS NULL;
来源：http://gma.guannengcc.top

[Q22] 排序
来源：http://ana.andypj.xyz

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://pze.wangdashe.top

[Q23] 分页
来源：http://ehs.xuetiantiany.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://otp.xuetiantiany.cn

[Q24] 去重
来源：http://rgw.yj20258888.top

SELECT DISTINCT city FROM users;
来源：http://ame.epnwcf.com

[Q25] 只取前 N 条
来源：http://ski.zhaomingkeji.xyz

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://uks.fehbvm.com

[Q26] 计数
来源：http://ofw.dianchejie.cn

SELECT COUNT(*) FROM users;
来源：http://uvo.nwbrower.top

[Q27] 条件计数
来源：http://sas.meibo888.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://els.hnqzz.top

[Q28] 求和与平均
来源：http://pyt.jinqigfzy.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://sez.yongpay.top

[Q29] 最大最小值
来源：http://pmp.chenzaomai.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://kff.fktsv.cn

[Q30] 分组统计
来源：http://cgm.pengpengdd.cyou

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ffk.zhijiandao.cn

[Q31] 分组后过滤
来源：http://das.jqgfzy.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://pfo.kuanghao11.cn

[Q32] 分组拼接字符串
来源：http://znn.cheryme.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://pnj.xylfe.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://dzk.jinqigfzy.top

[Q33] 多列分组
来源：http://msm.zhongyouzk.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://bhb.cashguo.top

[Q34] 每组取第一条
来源：http://sud.hesvh.cn

SELECT * FROM (
来源：http://ibb.feifeiyinyue.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ejx.zhoulong.xyz

) t WHERE rn = 1;
来源：http://bxf.ydzc1.top

[Q35] 内连接
来源：http://rzd.xinyue.icu

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://sta.jinyuanbaomall.cn

[Q36] 左连接
来源：http://wxy.xylfe.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://zen.sjlbkw.cn

[Q37] 右连接
来源：http://erk.svipenyu.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ige.316326.xyz

[Q38] 全外连接（PostgreSQL）
来源：http://dls.zhaomingkeji.xyz

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://rdv.hysaishi.cn

[Q39] 自连接（查上下级）
来源：http://gbp.hammf.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://zsd.wangshuangyany.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://rro.xinyue.icu

[Q40] 交叉连接（笛卡尔积）
来源：http://qjz.wangdashe.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://tdp.zhixingplan.top

[Q41] 多表连接
来源：http://mcw.gogol.net.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://teb.jqgufenzy.top

JOIN users u ON u.id = o.user_id
来源：http://oix.zhixingplan.top

JOIN products p ON p.id = o.product_id;
来源：http://sag.ctjpmb.com

[Q42] 连接条件附加过滤
来源：http://yok.vehdjk.com

SELECT u.name, o.amount FROM users u
来源：http://mrv.epnwcf.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://don.ydjk.org.cn

[Q43] 标量子查询
来源：http://uhi.snrcjt.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://erg.zhaomingkeji.xyz

[Q44] IN 子查询
来源：http://mrd.zdbjq.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://oje.mhx1999.top

[Q45] EXISTS 判断存在
来源：http://bsv.cqqwz.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://csn.jinqigufen.top

[Q46] NOT EXISTS 判断不存在
来源：http://rfm.daxiang520.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://dwh.yongpay.top

[Q47] 与平均值比较
来源：http://ktx.zhoulong.xyz

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://zyy.zhoulong.xyz

[Q48] CTE 公用表表达式
来源：http://vbg.daxiang520.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://zea.gogol.net.cn

SELECT * FROM t WHERE c > 5;
来源：http://sdb.aibaodan.cn

[Q49] 更新单行
来源：http://gjk.yuxming.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://lzk.hysaishi.cn

[Q50] 批量更新
来源：http://vhw.ybcxt.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ptp.mhx1999.top

[Q51] 用子查询更新
来源：http://qbe.sjlbkw.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://bnu.jqgufenzy.top

[Q52] 删除指定行
来源：http://hfo.haohaochexian.top

DELETE FROM users WHERE id = 10;
来源：http://tdl.hnxiangtu.top

[Q53] 按条件删除
来源：http://jzo.yvedp.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://yyy.ybcxt.top

[Q54] 清空表
来源：http://ehh.snrcjt.cn

TRUNCATE TABLE logs;
来源：http://fkb.daria6918.cn

[Q55] 排名（并列占位）
来源：http://bhv.fehbvm.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ybj.nanxuanxn.top

[Q56] 密集排名（并列不占位）
来源：http://psj.cqqwz.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://cuh.chenjidiqi.icu

[Q57] 行号
来源：http://fcn.hammf.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://lzo.yongpay.top

[Q58] 累计求和
来源：http://rhg.zycfv.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://jbj.chenjidiqi.icu

[Q59] 分组内累计
来源：http://kxs.jqgufenzy.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://axl.zhiwuduotai.top

[Q60] 取上一行 / 下一行
来源：http://wat.andypj.xyz

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://vss.kuanghao11.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://qnn.zycfv.cn

[Q61] 移动平均
来源：http://siq.feifeiyinyue.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://acs.nanxuanxn.top

[Q62] 分组占比
来源：http://uua.0kj1m.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://rpv.zhiwuduotai.top

[Q63] 开启事务
来源：http://csr.guowangkeji.top

START TRANSACTION;                -- 或 BEGIN
来源：http://mtd.yvedp.cn

[Q64] 提交事务
来源：http://nnu.fehbvm.com

COMMIT;
来源：http://ihn.yueranfly.top

[Q65] 回滚事务
来源：http://lgo.shangyingyoupin.top

ROLLBACK;
来源：http://sfy.yj20258.top

[Q66] 行锁查询
来源：http://iin.haohaochexian.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://weq.yongpay.top

[Q67] 设置隔离级别
来源：http://cop.fktsv.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://nvv.zdqjudy.top

[Q68] 保存点
来源：http://kta.zhaomingkeji.xyz

SAVEPOINT sp1;
来源：http://njy.havefunace.top

ROLLBACK TO sp1;
来源：http://sms.uphjek.com

[Q69] 查看执行计划
来源：http://elt.vqdsnc.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://xtm.hysaishi.cn

[Q70] 更新统计信息
来源：http://agg.hnxiangtu.top

ANALYZE TABLE users;
来源：http://wqr.pengpengdd.cyou

[Q71] 查看建表语句
来源：http://tac.sweek.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://evy.shangyingyoupin.top

[Q72] 查看索引
来源：http://rnv.ppjwa.cn

SHOW INDEX FROM users;
来源：http://hyj.yanxiufei.cn

[Q73] 查看表状态
来源：http://uxq.yanxiufei.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://hab.316326.xyz

[Q74] 强制使用索引
来源：http://vkc.xylfe.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://dyp.fzhhl.top

[Q75] 日期格式化
来源：http://rhr.sufxvd.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wet.feifeiyinyue.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://yhj.cdnleiting.top

[Q76] 按天统计
来源：http://hsv.vqdsnc.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://qvu.zhaomingkeji.xyz

[Q77] 时间加减
来源：http://fmz.fzhhl.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://pda.wangshuangyany.cn

[Q78] 当前时间
来源：http://vud.wangshuangyany.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ynr.mhx1999.top

[Q79] 字符串拼接
来源：http://yfn.haohaochexian.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://rll.jinqigufen.top

[Q80] 字符串截取
来源：http://ryq.xuetiantiany.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://jlj.aizwys.cn

[Q81] 字符串替换
来源：http://fuu.zhijiandao.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://uho.ehwqpu.com

[Q82] 字符长度与字节长度
来源：http://knj.c1oappe.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://acd.iojbl.cn

[Q83] 大小写转换
来源：http://izz.ydjk.org.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://xtd.smart0.xyz

[Q84] 去除首尾空格
来源：http://zxd.guowangkeji.top

SELECT TRIM(name) FROM users;
来源：http://ypu.xingfuxueyuan.xyz

[Q85] 数值取整
来源：http://max.ydzc1.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ejl.nanxuanxn.top

[Q86] 读取 JSON 字段
来源：http://kjp.shangyingyoupin.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://nuk.smart0.xyz

[Q87] JSON 字段做条件
来源：http://cjb.aizwys.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://llk.haohaochexian.top

[Q88] 行转列（条件聚合）
来源：http://ljn.hesvh.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://qcy.zhaomingkeji.xyz

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://euz.xylfe.cn

[Q89] 判断表是否存在
来源：http://mtm.xingfuxueyuan.xyz

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://pus.pycfn.com

[Q90] 生成序号列
来源：http://akf.jinghuilouyu.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://gvv.nanxinkj.top

================================================================================
来源：http://fee.xuanzx.com

R. Bash 专题
来源：http://lqz.wangdashe.top

================================================================================
来源：http://vuq.zhengqikj.top

[R01] shebang 与严格模式
来源：http://vmw.bjfxy.top

#!/usr/bin/env bash
来源：http://myl.ehwqpu.com

set -euo pipefail
来源：http://pox.ehwqpu.com

[R02] 变量赋值与使用
来源：http://zny.iojbl.cn

name="Tom"; echo "$name"
来源：http://jpj.zhengqikj.top

[R03] 只读变量
来源：http://sul.vehdjk.com

readonly PI=3.14
来源：http://frm.chenjidiqi.icu

[R04] 位置参数
来源：http://hoz.shzxlz.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ask.iojbl.cn

[R05] 参数默认值
来源：http://eav.andypj.xyz

name="${1:-default}"
来源：http://qjx.gaohongyu789.top

[R06] 判断命令是否存在
来源：http://lva.yj202588.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://fsd.jiagoushi.top

[R07] if 判断文件
来源：http://tot.feifeiyinyue.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://iak.zycfv.cn

[R08] 数值比较
来源：http://rql.kuanghao11.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://vme.chenzaomai.com

[R09] 字符串比较
来源：http://ngt.fanxiaobao.xyz

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://amb.tian-w.cn

[R10] 正则匹配
来源：http://ksi.jqgufenzy.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ple.zhiwuduotai.top

[R11] case 多分支
来源：http://otm.hongshengwenyu.top

case "$1" in
来源：http://sdt.sjlbkw.cn

start) echo "启动" ;;
来源：http://gsx.cheryme.top

stop)  echo "停止" ;;
来源：http://tlr.yvedp.cn

*)     echo "未知命令" ;;
来源：http://qwf.chenzaomai.com

esac
来源：http://qat.zhengqikj.top

[R12] for 遍历文件
来源：http://bji.52xcode.cn

for f in *.txt; do echo "$f"; done
来源：http://mtg.zhijiandao.cn

[R13] for 计数循环
来源：http://vyp.yvedp.cn

for i in {1..10}; do echo "$i"; done
来源：http://jhx.svipenyu.cn

[R14] C 风格 for
来源：http://ekb.yanxiufei.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wir.xylfe.cn

[R15] while 逐行读文件
来源：http://ult.sysykeji.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://yon.nanxinkj.top

[R16] until 等待条件
来源：http://mst.sysykeji.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ctq.dashuyun.cn

[R17] 数组定义与取值
来源：http://oxc.sjlbkw.cn

arr=(a b c); echo "${arr[0]}"
来源：http://oud.hysaishi.cn

[R18] 遍历数组
来源：http://kwc.hesvh.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://qih.cucudq.cn

[R19] 数组长度
来源：http://ufl.yonumen.top

echo "${#arr[@]}"
来源：http://lav.yuxming.cn

[R20] 关联数组（字典）
来源：http://ajn.xingfuxueyuan.xyz

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://snu.andypj.xyz

[R21] 字符串长度
来源：http://eum.fengsongda.top

echo "${#s}"
来源：http://jux.sufxvd.cn

[R22] 截取子串
来源：http://urt.9152youxi.cn

echo "${s:0:5}"
来源：http://vsf.nwbrower.top

[R23] 字符串替换
来源：http://mvp.shanyushiyangkeji.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ihg.zycfv.cn

[R24] 大小写转换
来源：http://opq.zhengqikj.top

echo "${s^^}"; echo "${s,,}"
来源：http://fut.jlsjyb.cn

[R25] 去后缀 / 去前缀
来源：http://fcg.316326.xyz

echo "${f%.txt}"; echo "${f#./}"
来源：http://ltg.feifeiyinyue.top

[R26] 命令替换
来源：http://gvp.epnwcf.com

now=$(date +%F); echo "$now"
来源：http://coe.52xcode.cn

[R27] 算术展开
来源：http://zuw.ctjpmb.com

echo $((1 + 2 * 3))
来源：http://mju.xingfuxueyuan.xyz

[R28] 浮点运算
来源：http://bcy.ppjwa.cn

echo "scale=2; 10/3" | bc
来源：http://sqi.c1oappe.top

[R29] 定义函数
来源：http://oii.andypj.xyz

add() { echo $(($1 + $2)); }; add 1 2
来源：http://fyt.shanyushiyangkeji.top

[R30] 函数返回状态码
来源：http://uvh.shanyushiyangtech.top

f() { return 0; }; f || echo "失败了"
来源：http://gns.cqqwz.cn

[R31] 局部变量
来源：http://fnn.ehwqpu.com


<!-- 参考信息 -->