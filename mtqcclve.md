代发 wailian999

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wal.xinyue.icu

[P06] 综合判空（null / 空串 / 空集合）
来源：http://yoe.ivvv.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://gpr.0kj1m.cn

PHP:  if (empty($x)) {}
来源：http://klq.cheryme.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://uus.shanyushiyangtech.top

TS:   if (x == null) {}
来源：http://krh.hesvh.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://igi.jlsjyb.cn

Go:   if x == nil {}
来源：http://vhg.ppjwa.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://vcu.bjfxy.top

C#:   if (x is null) {}
来源：http://yel.ydzc1.top

[P07] 防抖与节流
来源：http://mhu.fzhhl.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://odm.zhongyouzk.top

PHP:  // 手写时间戳比较
来源：http://elz.shuidangran.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yjj.yuxming.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gyk.52xcode.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://umu.gotoacloud.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://yce.fzhhl.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://udm.dashuyun.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://olr.guannengcc.top

[P08] 处理浮点精度问题
来源：http://bjd.yj202588.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://bsv.shangyingyoupin.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://uvx.epnwcf.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ltz.fktsv.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://fnw.aibaodan.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hxv.tarul.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ncp.shanyushiyangkeji.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://voh.ppjwa.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mtx.jqgfzy.top

================================================================================
来源：http://fgq.yj20258.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://doi.zhiwuduotai.top

================================================================================
来源：http://ibr.sweek.top

[Q01] 创建表
来源：http://okq.ydjk.org.cn

CREATE TABLE users (
来源：http://bnw.yj202588.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://pqb.sufxvd.cn

name VARCHAR(50) NOT NULL,
来源：http://crc.havefunace.top

email VARCHAR(100) UNIQUE,
来源：http://egy.jlsjyb.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://bsv.chenzaomai.com

);
来源：http://liw.shanyushiyangkeji.top

[Q02] 创建带外键的表
来源：http://ney.ehwqpu.com

CREATE TABLE orders (
来源：http://vsz.cucudq.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://dms.iojbl.cn

user_id INT NOT NULL,
来源：http://fpf.gogol.net.cn

amount DECIMAL(10, 2),
来源：http://vil.meibo888.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ajt.sjlbkw.cn

);
来源：http://xsz.0kj1m.cn

[Q03] 增加列
来源：http://crt.yj202588.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://oql.xylfe.cn

[Q04] 修改列类型
来源：http://ura.daria6918.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://evu.zhaomingkeji.xyz

[Q05] 重命名列
来源：http://hlw.daria6918.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ocd.hongshengwenyu.top

[Q06] 删除列
来源：http://wrk.dashuyun.cn

ALTER TABLE users DROP COLUMN age;
来源：http://saf.aizwys.cn

[Q07] 删除表
来源：http://law.yj20258.top

DROP TABLE IF EXISTS orders;
来源：http://mhq.jlsjyb.cn

[Q08] 创建普通索引
来源：http://igi.aibaodan.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://unl.andypj.xyz

[Q09] 创建唯一索引
来源：http://oxn.yanxiufei.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://gdv.hfpthk.cn

[Q10] 插入单行
来源：http://csj.shzxlz.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://vyt.jinghuilouyu.cn

[Q11] 一次插入多行
来源：http://ypg.aibaodan.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://tzc.cheryme.top

[Q12] 插入后取自增 ID
来源：http://pgm.ywan-chungtsiang.top

INSERT INTO users (name) VALUES ('C');
来源：http://iwv.ywan-chungtsiang.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://kfr.316326.xyz

[Q13] 忽略重复插入
来源：http://fyj.vqdsnc.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://eaz.hesvh.cn

[Q14] 存在则更新（upsert）
来源：http://pia.zdbjq.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://psv.daria6918.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://yyl.feifeiyinyue.top

[Q15] 查询全部
来源：http://scu.pengpengdd.cyou

SELECT * FROM users;
来源：http://yrd.tanke756.top

[Q16] 查询指定列
来源：http://thp.yj20258.top

SELECT id, name FROM users;
来源：http://wpf.mhx1999.top

[Q17] 条件查询
来源：http://mvi.zhiwuduotai.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://zay.quarkkingdee.top

[Q18] 模糊匹配
来源：http://mvg.yj202588.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://jhq.jinyuanbaomall.cn

[Q19] 范围查询
来源：http://kmp.jinghuilouyu.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ilo.bbcook.cn

[Q20] IN 列表
来源：http://iof.svipenyu.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://sqs.hfpthk.cn

[Q21] 空值判断
来源：http://krk.daxiang520.top

SELECT * FROM users WHERE email IS NULL;
来源：http://dlr.epnwcf.com

[Q22] 排序
来源：http://dfu.jinqigfzy.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://eqp.mhx1999.top

[Q23] 分页
来源：http://nhm.vqdsnc.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://utv.ctjpmb.com

[Q24] 去重
来源：http://nbq.redwolf501.top

SELECT DISTINCT city FROM users;
来源：http://szz.zycfv.cn

[Q25] 只取前 N 条
来源：http://ndf.fzhhl.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://bda.gogol.net.cn

[Q26] 计数
来源：http://idx.316326.xyz

SELECT COUNT(*) FROM users;
来源：http://ptv.52xcode.cn

[Q27] 条件计数
来源：http://gcz.shanyushiyangkeji.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://qxt.xuetiantiany.cn

[Q28] 求和与平均
来源：http://sxj.guowangkeji.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://pza.shangyingyoupin.top

[Q29] 最大最小值
来源：http://zes.316326.xyz

SELECT MAX(age), MIN(age) FROM users;
来源：http://wfu.uphjek.com

[Q30] 分组统计
来源：http://lat.sweek.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mec.vqdsnc.cn

[Q31] 分组后过滤
来源：http://uoy.smart0.xyz

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://emu.daxiang520.top

[Q32] 分组拼接字符串
来源：http://lzg.sxryk.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://tov.dashuyun.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://spb.pengpengdd.cyou

[Q33] 多列分组
来源：http://fou.meibo888.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wke.epnwcf.com

[Q34] 每组取第一条
来源：http://vvp.aizwys.cn

SELECT * FROM (
来源：http://gbm.jyoumei.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mjs.yuxming.cn

) t WHERE rn = 1;
来源：http://lxr.jinghuilouyu.cn

[Q35] 内连接
来源：http://azn.dianchejie.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://xsu.9152youxi.cn

[Q36] 左连接
来源：http://vaa.sysykeji.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://cwo.wangshuangyany.cn

[Q37] 右连接
来源：http://ltw.fehbvm.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://yzd.jiagoushi.top

[Q38] 全外连接（PostgreSQL）
来源：http://tak.epnwcf.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://bce.jinyuanbaomall.cn

[Q39] 自连接（查上下级）
来源：http://xog.yvedp.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://fmg.gzhubu.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://lmr.yueranfly.top

[Q40] 交叉连接（笛卡尔积）
来源：http://dre.kuanghao11.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://lpp.haohaochexian.top

[Q41] 多表连接
来源：http://cwr.tian-w.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://gbz.redwolf501.top

JOIN users u ON u.id = o.user_id
来源：http://ulw.yanxiufei.cn

JOIN products p ON p.id = o.product_id;
来源：http://qfo.pengpengdd.cyou

[Q42] 连接条件附加过滤
来源：http://jtq.shanyushiyangtech.top

SELECT u.name, o.amount FROM users u
来源：http://mol.cqqwz.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://jhv.jqgufenzy.top

[Q43] 标量子查询
来源：http://gem.andypj.xyz

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://brz.shzxlz.cn

[Q44] IN 子查询
来源：http://xfm.birdmap.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://vfr.fzhhl.top

[Q45] EXISTS 判断存在
来源：http://xal.yuanzhike.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vpr.mhx1999.top

[Q46] NOT EXISTS 判断不存在
来源：http://zko.redwolf501.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wol.yongpay.top

[Q47] 与平均值比较
来源：http://zkm.ybcxt.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://dru.bjfxy.top

[Q48] CTE 公用表表达式
来源：http://qhz.shanyushiyangkeji.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://abx.quarkkingdee.top

SELECT * FROM t WHERE c > 5;
来源：http://ocq.sweek.top

[Q49] 更新单行
来源：http://ugv.ybcxt.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ytu.cashguo.top

[Q50] 批量更新
来源：http://cqz.redwolf501.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wpm.0kj1m.cn

[Q51] 用子查询更新
来源：http://fki.yuanzhike.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://krf.fktsv.cn

[Q52] 删除指定行
来源：http://jwd.nanxuanxn.top

DELETE FROM users WHERE id = 10;
来源：http://umu.hysaishi.cn

[Q53] 按条件删除
来源：http://mag.0kj1m.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mbq.tanke756.top

[Q54] 清空表
来源：http://ddu.hongshengwenyu.top

TRUNCATE TABLE logs;
来源：http://txu.sysykeji.top

[Q55] 排名（并列占位）
来源：http://dms.yonumen.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://aru.pycfn.com

[Q56] 密集排名（并列不占位）
来源：http://zsa.sjlbkw.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ymq.feifeiyinyue.top

[Q57] 行号
来源：http://dkl.dianchejie.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://uzb.sweek.top

[Q58] 累计求和
来源：http://cui.9152youxi.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://vti.sufxvd.cn

[Q59] 分组内累计
来源：http://muq.hfpthk.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://jkw.xylfe.cn

[Q60] 取上一行 / 下一行
来源：http://ohk.aizwys.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://guo.gotoacloud.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wjw.hnqzz.top

[Q61] 移动平均
来源：http://piu.hywenlv.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://eun.jyoumei.cn

[Q62] 分组占比
来源：http://bml.guowangkeji.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wel.zhiwuduotai.top

[Q63] 开启事务
来源：http://psd.gaohongyu789.top

START TRANSACTION;                -- 或 BEGIN
来源：http://hps.zhoulong.xyz

[Q64] 提交事务
来源：http://wxm.jinqigfzy.top

COMMIT;
来源：http://gkk.redwolf501.top

[Q65] 回滚事务
来源：http://ecv.dashuyun.cn

ROLLBACK;
来源：http://qja.iojbl.cn

[Q66] 行锁查询
来源：http://lwd.52xcode.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://rpb.yangfankeji.com

[Q67] 设置隔离级别
来源：http://ppj.tarul.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://zok.shanyushiyangtech.top

[Q68] 保存点
来源：http://keh.hongshengwenyu.top

SAVEPOINT sp1;
来源：http://wln.jinghuilouyu.cn

ROLLBACK TO sp1;
来源：http://jkr.ybcxt.top

[Q69] 查看执行计划
来源：http://obo.hysaishi.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hwr.epnwcf.com

[Q70] 更新统计信息
来源：http://vij.nanxinkj.top

ANALYZE TABLE users;
来源：http://ctk.gotoacloud.top

[Q71] 查看建表语句
来源：http://rdg.aizwys.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wck.tanke756.top

[Q72] 查看索引
来源：http://jtb.hywenlv.cn

SHOW INDEX FROM users;
来源：http://zdn.xuanzx.com

[Q73] 查看表状态
来源：http://maf.jlsjyb.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://hqi.yanxiufei.cn

[Q74] 强制使用索引
来源：http://hsz.xingfuxueyuan.xyz

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://qgc.quarkkingdee.top

[Q75] 日期格式化
来源：http://rpo.0kj1m.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://jgo.jlsjyb.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ftn.daxiang520.top

[Q76] 按天统计
来源：http://gvj.zhengqikj.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://upy.xziqi.cn

[Q77] 时间加减
来源：http://led.havefunace.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ggs.c1oappe.top

[Q78] 当前时间
来源：http://puq.ywan-chungtsiang.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://cpn.tarul.cn

[Q79] 字符串拼接
来源：http://xmw.xuetiantiany.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://dzq.bjfxy.top

[Q80] 字符串截取
来源：http://bug.ctjpmb.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://dbt.sjlbkw.cn

[Q81] 字符串替换
来源：http://gcj.epnwcf.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://xee.gaohongyu789.top

[Q82] 字符长度与字节长度
来源：http://efi.tian-w.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://cbl.sweek.top

[Q83] 大小写转换
来源：http://xzx.xuetiantiany.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ape.quarkkingdee.top

[Q84] 去除首尾空格
来源：http://qub.quarkkingdee.top

SELECT TRIM(name) FROM users;
来源：http://eeb.jianghu66.top

[Q85] 数值取整
来源：http://efr.vqdsnc.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ybr.ywan-chungtsiang.top

[Q86] 读取 JSON 字段
来源：http://hei.sweek.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://kbg.cashguo.top

[Q87] JSON 字段做条件
来源：http://bwz.iojbl.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ihx.kuanghao11.cn

[Q88] 行转列（条件聚合）
来源：http://vvr.redwolf501.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://jno.redwolf501.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://qvk.cdnleiting.top

[Q89] 判断表是否存在
来源：http://yqi.yonumen.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ezf.fktsv.cn

[Q90] 生成序号列
来源：http://znr.gogol.net.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://cyt.zhaomingkeji.xyz

================================================================================
来源：http://nwc.cucudq.cn

R. Bash 专题
来源：http://yny.yueranfly.top

================================================================================
来源：http://vfx.yj202588.top

[R01] shebang 与严格模式
来源：http://evb.zhongyouzk.top

#!/usr/bin/env bash
来源：http://olj.wangdashe.top

set -euo pipefail
来源：http://bar.gaohongyu789.top

[R02] 变量赋值与使用
来源：http://zir.wangshuangyany.cn

name="Tom"; echo "$name"
来源：http://oqj.ybcxt.top

[R03] 只读变量
来源：http://erd.jinyuanbaomall.cn

readonly PI=3.14
来源：http://eay.fehbvm.com

[R04] 位置参数
来源：http://wys.fzhhl.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://jdq.zhiwuduotai.top

[R05] 参数默认值
来源：http://efd.dashuyun.cn

name="${1:-default}"
来源：http://fbz.yongpay.top

[R06] 判断命令是否存在
来源：http://bqb.uphjek.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://opn.hammf.cn

[R07] if 判断文件
来源：http://vix.zdqjudy.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://bis.dashuyun.cn

[R08] 数值比较
来源：http://tnx.daxiang520.top

if (( a > b )); then echo "a 更大"; fi
来源：http://lhd.meibo888.top

[R09] 字符串比较
来源：http://vcg.shuidangran.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://prq.chenlongwang.top

[R10] 正则匹配
来源：http://yqa.wangdashe.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ure.shuidangran.top

[R11] case 多分支
来源：http://aop.sufxvd.cn

case "$1" in
来源：http://hlc.chenlongwang.top

start) echo "启动" ;;
来源：http://aac.tianlin.xyz

stop)  echo "停止" ;;
来源：http://kcu.nanxuanxn.top

*)     echo "未知命令" ;;
来源：http://hfo.dianchejie.cn

esac
来源：http://vzn.52xcode.cn

[R12] for 遍历文件
来源：http://fit.jianghu66.top

for f in *.txt; do echo "$f"; done
来源：http://pco.xinyue.icu

[R13] for 计数循环
来源：http://ewx.jlsjyb.cn

for i in {1..10}; do echo "$i"; done
来源：http://pjz.pengpengdd.cyou

[R14] C 风格 for
来源：http://mcb.nwbrower.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://pdi.jianghu66.top

[R15] while 逐行读文件
来源：http://ond.haohaochexian.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://aro.jyoumei.cn

[R16] until 等待条件
来源：http://anz.andypj.xyz

until [[ -f done.flag ]]; do sleep 1; done
来源：http://bjs.yfazqb.com

[R17] 数组定义与取值
来源：http://bkm.shangyingyoupin.top

arr=(a b c); echo "${arr[0]}"
来源：http://qww.jinyuanbaomall.cn

[R18] 遍历数组
来源：http://jjb.aizwys.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mtm.yfazqb.com

[R19] 数组长度
来源：http://jvk.hammf.cn

echo "${#arr[@]}"
来源：http://jej.guannengcc.top

[R20] 关联数组（字典）
来源：http://trb.hywenlv.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wij.jyoumei.cn

[R21] 字符串长度
来源：http://saj.yanxiufei.cn

echo "${#s}"
来源：http://mdq.vehdjk.com

[R22] 截取子串
来源：http://wzy.meibo888.top

echo "${s:0:5}"
来源：http://hor.wangshuangyany.cn

[R23] 字符串替换
来源：http://hyi.havefunace.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ruy.jianghu66.top

[R24] 大小写转换
来源：http://ysb.uphjek.com

echo "${s^^}"; echo "${s,,}"
来源：http://wgk.zhijiandao.cn

[R25] 去后缀 / 去前缀
来源：http://jpn.meibo888.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://vdm.bjfxy.top

[R26] 命令替换
来源：http://zwu.epnwcf.com

now=$(date +%F); echo "$now"
来源：http://pxj.hcnkem.com

[R27] 算术展开
来源：http://msx.bjfxy.top

echo $((1 + 2 * 3))
来源：http://lin.zhaomingkeji.xyz

[R28] 浮点运算
来源：http://gwg.0kj1m.cn

echo "scale=2; 10/3" | bc
来源：http://taf.hfpthk.cn

[R29] 定义函数
来源：http://oao.52xcode.cn


<!-- 参考信息 -->