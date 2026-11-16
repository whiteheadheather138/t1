代发 wailian999

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://cdd.jinyuanbaomall.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ujo.cdnleiting.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ktd.zdbjq.cn

PHP:  if (empty($x)) {}
来源：http://mna.yangfankeji.com

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://zuq.hnxiangtu.top

TS:   if (x == null) {}
来源：http://mtx.vehdjk.com

Java: if (x == null || x.isEmpty()) {}
来源：http://dyi.yfazqb.com

Go:   if x == nil {}
来源：http://ftw.jianghu66.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://dlq.yuxming.cn

C#:   if (x is null) {}
来源：http://gco.ctjpmb.com

[P07] 防抖与节流
来源：http://dnv.gogol.net.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://pzk.zycfv.cn

PHP:  // 手写时间戳比较
来源：http://uhu.shuidangran.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tzr.xylfe.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mre.zhijiandao.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://kma.fktsv.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ggq.zhijiandao.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://zga.zhixingplan.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://kge.sweek.top

[P08] 处理浮点精度问题
来源：http://ekp.gaohongyu789.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mlu.yj20258.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://dwu.jqgfzy.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://gex.hesvh.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://uux.daria6918.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://sls.zdbjq.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://asy.andypj.xyz

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://kcm.aibaodan.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://xyd.quarkkingdee.top

================================================================================
来源：http://iuh.aizwys.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://iyo.pycfn.com

================================================================================
来源：http://jfk.tianlin.xyz

[Q01] 创建表
来源：http://wez.hesvh.cn

CREATE TABLE users (
来源：http://tul.hnxiangtu.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://eda.cucudq.cn

name VARCHAR(50) NOT NULL,
来源：http://tcq.yonumen.top

email VARCHAR(100) UNIQUE,
来源：http://ztq.hnxiangtu.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://fnl.meibo888.top

);
来源：http://jil.zhiwuduotai.top

[Q02] 创建带外键的表
来源：http://una.fehbvm.com

CREATE TABLE orders (
来源：http://uhh.fanxiaobao.xyz

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://cce.jinqigufen.top

user_id INT NOT NULL,
来源：http://ykv.shanyushiyangtech.top

amount DECIMAL(10, 2),
来源：http://prg.zhixingplan.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://thb.daxiang520.top

);
来源：http://lda.guowangkeji.top

[Q03] 增加列
来源：http://apm.uphjek.com

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ttv.fehbvm.com

[Q04] 修改列类型
来源：http://uai.xylfe.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://iug.xinyue.icu

[Q05] 重命名列
来源：http://wky.zhiwuduotai.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://iba.andypj.xyz

[Q06] 删除列
来源：http://cdf.ivvv.top

ALTER TABLE users DROP COLUMN age;
来源：http://xgi.jinqigufen.top

[Q07] 删除表
来源：http://kns.shzxlz.cn

DROP TABLE IF EXISTS orders;
来源：http://hyi.zhiwuduotai.top

[Q08] 创建普通索引
来源：http://amr.nanxuanxn.top

CREATE INDEX idx_users_email ON users(email);
来源：http://bfa.zhoulong.xyz

[Q09] 创建唯一索引
来源：http://rcm.snrcjt.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://neo.meibo888.top

[Q10] 插入单行
来源：http://mxa.vqdsnc.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://twl.mhx1999.top

[Q11] 一次插入多行
来源：http://bql.gotoacloud.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://jlb.fehbvm.com

[Q12] 插入后取自增 ID
来源：http://rju.jinqigfzy.top

INSERT INTO users (name) VALUES ('C');
来源：http://orl.xuetiantiany.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ejd.nanxinkj.top

[Q13] 忽略重复插入
来源：http://yfu.ywan-chungtsiang.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ppp.jqgfzy.top

[Q14] 存在则更新（upsert）
来源：http://gck.fktsv.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://weu.iojbl.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://qin.fengsongda.top

[Q15] 查询全部
来源：http://krt.sysykeji.top

SELECT * FROM users;
来源：http://clj.ctjpmb.com

[Q16] 查询指定列
来源：http://rvu.xinyue.icu

SELECT id, name FROM users;
来源：http://jbm.meibo888.top

[Q17] 条件查询
来源：http://kfk.yongpay.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://rqm.chenlongwang.top

[Q18] 模糊匹配
来源：http://iqk.52xcode.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://xwg.cqqwz.cn

[Q19] 范围查询
来源：http://twa.jinghuilouyu.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://zdj.nanxuanxn.top

[Q20] IN 列表
来源：http://afc.meibo888.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://pku.ehwqpu.com

[Q21] 空值判断
来源：http://ils.gaohongyu789.top

SELECT * FROM users WHERE email IS NULL;
来源：http://bmo.ydzc1.top

[Q22] 排序
来源：http://ylg.zdbjq.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://uai.tianlin.xyz

[Q23] 分页
来源：http://ssm.hongshengwenyu.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://pmg.dianchejie.cn

[Q24] 去重
来源：http://oik.jinqigufen.top

SELECT DISTINCT city FROM users;
来源：http://vur.0kj1m.cn

[Q25] 只取前 N 条
来源：http://svx.iojbl.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://xgf.nanxuanxn.top

[Q26] 计数
来源：http://fsc.yanxiufei.cn

SELECT COUNT(*) FROM users;
来源：http://baf.yueranfly.top

[Q27] 条件计数
来源：http://txg.vqdsnc.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://rmj.yvedp.cn

[Q28] 求和与平均
来源：http://fbn.0kj1m.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://syq.nanxuanxn.top

[Q29] 最大最小值
来源：http://fef.zdbjq.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://amc.xziqi.cn

[Q30] 分组统计
来源：http://uvi.9152youxi.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://zcp.ybcxt.top

[Q31] 分组后过滤
来源：http://gzn.pengpengdd.cyou

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://sng.zhengqikj.top

[Q32] 分组拼接字符串
来源：http://jsi.316326.xyz

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://lwm.hongshengwenyu.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://tts.gaohongyu789.top

[Q33] 多列分组
来源：http://evh.ydzc1.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://jqr.cucudq.cn

[Q34] 每组取第一条
来源：http://wsh.kuanghao11.cn

SELECT * FROM (
来源：http://xdg.yvedp.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mbr.quarkkingdee.top

) t WHERE rn = 1;
来源：http://yti.sweek.top

[Q35] 内连接
来源：http://dfm.yj20258888.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://jwm.vqdsnc.cn

[Q36] 左连接
来源：http://duy.0kj1m.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://qdl.bjfxy.top

[Q37] 右连接
来源：http://sow.zdbjq.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ppt.jqgufenzy.top

[Q38] 全外连接（PostgreSQL）
来源：http://utq.gotoacloud.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://pfc.bjfxy.top

[Q39] 自连接（查上下级）
来源：http://rzp.jlsjyb.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://bss.hysaishi.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://vbe.dianchejie.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ccg.havefunace.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://jra.zdbjq.cn

[Q41] 多表连接
来源：http://mpe.zycfv.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://sml.ywan-chungtsiang.top

JOIN users u ON u.id = o.user_id
来源：http://vmy.cqqwz.cn

JOIN products p ON p.id = o.product_id;
来源：http://yog.hongshengwenyu.top

[Q42] 连接条件附加过滤
来源：http://alc.jinqigfzy.top

SELECT u.name, o.amount FROM users u
来源：http://zxf.zhiwuduotai.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://sdo.tarul.cn

[Q43] 标量子查询
来源：http://czp.gaohongyu789.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://scd.zhengqikj.top

[Q44] IN 子查询
来源：http://ida.sjlbkw.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://gkv.xuanzx.com

[Q45] EXISTS 判断存在
来源：http://qji.guowangkeji.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ltl.52xcode.cn

[Q46] NOT EXISTS 判断不存在
来源：http://bkq.meibo888.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://yxs.zhixingplan.top

[Q47] 与平均值比较
来源：http://rub.zdqjudy.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://dyc.andypj.xyz

[Q48] CTE 公用表表达式
来源：http://wad.ctjpmb.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://lso.vehdjk.com

SELECT * FROM t WHERE c > 5;
来源：http://maz.shanyushiyangtech.top

[Q49] 更新单行
来源：http://zti.zhoulong.xyz

UPDATE users SET status = 1 WHERE id = 10;
来源：http://qwf.hnxiangtu.top

[Q50] 批量更新
来源：http://fgi.birdmap.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://rek.xuetiantiany.cn

[Q51] 用子查询更新
来源：http://vsd.fzhhl.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://pmf.cheryme.top

[Q52] 删除指定行
来源：http://icb.daria6918.cn

DELETE FROM users WHERE id = 10;
来源：http://riy.jinyuanbaomall.cn

[Q53] 按条件删除
来源：http://jxi.ppjwa.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://eoh.xziqi.cn

[Q54] 清空表
来源：http://miw.uphjek.com

TRUNCATE TABLE logs;
来源：http://ika.epnwcf.com

[Q55] 排名（并列占位）
来源：http://rnp.zhijiandao.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://box.wangshuangyany.cn

[Q56] 密集排名（并列不占位）
来源：http://miu.zhongyouzk.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://jzl.yj20258888.top

[Q57] 行号
来源：http://wpj.zhaomingkeji.xyz

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ypt.chenlongwang.top

[Q58] 累计求和
来源：http://wij.cashguo.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wms.ywan-chungtsiang.top

[Q59] 分组内累计
来源：http://akl.meibo888.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wxh.epnwcf.com

[Q60] 取上一行 / 下一行
来源：http://ksh.ctjpmb.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://yrj.sxryk.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://qgw.yuxming.cn

[Q61] 移动平均
来源：http://wyd.quarkkingdee.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://jpk.xingfuxueyuan.xyz

[Q62] 分组占比
来源：http://omp.fktsv.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ezz.zhengqikj.top

[Q63] 开启事务
来源：http://vuy.sysykeji.top

START TRANSACTION;                -- 或 BEGIN
来源：http://kfe.bbcook.cn

[Q64] 提交事务
来源：http://lhi.aizwys.cn

COMMIT;
来源：http://ano.gotoacloud.top

[Q65] 回滚事务
来源：http://foa.fehbvm.com

ROLLBACK;
来源：http://xkq.uphjek.com

[Q66] 行锁查询
来源：http://gtb.jinyuanbaomall.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://cpq.ywan-chungtsiang.top

[Q67] 设置隔离级别
来源：http://svv.tanke756.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://upy.hnxiangtu.top

[Q68] 保存点
来源：http://nbj.xingfuxueyuan.xyz

SAVEPOINT sp1;
来源：http://yyg.tanke756.top

ROLLBACK TO sp1;
来源：http://ccn.zdqjudy.top

[Q69] 查看执行计划
来源：http://qpj.dianchejie.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://jid.aizwys.cn

[Q70] 更新统计信息
来源：http://eou.gaohongyu789.top

ANALYZE TABLE users;
来源：http://msc.cheryme.top

[Q71] 查看建表语句
来源：http://tht.316326.xyz

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://cql.zhengqikj.top

[Q72] 查看索引
来源：http://bok.shanyushiyangkeji.top

SHOW INDEX FROM users;
来源：http://nqa.nanxuanxn.top

[Q73] 查看表状态
来源：http://cfq.jinghuilouyu.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://hmu.yj20258888.top

[Q74] 强制使用索引
来源：http://npr.haohaochexian.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hes.0kj1m.cn

[Q75] 日期格式化
来源：http://oqm.shangyingyoupin.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hpq.pycfn.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ews.redwolf501.top

[Q76] 按天统计
来源：http://rjr.zycfv.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://bjp.ctjpmb.com

[Q77] 时间加减
来源：http://qmf.yuanzhike.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ppf.yueranfly.top

[Q78] 当前时间
来源：http://oez.jlsjyb.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://vri.chenzaomai.com

[Q79] 字符串拼接
来源：http://wik.zhixingplan.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://rtu.tianlin.xyz

[Q80] 字符串截取
来源：http://oej.iojbl.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://saf.ehwqpu.com

[Q81] 字符串替换
来源：http://khp.kuanghao11.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://tfc.c1oappe.top

[Q82] 字符长度与字节长度
来源：http://ild.ctjpmb.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://bka.ydzc1.top

[Q83] 大小写转换
来源：http://ngt.chenzaomai.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://jyp.ivvv.top

[Q84] 去除首尾空格
来源：http://boo.hnqzz.top

SELECT TRIM(name) FROM users;
来源：http://pfl.daria6918.cn

[Q85] 数值取整
来源：http://bag.ywan-chungtsiang.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://sxl.zhijiandao.cn

[Q86] 读取 JSON 字段
来源：http://cdm.andypj.xyz

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://aey.dianchejie.cn

[Q87] JSON 字段做条件
来源：http://ugf.smart0.xyz

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://yfe.mhx1999.top

[Q88] 行转列（条件聚合）
来源：http://kkn.snrcjt.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://lbq.mhx1999.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://cuh.yongpay.top

[Q89] 判断表是否存在
来源：http://oww.dianchejie.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ziq.epnwcf.com

[Q90] 生成序号列
来源：http://rne.jqgufenzy.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://duy.xziqi.cn

================================================================================
来源：http://mzc.jqgfzy.top

R. Bash 专题
来源：http://yml.ybcxt.top

================================================================================
来源：http://nvy.zycfv.cn

[R01] shebang 与严格模式
来源：http://gzy.andypj.xyz

#!/usr/bin/env bash
来源：http://onx.tianlin.xyz

set -euo pipefail
来源：http://xge.gzhubu.top

[R02] 变量赋值与使用
来源：http://zgl.zdqjudy.top

name="Tom"; echo "$name"
来源：http://ycr.dianchejie.cn

[R03] 只读变量
来源：http://ssx.jianghu66.top

readonly PI=3.14
来源：http://smt.wangshuangyany.cn

[R04] 位置参数
来源：http://npp.yvedp.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://lmj.redwolf501.top

[R05] 参数默认值
来源：http://mph.gogol.net.cn

name="${1:-default}"
来源：http://sgr.chenlongwang.top

[R06] 判断命令是否存在
来源：http://utu.zhijiandao.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://lfo.bbcook.cn

[R07] if 判断文件
来源：http://nar.fzhhl.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wlt.iojbl.cn

[R08] 数值比较
来源：http://qem.hywenlv.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://bux.jiagoushi.top

[R09] 字符串比较
来源：http://hrw.yj20258888.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wgg.nanxinkj.top

[R10] 正则匹配
来源：http://ein.jinqigfzy.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://nvd.zhijiandao.cn

[R11] case 多分支
来源：http://lfl.nwbrower.top

case "$1" in
来源：http://iox.mhx1999.top

start) echo "启动" ;;
来源：http://feb.tian-w.cn

stop)  echo "停止" ;;
来源：http://enf.zhengqikj.top

*)     echo "未知命令" ;;
来源：http://rai.snrcjt.cn

esac
来源：http://plp.yanxiufei.cn

[R12] for 遍历文件
来源：http://ubo.wangdashe.top

for f in *.txt; do echo "$f"; done
来源：http://kcu.hysaishi.cn

[R13] for 计数循环
来源：http://suc.mhx1999.top

for i in {1..10}; do echo "$i"; done
来源：http://vaa.xinyue.icu

[R14] C 风格 for
来源：http://zre.cashguo.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://npk.52xcode.cn

[R15] while 逐行读文件
来源：http://ddn.haohaochexian.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://fkm.zhixingplan.top

[R16] until 等待条件
来源：http://hai.birdmap.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://zan.hesvh.cn

[R17] 数组定义与取值
来源：http://wfw.cdnleiting.top

arr=(a b c); echo "${arr[0]}"
来源：http://oxh.yongpay.top

[R18] 遍历数组
来源：http://tog.yueranfly.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://pci.xuetiantiany.cn

[R19] 数组长度
来源：http://bhm.52xcode.cn

echo "${#arr[@]}"
来源：http://ykt.yvedp.cn

[R20] 关联数组（字典）
来源：http://lzs.fengsongda.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://sdq.316326.xyz

[R21] 字符串长度
来源：http://etc.yvedp.cn

echo "${#s}"
来源：http://czg.ywan-chungtsiang.top

[R22] 截取子串
来源：http://wyb.jyoumei.cn

echo "${s:0:5}"
来源：http://aoq.guowangkeji.top

[R23] 字符串替换
来源：http://czk.0kj1m.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ncq.chenjidiqi.icu

[R24] 大小写转换
来源：http://npl.wangdashe.top

echo "${s^^}"; echo "${s,,}"
来源：http://zxx.sufxvd.cn

[R25] 去后缀 / 去前缀
来源：http://dut.nwbrower.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://rcu.yvedp.cn

[R26] 命令替换
来源：http://mtd.mhx1999.top

now=$(date +%F); echo "$now"
来源：http://fbx.hcnkem.com

[R27] 算术展开
来源：http://szn.sysykeji.top

echo $((1 + 2 * 3))
来源：http://guh.tanke756.top

[R28] 浮点运算
来源：http://lub.vehdjk.com

echo "scale=2; 10/3" | bc
来源：http://oso.52xcode.cn

[R29] 定义函数
来源：http://jex.ctjpmb.com


<!-- 参考信息 -->