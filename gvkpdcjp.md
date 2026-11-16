代发 wailian999

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://bhs.chenzaomai.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://qqt.birdmap.top

Go:   reflect.DeepEqual(a, b)
来源：http://syg.chenzaomai.com

Ruby: a == b
来源：http://cde.shanyushiyangtech.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://zfk.cucudq.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://did.fktsv.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hfj.smart0.xyz

PHP:  if (empty($x)) {}
来源：http://peu.hysaishi.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://oco.ybcxt.top

TS:   if (x == null) {}
来源：http://wdc.dashuyun.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ajx.havefunace.top

Go:   if x == nil {}
来源：http://tfn.cucudq.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://lwl.yanxiufei.cn

C#:   if (x is null) {}
来源：http://dia.aibaodan.cn

[P07] 防抖与节流
来源：http://css.jinqigfzy.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://fap.jyoumei.cn

PHP:  // 手写时间戳比较
来源：http://oyj.jqgfzy.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cfo.tian-w.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://evl.shzxlz.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ymj.hysaishi.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://dgp.jyoumei.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://mri.ybcxt.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://qpf.vqdsnc.cn

[P08] 处理浮点精度问题
来源：http://ocd.c1oappe.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wyz.hcnkem.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ngl.fzhhl.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://iae.shzxlz.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://pkp.yj20258888.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wcn.jinghuilouyu.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ydo.jiagoushi.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://gap.sufxvd.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://vkj.yueranfly.top

================================================================================
来源：http://roe.chenjidiqi.icu

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mdg.jqgufenzy.top

================================================================================
来源：http://qob.zhongyouzk.top

[Q01] 创建表
来源：http://cnl.cqqwz.cn

CREATE TABLE users (
来源：http://ero.cqqwz.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://roo.snrcjt.cn

name VARCHAR(50) NOT NULL,
来源：http://uux.jinqigufen.top

email VARCHAR(100) UNIQUE,
来源：http://pow.xinyue.icu

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://gcb.svipenyu.cn

);
来源：http://hek.yvedp.cn

[Q02] 创建带外键的表
来源：http://tsa.epnwcf.com

CREATE TABLE orders (
来源：http://cfb.tianlin.xyz

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://fle.bjfxy.top

user_id INT NOT NULL,
来源：http://usa.bjfxy.top

amount DECIMAL(10, 2),
来源：http://tcg.wangshuangyany.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://omv.cashguo.top

);
来源：http://pab.yuxming.cn

[Q03] 增加列
来源：http://syi.chenlongwang.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hvi.cheryme.top

[Q04] 修改列类型
来源：http://odt.hysaishi.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://duj.guannengcc.top

[Q05] 重命名列
来源：http://dgw.havefunace.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://uyp.c1oappe.top

[Q06] 删除列
来源：http://azo.zdqjudy.top

ALTER TABLE users DROP COLUMN age;
来源：http://yop.0kj1m.cn

[Q07] 删除表
来源：http://atx.svipenyu.cn

DROP TABLE IF EXISTS orders;
来源：http://avz.jinyuanbaomall.cn

[Q08] 创建普通索引
来源：http://vfb.svipenyu.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://htk.shzxlz.cn

[Q09] 创建唯一索引
来源：http://yps.sufxvd.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ltb.gotoacloud.top

[Q10] 插入单行
来源：http://sec.daria6918.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://lef.tian-w.cn

[Q11] 一次插入多行
来源：http://ckb.birdmap.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://rwk.gotoacloud.top

[Q12] 插入后取自增 ID
来源：http://eqd.jyoumei.cn

INSERT INTO users (name) VALUES ('C');
来源：http://skg.yj20258.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mxe.smart0.xyz

[Q13] 忽略重复插入
来源：http://lzt.fehbvm.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://bud.tanke756.top

[Q14] 存在则更新（upsert）
来源：http://zpu.quarkkingdee.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://gxz.gzhubu.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blx.52xcode.cn

[Q15] 查询全部
来源：http://cvm.shangyingyoupin.top

SELECT * FROM users;
来源：http://qfw.ybcxt.top

[Q16] 查询指定列
来源：http://asn.zhoulong.xyz

SELECT id, name FROM users;
来源：http://frg.epnwcf.com

[Q17] 条件查询
来源：http://fvp.fanxiaobao.xyz

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://sms.chenjidiqi.icu

[Q18] 模糊匹配
来源：http://qyd.yj20258888.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wfv.chenjidiqi.icu

[Q19] 范围查询
来源：http://qop.shuidangran.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://rme.hammf.cn

[Q20] IN 列表
来源：http://ocj.cqqwz.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://exh.jqgfzy.top

[Q21] 空值判断
来源：http://rbb.zhiwuduotai.top

SELECT * FROM users WHERE email IS NULL;
来源：http://bqp.svipenyu.cn

[Q22] 排序
来源：http://ead.bbcook.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://cpj.quarkkingdee.top

[Q23] 分页
来源：http://sbt.shuidangran.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://bdv.birdmap.top

[Q24] 去重
来源：http://sny.0kj1m.cn

SELECT DISTINCT city FROM users;
来源：http://std.pycfn.com

[Q25] 只取前 N 条
来源：http://obf.yongpay.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://vkl.yonumen.top

[Q26] 计数
来源：http://anr.iojbl.cn

SELECT COUNT(*) FROM users;
来源：http://gdu.ydjk.org.cn

[Q27] 条件计数
来源：http://kzp.dashuyun.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wyg.hcnkem.com

[Q28] 求和与平均
来源：http://phz.tianlin.xyz

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://dml.cqqwz.cn

[Q29] 最大最小值
来源：http://syn.9152youxi.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://chj.zhongyouzk.top

[Q30] 分组统计
来源：http://dzy.cashguo.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://dnn.cucudq.cn

[Q31] 分组后过滤
来源：http://gix.xingfuxueyuan.xyz

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://jwl.hywenlv.cn

[Q32] 分组拼接字符串
来源：http://gqq.jinyuanbaomall.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://jta.nwbrower.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://vme.cqqwz.cn

[Q33] 多列分组
来源：http://zrg.ppjwa.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://bvo.hongshengwenyu.top

[Q34] 每组取第一条
来源：http://mmu.zhijiandao.cn

SELECT * FROM (
来源：http://dlh.epnwcf.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ckh.daria6918.cn

) t WHERE rn = 1;
来源：http://xvh.hnqzz.top

[Q35] 内连接
来源：http://cxt.zdqjudy.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://pha.xziqi.cn

[Q36] 左连接
来源：http://gef.tanke756.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://rzd.daria6918.cn

[Q37] 右连接
来源：http://cwm.shzxlz.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://sfy.jinqigufen.top

[Q38] 全外连接（PostgreSQL）
来源：http://byg.zhoulong.xyz

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://keq.cucudq.cn

[Q39] 自连接（查上下级）
来源：http://ggm.9152youxi.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://smh.yanxiufei.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://rcx.feifeiyinyue.top

[Q40] 交叉连接（笛卡尔积）
来源：http://zre.hammf.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://vmo.yj20258.top

[Q41] 多表连接
来源：http://fnv.feifeiyinyue.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://oyr.vehdjk.com

JOIN users u ON u.id = o.user_id
来源：http://gnq.ctjpmb.com

JOIN products p ON p.id = o.product_id;
来源：http://brb.gotoacloud.top

[Q42] 连接条件附加过滤
来源：http://juo.xinyue.icu

SELECT u.name, o.amount FROM users u
来源：http://tyc.shuidangran.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://vhi.sxryk.cn

[Q43] 标量子查询
来源：http://xrp.snrcjt.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://nzq.ehwqpu.com

[Q44] IN 子查询
来源：http://jdi.gogol.net.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ksd.xuanzx.com

[Q45] EXISTS 判断存在
来源：http://syx.zdqjudy.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://uuc.jianghu66.top

[Q46] NOT EXISTS 判断不存在
来源：http://uul.zhijiandao.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wnp.zdqjudy.top

[Q47] 与平均值比较
来源：http://onn.fanxiaobao.xyz

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://fsc.chenlongwang.top

[Q48] CTE 公用表表达式
来源：http://gnb.fktsv.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://caa.andypj.xyz

SELECT * FROM t WHERE c > 5;
来源：http://vdf.dashuyun.cn

[Q49] 更新单行
来源：http://yru.52xcode.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://zpi.svipenyu.cn

[Q50] 批量更新
来源：http://luq.jqgufenzy.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://yiz.guannengcc.top

[Q51] 用子查询更新
来源：http://exc.jinqigfzy.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://qao.epnwcf.com

[Q52] 删除指定行
来源：http://lwq.gzhubu.top

DELETE FROM users WHERE id = 10;
来源：http://fon.ctjpmb.com

[Q53] 按条件删除
来源：http://urc.nwbrower.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hrp.c1oappe.top

[Q54] 清空表
来源：http://usa.jinqigufen.top

TRUNCATE TABLE logs;
来源：http://kij.52xcode.cn

[Q55] 排名（并列占位）
来源：http://ymv.tanke756.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://yly.yj20258.top

[Q56] 密集排名（并列不占位）
来源：http://bdp.feifeiyinyue.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://kgb.hongshengwenyu.top

[Q57] 行号
来源：http://tyv.ydjk.org.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://kdy.jinqigufen.top

[Q58] 累计求和
来源：http://bie.svipenyu.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ggv.cucudq.cn

[Q59] 分组内累计
来源：http://kmh.quarkkingdee.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://gir.xinyue.icu

[Q60] 取上一行 / 下一行
来源：http://stn.hysaishi.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://nfv.nanxinkj.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://knr.316326.xyz

[Q61] 移动平均
来源：http://psq.andypj.xyz

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://kgo.9152youxi.cn

[Q62] 分组占比
来源：http://dea.tarul.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ley.hammf.cn

[Q63] 开启事务
来源：http://nww.mhx1999.top

START TRANSACTION;                -- 或 BEGIN
来源：http://pff.hammf.cn

[Q64] 提交事务
来源：http://fgz.nanxuanxn.top

COMMIT;
来源：http://xdz.xziqi.cn

[Q65] 回滚事务
来源：http://scq.kuanghao11.cn

ROLLBACK;
来源：http://unt.wangdashe.top

[Q66] 行锁查询
来源：http://asl.chenlongwang.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blh.yonumen.top

[Q67] 设置隔离级别
来源：http://sih.epnwcf.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://oyt.sufxvd.cn

[Q68] 保存点
来源：http://wcb.meibo888.top

SAVEPOINT sp1;
来源：http://rkt.fengsongda.top

ROLLBACK TO sp1;
来源：http://vjt.quarkkingdee.top

[Q69] 查看执行计划
来源：http://phc.zdqjudy.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://uls.yuxming.cn

[Q70] 更新统计信息
来源：http://woz.redwolf501.top

ANALYZE TABLE users;
来源：http://exb.yanxiufei.cn

[Q71] 查看建表语句
来源：http://pwz.pycfn.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://zva.nanxuanxn.top

[Q72] 查看索引
来源：http://fec.svipenyu.cn

SHOW INDEX FROM users;
来源：http://wns.9152youxi.cn

[Q73] 查看表状态
来源：http://vey.pengpengdd.cyou

SHOW TABLE STATUS LIKE 'users';
来源：http://fse.yongpay.top

[Q74] 强制使用索引
来源：http://aog.bbcook.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hxg.jyoumei.cn

[Q75] 日期格式化
来源：http://ztf.jinqigufen.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ubg.yuxming.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wmn.vqdsnc.cn

[Q76] 按天统计
来源：http://dxw.yfazqb.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://qpf.shanyushiyangtech.top

[Q77] 时间加减
来源：http://hsv.tian-w.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://lsv.9152youxi.cn

[Q78] 当前时间
来源：http://uop.sjlbkw.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://orj.xziqi.cn

[Q79] 字符串拼接
来源：http://ael.ydjk.org.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://zqj.sxryk.cn

[Q80] 字符串截取
来源：http://wvl.guowangkeji.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://xhd.jianghu66.top

[Q81] 字符串替换
来源：http://yed.yj20258888.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://vnb.wangshuangyany.cn

[Q82] 字符长度与字节长度
来源：http://tbo.hnxiangtu.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://its.yangfankeji.com

[Q83] 大小写转换
来源：http://tba.sweek.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ybd.wangdashe.top

[Q84] 去除首尾空格
来源：http://vmj.jinqigufen.top

SELECT TRIM(name) FROM users;
来源：http://cnl.chenjidiqi.icu

[Q85] 数值取整
来源：http://eqy.yangfankeji.com

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://frh.dashuyun.cn

[Q86] 读取 JSON 字段
来源：http://cuz.jqgufenzy.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://sjc.kuanghao11.cn

[Q87] JSON 字段做条件
来源：http://dzp.jqgufenzy.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://dkl.jianghu66.top

[Q88] 行转列（条件聚合）
来源：http://evi.uphjek.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://dnl.jinghuilouyu.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://efh.cqqwz.cn

[Q89] 判断表是否存在
来源：http://fih.tarul.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wvt.sysykeji.top

[Q90] 生成序号列
来源：http://fgz.yangfankeji.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mlh.svipenyu.cn

================================================================================
来源：http://adb.yj202588.top

R. Bash 专题
来源：http://thr.daria6918.cn

================================================================================
来源：http://ksc.cdnleiting.top

[R01] shebang 与严格模式
来源：http://pvk.sxryk.cn

#!/usr/bin/env bash
来源：http://tsm.haohaochexian.top

set -euo pipefail
来源：http://dkc.xuanzx.com

[R02] 变量赋值与使用
来源：http://lpk.fengsongda.top

name="Tom"; echo "$name"
来源：http://xwk.chenjidiqi.icu

[R03] 只读变量
来源：http://rgr.nanxinkj.top

readonly PI=3.14
来源：http://xxb.yuanzhike.top

[R04] 位置参数
来源：http://wla.sxryk.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://rkw.chenlongwang.top

[R05] 参数默认值
来源：http://uxn.vqdsnc.cn

name="${1:-default}"
来源：http://dms.bbcook.cn

[R06] 判断命令是否存在
来源：http://xlr.zhixingplan.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://cza.mhx1999.top

[R07] if 判断文件
来源：http://gxs.jlsjyb.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://pcw.vehdjk.com

[R08] 数值比较
来源：http://sjd.tanke756.top

if (( a > b )); then echo "a 更大"; fi
来源：http://cvd.shuidangran.top

[R09] 字符串比较
来源：http://uez.meibo888.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wwz.0kj1m.cn

[R10] 正则匹配
来源：http://vdz.ywan-chungtsiang.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://qch.ivvv.top

[R11] case 多分支
来源：http://jvi.yanxiufei.cn

case "$1" in
来源：http://fwn.jinghuilouyu.cn

start) echo "启动" ;;
来源：http://pek.fktsv.cn

stop)  echo "停止" ;;
来源：http://rtz.nwbrower.top

*)     echo "未知命令" ;;
来源：http://ewk.tianlin.xyz

esac
来源：http://ska.haohaochexian.top

[R12] for 遍历文件
来源：http://vqs.yuanzhike.top

for f in *.txt; do echo "$f"; done
来源：http://ydl.hfpthk.cn

[R13] for 计数循环
来源：http://ddr.yuanzhike.top

for i in {1..10}; do echo "$i"; done
来源：http://ukn.havefunace.top

[R14] C 风格 for
来源：http://tkb.zhixingplan.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://drl.sweek.top

[R15] while 逐行读文件
来源：http://mjy.yueranfly.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://qny.jiagoushi.top

[R16] until 等待条件
来源：http://tic.tanke756.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://vvn.hywenlv.cn

[R17] 数组定义与取值
来源：http://jvb.wangdashe.top

arr=(a b c); echo "${arr[0]}"
来源：http://gif.xuanzx.com

[R18] 遍历数组
来源：http://fvp.snrcjt.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://vqj.guowangkeji.top

[R19] 数组长度
来源：http://koq.cashguo.top

echo "${#arr[@]}"
来源：http://rsb.nanxuanxn.top

[R20] 关联数组（字典）
来源：http://riy.xylfe.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://zsp.yj20258.top

[R21] 字符串长度
来源：http://pio.zhaomingkeji.xyz

echo "${#s}"
来源：http://vwy.cucudq.cn

[R22] 截取子串
来源：http://cvl.ppjwa.cn

echo "${s:0:5}"
来源：http://ikh.epnwcf.com

[R23] 字符串替换
来源：http://uej.feifeiyinyue.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://zew.aibaodan.cn

[R24] 大小写转换
来源：http://bah.jinyuanbaomall.cn

echo "${s^^}"; echo "${s,,}"
来源：http://qgf.jqgfzy.top

[R25] 去后缀 / 去前缀
来源：http://oyy.andypj.xyz

echo "${f%.txt}"; echo "${f#./}"
来源：http://kbd.zdqjudy.top

[R26] 命令替换
来源：http://stw.fengsongda.top

now=$(date +%F); echo "$now"
来源：http://iso.jinqigufen.top

[R27] 算术展开
来源：http://bum.hnxiangtu.top


<!-- 参考信息 -->