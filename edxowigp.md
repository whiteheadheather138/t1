代发 wailian999

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://rbd.aizwys.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://zqz.smart0.xyz

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://qdf.gogol.net.cn

PHP:  if (empty($x)) {}
来源：http://ffk.andypj.xyz

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://czt.feifeiyinyue.top

TS:   if (x == null) {}
来源：http://ffo.hnqzz.top

Java: if (x == null || x.isEmpty()) {}
来源：http://fco.yj20258888.top

Go:   if x == nil {}
来源：http://fxf.cdnleiting.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://bpq.shzxlz.cn

C#:   if (x is null) {}
来源：http://phu.ywan-chungtsiang.top

[P07] 防抖与节流
来源：http://lxq.wangshuangyany.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://jfv.shzxlz.cn

PHP:  // 手写时间戳比较
来源：http://get.nwbrower.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://siy.gotoacloud.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rqj.xziqi.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://vkq.haohaochexian.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://fnr.cashguo.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://ale.kuanghao11.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://lgj.jinghuilouyu.cn

[P08] 处理浮点精度问题
来源：http://vfu.sysykeji.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://odo.jiagoushi.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hrd.hongshengwenyu.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://zvw.yj202588.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://juv.9152youxi.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://avx.hcnkem.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://rjy.aizwys.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://tep.cdnleiting.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://rar.shangyingyoupin.top

================================================================================
来源：http://ukm.sweek.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://dny.hnqzz.top

================================================================================
来源：http://zie.jlsjyb.cn

[Q01] 创建表
来源：http://bwf.ybcxt.top

CREATE TABLE users (
来源：http://bxh.xziqi.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hgv.yuanzhike.top

name VARCHAR(50) NOT NULL,
来源：http://khj.yj20258888.top

email VARCHAR(100) UNIQUE,
来源：http://uox.snrcjt.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://geq.shzxlz.cn

);
来源：http://rws.redwolf501.top

[Q02] 创建带外键的表
来源：http://pac.gaohongyu789.top

CREATE TABLE orders (
来源：http://zrv.zhijiandao.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://xks.zycfv.cn

user_id INT NOT NULL,
来源：http://dbv.hesvh.cn

amount DECIMAL(10, 2),
来源：http://hyq.hnqzz.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://pez.jqgfzy.top

);
来源：http://grx.jlsjyb.cn

[Q03] 增加列
来源：http://xmp.bjfxy.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://izk.jinqigufen.top

[Q04] 修改列类型
来源：http://vyd.shangyingyoupin.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://zdq.316326.xyz

[Q05] 重命名列
来源：http://wma.fktsv.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://cpe.haohaochexian.top

[Q06] 删除列
来源：http://nch.shzxlz.cn

ALTER TABLE users DROP COLUMN age;
来源：http://vuq.bjfxy.top

[Q07] 删除表
来源：http://zhc.svipenyu.cn

DROP TABLE IF EXISTS orders;
来源：http://ipu.cashguo.top

[Q08] 创建普通索引
来源：http://sap.jinghuilouyu.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://byq.shanyushiyangtech.top

[Q09] 创建唯一索引
来源：http://bzs.vqdsnc.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mod.tarul.cn

[Q10] 插入单行
来源：http://ndp.ehwqpu.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://kno.fanxiaobao.xyz

[Q11] 一次插入多行
来源：http://rqz.ivvv.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://xwd.guannengcc.top

[Q12] 插入后取自增 ID
来源：http://bei.nanxuanxn.top

INSERT INTO users (name) VALUES ('C');
来源：http://fbo.kuanghao11.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://zwy.yj202588.top

[Q13] 忽略重复插入
来源：http://vir.svipenyu.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://idr.yfazqb.com

[Q14] 存在则更新（upsert）
来源：http://mmp.9152youxi.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://nii.nanxuanxn.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://vyz.zhengqikj.top

[Q15] 查询全部
来源：http://bhu.snrcjt.cn

SELECT * FROM users;
来源：http://toa.fktsv.cn

[Q16] 查询指定列
来源：http://axl.snrcjt.cn

SELECT id, name FROM users;
来源：http://cfa.guannengcc.top

[Q17] 条件查询
来源：http://lku.zhengqikj.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://qgv.guowangkeji.top

[Q18] 模糊匹配
来源：http://bhc.feifeiyinyue.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://kph.fanxiaobao.xyz

[Q19] 范围查询
来源：http://xjk.vehdjk.com

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://fpw.dashuyun.cn

[Q20] IN 列表
来源：http://bty.9152youxi.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://avc.shuidangran.top

[Q21] 空值判断
来源：http://phw.svipenyu.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://umy.fktsv.cn

[Q22] 排序
来源：http://lyd.uphjek.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://dyg.havefunace.top

[Q23] 分页
来源：http://zxu.vehdjk.com

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://fhl.tarul.cn

[Q24] 去重
来源：http://act.guowangkeji.top

SELECT DISTINCT city FROM users;
来源：http://kci.yj20258.top

[Q25] 只取前 N 条
来源：http://bwx.52xcode.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ith.shangyingyoupin.top

[Q26] 计数
来源：http://ikr.fzhhl.top

SELECT COUNT(*) FROM users;
来源：http://npr.zhengqikj.top

[Q27] 条件计数
来源：http://dyh.jlsjyb.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ltk.zhixingplan.top

[Q28] 求和与平均
来源：http://cgy.mhx1999.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ype.gaohongyu789.top

[Q29] 最大最小值
来源：http://nnq.nanxinkj.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://pmg.pycfn.com

[Q30] 分组统计
来源：http://svs.316326.xyz

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://rxq.zhengqikj.top

[Q31] 分组后过滤
来源：http://kot.xingfuxueyuan.xyz

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://dpo.pengpengdd.cyou

[Q32] 分组拼接字符串
来源：http://sbv.zhijiandao.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://akg.svipenyu.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://lun.aizwys.cn

[Q33] 多列分组
来源：http://iaz.ivvv.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://pjr.hcnkem.com

[Q34] 每组取第一条
来源：http://yqn.yonumen.top

SELECT * FROM (
来源：http://fhz.jinghuilouyu.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://agg.wangshuangyany.cn

) t WHERE rn = 1;
来源：http://dxw.52xcode.cn

[Q35] 内连接
来源：http://ckr.sufxvd.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ljf.316326.xyz

[Q36] 左连接
来源：http://bui.vqdsnc.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://cys.52xcode.cn

[Q37] 右连接
来源：http://tjy.yongpay.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://vbh.fzhhl.top

[Q38] 全外连接（PostgreSQL）
来源：http://nec.fengsongda.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ekh.ydjk.org.cn

[Q39] 自连接（查上下级）
来源：http://fvq.bjfxy.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://bbc.hfpthk.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://yxt.fanxiaobao.xyz

[Q40] 交叉连接（笛卡尔积）
来源：http://yss.shangyingyoupin.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://pqd.gaohongyu789.top

[Q41] 多表连接
来源：http://sui.xuetiantiany.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://lga.haohaochexian.top

JOIN users u ON u.id = o.user_id
来源：http://pxi.kuanghao11.cn

JOIN products p ON p.id = o.product_id;
来源：http://vna.snrcjt.cn

[Q42] 连接条件附加过滤
来源：http://ogh.shuidangran.top

SELECT u.name, o.amount FROM users u
来源：http://ltq.pengpengdd.cyou

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hve.guowangkeji.top

[Q43] 标量子查询
来源：http://pkb.zdqjudy.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://bim.uphjek.com

[Q44] IN 子查询
来源：http://ixe.shanyushiyangkeji.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://gsf.birdmap.top

[Q45] EXISTS 判断存在
来源：http://ujp.fehbvm.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://yzs.guowangkeji.top

[Q46] NOT EXISTS 判断不存在
来源：http://rpo.chenjidiqi.icu

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hmh.smart0.xyz

[Q47] 与平均值比较
来源：http://fdp.ybcxt.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://vul.ivvv.top

[Q48] CTE 公用表表达式
来源：http://qms.ydjk.org.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ysz.fzhhl.top

SELECT * FROM t WHERE c > 5;
来源：http://zsb.gogol.net.cn

[Q49] 更新单行
来源：http://bjl.zdqjudy.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://nno.bbcook.cn

[Q50] 批量更新
来源：http://jub.fktsv.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://qpg.fengsongda.top

[Q51] 用子查询更新
来源：http://dsa.haohaochexian.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://cgk.shuidangran.top

[Q52] 删除指定行
来源：http://xfy.sysykeji.top

DELETE FROM users WHERE id = 10;
来源：http://zdm.zhongyouzk.top

[Q53] 按条件删除
来源：http://icl.iojbl.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ncg.tarul.cn

[Q54] 清空表
来源：http://qkk.chenjidiqi.icu

TRUNCATE TABLE logs;
来源：http://znh.vqdsnc.cn

[Q55] 排名（并列占位）
来源：http://fue.hnqzz.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://qgv.uphjek.com

[Q56] 密集排名（并列不占位）
来源：http://jyn.jianghu66.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://jgr.pycfn.com

[Q57] 行号
来源：http://pww.feifeiyinyue.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://shb.jiagoushi.top

[Q58] 累计求和
来源：http://acg.sysykeji.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://tlj.gotoacloud.top

[Q59] 分组内累计
来源：http://whl.xinyue.icu

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mbl.ywan-chungtsiang.top

[Q60] 取上一行 / 下一行
来源：http://pkv.yuxming.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ibl.shanyushiyangtech.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://sou.dianchejie.cn

[Q61] 移动平均
来源：http://oej.pycfn.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wdn.jiagoushi.top

[Q62] 分组占比
来源：http://bqh.ydjk.org.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://krw.fzhhl.top

[Q63] 开启事务
来源：http://kpt.pycfn.com

START TRANSACTION;                -- 或 BEGIN
来源：http://xor.kuanghao11.cn

[Q64] 提交事务
来源：http://bpz.shuidangran.top

COMMIT;
来源：http://paf.fehbvm.com

[Q65] 回滚事务
来源：http://uzb.hfpthk.cn

ROLLBACK;
来源：http://ncs.svipenyu.cn

[Q66] 行锁查询
来源：http://esj.ydzc1.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://cwt.fehbvm.com

[Q67] 设置隔离级别
来源：http://niy.cqqwz.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://kdu.gogol.net.cn

[Q68] 保存点
来源：http://stu.ppjwa.cn

SAVEPOINT sp1;
来源：http://oms.cqqwz.cn

ROLLBACK TO sp1;
来源：http://fbe.yfazqb.com

[Q69] 查看执行计划
来源：http://bby.fengsongda.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://teh.zdqjudy.top

[Q70] 更新统计信息
来源：http://dwd.chenjidiqi.icu

ANALYZE TABLE users;
来源：http://ist.zdbjq.cn

[Q71] 查看建表语句
来源：http://lte.xingfuxueyuan.xyz

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://xir.shanyushiyangkeji.top

[Q72] 查看索引
来源：http://fcf.0kj1m.cn

SHOW INDEX FROM users;
来源：http://dui.xuanzx.com

[Q73] 查看表状态
来源：http://gyf.yonumen.top

SHOW TABLE STATUS LIKE 'users';
来源：http://mjh.fktsv.cn

[Q74] 强制使用索引
来源：http://wbu.xylfe.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ldy.yfazqb.com

[Q75] 日期格式化
来源：http://obj.yfazqb.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://rhy.gaohongyu789.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://xfh.ydzc1.top

[Q76] 按天统计
来源：http://bpk.nwbrower.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://gmz.wangdashe.top

[Q77] 时间加减
来源：http://arb.sysykeji.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://qvv.yvedp.cn

[Q78] 当前时间
来源：http://yhl.guowangkeji.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wts.jinqigufen.top

[Q79] 字符串拼接
来源：http://yhq.yanxiufei.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://uoo.wangshuangyany.cn

[Q80] 字符串截取
来源：http://fzm.cqqwz.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://nuw.hammf.cn

[Q81] 字符串替换
来源：http://tvt.hnqzz.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ymn.zhengqikj.top

[Q82] 字符长度与字节长度
来源：http://hhj.pycfn.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://lmk.guannengcc.top

[Q83] 大小写转换
来源：http://znx.c1oappe.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://vqm.gaohongyu789.top

[Q84] 去除首尾空格
来源：http://kvo.ctjpmb.com

SELECT TRIM(name) FROM users;
来源：http://rdf.hywenlv.cn

[Q85] 数值取整
来源：http://wfk.52xcode.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://vih.ivvv.top

[Q86] 读取 JSON 字段
来源：http://mos.cheryme.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://unf.tian-w.cn

[Q87] JSON 字段做条件
来源：http://iaa.9152youxi.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://luw.andypj.xyz

[Q88] 行转列（条件聚合）
来源：http://gtk.feifeiyinyue.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wen.zhaomingkeji.xyz

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://eob.nanxinkj.top

[Q89] 判断表是否存在
来源：http://njx.shangyingyoupin.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://nrs.tanke756.top

[Q90] 生成序号列
来源：http://nkv.dashuyun.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://vug.shuidangran.top

================================================================================
来源：http://zxu.shuidangran.top

R. Bash 专题
来源：http://bhh.aizwys.cn

================================================================================
来源：http://cxb.zhengqikj.top

[R01] shebang 与严格模式
来源：http://nld.jinqigufen.top

#!/usr/bin/env bash
来源：http://nyz.zhiwuduotai.top

set -euo pipefail
来源：http://vjq.hcnkem.com

[R02] 变量赋值与使用
来源：http://hgf.redwolf501.top

name="Tom"; echo "$name"
来源：http://lvv.ivvv.top

[R03] 只读变量
来源：http://agr.ybcxt.top

readonly PI=3.14
来源：http://tzj.sjlbkw.cn

[R04] 位置参数
来源：http://uuz.ehwqpu.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://awm.wangdashe.top

[R05] 参数默认值
来源：http://xef.0kj1m.cn

name="${1:-default}"
来源：http://mjh.tanke756.top

[R06] 判断命令是否存在
来源：http://fer.feifeiyinyue.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://kkc.aibaodan.cn

[R07] if 判断文件
来源：http://nuz.mhx1999.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ybd.tarul.cn

[R08] 数值比较
来源：http://pkw.haohaochexian.top

if (( a > b )); then echo "a 更大"; fi
来源：http://pgy.nwbrower.top

[R09] 字符串比较
来源：http://smu.sjlbkw.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://noh.yongpay.top

[R10] 正则匹配
来源：http://btq.dashuyun.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://eef.cashguo.top

[R11] case 多分支
来源：http://blf.yfazqb.com

case "$1" in
来源：http://qon.meibo888.top

start) echo "启动" ;;
来源：http://ckb.zhijiandao.cn

stop)  echo "停止" ;;
来源：http://qln.cdnleiting.top

*)     echo "未知命令" ;;
来源：http://pxg.cqqwz.cn

esac
来源：http://ztc.xziqi.cn

[R12] for 遍历文件
来源：http://byu.redwolf501.top

for f in *.txt; do echo "$f"; done
来源：http://dml.xingfuxueyuan.xyz

[R13] for 计数循环
来源：http://lgl.gotoacloud.top

for i in {1..10}; do echo "$i"; done
来源：http://jra.birdmap.top

[R14] C 风格 for
来源：http://aol.yueranfly.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mtm.yj202588.top

[R15] while 逐行读文件
来源：http://gbq.sjlbkw.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://epd.sysykeji.top

[R16] until 等待条件
来源：http://fwh.yonumen.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://jxt.hfpthk.cn

[R17] 数组定义与取值
来源：http://vci.uphjek.com

arr=(a b c); echo "${arr[0]}"
来源：http://rev.jlsjyb.cn

[R18] 遍历数组
来源：http://mvr.tanke756.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://nsq.yj20258.top

[R19] 数组长度
来源：http://lqd.cheryme.top

echo "${#arr[@]}"
来源：http://qqd.chenzaomai.com

[R20] 关联数组（字典）
来源：http://fpg.yfazqb.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://iwr.uphjek.com

[R21] 字符串长度
来源：http://tgz.xziqi.cn

echo "${#s}"
来源：http://unp.ydjk.org.cn

[R22] 截取子串
来源：http://ggo.wangdashe.top

echo "${s:0:5}"
来源：http://yzb.meibo888.top

[R23] 字符串替换
来源：http://nhi.cqqwz.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://vbf.jinyuanbaomall.cn

[R24] 大小写转换
来源：http://qnq.jinghuilouyu.cn

echo "${s^^}"; echo "${s,,}"
来源：http://nyg.cdnleiting.top

[R25] 去后缀 / 去前缀
来源：http://upl.yangfankeji.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://mqa.tian-w.cn

[R26] 命令替换
来源：http://xak.sufxvd.cn

now=$(date +%F); echo "$now"
来源：http://wei.chenjidiqi.icu

[R27] 算术展开
来源：http://cgx.nwbrower.top

echo $((1 + 2 * 3))
来源：http://hpa.xuetiantiany.cn

[R28] 浮点运算
来源：http://fxj.iojbl.cn

echo "scale=2; 10/3" | bc
来源：http://dfc.daria6918.cn

[R29] 定义函数
来源：http://llk.shangyingyoupin.top


<!-- 参考信息 -->