代发 wailian999

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://zao.ppjwa.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://vrq.bjfxy.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://qxo.pycfn.com

PHP:  if (empty($x)) {}
来源：http://uoo.bjfxy.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://vwa.hongshengwenyu.top

TS:   if (x == null) {}
来源：http://rju.tian-w.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://she.zhongyouzk.top

Go:   if x == nil {}
来源：http://hgd.epnwcf.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ctl.sufxvd.cn

C#:   if (x is null) {}
来源：http://veh.fktsv.cn

[P07] 防抖与节流
来源：http://sgd.daria6918.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://sxw.hywenlv.cn

PHP:  // 手写时间戳比较
来源：http://khv.feifeiyinyue.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mpj.ywan-chungtsiang.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://akv.mhx1999.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://kbb.ywan-chungtsiang.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://geh.zhiwuduotai.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://mrz.hywenlv.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://cqa.jinghuilouyu.cn

[P08] 处理浮点精度问题
来源：http://kxo.ctjpmb.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ibb.yonumen.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://eaf.shanyushiyangtech.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://spt.yj202588.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://prg.quarkkingdee.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://vns.feifeiyinyue.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ssx.havefunace.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ukl.fktsv.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://eey.ehwqpu.com

================================================================================
来源：http://ntv.zhijiandao.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://dfl.yfazqb.com

================================================================================
来源：http://qwk.pengpengdd.cyou

[Q01] 创建表
来源：http://nfy.zhengqikj.top

CREATE TABLE users (
来源：http://hzi.pengpengdd.cyou

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://rdw.gogol.net.cn

name VARCHAR(50) NOT NULL,
来源：http://srf.uphjek.com

email VARCHAR(100) UNIQUE,
来源：http://gev.kuanghao11.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ltt.chenlongwang.top

);
来源：http://eqy.yueranfly.top

[Q02] 创建带外键的表
来源：http://jzm.kuanghao11.cn

CREATE TABLE orders (
来源：http://bcp.jianghu66.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://fks.pengpengdd.cyou

user_id INT NOT NULL,
来源：http://tlt.zdqjudy.top

amount DECIMAL(10, 2),
来源：http://ysk.yfazqb.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://dfm.mhx1999.top

);
来源：http://dpd.chenlongwang.top

[Q03] 增加列
来源：http://mdx.nanxuanxn.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://rjk.zycfv.cn

[Q04] 修改列类型
来源：http://wns.yuxming.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://kpr.fzhhl.top

[Q05] 重命名列
来源：http://jcq.zdbjq.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://rmw.316326.xyz

[Q06] 删除列
来源：http://ufo.zhiwuduotai.top

ALTER TABLE users DROP COLUMN age;
来源：http://jcf.ctjpmb.com

[Q07] 删除表
来源：http://cyw.chenjidiqi.icu

DROP TABLE IF EXISTS orders;
来源：http://dnl.jinyuanbaomall.cn

[Q08] 创建普通索引
来源：http://uoq.shanyushiyangkeji.top

CREATE INDEX idx_users_email ON users(email);
来源：http://qtj.9152youxi.cn

[Q09] 创建唯一索引
来源：http://pio.fanxiaobao.xyz

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://lel.jqgfzy.top

[Q10] 插入单行
来源：http://qcw.zhixingplan.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://prp.yj20258.top

[Q11] 一次插入多行
来源：http://fgx.hnxiangtu.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://dvr.ydjk.org.cn

[Q12] 插入后取自增 ID
来源：http://pbz.shzxlz.cn

INSERT INTO users (name) VALUES ('C');
来源：http://qex.pengpengdd.cyou

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://msy.pycfn.com

[Q13] 忽略重复插入
来源：http://vya.zhengqikj.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://gaj.chenlongwang.top

[Q14] 存在则更新（upsert）
来源：http://oqk.fengsongda.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mpb.9152youxi.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://xni.yuanzhike.top

[Q15] 查询全部
来源：http://gug.quarkkingdee.top

SELECT * FROM users;
来源：http://fnb.jinqigufen.top

[Q16] 查询指定列
来源：http://hal.fktsv.cn

SELECT id, name FROM users;
来源：http://ret.meibo888.top

[Q17] 条件查询
来源：http://dnd.9152youxi.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wwl.xziqi.cn

[Q18] 模糊匹配
来源：http://ucj.nanxinkj.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://agl.svipenyu.cn

[Q19] 范围查询
来源：http://hbc.jlsjyb.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://fpz.hcnkem.com

[Q20] IN 列表
来源：http://rpa.yvedp.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://kzq.fzhhl.top

[Q21] 空值判断
来源：http://vtw.haohaochexian.top

SELECT * FROM users WHERE email IS NULL;
来源：http://wrh.gogol.net.cn

[Q22] 排序
来源：http://jdj.xziqi.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://xwz.0kj1m.cn

[Q23] 分页
来源：http://nuj.andypj.xyz

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://enz.iojbl.cn

[Q24] 去重
来源：http://kab.hongshengwenyu.top

SELECT DISTINCT city FROM users;
来源：http://daf.jinqigufen.top

[Q25] 只取前 N 条
来源：http://hux.ybcxt.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mej.andypj.xyz

[Q26] 计数
来源：http://dqa.yj20258888.top

SELECT COUNT(*) FROM users;
来源：http://ftw.shzxlz.cn

[Q27] 条件计数
来源：http://ubp.jianghu66.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://zwg.pycfn.com

[Q28] 求和与平均
来源：http://egn.pycfn.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://yag.ppjwa.cn

[Q29] 最大最小值
来源：http://ikb.xuanzx.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://xdu.cashguo.top

[Q30] 分组统计
来源：http://vax.xuanzx.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://noz.gogol.net.cn

[Q31] 分组后过滤
来源：http://ckg.xingfuxueyuan.xyz

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://whi.ywan-chungtsiang.top

[Q32] 分组拼接字符串
来源：http://gma.quarkkingdee.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hej.fktsv.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://huc.tianlin.xyz

[Q33] 多列分组
来源：http://tnx.hcnkem.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mrf.yanxiufei.cn

[Q34] 每组取第一条
来源：http://mmd.shzxlz.cn

SELECT * FROM (
来源：http://uva.sjlbkw.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mpv.wangdashe.top

) t WHERE rn = 1;
来源：http://zhk.yanxiufei.cn

[Q35] 内连接
来源：http://fph.52xcode.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://asy.cucudq.cn

[Q36] 左连接
来源：http://dmd.aibaodan.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://jfb.wangshuangyany.cn

[Q37] 右连接
来源：http://bue.kuanghao11.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://zqk.chenzaomai.com

[Q38] 全外连接（PostgreSQL）
来源：http://coo.cdnleiting.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://zak.zhijiandao.cn

[Q39] 自连接（查上下级）
来源：http://ybu.epnwcf.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://hjs.jinqigufen.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://qhl.hywenlv.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://lvd.guowangkeji.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://rmq.aizwys.cn

[Q41] 多表连接
来源：http://lvs.pycfn.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://qje.xuetiantiany.cn

JOIN users u ON u.id = o.user_id
来源：http://vix.yj20258.top

JOIN products p ON p.id = o.product_id;
来源：http://vta.xziqi.cn

[Q42] 连接条件附加过滤
来源：http://hhx.nwbrower.top

SELECT u.name, o.amount FROM users u
来源：http://tul.ctjpmb.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://rln.yuanzhike.top

[Q43] 标量子查询
来源：http://ypb.bbcook.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://yxe.zhiwuduotai.top

[Q44] IN 子查询
来源：http://djy.yfazqb.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://zto.sufxvd.cn

[Q45] EXISTS 判断存在
来源：http://kwr.nanxuanxn.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kxn.jqgfzy.top

[Q46] NOT EXISTS 判断不存在
来源：http://swh.nanxinkj.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wti.daria6918.cn

[Q47] 与平均值比较
来源：http://yjl.shangyingyoupin.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://whr.ydzc1.top

[Q48] CTE 公用表表达式
来源：http://mmw.zhiwuduotai.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mfk.haohaochexian.top

SELECT * FROM t WHERE c > 5;
来源：http://bml.cdnleiting.top

[Q49] 更新单行
来源：http://amn.yueranfly.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://kap.xylfe.cn

[Q50] 批量更新
来源：http://lzq.andypj.xyz

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ras.svipenyu.cn

[Q51] 用子查询更新
来源：http://zrh.hongshengwenyu.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://lqp.cqqwz.cn

[Q52] 删除指定行
来源：http://xth.shanyushiyangtech.top

DELETE FROM users WHERE id = 10;
来源：http://egp.0kj1m.cn

[Q53] 按条件删除
来源：http://rke.ppjwa.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ufy.guannengcc.top

[Q54] 清空表
来源：http://upk.hnqzz.top

TRUNCATE TABLE logs;
来源：http://uql.redwolf501.top

[Q55] 排名（并列占位）
来源：http://zqk.jinqigfzy.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://kwk.pengpengdd.cyou

[Q56] 密集排名（并列不占位）
来源：http://yoc.zhongyouzk.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hsw.yj202588.top

[Q57] 行号
来源：http://iax.zhoulong.xyz

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://rxq.pycfn.com

[Q58] 累计求和
来源：http://sms.pycfn.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://gvo.fengsongda.top

[Q59] 分组内累计
来源：http://duu.yangfankeji.com

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://tld.kuanghao11.cn

[Q60] 取上一行 / 下一行
来源：http://scn.hfpthk.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://omf.jinqigufen.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://gdg.ybcxt.top

[Q61] 移动平均
来源：http://bxt.daxiang520.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://kqm.dashuyun.cn

[Q62] 分组占比
来源：http://fvc.52xcode.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://nwb.fzhhl.top

[Q63] 开启事务
来源：http://qyh.cheryme.top

START TRANSACTION;                -- 或 BEGIN
来源：http://oqr.ywan-chungtsiang.top

[Q64] 提交事务
来源：http://lrx.cashguo.top

COMMIT;
来源：http://vto.yangfankeji.com

[Q65] 回滚事务
来源：http://olv.snrcjt.cn

ROLLBACK;
来源：http://unf.smart0.xyz

[Q66] 行锁查询
来源：http://juj.jiagoushi.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://seg.uphjek.com

[Q67] 设置隔离级别
来源：http://lkh.fengsongda.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://rkh.shanyushiyangkeji.top

[Q68] 保存点
来源：http://vpi.dianchejie.cn

SAVEPOINT sp1;
来源：http://xtw.zhijiandao.cn

ROLLBACK TO sp1;
来源：http://kay.hesvh.cn

[Q69] 查看执行计划
来源：http://fon.chenlongwang.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://kin.cashguo.top

[Q70] 更新统计信息
来源：http://pcg.ivvv.top

ANALYZE TABLE users;
来源：http://lgg.bbcook.cn

[Q71] 查看建表语句
来源：http://pid.snrcjt.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://lej.shanyushiyangtech.top

[Q72] 查看索引
来源：http://slg.shangyingyoupin.top

SHOW INDEX FROM users;
来源：http://cfw.sufxvd.cn

[Q73] 查看表状态
来源：http://ase.zdbjq.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://mja.0kj1m.cn

[Q74] 强制使用索引
来源：http://dng.cashguo.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://fmq.cashguo.top

[Q75] 日期格式化
来源：http://rrb.jqgufenzy.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://lqi.aizwys.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://prg.guannengcc.top

[Q76] 按天统计
来源：http://lvc.hnqzz.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://jbd.yj20258888.top

[Q77] 时间加减
来源：http://ldp.jinqigfzy.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://kxy.fzhhl.top

[Q78] 当前时间
来源：http://xpm.sweek.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hne.sxryk.cn

[Q79] 字符串拼接
来源：http://tvt.xylfe.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://eyh.vqdsnc.cn

[Q80] 字符串截取
来源：http://ppe.bbcook.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://kss.xylfe.cn

[Q81] 字符串替换
来源：http://dkp.mhx1999.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://gpb.hnqzz.top

[Q82] 字符长度与字节长度
来源：http://yol.dianchejie.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://vro.sysykeji.top

[Q83] 大小写转换
来源：http://tmk.zycfv.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ndn.ydzc1.top

[Q84] 去除首尾空格
来源：http://qem.gzhubu.top

SELECT TRIM(name) FROM users;
来源：http://mvn.jianghu66.top

[Q85] 数值取整
来源：http://vuh.sufxvd.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://lrj.yj20258888.top

[Q86] 读取 JSON 字段
来源：http://vka.yj202588.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://llh.jyoumei.cn

[Q87] JSON 字段做条件
来源：http://wyo.kuanghao11.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://jfm.xziqi.cn

[Q88] 行转列（条件聚合）
来源：http://vyj.jinqigufen.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ewh.snrcjt.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://edf.fengsongda.top

[Q89] 判断表是否存在
来源：http://frz.dianchejie.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mbw.mhx1999.top

[Q90] 生成序号列
来源：http://ccj.zdbjq.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ost.316326.xyz

================================================================================
来源：http://dcc.uphjek.com

R. Bash 专题
来源：http://omu.cheryme.top

================================================================================
来源：http://svc.yj202588.top

[R01] shebang 与严格模式
来源：http://vgs.xingfuxueyuan.xyz

#!/usr/bin/env bash
来源：http://zko.zhijiandao.cn

set -euo pipefail
来源：http://lgo.yuxming.cn

[R02] 变量赋值与使用
来源：http://vog.jqgufenzy.top

name="Tom"; echo "$name"
来源：http://ssx.yj20258888.top

[R03] 只读变量
来源：http://ocs.cdnleiting.top

readonly PI=3.14
来源：http://lsm.hywenlv.cn

[R04] 位置参数
来源：http://bqb.yj20258.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://jgp.zhongyouzk.top

[R05] 参数默认值
来源：http://ipp.yueranfly.top

name="${1:-default}"
来源：http://fst.fzhhl.top

[R06] 判断命令是否存在
来源：http://uev.zhoulong.xyz

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://cgb.bbcook.cn

[R07] if 判断文件
来源：http://flk.cucudq.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://vme.snrcjt.cn

[R08] 数值比较
来源：http://dal.hnqzz.top

if (( a > b )); then echo "a 更大"; fi
来源：http://bnr.zhongyouzk.top

[R09] 字符串比较
来源：http://lth.iojbl.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://awk.chenlongwang.top

[R10] 正则匹配
来源：http://oqj.xuanzx.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://qfn.feifeiyinyue.top

[R11] case 多分支
来源：http://xaj.yuxming.cn

case "$1" in
来源：http://ikf.sjlbkw.cn

start) echo "启动" ;;
来源：http://woh.zhoulong.xyz

stop)  echo "停止" ;;
来源：http://asm.jinqigfzy.top

*)     echo "未知命令" ;;
来源：http://sdz.0kj1m.cn

esac
来源：http://hbz.316326.xyz

[R12] for 遍历文件
来源：http://cju.vqdsnc.cn

for f in *.txt; do echo "$f"; done
来源：http://cuy.c1oappe.top

[R13] for 计数循环
来源：http://ykv.mhx1999.top

for i in {1..10}; do echo "$i"; done
来源：http://axb.xuetiantiany.cn

[R14] C 风格 for
来源：http://qtf.zhongyouzk.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://aea.nanxinkj.top

[R15] while 逐行读文件
来源：http://fdk.quarkkingdee.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://loa.yonumen.top

[R16] until 等待条件
来源：http://lqp.hywenlv.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mfm.feifeiyinyue.top

[R17] 数组定义与取值
来源：http://yak.9152youxi.cn

arr=(a b c); echo "${arr[0]}"
来源：http://oyb.haohaochexian.top

[R18] 遍历数组
来源：http://kue.ybcxt.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://sam.kuanghao11.cn

[R19] 数组长度
来源：http://zev.quarkkingdee.top

echo "${#arr[@]}"
来源：http://gpd.52xcode.cn

[R20] 关联数组（字典）
来源：http://szt.pycfn.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ewy.epnwcf.com

[R21] 字符串长度
来源：http://fbu.jianghu66.top

echo "${#s}"
来源：http://uzx.andypj.xyz

[R22] 截取子串
来源：http://zur.meibo888.top

echo "${s:0:5}"
来源：http://yxj.zycfv.cn

[R23] 字符串替换
来源：http://doa.bbcook.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://xor.yuanzhike.top

[R24] 大小写转换
来源：http://nwa.ybcxt.top

echo "${s^^}"; echo "${s,,}"
来源：http://ufr.cheryme.top

[R25] 去后缀 / 去前缀
来源：http://wby.cdnleiting.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://vxf.zhixingplan.top

[R26] 命令替换
来源：http://sff.yuanzhike.top

now=$(date +%F); echo "$now"
来源：http://eyj.sxryk.cn

[R27] 算术展开
来源：http://hhq.pengpengdd.cyou

echo $((1 + 2 * 3))
来源：http://ejs.shanyushiyangkeji.top

[R28] 浮点运算
来源：http://hun.cdnleiting.top

echo "scale=2; 10/3" | bc
来源：http://qcn.iojbl.cn

[R29] 定义函数
来源：http://ogp.yongpay.top


<!-- 参考信息 -->