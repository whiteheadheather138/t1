代发 wailian999

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://qvw.52xcode.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://soo.aizwys.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://spk.tian-w.cn

PHP:  if (empty($x)) {}
来源：http://wra.xuetiantiany.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://adf.yangfankeji.com

TS:   if (x == null) {}
来源：http://mgf.hcnkem.com

Java: if (x == null || x.isEmpty()) {}
来源：http://ovj.quarkkingdee.top

Go:   if x == nil {}
来源：http://rvn.meibo888.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://fvk.shangyingyoupin.top

C#:   if (x is null) {}
来源：http://ovp.316326.xyz

[P07] 防抖与节流
来源：http://jkp.pengpengdd.cyou

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://kuf.ehwqpu.com

PHP:  // 手写时间戳比较
来源：http://mhu.chenlongwang.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://udz.hesvh.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wnr.yj202588.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://zol.smart0.xyz

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://egp.zhoulong.xyz

Ruby: // 手写闭包 + Time.now 判断
来源：http://wib.gaohongyu789.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://eed.daria6918.cn

[P08] 处理浮点精度问题
来源：http://vvq.gzhubu.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://vfy.snrcjt.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://efl.nanxinkj.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://gso.ywan-chungtsiang.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://yiq.jinyuanbaomall.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://flr.vehdjk.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://nqy.smart0.xyz

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://clq.dashuyun.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://udg.nanxinkj.top

================================================================================
来源：http://gjc.aibaodan.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hmn.gogol.net.cn

================================================================================
来源：http://xuk.zhijiandao.cn

[Q01] 创建表
来源：http://awy.ybcxt.top

CREATE TABLE users (
来源：http://quv.gaohongyu789.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://npq.nanxuanxn.top

name VARCHAR(50) NOT NULL,
来源：http://xow.fzhhl.top

email VARCHAR(100) UNIQUE,
来源：http://kia.yj202588.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ivj.aizwys.cn

);
来源：http://unx.tian-w.cn

[Q02] 创建带外键的表
来源：http://hvj.birdmap.top

CREATE TABLE orders (
来源：http://qgm.jlsjyb.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://yhv.meibo888.top

user_id INT NOT NULL,
来源：http://dwe.hysaishi.cn

amount DECIMAL(10, 2),
来源：http://jis.yonumen.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://dzb.yvedp.cn

);
来源：http://srj.bjfxy.top

[Q03] 增加列
来源：http://xkk.hnqzz.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://xun.meibo888.top

[Q04] 修改列类型
来源：http://hbj.zhoulong.xyz

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://dvs.xuanzx.com

[Q05] 重命名列
来源：http://myo.fzhhl.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://sva.jqgufenzy.top

[Q06] 删除列
来源：http://qbb.tanke756.top

ALTER TABLE users DROP COLUMN age;
来源：http://ebn.nanxuanxn.top

[Q07] 删除表
来源：http://tth.jyoumei.cn

DROP TABLE IF EXISTS orders;
来源：http://mov.yvedp.cn

[Q08] 创建普通索引
来源：http://npn.jiagoushi.top

CREATE INDEX idx_users_email ON users(email);
来源：http://uqc.yj202588.top

[Q09] 创建唯一索引
来源：http://gpy.iojbl.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ela.yangfankeji.com

[Q10] 插入单行
来源：http://lxy.fktsv.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://gxt.jianghu66.top

[Q11] 一次插入多行
来源：http://ndq.zhiwuduotai.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://nlf.fktsv.cn

[Q12] 插入后取自增 ID
来源：http://zts.xinyue.icu

INSERT INTO users (name) VALUES ('C');
来源：http://pmq.cucudq.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mrk.tianlin.xyz

[Q13] 忽略重复插入
来源：http://thr.ybcxt.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://dmr.zhaomingkeji.xyz

[Q14] 存在则更新（upsert）
来源：http://caj.shanyushiyangkeji.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://xtt.jqgufenzy.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://udu.yj20258888.top

[Q15] 查询全部
来源：http://xxz.pycfn.com

SELECT * FROM users;
来源：http://kmk.haohaochexian.top

[Q16] 查询指定列
来源：http://jph.shuidangran.top

SELECT id, name FROM users;
来源：http://kxy.hongshengwenyu.top

[Q17] 条件查询
来源：http://eel.hammf.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://gqb.iojbl.cn

[Q18] 模糊匹配
来源：http://rkg.jlsjyb.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://axq.pengpengdd.cyou

[Q19] 范围查询
来源：http://xex.zdqjudy.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://rnf.ehwqpu.com

[Q20] IN 列表
来源：http://aew.yj20258888.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://izm.yuxming.cn

[Q21] 空值判断
来源：http://fxh.kuanghao11.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://cqz.hammf.cn

[Q22] 排序
来源：http://zni.xylfe.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://euc.52xcode.cn

[Q23] 分页
来源：http://gvc.snrcjt.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ior.52xcode.cn

[Q24] 去重
来源：http://ghs.yuanzhike.top

SELECT DISTINCT city FROM users;
来源：http://zco.zhaomingkeji.xyz

[Q25] 只取前 N 条
来源：http://ggm.gzhubu.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://qnr.jinghuilouyu.cn

[Q26] 计数
来源：http://kdi.hammf.cn

SELECT COUNT(*) FROM users;
来源：http://jbc.shanyushiyangkeji.top

[Q27] 条件计数
来源：http://nww.tian-w.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://kzj.zdbjq.cn

[Q28] 求和与平均
来源：http://ffe.meibo888.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://zcq.hammf.cn

[Q29] 最大最小值
来源：http://lww.chenjidiqi.icu

SELECT MAX(age), MIN(age) FROM users;
来源：http://ctj.havefunace.top

[Q30] 分组统计
来源：http://uav.shanyushiyangkeji.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://kyl.tarul.cn

[Q31] 分组后过滤
来源：http://hqo.fengsongda.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://kyn.hywenlv.cn

[Q32] 分组拼接字符串
来源：http://pco.andypj.xyz

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://obv.zhiwuduotai.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://qlb.hywenlv.cn

[Q33] 多列分组
来源：http://vwp.ybcxt.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ada.shanyushiyangkeji.top

[Q34] 每组取第一条
来源：http://dcr.quarkkingdee.top

SELECT * FROM (
来源：http://bwp.fzhhl.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://tsg.aizwys.cn

) t WHERE rn = 1;
来源：http://qic.hnxiangtu.top

[Q35] 内连接
来源：http://kxn.fanxiaobao.xyz

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://gqs.zhengqikj.top

[Q36] 左连接
来源：http://hgr.zhaomingkeji.xyz

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://gbc.cdnleiting.top

[Q37] 右连接
来源：http://dwg.shangyingyoupin.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://awz.fanxiaobao.xyz

[Q38] 全外连接（PostgreSQL）
来源：http://dxn.cashguo.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://sog.wangdashe.top

[Q39] 自连接（查上下级）
来源：http://wop.yangfankeji.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://fyk.ydzc1.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://uca.cdnleiting.top

[Q40] 交叉连接（笛卡尔积）
来源：http://xpv.jianghu66.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ejp.bbcook.cn

[Q41] 多表连接
来源：http://atb.pycfn.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://iym.quarkkingdee.top

JOIN users u ON u.id = o.user_id
来源：http://jcq.gaohongyu789.top

JOIN products p ON p.id = o.product_id;
来源：http://lor.smart0.xyz

[Q42] 连接条件附加过滤
来源：http://fnw.xingfuxueyuan.xyz

SELECT u.name, o.amount FROM users u
来源：http://jaa.svipenyu.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://doz.nwbrower.top

[Q43] 标量子查询
来源：http://res.zhongyouzk.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://rya.yuanzhike.top

[Q44] IN 子查询
来源：http://jfv.gogol.net.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://kno.havefunace.top

[Q45] EXISTS 判断存在
来源：http://mwy.tarul.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bte.xingfuxueyuan.xyz

[Q46] NOT EXISTS 判断不存在
来源：http://jzd.epnwcf.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://juq.aizwys.cn

[Q47] 与平均值比较
来源：http://ffy.tian-w.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://yai.yongpay.top

[Q48] CTE 公用表表达式
来源：http://mob.yfazqb.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://fra.vehdjk.com

SELECT * FROM t WHERE c > 5;
来源：http://oxm.fengsongda.top

[Q49] 更新单行
来源：http://hve.sysykeji.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://umr.shzxlz.cn

[Q50] 批量更新
来源：http://pnl.tarul.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://asa.zhiwuduotai.top

[Q51] 用子查询更新
来源：http://tcd.jinyuanbaomall.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://daf.jlsjyb.cn

[Q52] 删除指定行
来源：http://awm.shzxlz.cn

DELETE FROM users WHERE id = 10;
来源：http://aoh.tianlin.xyz

[Q53] 按条件删除
来源：http://xfo.kuanghao11.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ulo.chenzaomai.com

[Q54] 清空表
来源：http://pdb.wangdashe.top

TRUNCATE TABLE logs;
来源：http://tph.tianlin.xyz

[Q55] 排名（并列占位）
来源：http://ekd.bbcook.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://tki.jinyuanbaomall.cn

[Q56] 密集排名（并列不占位）
来源：http://wsu.chenzaomai.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ybf.fanxiaobao.xyz

[Q57] 行号
来源：http://axt.ydjk.org.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://gvm.yfazqb.com

[Q58] 累计求和
来源：http://chw.yanxiufei.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://lty.nanxinkj.top

[Q59] 分组内累计
来源：http://knj.mhx1999.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://vqr.epnwcf.com

[Q60] 取上一行 / 下一行
来源：http://kym.bjfxy.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ucc.zhongyouzk.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ecr.ydjk.org.cn

[Q61] 移动平均
来源：http://qag.yangfankeji.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://fzr.chenlongwang.top

[Q62] 分组占比
来源：http://rte.hnxiangtu.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://lsh.yj20258888.top

[Q63] 开启事务
来源：http://bkt.cheryme.top

START TRANSACTION;                -- 或 BEGIN
来源：http://hfc.dianchejie.cn

[Q64] 提交事务
来源：http://qqg.vqdsnc.cn

COMMIT;
来源：http://xfz.ywan-chungtsiang.top

[Q65] 回滚事务
来源：http://lxb.gaohongyu789.top

ROLLBACK;
来源：http://kbt.redwolf501.top

[Q66] 行锁查询
来源：http://tmb.wangdashe.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://owt.andypj.xyz

[Q67] 设置隔离级别
来源：http://kbt.quarkkingdee.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://lzz.zycfv.cn

[Q68] 保存点
来源：http://mlg.haohaochexian.top

SAVEPOINT sp1;
来源：http://tti.wangdashe.top

ROLLBACK TO sp1;
来源：http://fnv.zhiwuduotai.top

[Q69] 查看执行计划
来源：http://zrj.daria6918.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://yve.yuxming.cn

[Q70] 更新统计信息
来源：http://kmk.hcnkem.com

ANALYZE TABLE users;
来源：http://mew.jinyuanbaomall.cn

[Q71] 查看建表语句
来源：http://vrv.xziqi.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://fks.tian-w.cn

[Q72] 查看索引
来源：http://xik.9152youxi.cn

SHOW INDEX FROM users;
来源：http://ued.cdnleiting.top

[Q73] 查看表状态
来源：http://wtg.jianghu66.top

SHOW TABLE STATUS LIKE 'users';
来源：http://nir.hnxiangtu.top

[Q74] 强制使用索引
来源：http://bxt.birdmap.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://stm.yonumen.top

[Q75] 日期格式化
来源：http://cvm.jqgfzy.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://aww.chenzaomai.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://aof.hnxiangtu.top

[Q76] 按天统计
来源：http://irs.jqgufenzy.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://jpf.andypj.xyz

[Q77] 时间加减
来源：http://idy.smart0.xyz

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blt.shanyushiyangtech.top

[Q78] 当前时间
来源：http://nba.hysaishi.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://evp.hongshengwenyu.top

[Q79] 字符串拼接
来源：http://erm.birdmap.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://rbd.yonumen.top

[Q80] 字符串截取
来源：http://hxx.yangfankeji.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://dyi.hcnkem.com

[Q81] 字符串替换
来源：http://xwa.bbcook.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://iyl.birdmap.top

[Q82] 字符长度与字节长度
来源：http://rga.0kj1m.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://muy.jiagoushi.top

[Q83] 大小写转换
来源：http://onm.svipenyu.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ojl.ydjk.org.cn

[Q84] 去除首尾空格
来源：http://szj.ybcxt.top

SELECT TRIM(name) FROM users;
来源：http://ktz.jyoumei.cn

[Q85] 数值取整
来源：http://cxq.yvedp.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://cpr.jinyuanbaomall.cn

[Q86] 读取 JSON 字段
来源：http://yxr.dianchejie.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hje.jianghu66.top

[Q87] JSON 字段做条件
来源：http://ujx.ybcxt.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://agj.ehwqpu.com

[Q88] 行转列（条件聚合）
来源：http://fje.52xcode.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://syc.zycfv.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://jhl.cashguo.top

[Q89] 判断表是否存在
来源：http://wik.yanxiufei.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://lxd.fehbvm.com

[Q90] 生成序号列
来源：http://nes.tian-w.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://etf.kuanghao11.cn

================================================================================
来源：http://dgt.9152youxi.cn

R. Bash 专题
来源：http://jvc.cucudq.cn

================================================================================
来源：http://mur.ywan-chungtsiang.top

[R01] shebang 与严格模式
来源：http://nwy.yj20258888.top

#!/usr/bin/env bash
来源：http://btr.yueranfly.top

set -euo pipefail
来源：http://mkt.jyoumei.cn

[R02] 变量赋值与使用
来源：http://uhg.zdbjq.cn

name="Tom"; echo "$name"
来源：http://jdn.vehdjk.com

[R03] 只读变量
来源：http://hne.yfazqb.com

readonly PI=3.14
来源：http://wdu.xingfuxueyuan.xyz

[R04] 位置参数
来源：http://nnk.yj20258888.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://qdn.hfpthk.cn

[R05] 参数默认值
来源：http://pyy.0kj1m.cn

name="${1:-default}"
来源：http://dfv.xylfe.cn

[R06] 判断命令是否存在
来源：http://rrm.jinyuanbaomall.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://iwk.shangyingyoupin.top

[R07] if 判断文件
来源：http://rmn.xuanzx.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ogd.hongshengwenyu.top

[R08] 数值比较
来源：http://bds.chenzaomai.com

if (( a > b )); then echo "a 更大"; fi
来源：http://qdh.uphjek.com

[R09] 字符串比较
来源：http://ida.chenlongwang.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hkb.feifeiyinyue.top

[R10] 正则匹配
来源：http://vfr.bbcook.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://smn.sweek.top

[R11] case 多分支
来源：http://xjy.yuanzhike.top

case "$1" in
来源：http://qix.iojbl.cn

start) echo "启动" ;;
来源：http://bql.ivvv.top

stop)  echo "停止" ;;
来源：http://xbf.52xcode.cn

*)     echo "未知命令" ;;
来源：http://yav.xinyue.icu

esac
来源：http://scs.ydjk.org.cn

[R12] for 遍历文件
来源：http://fhg.zhixingplan.top

for f in *.txt; do echo "$f"; done
来源：http://tut.yuanzhike.top

[R13] for 计数循环
来源：http://loc.shzxlz.cn

for i in {1..10}; do echo "$i"; done
来源：http://zxp.hesvh.cn

[R14] C 风格 for
来源：http://eyi.yanxiufei.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ndx.andypj.xyz

[R15] while 逐行读文件
来源：http://kxo.gaohongyu789.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://fbd.fzhhl.top

[R16] until 等待条件
来源：http://zzy.zdbjq.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://jfa.ydjk.org.cn

[R17] 数组定义与取值
来源：http://jra.yuanzhike.top

arr=(a b c); echo "${arr[0]}"
来源：http://nzj.hnxiangtu.top

[R18] 遍历数组
来源：http://uge.meibo888.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hhf.fengsongda.top

[R19] 数组长度
来源：http://flr.yj20258888.top

echo "${#arr[@]}"
来源：http://xkc.ivvv.top

[R20] 关联数组（字典）
来源：http://elp.ppjwa.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://flw.jqgufenzy.top

[R21] 字符串长度
来源：http://atk.hesvh.cn

echo "${#s}"
来源：http://zyd.quarkkingdee.top

[R22] 截取子串
来源：http://wmw.c1oappe.top

echo "${s:0:5}"
来源：http://ska.jianghu66.top

[R23] 字符串替换
来源：http://lvs.xingfuxueyuan.xyz

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://aph.shzxlz.cn

[R24] 大小写转换
来源：http://hak.zdbjq.cn

echo "${s^^}"; echo "${s,,}"
来源：http://gdh.vehdjk.com

[R25] 去后缀 / 去前缀
来源：http://olq.fanxiaobao.xyz

echo "${f%.txt}"; echo "${f#./}"
来源：http://mux.jinqigfzy.top

[R26] 命令替换
来源：http://app.kuanghao11.cn

now=$(date +%F); echo "$now"
来源：http://dqq.sysykeji.top

[R27] 算术展开
来源：http://jud.yuxming.cn

echo $((1 + 2 * 3))
来源：http://zcl.zdbjq.cn

[R28] 浮点运算
来源：http://qkr.ywan-chungtsiang.top

echo "scale=2; 10/3" | bc
来源：http://upa.ppjwa.cn

[R29] 定义函数
来源：http://ylk.zhongyouzk.top


<!-- 参考信息 -->