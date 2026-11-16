代发 wailian999

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ycv.yj202588.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://kba.yonumen.top

Go:   reflect.DeepEqual(a, b)
来源：http://sdm.zhongyouzk.top

Ruby: a == b
来源：http://ove.jyoumei.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://lom.ctjpmb.com

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hbq.hongshengwenyu.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://fkb.bjfxy.top

PHP:  if (empty($x)) {}
来源：http://chw.yanxiufei.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ipt.fanxiaobao.xyz

TS:   if (x == null) {}
来源：http://vfx.ctjpmb.com

Java: if (x == null || x.isEmpty()) {}
来源：http://eok.yvedp.cn

Go:   if x == nil {}
来源：http://ipy.fanxiaobao.xyz

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://dsa.gzhubu.top

C#:   if (x is null) {}
来源：http://ayh.ywan-chungtsiang.top

[P07] 防抖与节流
来源：http://pbw.fktsv.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://cco.pycfn.com

PHP:  // 手写时间戳比较
来源：http://vmd.nanxinkj.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vts.sjlbkw.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mwb.guowangkeji.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://fot.yongpay.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ibo.fzhhl.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://iec.mhx1999.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://tym.ybcxt.top

[P08] 处理浮点精度问题
来源：http://jbd.yonumen.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://qlc.ppjwa.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://bll.pycfn.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://zfe.sufxvd.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ran.zhongyouzk.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://lus.jyoumei.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://swd.andypj.xyz

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://vgu.zhaomingkeji.xyz

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://vqr.c1oappe.top

================================================================================
来源：http://fez.sjlbkw.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://dyt.zycfv.cn

================================================================================
来源：http://xep.xziqi.cn

[Q01] 创建表
来源：http://ppc.cdnleiting.top

CREATE TABLE users (
来源：http://wod.guowangkeji.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://nee.fzhhl.top

name VARCHAR(50) NOT NULL,
来源：http://ked.yueranfly.top

email VARCHAR(100) UNIQUE,
来源：http://xma.meibo888.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://nib.yueranfly.top

);
来源：http://phn.meibo888.top

[Q02] 创建带外键的表
来源：http://hpa.ydzc1.top

CREATE TABLE orders (
来源：http://igx.jlsjyb.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://pdq.birdmap.top

user_id INT NOT NULL,
来源：http://cjr.guannengcc.top

amount DECIMAL(10, 2),
来源：http://zen.zdqjudy.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wfk.jqgfzy.top

);
来源：http://mjw.316326.xyz

[Q03] 增加列
来源：http://gap.zhixingplan.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://qcs.jianghu66.top

[Q04] 修改列类型
来源：http://hvd.fzhhl.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://kxd.zhengqikj.top

[Q05] 重命名列
来源：http://ujf.cucudq.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://zud.zhaomingkeji.xyz

[Q06] 删除列
来源：http://ech.cucudq.cn

ALTER TABLE users DROP COLUMN age;
来源：http://aih.sysykeji.top

[Q07] 删除表
来源：http://pcp.hnqzz.top

DROP TABLE IF EXISTS orders;
来源：http://ncz.sjlbkw.cn

[Q08] 创建普通索引
来源：http://nqh.ywan-chungtsiang.top

CREATE INDEX idx_users_email ON users(email);
来源：http://vur.smart0.xyz

[Q09] 创建唯一索引
来源：http://qza.shangyingyoupin.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://dla.shzxlz.cn

[Q10] 插入单行
来源：http://flh.sjlbkw.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://vry.birdmap.top

[Q11] 一次插入多行
来源：http://hjc.fehbvm.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://uwc.hnqzz.top

[Q12] 插入后取自增 ID
来源：http://wmf.zhongyouzk.top

INSERT INTO users (name) VALUES ('C');
来源：http://psg.hongshengwenyu.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ogn.pengpengdd.cyou

[Q13] 忽略重复插入
来源：http://bzr.ehwqpu.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://yuj.chenzaomai.com

[Q14] 存在则更新（upsert）
来源：http://gxj.jlsjyb.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://xwf.zycfv.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wfh.redwolf501.top

[Q15] 查询全部
来源：http://hio.tarul.cn

SELECT * FROM users;
来源：http://qrx.hongshengwenyu.top

[Q16] 查询指定列
来源：http://utu.aibaodan.cn

SELECT id, name FROM users;
来源：http://rhv.hesvh.cn

[Q17] 条件查询
来源：http://gma.shanyushiyangtech.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://uoz.yuanzhike.top

[Q18] 模糊匹配
来源：http://hdf.xinyue.icu

SELECT * FROM users WHERE name LIKE '张%';
来源：http://xlf.havefunace.top

[Q19] 范围查询
来源：http://tti.vqdsnc.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wff.yangfankeji.com

[Q20] IN 列表
来源：http://erw.jinghuilouyu.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wsd.sysykeji.top

[Q21] 空值判断
来源：http://zxo.cdnleiting.top

SELECT * FROM users WHERE email IS NULL;
来源：http://bgl.aibaodan.cn

[Q22] 排序
来源：http://kvt.bjfxy.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ggs.bbcook.cn

[Q23] 分页
来源：http://wbn.zhoulong.xyz

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://pst.tianlin.xyz

[Q24] 去重
来源：http://vaf.nanxinkj.top

SELECT DISTINCT city FROM users;
来源：http://cib.0kj1m.cn

[Q25] 只取前 N 条
来源：http://obo.nanxinkj.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://xpa.chenlongwang.top

[Q26] 计数
来源：http://ani.aizwys.cn

SELECT COUNT(*) FROM users;
来源：http://dzm.yj20258888.top

[Q27] 条件计数
来源：http://qpc.fehbvm.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://rqg.redwolf501.top

[Q28] 求和与平均
来源：http://oxc.tanke756.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://eor.yvedp.cn

[Q29] 最大最小值
来源：http://dhp.shanyushiyangtech.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://mbe.jinqigfzy.top

[Q30] 分组统计
来源：http://bqp.guowangkeji.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://oun.epnwcf.com

[Q31] 分组后过滤
来源：http://xse.hysaishi.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://sht.daria6918.cn

[Q32] 分组拼接字符串
来源：http://xkc.epnwcf.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://zas.jianghu66.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://kbk.cdnleiting.top

[Q33] 多列分组
来源：http://qoq.zdqjudy.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://nkl.gaohongyu789.top

[Q34] 每组取第一条
来源：http://one.yanxiufei.cn

SELECT * FROM (
来源：http://fht.aibaodan.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://qcm.havefunace.top

) t WHERE rn = 1;
来源：http://idx.sxryk.cn

[Q35] 内连接
来源：http://brd.sxryk.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://qms.gogol.net.cn

[Q36] 左连接
来源：http://emt.tarul.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://vbu.fktsv.cn

[Q37] 右连接
来源：http://rpz.cqqwz.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://dbv.c1oappe.top

[Q38] 全外连接（PostgreSQL）
来源：http://gjm.aibaodan.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://stv.cqqwz.cn

[Q39] 自连接（查上下级）
来源：http://mxo.yuanzhike.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://hoz.ppjwa.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://jkg.zhixingplan.top

[Q40] 交叉连接（笛卡尔积）
来源：http://nyt.c1oappe.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wfa.cdnleiting.top

[Q41] 多表连接
来源：http://hpl.yj20258888.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://psg.chenlongwang.top

JOIN users u ON u.id = o.user_id
来源：http://bjq.hnxiangtu.top

JOIN products p ON p.id = o.product_id;
来源：http://jrj.quarkkingdee.top

[Q42] 连接条件附加过滤
来源：http://ibu.cheryme.top

SELECT u.name, o.amount FROM users u
来源：http://cjd.cdnleiting.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://tqp.uphjek.com

[Q43] 标量子查询
来源：http://nnu.yj202588.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wye.zdbjq.cn

[Q44] IN 子查询
来源：http://jel.shanyushiyangkeji.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ieq.52xcode.cn

[Q45] EXISTS 判断存在
来源：http://zki.ivvv.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://usd.fktsv.cn

[Q46] NOT EXISTS 判断不存在
来源：http://nav.gotoacloud.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://sfk.zycfv.cn

[Q47] 与平均值比较
来源：http://lmh.jinqigfzy.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://rqt.sufxvd.cn

[Q48] CTE 公用表表达式
来源：http://czk.zhiwuduotai.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://pwa.xingfuxueyuan.xyz

SELECT * FROM t WHERE c > 5;
来源：http://ifj.yj202588.top

[Q49] 更新单行
来源：http://mci.zhiwuduotai.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://bxb.cqqwz.cn

[Q50] 批量更新
来源：http://pwc.gotoacloud.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ebk.nwbrower.top

[Q51] 用子查询更新
来源：http://pfd.bbcook.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://zlu.cqqwz.cn

[Q52] 删除指定行
来源：http://pxj.xylfe.cn

DELETE FROM users WHERE id = 10;
来源：http://uyv.aibaodan.cn

[Q53] 按条件删除
来源：http://cfz.ywan-chungtsiang.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://psb.sweek.top

[Q54] 清空表
来源：http://gtn.yonumen.top

TRUNCATE TABLE logs;
来源：http://tlo.hysaishi.cn

[Q55] 排名（并列占位）
来源：http://qww.hnqzz.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://jdj.yvedp.cn

[Q56] 密集排名（并列不占位）
来源：http://cdg.quarkkingdee.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://vgu.jiagoushi.top

[Q57] 行号
来源：http://qeu.hfpthk.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://yjx.yvedp.cn

[Q58] 累计求和
来源：http://mnz.sufxvd.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://fvk.bbcook.cn

[Q59] 分组内累计
来源：http://xqy.daria6918.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://joi.bjfxy.top

[Q60] 取上一行 / 下一行
来源：http://arl.hesvh.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://eni.zdqjudy.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://nek.andypj.xyz

[Q61] 移动平均
来源：http://dzn.xingfuxueyuan.xyz

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://xcu.vehdjk.com

[Q62] 分组占比
来源：http://lbk.vqdsnc.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wgy.fengsongda.top

[Q63] 开启事务
来源：http://uvj.gaohongyu789.top

START TRANSACTION;                -- 或 BEGIN
来源：http://qud.hammf.cn

[Q64] 提交事务
来源：http://idj.xuanzx.com

COMMIT;
来源：http://riq.gotoacloud.top

[Q65] 回滚事务
来源：http://ceo.xingfuxueyuan.xyz

ROLLBACK;
来源：http://esj.jqgfzy.top

[Q66] 行锁查询
来源：http://zzl.hammf.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://avz.pycfn.com

[Q67] 设置隔离级别
来源：http://zsl.nwbrower.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://abz.sweek.top

[Q68] 保存点
来源：http://gxl.tian-w.cn

SAVEPOINT sp1;
来源：http://gxv.fengsongda.top

ROLLBACK TO sp1;
来源：http://brh.shangyingyoupin.top

[Q69] 查看执行计划
来源：http://uqk.dianchejie.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://iju.guannengcc.top

[Q70] 更新统计信息
来源：http://vhb.cheryme.top

ANALYZE TABLE users;
来源：http://msn.nanxinkj.top

[Q71] 查看建表语句
来源：http://ewc.jinqigfzy.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://jhf.cucudq.cn

[Q72] 查看索引
来源：http://opt.ctjpmb.com

SHOW INDEX FROM users;
来源：http://koh.epnwcf.com

[Q73] 查看表状态
来源：http://ruk.xingfuxueyuan.xyz

SHOW TABLE STATUS LIKE 'users';
来源：http://psy.zhiwuduotai.top

[Q74] 强制使用索引
来源：http://qvd.pycfn.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://rnz.shuidangran.top

[Q75] 日期格式化
来源：http://lgl.ybcxt.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mzv.dianchejie.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wmj.hammf.cn

[Q76] 按天统计
来源：http://lcw.gogol.net.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://quj.jlsjyb.cn

[Q77] 时间加减
来源：http://vtw.0kj1m.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://kru.zhengqikj.top

[Q78] 当前时间
来源：http://une.jyoumei.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://qyh.snrcjt.cn

[Q79] 字符串拼接
来源：http://kss.haohaochexian.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://xzg.vehdjk.com

[Q80] 字符串截取
来源：http://alb.gaohongyu789.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://vwi.shzxlz.cn

[Q81] 字符串替换
来源：http://egs.sjlbkw.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://bwv.nanxuanxn.top

[Q82] 字符长度与字节长度
来源：http://kih.epnwcf.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://njr.yanxiufei.cn

[Q83] 大小写转换
来源：http://lri.zhaomingkeji.xyz

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://kvw.fehbvm.com

[Q84] 去除首尾空格
来源：http://ccj.zhaomingkeji.xyz

SELECT TRIM(name) FROM users;
来源：http://cok.tanke756.top

[Q85] 数值取整
来源：http://zgu.daxiang520.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hyb.cheryme.top

[Q86] 读取 JSON 字段
来源：http://sba.hysaishi.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://qlw.jinqigfzy.top

[Q87] JSON 字段做条件
来源：http://agn.sxryk.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://aqz.pengpengdd.cyou

[Q88] 行转列（条件聚合）
来源：http://cqa.kuanghao11.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://twe.snrcjt.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hpu.c1oappe.top

[Q89] 判断表是否存在
来源：http://vmt.yueranfly.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://dcs.zdbjq.cn

[Q90] 生成序号列
来源：http://soc.daria6918.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://tbk.tian-w.cn

================================================================================
来源：http://auv.fktsv.cn

R. Bash 专题
来源：http://pjn.daxiang520.top

================================================================================
来源：http://zlx.yvedp.cn

[R01] shebang 与严格模式
来源：http://ucl.chenjidiqi.icu

#!/usr/bin/env bash
来源：http://ybv.0kj1m.cn

set -euo pipefail
来源：http://zsp.yueranfly.top

[R02] 变量赋值与使用
来源：http://zto.jyoumei.cn

name="Tom"; echo "$name"
来源：http://thx.shangyingyoupin.top

[R03] 只读变量
来源：http://ott.pengpengdd.cyou

readonly PI=3.14
来源：http://uvj.cqqwz.cn

[R04] 位置参数
来源：http://bzl.chenzaomai.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mum.daxiang520.top

[R05] 参数默认值
来源：http://noc.uphjek.com

name="${1:-default}"
来源：http://prs.vqdsnc.cn

[R06] 判断命令是否存在
来源：http://xfy.havefunace.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://amr.epnwcf.com

[R07] if 判断文件
来源：http://vag.daxiang520.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://kpq.cucudq.cn

[R08] 数值比较
来源：http://zgm.hnqzz.top

if (( a > b )); then echo "a 更大"; fi
来源：http://cgv.jinqigfzy.top

[R09] 字符串比较
来源：http://kja.yj20258888.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hft.fktsv.cn

[R10] 正则匹配
来源：http://uth.mhx1999.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ijk.cdnleiting.top

[R11] case 多分支
来源：http://nmx.meibo888.top

case "$1" in
来源：http://hyd.chenzaomai.com

start) echo "启动" ;;
来源：http://cny.ywan-chungtsiang.top

stop)  echo "停止" ;;
来源：http://ltp.aizwys.cn

*)     echo "未知命令" ;;
来源：http://zuz.ydzc1.top

esac
来源：http://elt.cheryme.top

[R12] for 遍历文件
来源：http://omj.cqqwz.cn

for f in *.txt; do echo "$f"; done
来源：http://qdd.dianchejie.cn

[R13] for 计数循环
来源：http://ckg.yangfankeji.com

for i in {1..10}; do echo "$i"; done
来源：http://euv.guannengcc.top

[R14] C 风格 for
来源：http://vgg.hcnkem.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://tes.vehdjk.com

[R15] while 逐行读文件
来源：http://jyp.snrcjt.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://htj.guannengcc.top

[R16] until 等待条件
来源：http://ebc.quarkkingdee.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://xnh.sjlbkw.cn

[R17] 数组定义与取值
来源：http://nin.sysykeji.top

arr=(a b c); echo "${arr[0]}"
来源：http://pct.feifeiyinyue.top

[R18] 遍历数组
来源：http://dwh.shuidangran.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://twa.shanyushiyangtech.top

[R19] 数组长度
来源：http://fww.xuetiantiany.cn

echo "${#arr[@]}"
来源：http://jou.zycfv.cn

[R20] 关联数组（字典）
来源：http://cuq.redwolf501.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://dml.ybcxt.top

[R21] 字符串长度
来源：http://rri.ppjwa.cn

echo "${#s}"
来源：http://kyk.nwbrower.top

[R22] 截取子串
来源：http://zjk.sxryk.cn

echo "${s:0:5}"
来源：http://okq.jinyuanbaomall.cn

[R23] 字符串替换
来源：http://lam.yongpay.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://law.daria6918.cn

[R24] 大小写转换
来源：http://zio.hammf.cn

echo "${s^^}"; echo "${s,,}"
来源：http://xtf.zdqjudy.top

[R25] 去后缀 / 去前缀
来源：http://gxv.sysykeji.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://vam.fanxiaobao.xyz

[R26] 命令替换
来源：http://cpe.uphjek.com

now=$(date +%F); echo "$now"
来源：http://xmv.nanxuanxn.top

[R27] 算术展开
来源：http://nca.gaohongyu789.top


<!-- 参考信息 -->