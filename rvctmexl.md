代发 wailian999

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://yzk.dashuyun.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://xsl.uphjek.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://utv.jiagoushi.top

PHP:  if (empty($x)) {}
来源：http://mus.jqgufenzy.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://suj.nanxinkj.top

TS:   if (x == null) {}
来源：http://uqx.sjlbkw.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://adz.aizwys.cn

Go:   if x == nil {}
来源：http://qda.gogol.net.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://fsf.meibo888.top

C#:   if (x is null) {}
来源：http://uuq.guowangkeji.top

[P07] 防抖与节流
来源：http://muz.jinqigfzy.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://pzv.ehwqpu.com

PHP:  // 手写时间戳比较
来源：http://qyz.aizwys.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://leh.zhixingplan.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pux.jinghuilouyu.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mxw.sweek.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://cfg.dashuyun.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://esp.yuanzhike.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wcx.hnqzz.top

[P08] 处理浮点精度问题
来源：http://gbd.sufxvd.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://glk.yuxming.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://nir.snrcjt.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://vyi.yj20258888.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://xka.9152youxi.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://sga.yongpay.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ofi.xinyue.icu

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://xho.jqgfzy.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://rvt.pycfn.com

================================================================================
来源：http://hzj.hnxiangtu.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ccf.zhongyouzk.top

================================================================================
来源：http://xfi.fanxiaobao.xyz

[Q01] 创建表
来源：http://gbd.havefunace.top

CREATE TABLE users (
来源：http://yby.hongshengwenyu.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://tyw.fehbvm.com

name VARCHAR(50) NOT NULL,
来源：http://urx.tanke756.top

email VARCHAR(100) UNIQUE,
来源：http://dvz.9152youxi.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://djh.iojbl.cn

);
来源：http://mqu.xuanzx.com

[Q02] 创建带外键的表
来源：http://ikk.zhiwuduotai.top

CREATE TABLE orders (
来源：http://fjk.yonumen.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://htx.feifeiyinyue.top

user_id INT NOT NULL,
来源：http://rjm.cheryme.top

amount DECIMAL(10, 2),
来源：http://cdx.ivvv.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hnj.guowangkeji.top

);
来源：http://rfb.cdnleiting.top

[Q03] 增加列
来源：http://pwo.fktsv.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://bpe.yfazqb.com

[Q04] 修改列类型
来源：http://khe.snrcjt.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://qil.daria6918.cn

[Q05] 重命名列
来源：http://pbm.hfpthk.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://bfq.shuidangran.top

[Q06] 删除列
来源：http://wio.0kj1m.cn

ALTER TABLE users DROP COLUMN age;
来源：http://orf.birdmap.top

[Q07] 删除表
来源：http://rpp.nanxinkj.top

DROP TABLE IF EXISTS orders;
来源：http://dbs.zhiwuduotai.top

[Q08] 创建普通索引
来源：http://ien.ywan-chungtsiang.top

CREATE INDEX idx_users_email ON users(email);
来源：http://sxp.jyoumei.cn

[Q09] 创建唯一索引
来源：http://lxy.svipenyu.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://htk.shanyushiyangkeji.top

[Q10] 插入单行
来源：http://bya.yuxming.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://dig.aizwys.cn

[Q11] 一次插入多行
来源：http://uab.haohaochexian.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ajm.andypj.xyz

[Q12] 插入后取自增 ID
来源：http://tbs.kuanghao11.cn

INSERT INTO users (name) VALUES ('C');
来源：http://eqs.ppjwa.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://pss.wangdashe.top

[Q13] 忽略重复插入
来源：http://cnw.yuanzhike.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://tfx.feifeiyinyue.top

[Q14] 存在则更新（upsert）
来源：http://efy.sjlbkw.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://nfh.ywan-chungtsiang.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://lvo.aizwys.cn

[Q15] 查询全部
来源：http://zlc.vqdsnc.cn

SELECT * FROM users;
来源：http://zzh.chenzaomai.com

[Q16] 查询指定列
来源：http://ptx.xuanzx.com

SELECT id, name FROM users;
来源：http://fco.bbcook.cn

[Q17] 条件查询
来源：http://bye.sjlbkw.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ypp.sweek.top

[Q18] 模糊匹配
来源：http://hpr.fengsongda.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ooo.kuanghao11.cn

[Q19] 范围查询
来源：http://enm.cdnleiting.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wvm.bbcook.cn

[Q20] IN 列表
来源：http://ccu.xuanzx.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://yhs.yuanzhike.top

[Q21] 空值判断
来源：http://ppb.tian-w.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://dmd.smart0.xyz

[Q22] 排序
来源：http://voe.svipenyu.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://gci.bjfxy.top

[Q23] 分页
来源：http://mlp.fzhhl.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://pmq.zdbjq.cn

[Q24] 去重
来源：http://uji.quarkkingdee.top

SELECT DISTINCT city FROM users;
来源：http://wee.yj202588.top

[Q25] 只取前 N 条
来源：http://gzl.yueranfly.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://cso.shzxlz.cn

[Q26] 计数
来源：http://val.birdmap.top

SELECT COUNT(*) FROM users;
来源：http://hsu.zdqjudy.top

[Q27] 条件计数
来源：http://cmq.jqgufenzy.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://jfb.wangshuangyany.cn

[Q28] 求和与平均
来源：http://tzm.cucudq.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://aio.nwbrower.top

[Q29] 最大最小值
来源：http://hhw.cashguo.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://jnm.aizwys.cn

[Q30] 分组统计
来源：http://psf.fengsongda.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://bdr.daxiang520.top

[Q31] 分组后过滤
来源：http://itk.andypj.xyz

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ibs.smart0.xyz

[Q32] 分组拼接字符串
来源：http://asn.shzxlz.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://fpk.wangshuangyany.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mzl.sufxvd.cn

[Q33] 多列分组
来源：http://qps.guannengcc.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://eok.chenlongwang.top

[Q34] 每组取第一条
来源：http://vhc.guowangkeji.top

SELECT * FROM (
来源：http://iza.fzhhl.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://dsp.zhongyouzk.top

) t WHERE rn = 1;
来源：http://nwr.chenlongwang.top

[Q35] 内连接
来源：http://gcg.pycfn.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wjk.jlsjyb.cn

[Q36] 左连接
来源：http://rmr.fktsv.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://owq.nanxuanxn.top

[Q37] 右连接
来源：http://nba.daria6918.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://cvj.jinyuanbaomall.cn

[Q38] 全外连接（PostgreSQL）
来源：http://czt.yfazqb.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://xub.xylfe.cn

[Q39] 自连接（查上下级）
来源：http://tlf.kuanghao11.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ijo.svipenyu.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://tpk.iojbl.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://fud.quarkkingdee.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://otp.snrcjt.cn

[Q41] 多表连接
来源：http://rze.redwolf501.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://pbm.ywan-chungtsiang.top

JOIN users u ON u.id = o.user_id
来源：http://bjq.ywan-chungtsiang.top

JOIN products p ON p.id = o.product_id;
来源：http://tqt.zycfv.cn

[Q42] 连接条件附加过滤
来源：http://ljq.cheryme.top

SELECT u.name, o.amount FROM users u
来源：http://ryc.ppjwa.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://gbb.zhaomingkeji.xyz

[Q43] 标量子查询
来源：http://yoi.yonumen.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://tnk.xziqi.cn

[Q44] IN 子查询
来源：http://fqu.tarul.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://yfa.xziqi.cn

[Q45] EXISTS 判断存在
来源：http://fer.jianghu66.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://veu.daria6918.cn

[Q46] NOT EXISTS 判断不存在
来源：http://fnk.cashguo.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://lzd.bbcook.cn

[Q47] 与平均值比较
来源：http://uad.sweek.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mmt.gotoacloud.top

[Q48] CTE 公用表表达式
来源：http://swc.316326.xyz

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://asb.sjlbkw.cn

SELECT * FROM t WHERE c > 5;
来源：http://lwy.zhixingplan.top

[Q49] 更新单行
来源：http://jxw.xinyue.icu

UPDATE users SET status = 1 WHERE id = 10;
来源：http://uxa.zdbjq.cn

[Q50] 批量更新
来源：http://hju.316326.xyz

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://rgx.meibo888.top

[Q51] 用子查询更新
来源：http://ugg.ppjwa.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ron.tianlin.xyz

[Q52] 删除指定行
来源：http://aqd.c1oappe.top

DELETE FROM users WHERE id = 10;
来源：http://dwp.ywan-chungtsiang.top

[Q53] 按条件删除
来源：http://nxk.hammf.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://bqt.hesvh.cn

[Q54] 清空表
来源：http://avr.hongshengwenyu.top

TRUNCATE TABLE logs;
来源：http://sno.xuanzx.com

[Q55] 排名（并列占位）
来源：http://nui.snrcjt.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://uys.gogol.net.cn

[Q56] 密集排名（并列不占位）
来源：http://ubq.guannengcc.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://kjm.tarul.cn

[Q57] 行号
来源：http://wlt.ybcxt.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://epn.0kj1m.cn

[Q58] 累计求和
来源：http://nld.fengsongda.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://itk.guowangkeji.top

[Q59] 分组内累计
来源：http://ysb.iojbl.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://dty.wangdashe.top

[Q60] 取上一行 / 下一行
来源：http://vhp.pycfn.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://sfw.0kj1m.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hpn.yueranfly.top

[Q61] 移动平均
来源：http://yce.shanyushiyangkeji.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://yht.yj20258888.top

[Q62] 分组占比
来源：http://smt.ywan-chungtsiang.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://oew.pycfn.com

[Q63] 开启事务
来源：http://jmf.haohaochexian.top

START TRANSACTION;                -- 或 BEGIN
来源：http://qfg.yanxiufei.cn

[Q64] 提交事务
来源：http://hgd.chenjidiqi.icu

COMMIT;
来源：http://sqg.snrcjt.cn

[Q65] 回滚事务
来源：http://nry.dianchejie.cn

ROLLBACK;
来源：http://qma.bbcook.cn

[Q66] 行锁查询
来源：http://ace.hnxiangtu.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://jvx.feifeiyinyue.top

[Q67] 设置隔离级别
来源：http://jow.nwbrower.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mmv.ivvv.top

[Q68] 保存点
来源：http://ibf.fktsv.cn

SAVEPOINT sp1;
来源：http://zvr.jlsjyb.cn

ROLLBACK TO sp1;
来源：http://qph.daria6918.cn

[Q69] 查看执行计划
来源：http://pgq.cashguo.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://tbr.birdmap.top

[Q70] 更新统计信息
来源：http://bvr.tianlin.xyz

ANALYZE TABLE users;
来源：http://kye.52xcode.cn

[Q71] 查看建表语句
来源：http://fsl.xuanzx.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://inb.redwolf501.top

[Q72] 查看索引
来源：http://vyl.xziqi.cn

SHOW INDEX FROM users;
来源：http://bgx.xingfuxueyuan.xyz

[Q73] 查看表状态
来源：http://iua.hywenlv.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://rwy.chenlongwang.top

[Q74] 强制使用索引
来源：http://emm.shuidangran.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://xto.yj20258888.top

[Q75] 日期格式化
来源：http://hnv.bbcook.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://por.jyoumei.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://oum.uphjek.com

[Q76] 按天统计
来源：http://aws.c1oappe.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://rei.gotoacloud.top

[Q77] 时间加减
来源：http://jku.0kj1m.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://uuy.ydzc1.top

[Q78] 当前时间
来源：http://rdv.havefunace.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://vpq.ydzc1.top

[Q79] 字符串拼接
来源：http://dzj.yanxiufei.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://vsp.smart0.xyz

[Q80] 字符串截取
来源：http://vgc.xziqi.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://dmy.sweek.top

[Q81] 字符串替换
来源：http://zfl.xuanzx.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://qor.yuxming.cn

[Q82] 字符长度与字节长度
来源：http://ofk.52xcode.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://tkh.shanyushiyangkeji.top

[Q83] 大小写转换
来源：http://cfh.c1oappe.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://znw.yvedp.cn

[Q84] 去除首尾空格
来源：http://pno.sweek.top

SELECT TRIM(name) FROM users;
来源：http://oub.ehwqpu.com

[Q85] 数值取整
来源：http://tva.shanyushiyangtech.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://nqe.cqqwz.cn

[Q86] 读取 JSON 字段
来源：http://rkd.quarkkingdee.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://yqa.chenlongwang.top

[Q87] JSON 字段做条件
来源：http://tso.yangfankeji.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://scq.yuxming.cn

[Q88] 行转列（条件聚合）
来源：http://mxq.vehdjk.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://jvg.ydjk.org.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wat.ppjwa.cn

[Q89] 判断表是否存在
来源：http://iby.hnxiangtu.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://lky.xuetiantiany.cn

[Q90] 生成序号列
来源：http://kiy.hesvh.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://rby.hammf.cn

================================================================================
来源：http://gep.52xcode.cn

R. Bash 专题
来源：http://xgt.fengsongda.top

================================================================================
来源：http://zgw.guannengcc.top

[R01] shebang 与严格模式
来源：http://ymy.xuanzx.com

#!/usr/bin/env bash
来源：http://uro.aibaodan.cn

set -euo pipefail
来源：http://xig.fehbvm.com

[R02] 变量赋值与使用
来源：http://xqp.zdqjudy.top

name="Tom"; echo "$name"
来源：http://nvh.tanke756.top

[R03] 只读变量
来源：http://kjh.jqgufenzy.top

readonly PI=3.14
来源：http://duf.havefunace.top

[R04] 位置参数
来源：http://xqr.yj20258888.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://htq.zhiwuduotai.top

[R05] 参数默认值
来源：http://fss.xuanzx.com

name="${1:-default}"
来源：http://uof.sweek.top

[R06] 判断命令是否存在
来源：http://qkm.dashuyun.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ipi.aizwys.cn

[R07] if 判断文件
来源：http://ane.yfazqb.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wnv.chenlongwang.top

[R08] 数值比较
来源：http://ffg.svipenyu.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://mix.daxiang520.top

[R09] 字符串比较
来源：http://qjw.fktsv.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://xhq.yvedp.cn

[R10] 正则匹配
来源：http://wnx.zycfv.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://czu.epnwcf.com

[R11] case 多分支
来源：http://jfz.hnqzz.top

case "$1" in
来源：http://gyd.yfazqb.com

start) echo "启动" ;;
来源：http://njs.jinyuanbaomall.cn

stop)  echo "停止" ;;
来源：http://hqz.yuxming.cn

*)     echo "未知命令" ;;
来源：http://gvb.guannengcc.top

esac
来源：http://paa.daria6918.cn

[R12] for 遍历文件
来源：http://isb.yvedp.cn

for f in *.txt; do echo "$f"; done
来源：http://qnl.redwolf501.top

[R13] for 计数循环
来源：http://ogg.aizwys.cn

for i in {1..10}; do echo "$i"; done
来源：http://xeu.jqgfzy.top

[R14] C 风格 for
来源：http://ekm.fzhhl.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://qmh.meibo888.top

[R15] while 逐行读文件
来源：http://mxf.nanxuanxn.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://bym.ehwqpu.com

[R16] until 等待条件
来源：http://lme.xziqi.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://yzg.dianchejie.cn

[R17] 数组定义与取值
来源：http://aqn.jianghu66.top

arr=(a b c); echo "${arr[0]}"
来源：http://atw.meibo888.top

[R18] 遍历数组
来源：http://ovz.wangshuangyany.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://xnq.chenjidiqi.icu

[R19] 数组长度
来源：http://pfz.pengpengdd.cyou

echo "${#arr[@]}"
来源：http://uef.gogol.net.cn

[R20] 关联数组（字典）
来源：http://hwk.yj20258888.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://jyn.smart0.xyz

[R21] 字符串长度
来源：http://vkl.ivvv.top

echo "${#s}"
来源：http://cin.ydjk.org.cn

[R22] 截取子串
来源：http://nym.iojbl.cn

echo "${s:0:5}"
来源：http://gki.dashuyun.cn

[R23] 字符串替换
来源：http://omd.snrcjt.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://fpm.havefunace.top

[R24] 大小写转换
来源：http://wqn.wangshuangyany.cn

echo "${s^^}"; echo "${s,,}"
来源：http://wvq.haohaochexian.top

[R25] 去后缀 / 去前缀
来源：http://fyh.cqqwz.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ahr.ybcxt.top

[R26] 命令替换
来源：http://kwn.svipenyu.cn

now=$(date +%F); echo "$now"
来源：http://yby.wangshuangyany.cn

[R27] 算术展开
来源：http://hqj.vqdsnc.cn

echo $((1 + 2 * 3))
来源：http://ujj.yj20258888.top

[R28] 浮点运算
来源：http://voa.yuanzhike.top

echo "scale=2; 10/3" | bc
来源：http://feh.zhaomingkeji.xyz

[R29] 定义函数
来源：http://oaq.jiagoushi.top


<!-- 参考信息 -->