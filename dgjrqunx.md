代发 wailian999

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://bnz.redwolf501.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://jrw.yj20258888.top

Go:   reflect.DeepEqual(a, b)
来源：http://pcp.gogol.net.cn

Ruby: a == b
来源：http://ukc.yueranfly.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ygk.uphjek.com

[P06] 综合判空（null / 空串 / 空集合）
来源：http://oii.wangshuangyany.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ecm.jqgufenzy.top

PHP:  if (empty($x)) {}
来源：http://ahs.pycfn.com

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://xtb.gotoacloud.top

TS:   if (x == null) {}
来源：http://gsc.cucudq.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://gtf.vehdjk.com

Go:   if x == nil {}
来源：http://frs.hesvh.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://rji.yueranfly.top

C#:   if (x is null) {}
来源：http://sdb.sufxvd.cn

[P07] 防抖与节流
来源：http://eig.xuanzx.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://yfo.hammf.cn

PHP:  // 手写时间戳比较
来源：http://ypc.cheryme.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://eir.daria6918.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dqo.xylfe.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://dkt.xingfuxueyuan.xyz

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://fmo.birdmap.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://ugi.hesvh.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://lug.jinqigufen.top

[P08] 处理浮点精度问题
来源：http://cir.zhengqikj.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://rju.yuanzhike.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://lmc.chenzaomai.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://rif.cqqwz.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://lyv.yongpay.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://zcu.redwolf501.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hmz.cashguo.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://fqv.haohaochexian.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ilu.cdnleiting.top

================================================================================
来源：http://dhx.pengpengdd.cyou

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hyy.cucudq.cn

================================================================================
来源：http://pnh.316326.xyz

[Q01] 创建表
来源：http://qvm.cdnleiting.top

CREATE TABLE users (
来源：http://btr.jyoumei.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://gvf.cashguo.top

name VARCHAR(50) NOT NULL,
来源：http://hjj.chenzaomai.com

email VARCHAR(100) UNIQUE,
来源：http://yxw.bbcook.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://jcm.chenjidiqi.icu

);
来源：http://csg.tian-w.cn

[Q02] 创建带外键的表
来源：http://zff.feifeiyinyue.top

CREATE TABLE orders (
来源：http://nql.sufxvd.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mbi.sxryk.cn

user_id INT NOT NULL,
来源：http://aea.xinyue.icu

amount DECIMAL(10, 2),
来源：http://ffd.c1oappe.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://udd.9152youxi.cn

);
来源：http://nqd.aizwys.cn

[Q03] 增加列
来源：http://zvm.sweek.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://drn.ivvv.top

[Q04] 修改列类型
来源：http://uqe.9152youxi.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://usl.daria6918.cn

[Q05] 重命名列
来源：http://yfa.wangdashe.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://yfe.smart0.xyz

[Q06] 删除列
来源：http://vkm.quarkkingdee.top

ALTER TABLE users DROP COLUMN age;
来源：http://rep.yj20258.top

[Q07] 删除表
来源：http://vzu.yuanzhike.top

DROP TABLE IF EXISTS orders;
来源：http://vmi.mhx1999.top

[Q08] 创建普通索引
来源：http://vfy.yuanzhike.top

CREATE INDEX idx_users_email ON users(email);
来源：http://vvn.fzhhl.top

[Q09] 创建唯一索引
来源：http://krm.yj20258.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ody.shanyushiyangkeji.top

[Q10] 插入单行
来源：http://hrh.tian-w.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hyy.fengsongda.top

[Q11] 一次插入多行
来源：http://bqb.pycfn.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://qhv.zhoulong.xyz

[Q12] 插入后取自增 ID
来源：http://hcf.yj20258888.top

INSERT INTO users (name) VALUES ('C');
来源：http://ocq.jyoumei.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://pif.9152youxi.cn

[Q13] 忽略重复插入
来源：http://fus.hfpthk.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://bin.cheryme.top

[Q14] 存在则更新（upsert）
来源：http://xvb.sxryk.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://eqt.guannengcc.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://fyi.zycfv.cn

[Q15] 查询全部
来源：http://ttg.yuanzhike.top

SELECT * FROM users;
来源：http://mbk.kuanghao11.cn

[Q16] 查询指定列
来源：http://dnl.jinyuanbaomall.cn

SELECT id, name FROM users;
来源：http://gwu.yj20258888.top

[Q17] 条件查询
来源：http://ztp.zdqjudy.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://qsu.daria6918.cn

[Q18] 模糊匹配
来源：http://yuq.jqgufenzy.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ned.aizwys.cn

[Q19] 范围查询
来源：http://drd.haohaochexian.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mai.guannengcc.top

[Q20] IN 列表
来源：http://ubs.xingfuxueyuan.xyz

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://cee.sweek.top

[Q21] 空值判断
来源：http://qnv.cdnleiting.top

SELECT * FROM users WHERE email IS NULL;
来源：http://qqp.sxryk.cn

[Q22] 排序
来源：http://zjm.daxiang520.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://vhy.hammf.cn

[Q23] 分页
来源：http://txb.xylfe.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mit.jinqigfzy.top

[Q24] 去重
来源：http://juk.shanyushiyangkeji.top

SELECT DISTINCT city FROM users;
来源：http://mvp.shuidangran.top

[Q25] 只取前 N 条
来源：http://qil.snrcjt.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://esc.yongpay.top

[Q26] 计数
来源：http://zep.jinghuilouyu.cn

SELECT COUNT(*) FROM users;
来源：http://soj.bbcook.cn

[Q27] 条件计数
来源：http://tae.fengsongda.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://yjc.svipenyu.cn

[Q28] 求和与平均
来源：http://vhp.xylfe.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://vvm.hfpthk.cn

[Q29] 最大最小值
来源：http://rxb.tianlin.xyz

SELECT MAX(age), MIN(age) FROM users;
来源：http://qgp.cashguo.top

[Q30] 分组统计
来源：http://iwy.yfazqb.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://fqw.ppjwa.cn

[Q31] 分组后过滤
来源：http://yrt.hcnkem.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wce.jiagoushi.top

[Q32] 分组拼接字符串
来源：http://jmj.ybcxt.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://myc.chenjidiqi.icu

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://tea.zhijiandao.cn

[Q33] 多列分组
来源：http://tze.zhixingplan.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://qbj.jyoumei.cn

[Q34] 每组取第一条
来源：http://zob.zhiwuduotai.top

SELECT * FROM (
来源：http://ctx.xuanzx.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://nep.hcnkem.com

) t WHERE rn = 1;
来源：http://rpk.zycfv.cn

[Q35] 内连接
来源：http://nho.redwolf501.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://bqy.guowangkeji.top

[Q36] 左连接
来源：http://gpi.hesvh.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://fts.jqgfzy.top

[Q37] 右连接
来源：http://odf.shanyushiyangkeji.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ian.yongpay.top

[Q38] 全外连接（PostgreSQL）
来源：http://ipk.pengpengdd.cyou

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://tev.cashguo.top

[Q39] 自连接（查上下级）
来源：http://qid.jinqigufen.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://dci.316326.xyz

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://jtc.quarkkingdee.top

[Q40] 交叉连接（笛卡尔积）
来源：http://mmv.ybcxt.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wwj.0kj1m.cn

[Q41] 多表连接
来源：http://qfv.gotoacloud.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://fxn.sysykeji.top

JOIN users u ON u.id = o.user_id
来源：http://udp.yangfankeji.com

JOIN products p ON p.id = o.product_id;
来源：http://jii.jqgfzy.top

[Q42] 连接条件附加过滤
来源：http://muw.andypj.xyz

SELECT u.name, o.amount FROM users u
来源：http://gmw.fzhhl.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://phr.sxryk.cn

[Q43] 标量子查询
来源：http://unp.gotoacloud.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ray.yuanzhike.top

[Q44] IN 子查询
来源：http://kup.dianchejie.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://gcr.hysaishi.cn

[Q45] EXISTS 判断存在
来源：http://pbm.gotoacloud.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zjd.meibo888.top

[Q46] NOT EXISTS 判断不存在
来源：http://gkb.cucudq.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bdi.hysaishi.cn

[Q47] 与平均值比较
来源：http://xld.zdbjq.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://bpi.zdqjudy.top

[Q48] CTE 公用表表达式
来源：http://xoy.ppjwa.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://abe.cucudq.cn

SELECT * FROM t WHERE c > 5;
来源：http://ssp.jinqigfzy.top

[Q49] 更新单行
来源：http://ymm.shuidangran.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://qpu.yj20258.top

[Q50] 批量更新
来源：http://roa.cheryme.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://huw.shuidangran.top

[Q51] 用子查询更新
来源：http://hef.nwbrower.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://vwz.chenlongwang.top

[Q52] 删除指定行
来源：http://zfy.316326.xyz

DELETE FROM users WHERE id = 10;
来源：http://tkh.cucudq.cn

[Q53] 按条件删除
来源：http://gee.feifeiyinyue.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://gsq.zhijiandao.cn

[Q54] 清空表
来源：http://ekl.hnxiangtu.top

TRUNCATE TABLE logs;
来源：http://vct.wangshuangyany.cn

[Q55] 排名（并列占位）
来源：http://xii.iojbl.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://giz.yfazqb.com

[Q56] 密集排名（并列不占位）
来源：http://gbr.iojbl.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://bvm.nanxinkj.top

[Q57] 行号
来源：http://yqx.zhengqikj.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://qbv.bbcook.cn

[Q58] 累计求和
来源：http://rxw.tarul.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://aca.zhoulong.xyz

[Q59] 分组内累计
来源：http://cfs.yj202588.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ugq.smart0.xyz

[Q60] 取上一行 / 下一行
来源：http://ahd.yj20258.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://dmi.vehdjk.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://jmt.hysaishi.cn

[Q61] 移动平均
来源：http://zhh.gotoacloud.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://nbq.zhixingplan.top

[Q62] 分组占比
来源：http://cdl.vqdsnc.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://yna.feifeiyinyue.top

[Q63] 开启事务
来源：http://nss.zhengqikj.top

START TRANSACTION;                -- 或 BEGIN
来源：http://axs.nwbrower.top

[Q64] 提交事务
来源：http://fxf.hcnkem.com

COMMIT;
来源：http://zvz.zhaomingkeji.xyz

[Q65] 回滚事务
来源：http://pju.fehbvm.com

ROLLBACK;
来源：http://fgk.fzhhl.top

[Q66] 行锁查询
来源：http://cph.yueranfly.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://enw.yangfankeji.com

[Q67] 设置隔离级别
来源：http://sli.cqqwz.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://jmw.0kj1m.cn

[Q68] 保存点
来源：http://hxs.guowangkeji.top

SAVEPOINT sp1;
来源：http://pgr.sysykeji.top

ROLLBACK TO sp1;
来源：http://wvf.pycfn.com

[Q69] 查看执行计划
来源：http://voh.epnwcf.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://xzb.fengsongda.top

[Q70] 更新统计信息
来源：http://zfq.feifeiyinyue.top

ANALYZE TABLE users;
来源：http://uxx.cqqwz.cn

[Q71] 查看建表语句
来源：http://yrm.ehwqpu.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://uer.sysykeji.top

[Q72] 查看索引
来源：http://jef.bjfxy.top

SHOW INDEX FROM users;
来源：http://axf.tianlin.xyz

[Q73] 查看表状态
来源：http://ylb.quarkkingdee.top

SHOW TABLE STATUS LIKE 'users';
来源：http://xza.quarkkingdee.top

[Q74] 强制使用索引
来源：http://axq.hcnkem.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://yna.jiagoushi.top

[Q75] 日期格式化
来源：http://elu.cashguo.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mug.hesvh.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wua.zhaomingkeji.xyz

[Q76] 按天统计
来源：http://fzw.wangshuangyany.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://pao.fktsv.cn

[Q77] 时间加减
来源：http://twv.aibaodan.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://dmz.xuanzx.com

[Q78] 当前时间
来源：http://nwf.ybcxt.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://nmf.zhongyouzk.top

[Q79] 字符串拼接
来源：http://ydt.wangshuangyany.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://vyp.fzhhl.top

[Q80] 字符串截取
来源：http://psx.ehwqpu.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://izp.vqdsnc.cn

[Q81] 字符串替换
来源：http://rxa.jianghu66.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://clf.gogol.net.cn

[Q82] 字符长度与字节长度
来源：http://top.jlsjyb.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://rms.zycfv.cn

[Q83] 大小写转换
来源：http://uno.uphjek.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://xrr.xuetiantiany.cn

[Q84] 去除首尾空格
来源：http://trg.yuanzhike.top

SELECT TRIM(name) FROM users;
来源：http://osl.tarul.cn

[Q85] 数值取整
来源：http://vht.chenjidiqi.icu

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://fjk.epnwcf.com

[Q86] 读取 JSON 字段
来源：http://plb.nwbrower.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://fke.jqgufenzy.top

[Q87] JSON 字段做条件
来源：http://obw.daria6918.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://sto.nanxinkj.top

[Q88] 行转列（条件聚合）
来源：http://jgh.316326.xyz

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://zpb.xylfe.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://bgs.chenlongwang.top

[Q89] 判断表是否存在
来源：http://nql.svipenyu.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://sww.yueranfly.top

[Q90] 生成序号列
来源：http://tnq.xuetiantiany.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hra.0kj1m.cn

================================================================================
来源：http://oxw.hysaishi.cn

R. Bash 专题
来源：http://yjl.316326.xyz

================================================================================
来源：http://rrm.zycfv.cn

[R01] shebang 与严格模式
来源：http://nbd.uphjek.com

#!/usr/bin/env bash
来源：http://vtv.shzxlz.cn

set -euo pipefail
来源：http://nip.hesvh.cn

[R02] 变量赋值与使用
来源：http://kna.wangdashe.top

name="Tom"; echo "$name"
来源：http://lhc.dianchejie.cn

[R03] 只读变量
来源：http://cmd.gotoacloud.top

readonly PI=3.14
来源：http://oaw.hywenlv.cn

[R04] 位置参数
来源：http://xec.tarul.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://eqq.cashguo.top

[R05] 参数默认值
来源：http://xjy.yj20258888.top

name="${1:-default}"
来源：http://xiw.nanxinkj.top

[R06] 判断命令是否存在
来源：http://wcj.tian-w.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://poq.yvedp.cn

[R07] if 判断文件
来源：http://uhk.jlsjyb.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://vig.ppjwa.cn

[R08] 数值比较
来源：http://cqa.chenlongwang.top

if (( a > b )); then echo "a 更大"; fi
来源：http://lwh.dianchejie.cn

[R09] 字符串比较
来源：http://ycc.fehbvm.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://xxe.nanxinkj.top

[R10] 正则匹配
来源：http://kzt.dianchejie.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://aud.nanxinkj.top

[R11] case 多分支
来源：http://gcn.yongpay.top

case "$1" in
来源：http://qqv.316326.xyz

start) echo "启动" ;;
来源：http://fke.sufxvd.cn

stop)  echo "停止" ;;
来源：http://jaz.jianghu66.top

*)     echo "未知命令" ;;
来源：http://hbn.mhx1999.top

esac
来源：http://dvz.tianlin.xyz

[R12] for 遍历文件
来源：http://yjx.ybcxt.top

for f in *.txt; do echo "$f"; done
来源：http://xsf.yj20258888.top

[R13] for 计数循环
来源：http://qkb.fehbvm.com

for i in {1..10}; do echo "$i"; done
来源：http://hso.c1oappe.top

[R14] C 风格 for
来源：http://aoz.iojbl.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hwk.haohaochexian.top

[R15] while 逐行读文件
来源：http://jsd.gzhubu.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://viw.cucudq.cn

[R16] until 等待条件
来源：http://bjt.tanke756.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://amb.fanxiaobao.xyz

[R17] 数组定义与取值
来源：http://vfk.zhongyouzk.top

arr=(a b c); echo "${arr[0]}"
来源：http://mrg.xuanzx.com

[R18] 遍历数组
来源：http://qjg.nwbrower.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://pqv.nanxuanxn.top

[R19] 数组长度
来源：http://hvb.cheryme.top

echo "${#arr[@]}"
来源：http://wxu.guannengcc.top

[R20] 关联数组（字典）
来源：http://kca.chenjidiqi.icu

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ddp.tian-w.cn

[R21] 字符串长度
来源：http://fcv.aibaodan.cn

echo "${#s}"
来源：http://eca.haohaochexian.top

[R22] 截取子串
来源：http://pfg.zhongyouzk.top

echo "${s:0:5}"
来源：http://jxz.ivvv.top

[R23] 字符串替换
来源：http://lcx.gotoacloud.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://glf.0kj1m.cn

[R24] 大小写转换
来源：http://pqc.andypj.xyz

echo "${s^^}"; echo "${s,,}"
来源：http://pyl.yj20258.top

[R25] 去后缀 / 去前缀
来源：http://olo.birdmap.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://nnk.svipenyu.cn

[R26] 命令替换
来源：http://syv.hysaishi.cn

now=$(date +%F); echo "$now"
来源：http://yxn.birdmap.top

[R27] 算术展开
来源：http://qcp.guannengcc.top


<!-- 参考信息 -->