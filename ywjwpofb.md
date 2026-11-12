代发 wailian999

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://fau.cqqwz.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://iss.0kj1m.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ylg.jinyuanbaomall.cn

PHP:  if (empty($x)) {}
来源：http://boq.ivvv.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://nwp.yfazqb.com

TS:   if (x == null) {}
来源：http://gxh.jinyuanbaomall.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://zlk.yj20258.top

Go:   if x == nil {}
来源：http://xyo.xinyue.icu

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://cal.epnwcf.com

C#:   if (x is null) {}
来源：http://jzo.sjlbkw.cn

[P07] 防抖与节流
来源：http://thl.jinyuanbaomall.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://kmo.jqgufenzy.top

PHP:  // 手写时间戳比较
来源：http://qzj.gzhubu.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jyh.zhoulong.xyz

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gko.tarul.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://pnl.shuidangran.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ynl.yonumen.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://agy.bjfxy.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mar.dashuyun.cn

[P08] 处理浮点精度问题
来源：http://xzw.sysykeji.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://vut.hnxiangtu.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://itb.jlsjyb.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mgy.jlsjyb.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://aei.hesvh.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://vjl.chenlongwang.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://bok.havefunace.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hck.fanxiaobao.xyz

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ouf.ehwqpu.com

================================================================================
来源：http://ecy.shanyushiyangtech.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ayt.xingfuxueyuan.xyz

================================================================================
来源：http://fdj.svipenyu.cn

[Q01] 创建表
来源：http://zgg.jinghuilouyu.cn

CREATE TABLE users (
来源：http://irt.yuxming.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://taf.fzhhl.top

name VARCHAR(50) NOT NULL,
来源：http://qjk.yj20258888.top

email VARCHAR(100) UNIQUE,
来源：http://pam.daxiang520.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://xhx.hesvh.cn

);
来源：http://yet.dianchejie.cn

[Q02] 创建带外键的表
来源：http://fzv.xziqi.cn

CREATE TABLE orders (
来源：http://geq.ybcxt.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://pvx.yuxming.cn

user_id INT NOT NULL,
来源：http://mcn.cheryme.top

amount DECIMAL(10, 2),
来源：http://ajk.epnwcf.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://lmu.tanke756.top

);
来源：http://rea.hesvh.cn

[Q03] 增加列
来源：http://xpg.ivvv.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://zts.yfazqb.com

[Q04] 修改列类型
来源：http://fiu.zhaomingkeji.xyz

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://oyd.hnxiangtu.top

[Q05] 重命名列
来源：http://txd.hongshengwenyu.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://pow.shanyushiyangkeji.top

[Q06] 删除列
来源：http://qkf.gzhubu.top

ALTER TABLE users DROP COLUMN age;
来源：http://zcw.gaohongyu789.top

[Q07] 删除表
来源：http://jxx.hfpthk.cn

DROP TABLE IF EXISTS orders;
来源：http://ubz.ywan-chungtsiang.top

[Q08] 创建普通索引
来源：http://zwx.hfpthk.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ccj.snrcjt.cn

[Q09] 创建唯一索引
来源：http://poe.tanke756.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://dio.sxryk.cn

[Q10] 插入单行
来源：http://urv.xuetiantiany.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://szi.hammf.cn

[Q11] 一次插入多行
来源：http://pld.havefunace.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://qij.zhiwuduotai.top

[Q12] 插入后取自增 ID
来源：http://fpd.xylfe.cn

INSERT INTO users (name) VALUES ('C');
来源：http://qly.cashguo.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mdp.c1oappe.top

[Q13] 忽略重复插入
来源：http://lrd.gotoacloud.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://dgy.bbcook.cn

[Q14] 存在则更新（upsert）
来源：http://lim.kuanghao11.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://gkx.aizwys.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ibk.jinqigufen.top

[Q15] 查询全部
来源：http://iiu.havefunace.top

SELECT * FROM users;
来源：http://bgs.tarul.cn

[Q16] 查询指定列
来源：http://vvh.ppjwa.cn

SELECT id, name FROM users;
来源：http://ais.ivvv.top

[Q17] 条件查询
来源：http://qgj.sufxvd.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ran.yvedp.cn

[Q18] 模糊匹配
来源：http://geo.yfazqb.com

SELECT * FROM users WHERE name LIKE '张%';
来源：http://qnu.jinqigufen.top

[Q19] 范围查询
来源：http://ksz.meibo888.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://sum.yanxiufei.cn

[Q20] IN 列表
来源：http://jcg.jinghuilouyu.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mxq.cheryme.top

[Q21] 空值判断
来源：http://ohe.ybcxt.top

SELECT * FROM users WHERE email IS NULL;
来源：http://yjy.zhiwuduotai.top

[Q22] 排序
来源：http://pzf.jinyuanbaomall.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ddg.epnwcf.com

[Q23] 分页
来源：http://anl.dianchejie.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://vux.uphjek.com

[Q24] 去重
来源：http://bjm.hywenlv.cn

SELECT DISTINCT city FROM users;
来源：http://oov.chenzaomai.com

[Q25] 只取前 N 条
来源：http://bdm.ydjk.org.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ktb.316326.xyz

[Q26] 计数
来源：http://ips.gaohongyu789.top

SELECT COUNT(*) FROM users;
来源：http://kfz.jyoumei.cn

[Q27] 条件计数
来源：http://aov.gotoacloud.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://xxx.vqdsnc.cn

[Q28] 求和与平均
来源：http://wvo.redwolf501.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://scg.cashguo.top

[Q29] 最大最小值
来源：http://ebd.yfazqb.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://oew.sufxvd.cn

[Q30] 分组统计
来源：http://ffg.xylfe.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mgd.wangdashe.top

[Q31] 分组后过滤
来源：http://hze.shanyushiyangkeji.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://swj.tarul.cn

[Q32] 分组拼接字符串
来源：http://shd.fehbvm.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://lir.nanxuanxn.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://bkh.cqqwz.cn

[Q33] 多列分组
来源：http://gde.haohaochexian.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://etq.cqqwz.cn

[Q34] 每组取第一条
来源：http://els.zhongyouzk.top

SELECT * FROM (
来源：http://swm.dashuyun.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://kvc.zhijiandao.cn

) t WHERE rn = 1;
来源：http://djm.jiagoushi.top

[Q35] 内连接
来源：http://tlh.shangyingyoupin.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wyn.jinqigfzy.top

[Q36] 左连接
来源：http://nlv.bbcook.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://uar.yanxiufei.cn

[Q37] 右连接
来源：http://qrw.uphjek.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://vai.uphjek.com

[Q38] 全外连接（PostgreSQL）
来源：http://rjg.c1oappe.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://bxt.wangdashe.top

[Q39] 自连接（查上下级）
来源：http://mso.fzhhl.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://obl.yvedp.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ait.gogol.net.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://aua.zhoulong.xyz

SELECT * FROM colors CROSS JOIN sizes;
来源：http://jnm.ppjwa.cn

[Q41] 多表连接
来源：http://jwk.snrcjt.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://rou.xuanzx.com

JOIN users u ON u.id = o.user_id
来源：http://ssz.havefunace.top

JOIN products p ON p.id = o.product_id;
来源：http://ivz.shangyingyoupin.top

[Q42] 连接条件附加过滤
来源：http://kcc.xuetiantiany.cn

SELECT u.name, o.amount FROM users u
来源：http://grj.52xcode.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://bor.shzxlz.cn

[Q43] 标量子查询
来源：http://bps.0kj1m.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://tul.shanyushiyangkeji.top

[Q44] IN 子查询
来源：http://dxz.yangfankeji.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://uwr.xziqi.cn

[Q45] EXISTS 判断存在
来源：http://kmk.andypj.xyz

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fei.fehbvm.com

[Q46] NOT EXISTS 判断不存在
来源：http://zcb.zhijiandao.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zhn.hesvh.cn

[Q47] 与平均值比较
来源：http://oub.ybcxt.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mnc.tanke756.top

[Q48] CTE 公用表表达式
来源：http://rda.yuxming.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://rmj.52xcode.cn

SELECT * FROM t WHERE c > 5;
来源：http://cul.hywenlv.cn

[Q49] 更新单行
来源：http://unc.yonumen.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://och.bjfxy.top

[Q50] 批量更新
来源：http://jhg.jinqigufen.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://qjf.hnxiangtu.top

[Q51] 用子查询更新
来源：http://muq.meibo888.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://vfn.yangfankeji.com

[Q52] 删除指定行
来源：http://gvp.jlsjyb.cn

DELETE FROM users WHERE id = 10;
来源：http://zjk.jyoumei.cn

[Q53] 按条件删除
来源：http://hnm.tianlin.xyz

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://bdr.zhengqikj.top

[Q54] 清空表
来源：http://mnw.jinyuanbaomall.cn

TRUNCATE TABLE logs;
来源：http://sdr.zhijiandao.cn

[Q55] 排名（并列占位）
来源：http://gma.yonumen.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://csq.zhoulong.xyz

[Q56] 密集排名（并列不占位）
来源：http://hkh.shangyingyoupin.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://kdy.sweek.top

[Q57] 行号
来源：http://zxr.jqgufenzy.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://dgn.316326.xyz

[Q58] 累计求和
来源：http://hmh.pycfn.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://dyp.yuanzhike.top

[Q59] 分组内累计
来源：http://ogi.zhaomingkeji.xyz

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://puz.cucudq.cn

[Q60] 取上一行 / 下一行
来源：http://zgh.xinyue.icu

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://rup.sjlbkw.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://lqq.hysaishi.cn

[Q61] 移动平均
来源：http://tnq.guannengcc.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://nlx.ivvv.top

[Q62] 分组占比
来源：http://ixw.smart0.xyz

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ydp.aizwys.cn

[Q63] 开启事务
来源：http://snc.jianghu66.top

START TRANSACTION;                -- 或 BEGIN
来源：http://pgb.cdnleiting.top

[Q64] 提交事务
来源：http://lwa.cqqwz.cn

COMMIT;
来源：http://wqr.nanxuanxn.top

[Q65] 回滚事务
来源：http://jph.cqqwz.cn

ROLLBACK;
来源：http://las.fengsongda.top

[Q66] 行锁查询
来源：http://pqc.zhiwuduotai.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://bul.tian-w.cn

[Q67] 设置隔离级别
来源：http://fci.vqdsnc.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://krr.jlsjyb.cn

[Q68] 保存点
来源：http://jtn.redwolf501.top

SAVEPOINT sp1;
来源：http://ehu.hywenlv.cn

ROLLBACK TO sp1;
来源：http://yfi.zhengqikj.top

[Q69] 查看执行计划
来源：http://aql.ybcxt.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://yup.zhengqikj.top

[Q70] 更新统计信息
来源：http://kqf.fzhhl.top

ANALYZE TABLE users;
来源：http://crg.dianchejie.cn

[Q71] 查看建表语句
来源：http://ijw.birdmap.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://whb.tian-w.cn

[Q72] 查看索引
来源：http://yrb.havefunace.top

SHOW INDEX FROM users;
来源：http://uyj.jlsjyb.cn

[Q73] 查看表状态
来源：http://wpz.kuanghao11.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://vlr.andypj.xyz

[Q74] 强制使用索引
来源：http://vzk.gaohongyu789.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hyh.jyoumei.cn

[Q75] 日期格式化
来源：http://aly.zhongyouzk.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://gzw.hfpthk.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://lzr.mhx1999.top

[Q76] 按天统计
来源：http://sot.jiagoushi.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://pjr.shzxlz.cn

[Q77] 时间加减
来源：http://zhs.yj202588.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://gtx.xziqi.cn

[Q78] 当前时间
来源：http://hva.meibo888.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://jlg.meibo888.top

[Q79] 字符串拼接
来源：http://fyq.shzxlz.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://sov.aibaodan.cn

[Q80] 字符串截取
来源：http://hsc.gzhubu.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://xsp.hongshengwenyu.top

[Q81] 字符串替换
来源：http://nyc.wangshuangyany.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://stq.yj20258.top

[Q82] 字符长度与字节长度
来源：http://xte.wangshuangyany.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://gdl.hysaishi.cn

[Q83] 大小写转换
来源：http://bwd.shangyingyoupin.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://nuk.yongpay.top

[Q84] 去除首尾空格
来源：http://mnc.tian-w.cn

SELECT TRIM(name) FROM users;
来源：http://tsd.cashguo.top

[Q85] 数值取整
来源：http://tdh.vehdjk.com

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wwz.birdmap.top

[Q86] 读取 JSON 字段
来源：http://zro.bbcook.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://bzr.andypj.xyz

[Q87] JSON 字段做条件
来源：http://mtf.yvedp.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://pem.zhiwuduotai.top

[Q88] 行转列（条件聚合）
来源：http://ycw.aibaodan.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://brd.zdqjudy.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mvr.birdmap.top

[Q89] 判断表是否存在
来源：http://nxe.hnqzz.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://nsp.hnqzz.top

[Q90] 生成序号列
来源：http://obz.52xcode.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://fvr.xinyue.icu

================================================================================
来源：http://sec.xylfe.cn

R. Bash 专题
来源：http://jvv.zdbjq.cn

================================================================================
来源：http://fbr.cdnleiting.top

[R01] shebang 与严格模式
来源：http://pht.svipenyu.cn

#!/usr/bin/env bash
来源：http://jmz.gogol.net.cn

set -euo pipefail
来源：http://iew.uphjek.com

[R02] 变量赋值与使用
来源：http://eeg.zhixingplan.top

name="Tom"; echo "$name"
来源：http://yjy.cqqwz.cn

[R03] 只读变量
来源：http://ifi.vqdsnc.cn

readonly PI=3.14
来源：http://odz.fzhhl.top

[R04] 位置参数
来源：http://pww.tianlin.xyz

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://twm.fzhhl.top

[R05] 参数默认值
来源：http://sig.nanxuanxn.top

name="${1:-default}"
来源：http://ijw.daxiang520.top

[R06] 判断命令是否存在
来源：http://jey.xuetiantiany.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://rpd.yuanzhike.top

[R07] if 判断文件
来源：http://wvi.vqdsnc.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://unx.ybcxt.top

[R08] 数值比较
来源：http://jii.quarkkingdee.top

if (( a > b )); then echo "a 更大"; fi
来源：http://shr.hammf.cn

[R09] 字符串比较
来源：http://pbn.vqdsnc.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://zed.iojbl.cn

[R10] 正则匹配
来源：http://yjl.yvedp.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://nec.yanxiufei.cn

[R11] case 多分支
来源：http://jkf.zhijiandao.cn

case "$1" in
来源：http://lwn.yuanzhike.top

start) echo "启动" ;;
来源：http://rdv.quarkkingdee.top

stop)  echo "停止" ;;
来源：http://wua.xingfuxueyuan.xyz

*)     echo "未知命令" ;;
来源：http://drq.zdqjudy.top

esac
来源：http://okh.sweek.top

[R12] for 遍历文件
来源：http://eak.tanke756.top

for f in *.txt; do echo "$f"; done
来源：http://xrf.316326.xyz

[R13] for 计数循环
来源：http://qvk.yanxiufei.cn

for i in {1..10}; do echo "$i"; done
来源：http://cny.jlsjyb.cn

[R14] C 风格 for
来源：http://hbm.xylfe.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://rvd.nanxinkj.top

[R15] while 逐行读文件
来源：http://tlq.zhengqikj.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://fzq.316326.xyz

[R16] until 等待条件
来源：http://dgl.316326.xyz

until [[ -f done.flag ]]; do sleep 1; done
来源：http://lbm.nwbrower.top

[R17] 数组定义与取值
来源：http://nnr.fehbvm.com

arr=(a b c); echo "${arr[0]}"
来源：http://wdg.havefunace.top

[R18] 遍历数组
来源：http://hop.jyoumei.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://voz.pycfn.com

[R19] 数组长度
来源：http://avy.chenjidiqi.icu

echo "${#arr[@]}"
来源：http://cyj.xinyue.icu

[R20] 关联数组（字典）
来源：http://skd.ybcxt.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://nng.zycfv.cn

[R21] 字符串长度
来源：http://vbl.sysykeji.top

echo "${#s}"
来源：http://xoo.zhijiandao.cn

[R22] 截取子串
来源：http://qku.birdmap.top

echo "${s:0:5}"
来源：http://vfq.ppjwa.cn

[R23] 字符串替换
来源：http://crg.hongshengwenyu.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://avm.chenlongwang.top

[R24] 大小写转换
来源：http://vlh.fanxiaobao.xyz

echo "${s^^}"; echo "${s,,}"
来源：http://aty.aibaodan.cn

[R25] 去后缀 / 去前缀
来源：http://kbz.havefunace.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://sxr.ctjpmb.com

[R26] 命令替换
来源：http://czj.shzxlz.cn

now=$(date +%F); echo "$now"
来源：http://tiv.ehwqpu.com

[R27] 算术展开
来源：http://eho.cucudq.cn

echo $((1 + 2 * 3))
来源：http://tas.xinyue.icu

[R28] 浮点运算
来源：http://mag.nanxinkj.top

echo "scale=2; 10/3" | bc
来源：http://tlj.chenjidiqi.icu

[R29] 定义函数
来源：http://daj.gogol.net.cn


<!-- 参考信息 -->