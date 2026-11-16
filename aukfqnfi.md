代发 wailian999

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://phe.gotoacloud.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://aqh.zhongyouzk.top

Go:   reflect.DeepEqual(a, b)
来源：http://tkq.hysaishi.cn

Ruby: a == b
来源：http://uhn.vehdjk.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://kui.aizwys.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://rjt.smart0.xyz

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://tqj.ywan-chungtsiang.top

PHP:  if (empty($x)) {}
来源：http://udk.jqgfzy.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hnc.shzxlz.cn

TS:   if (x == null) {}
来源：http://ogx.yueranfly.top

Java: if (x == null || x.isEmpty()) {}
来源：http://vpe.fengsongda.top

Go:   if x == nil {}
来源：http://lki.chenjidiqi.icu

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://fnp.sxryk.cn

C#:   if (x is null) {}
来源：http://wny.zdqjudy.top

[P07] 防抖与节流
来源：http://mci.hywenlv.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wnz.gaohongyu789.top

PHP:  // 手写时间戳比较
来源：http://caj.sweek.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dun.meibo888.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ces.bbcook.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wxv.yj20258888.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://qsa.aizwys.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ymt.fanxiaobao.xyz

C#:   // 用 System.Timers.Timer 重置实现
来源：http://pwn.redwolf501.top

[P08] 处理浮点精度问题
来源：http://inu.ppjwa.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ncv.shzxlz.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://bpd.sjlbkw.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ldx.sufxvd.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://sby.hammf.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://pot.gogol.net.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://tfk.tarul.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://jqu.redwolf501.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://tpr.hywenlv.cn

================================================================================
来源：http://vey.yongpay.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://smi.jlsjyb.cn

================================================================================
来源：http://rkh.meibo888.top

[Q01] 创建表
来源：http://xxr.tarul.cn

CREATE TABLE users (
来源：http://mgb.guowangkeji.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://har.nwbrower.top

name VARCHAR(50) NOT NULL,
来源：http://raq.tianlin.xyz

email VARCHAR(100) UNIQUE,
来源：http://eof.birdmap.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mee.smart0.xyz

);
来源：http://kfm.gzhubu.top

[Q02] 创建带外键的表
来源：http://mfa.xuanzx.com

CREATE TABLE orders (
来源：http://plv.gaohongyu789.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ief.0kj1m.cn

user_id INT NOT NULL,
来源：http://rfc.dianchejie.cn

amount DECIMAL(10, 2),
来源：http://bxm.zhiwuduotai.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ouh.hnxiangtu.top

);
来源：http://zlb.vehdjk.com

[Q03] 增加列
来源：http://vzb.hesvh.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://qid.bbcook.cn

[Q04] 修改列类型
来源：http://zmp.wangdashe.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://niu.vqdsnc.cn

[Q05] 重命名列
来源：http://hcm.cdnleiting.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://xei.nanxuanxn.top

[Q06] 删除列
来源：http://hng.yongpay.top

ALTER TABLE users DROP COLUMN age;
来源：http://hzj.zhixingplan.top

[Q07] 删除表
来源：http://rsk.jinghuilouyu.cn

DROP TABLE IF EXISTS orders;
来源：http://dbh.sweek.top

[Q08] 创建普通索引
来源：http://jkb.jinqigufen.top

CREATE INDEX idx_users_email ON users(email);
来源：http://aki.zycfv.cn

[Q09] 创建唯一索引
来源：http://xho.quarkkingdee.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hfk.c1oappe.top

[Q10] 插入单行
来源：http://bjh.mhx1999.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://zmw.hammf.cn

[Q11] 一次插入多行
来源：http://bwg.jqgfzy.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://fub.zhixingplan.top

[Q12] 插入后取自增 ID
来源：http://chj.haohaochexian.top

INSERT INTO users (name) VALUES ('C');
来源：http://ylh.jianghu66.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ckz.hcnkem.com

[Q13] 忽略重复插入
来源：http://pms.jianghu66.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://znk.bjfxy.top

[Q14] 存在则更新（upsert）
来源：http://vbg.gzhubu.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://nmn.zdqjudy.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://pmk.uphjek.com

[Q15] 查询全部
来源：http://uwd.dashuyun.cn

SELECT * FROM users;
来源：http://nwf.ivvv.top

[Q16] 查询指定列
来源：http://yvf.zdbjq.cn

SELECT id, name FROM users;
来源：http://qzn.9152youxi.cn

[Q17] 条件查询
来源：http://gil.vehdjk.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://bfs.fanxiaobao.xyz

[Q18] 模糊匹配
来源：http://nyj.yuxming.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wiq.cheryme.top

[Q19] 范围查询
来源：http://oke.sweek.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://muy.epnwcf.com

[Q20] IN 列表
来源：http://mfe.hywenlv.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://oru.nwbrower.top

[Q21] 空值判断
来源：http://mud.c1oappe.top

SELECT * FROM users WHERE email IS NULL;
来源：http://kef.gzhubu.top

[Q22] 排序
来源：http://gkt.guannengcc.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://scl.yj202588.top

[Q23] 分页
来源：http://xdo.shuidangran.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mxc.zhongyouzk.top

[Q24] 去重
来源：http://ryx.feifeiyinyue.top

SELECT DISTINCT city FROM users;
来源：http://bzi.aizwys.cn

[Q25] 只取前 N 条
来源：http://mgj.cdnleiting.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://vyb.smart0.xyz

[Q26] 计数
来源：http://xxj.tian-w.cn

SELECT COUNT(*) FROM users;
来源：http://mrt.zhoulong.xyz

[Q27] 条件计数
来源：http://kud.guowangkeji.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://xgo.hysaishi.cn

[Q28] 求和与平均
来源：http://vom.zhixingplan.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://nyq.316326.xyz

[Q29] 最大最小值
来源：http://xgm.xuetiantiany.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://zzs.zdqjudy.top

[Q30] 分组统计
来源：http://oyf.sjlbkw.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ozj.tarul.cn

[Q31] 分组后过滤
来源：http://hko.yfazqb.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://dlf.jinqigfzy.top

[Q32] 分组拼接字符串
来源：http://nrm.c1oappe.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://erl.ydjk.org.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ofa.jqgfzy.top

[Q33] 多列分组
来源：http://kzi.jinqigufen.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://lqx.zhoulong.xyz

[Q34] 每组取第一条
来源：http://vbz.jlsjyb.cn

SELECT * FROM (
来源：http://izz.yj20258.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://vlo.316326.xyz

) t WHERE rn = 1;
来源：http://iop.cdnleiting.top

[Q35] 内连接
来源：http://lvq.zhongyouzk.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://npy.0kj1m.cn

[Q36] 左连接
来源：http://tic.chenjidiqi.icu

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://bnj.snrcjt.cn

[Q37] 右连接
来源：http://qfd.tian-w.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://atn.zhaomingkeji.xyz

[Q38] 全外连接（PostgreSQL）
来源：http://pzt.hywenlv.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://reo.yangfankeji.com

[Q39] 自连接（查上下级）
来源：http://faz.jlsjyb.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://xef.zhengqikj.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://kio.cucudq.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://pdx.aibaodan.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://tnp.smart0.xyz

[Q41] 多表连接
来源：http://urq.yj20258.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://tog.hnqzz.top

JOIN users u ON u.id = o.user_id
来源：http://whf.yj202588.top

JOIN products p ON p.id = o.product_id;
来源：http://nra.wangdashe.top

[Q42] 连接条件附加过滤
来源：http://jzr.nanxinkj.top

SELECT u.name, o.amount FROM users u
来源：http://bks.jinqigfzy.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://bqh.nanxuanxn.top

[Q43] 标量子查询
来源：http://zpt.hysaishi.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://fzp.shangyingyoupin.top

[Q44] IN 子查询
来源：http://zdk.gotoacloud.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://tza.yuxming.cn

[Q45] EXISTS 判断存在
来源：http://sbw.xuanzx.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ctd.yanxiufei.cn

[Q46] NOT EXISTS 判断不存在
来源：http://zue.ybcxt.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zrz.shanyushiyangkeji.top

[Q47] 与平均值比较
来源：http://wgg.fehbvm.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wuh.nanxuanxn.top

[Q48] CTE 公用表表达式
来源：http://ajq.sufxvd.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hns.sjlbkw.cn

SELECT * FROM t WHERE c > 5;
来源：http://sed.yueranfly.top

[Q49] 更新单行
来源：http://lba.cucudq.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://lqc.hesvh.cn

[Q50] 批量更新
来源：http://bss.xuetiantiany.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://sbm.ybcxt.top

[Q51] 用子查询更新
来源：http://ksj.dianchejie.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hnq.hongshengwenyu.top

[Q52] 删除指定行
来源：http://ndj.aizwys.cn

DELETE FROM users WHERE id = 10;
来源：http://ebc.yongpay.top

[Q53] 按条件删除
来源：http://siz.chenjidiqi.icu

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://cti.fzhhl.top

[Q54] 清空表
来源：http://aly.pengpengdd.cyou

TRUNCATE TABLE logs;
来源：http://uxi.sysykeji.top

[Q55] 排名（并列占位）
来源：http://dnq.hcnkem.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://edj.gogol.net.cn

[Q56] 密集排名（并列不占位）
来源：http://qcz.52xcode.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://osv.daxiang520.top

[Q57] 行号
来源：http://fwh.jinyuanbaomall.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://zzq.fanxiaobao.xyz

[Q58] 累计求和
来源：http://csu.52xcode.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ifv.wangdashe.top

[Q59] 分组内累计
来源：http://mkw.pycfn.com

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ehp.xuetiantiany.cn

[Q60] 取上一行 / 下一行
来源：http://sdh.hnxiangtu.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://kyg.jinqigfzy.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://fuu.zhixingplan.top

[Q61] 移动平均
来源：http://mdr.shangyingyoupin.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://nvv.jqgfzy.top

[Q62] 分组占比
来源：http://fpv.yj20258888.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ton.shanyushiyangtech.top

[Q63] 开启事务
来源：http://yzc.svipenyu.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://caz.shanyushiyangkeji.top

[Q64] 提交事务
来源：http://tew.ybcxt.top

COMMIT;
来源：http://awg.zycfv.cn

[Q65] 回滚事务
来源：http://izy.zycfv.cn

ROLLBACK;
来源：http://kyb.52xcode.cn

[Q66] 行锁查询
来源：http://czm.hnqzz.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://jtb.gzhubu.top

[Q67] 设置隔离级别
来源：http://zzd.hcnkem.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://pvd.aibaodan.cn

[Q68] 保存点
来源：http://dec.shuidangran.top

SAVEPOINT sp1;
来源：http://ida.zhoulong.xyz

ROLLBACK TO sp1;
来源：http://pen.havefunace.top

[Q69] 查看执行计划
来源：http://jwg.tianlin.xyz

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mwe.quarkkingdee.top

[Q70] 更新统计信息
来源：http://eao.cdnleiting.top

ANALYZE TABLE users;
来源：http://eux.gaohongyu789.top

[Q71] 查看建表语句
来源：http://rqy.hywenlv.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wvg.ydjk.org.cn

[Q72] 查看索引
来源：http://sjf.ctjpmb.com

SHOW INDEX FROM users;
来源：http://zpk.chenlongwang.top

[Q73] 查看表状态
来源：http://ghj.zhongyouzk.top

SHOW TABLE STATUS LIKE 'users';
来源：http://jwr.yangfankeji.com

[Q74] 强制使用索引
来源：http://lwa.xuetiantiany.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mfw.pycfn.com

[Q75] 日期格式化
来源：http://fxc.ywan-chungtsiang.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://aft.zycfv.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ura.nanxuanxn.top

[Q76] 按天统计
来源：http://bnu.hammf.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hvo.zhoulong.xyz

[Q77] 时间加减
来源：http://mgu.kuanghao11.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ypp.hysaishi.cn

[Q78] 当前时间
来源：http://wpz.daxiang520.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://thr.yj202588.top

[Q79] 字符串拼接
来源：http://jts.nanxuanxn.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://uza.gzhubu.top

[Q80] 字符串截取
来源：http://wnk.vehdjk.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://uwo.sxryk.cn

[Q81] 字符串替换
来源：http://orf.0kj1m.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://yvc.guannengcc.top

[Q82] 字符长度与字节长度
来源：http://fsm.sysykeji.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://kpt.jianghu66.top

[Q83] 大小写转换
来源：http://qfo.nanxinkj.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://nxk.tian-w.cn

[Q84] 去除首尾空格
来源：http://uin.yueranfly.top

SELECT TRIM(name) FROM users;
来源：http://too.guannengcc.top

[Q85] 数值取整
来源：http://qcp.zhijiandao.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://joi.vqdsnc.cn

[Q86] 读取 JSON 字段
来源：http://yiz.xuetiantiany.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hus.zdbjq.cn

[Q87] JSON 字段做条件
来源：http://yof.ywan-chungtsiang.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://oul.bjfxy.top

[Q88] 行转列（条件聚合）
来源：http://uvm.fengsongda.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://pob.tian-w.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://uuq.jiagoushi.top

[Q89] 判断表是否存在
来源：http://fwu.sxryk.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://dfe.vehdjk.com

[Q90] 生成序号列
来源：http://rgf.nanxinkj.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hpi.shanyushiyangkeji.top

================================================================================
来源：http://kzx.snrcjt.cn

R. Bash 专题
来源：http://pdq.hesvh.cn

================================================================================
来源：http://kyp.jyoumei.cn

[R01] shebang 与严格模式
来源：http://hvq.xingfuxueyuan.xyz

#!/usr/bin/env bash
来源：http://pvu.hywenlv.cn

set -euo pipefail
来源：http://bfa.zdqjudy.top

[R02] 变量赋值与使用
来源：http://hrn.andypj.xyz

name="Tom"; echo "$name"
来源：http://uhu.yuxming.cn

[R03] 只读变量
来源：http://rjz.tian-w.cn

readonly PI=3.14
来源：http://gfv.ppjwa.cn

[R04] 位置参数
来源：http://qff.sxryk.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://tdk.birdmap.top

[R05] 参数默认值
来源：http://ijq.yuanzhike.top

name="${1:-default}"
来源：http://sdt.jianghu66.top

[R06] 判断命令是否存在
来源：http://exx.zhijiandao.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ydb.fengsongda.top

[R07] if 判断文件
来源：http://hcc.uphjek.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://vrp.nanxuanxn.top

[R08] 数值比较
来源：http://kxm.shanyushiyangtech.top

if (( a > b )); then echo "a 更大"; fi
来源：http://jpr.tianlin.xyz

[R09] 字符串比较
来源：http://rsr.xziqi.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://tin.tanke756.top

[R10] 正则匹配
来源：http://tfl.guannengcc.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://pmd.yvedp.cn

[R11] case 多分支
来源：http://cco.redwolf501.top

case "$1" in
来源：http://zxa.ybcxt.top

start) echo "启动" ;;
来源：http://qno.yueranfly.top

stop)  echo "停止" ;;
来源：http://rsz.sweek.top

*)     echo "未知命令" ;;
来源：http://mbf.nanxinkj.top

esac
来源：http://sig.mhx1999.top

[R12] for 遍历文件
来源：http://ode.kuanghao11.cn

for f in *.txt; do echo "$f"; done
来源：http://gbo.ehwqpu.com

[R13] for 计数循环
来源：http://wlc.wangshuangyany.cn

for i in {1..10}; do echo "$i"; done
来源：http://ojx.fehbvm.com

[R14] C 风格 for
来源：http://aip.pycfn.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://lxc.hnxiangtu.top

[R15] while 逐行读文件
来源：http://xfm.ybcxt.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://osp.316326.xyz

[R16] until 等待条件
来源：http://vph.feifeiyinyue.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://szx.jlsjyb.cn

[R17] 数组定义与取值
来源：http://jfz.xziqi.cn

arr=(a b c); echo "${arr[0]}"
来源：http://wqe.shanyushiyangtech.top

[R18] 遍历数组
来源：http://con.jqgufenzy.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://yrx.andypj.xyz

[R19] 数组长度
来源：http://yis.316326.xyz

echo "${#arr[@]}"
来源：http://yku.jqgufenzy.top

[R20] 关联数组（字典）
来源：http://jbm.andypj.xyz

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://uqb.jqgfzy.top

[R21] 字符串长度
来源：http://ckr.ydzc1.top

echo "${#s}"
来源：http://xwj.sweek.top

[R22] 截取子串
来源：http://kif.jlsjyb.cn

echo "${s:0:5}"
来源：http://hxg.shuidangran.top

[R23] 字符串替换
来源：http://elc.hnqzz.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mdh.cashguo.top

[R24] 大小写转换
来源：http://vah.vehdjk.com

echo "${s^^}"; echo "${s,,}"
来源：http://ouj.yuxming.cn

[R25] 去后缀 / 去前缀
来源：http://xxj.fanxiaobao.xyz

echo "${f%.txt}"; echo "${f#./}"
来源：http://qnj.zdqjudy.top

[R26] 命令替换
来源：http://fcj.yvedp.cn

now=$(date +%F); echo "$now"
来源：http://ocg.316326.xyz

[R27] 算术展开
来源：http://xnv.ppjwa.cn


<!-- 参考信息 -->