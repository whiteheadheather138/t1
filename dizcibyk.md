代发 wailian999

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://pip.yj20258888.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://sup.zycfv.cn

Go:   reflect.DeepEqual(a, b)
来源：http://dfs.fehbvm.com

Ruby: a == b
来源：http://aev.jinqigufen.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://uot.bbcook.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://lsk.havefunace.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wef.xuetiantiany.cn

PHP:  if (empty($x)) {}
来源：http://uys.kuanghao11.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://eoq.ivvv.top

TS:   if (x == null) {}
来源：http://mxv.bjfxy.top

Java: if (x == null || x.isEmpty()) {}
来源：http://lje.fzhhl.top

Go:   if x == nil {}
来源：http://ezf.zdqjudy.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://dfv.iojbl.cn

C#:   if (x is null) {}
来源：http://ljj.uphjek.com

[P07] 防抖与节流
来源：http://wjz.ehwqpu.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://duu.dianchejie.cn

PHP:  // 手写时间戳比较
来源：http://zqk.daxiang520.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://paj.ydzc1.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kvk.zycfv.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hdh.feifeiyinyue.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://brj.birdmap.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://era.hywenlv.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://aaj.chenzaomai.com

[P08] 处理浮点精度问题
来源：http://bga.zycfv.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://gkr.sweek.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://vwg.fktsv.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://tjh.shzxlz.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://kvq.daria6918.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://pin.yuxming.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://njz.daria6918.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://xrw.chenjidiqi.icu

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://kox.ivvv.top

================================================================================
来源：http://nqu.vqdsnc.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://rkp.yj20258888.top

================================================================================
来源：http://ivy.sufxvd.cn

[Q01] 创建表
来源：http://inx.gzhubu.top

CREATE TABLE users (
来源：http://llx.snrcjt.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://efs.zhongyouzk.top

name VARCHAR(50) NOT NULL,
来源：http://bft.meibo888.top

email VARCHAR(100) UNIQUE,
来源：http://fsi.gaohongyu789.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://fwd.jiagoushi.top

);
来源：http://frn.ctjpmb.com

[Q02] 创建带外键的表
来源：http://kex.haohaochexian.top

CREATE TABLE orders (
来源：http://uio.ppjwa.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://zfl.wangshuangyany.cn

user_id INT NOT NULL,
来源：http://kki.jianghu66.top

amount DECIMAL(10, 2),
来源：http://ikp.epnwcf.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://fow.ctjpmb.com

);
来源：http://uup.zhixingplan.top

[Q03] 增加列
来源：http://ecf.zhixingplan.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ufu.sweek.top

[Q04] 修改列类型
来源：http://zkl.shuidangran.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://yei.xinyue.icu

[Q05] 重命名列
来源：http://egs.nanxinkj.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://jjt.zhijiandao.cn

[Q06] 删除列
来源：http://ahz.yvedp.cn

ALTER TABLE users DROP COLUMN age;
来源：http://kol.shanyushiyangkeji.top

[Q07] 删除表
来源：http://hbc.yuanzhike.top

DROP TABLE IF EXISTS orders;
来源：http://cox.xingfuxueyuan.xyz

[Q08] 创建普通索引
来源：http://hjg.aibaodan.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://tjk.gogol.net.cn

[Q09] 创建唯一索引
来源：http://hml.birdmap.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wuh.yj20258888.top

[Q10] 插入单行
来源：http://hds.chenlongwang.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wsn.yvedp.cn

[Q11] 一次插入多行
来源：http://dks.aizwys.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://cba.tanke756.top

[Q12] 插入后取自增 ID
来源：http://cbn.yuxming.cn

INSERT INTO users (name) VALUES ('C');
来源：http://vpq.meibo888.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ngs.bjfxy.top

[Q13] 忽略重复插入
来源：http://nps.gogol.net.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://xoq.zycfv.cn

[Q14] 存在则更新（upsert）
来源：http://lka.zhiwuduotai.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://bpv.bbcook.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://asi.mhx1999.top

[Q15] 查询全部
来源：http://mqz.ybcxt.top

SELECT * FROM users;
来源：http://cqr.jinghuilouyu.cn

[Q16] 查询指定列
来源：http://nel.xingfuxueyuan.xyz

SELECT id, name FROM users;
来源：http://rrl.shanyushiyangkeji.top

[Q17] 条件查询
来源：http://ecl.hysaishi.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://iyp.kuanghao11.cn

[Q18] 模糊匹配
来源：http://ach.zhongyouzk.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://tqc.sxryk.cn

[Q19] 范围查询
来源：http://hfw.andypj.xyz

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ktv.cqqwz.cn

[Q20] IN 列表
来源：http://nft.chenzaomai.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://gpf.guannengcc.top

[Q21] 空值判断
来源：http://ena.snrcjt.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://knm.9152youxi.cn

[Q22] 排序
来源：http://ism.zhengqikj.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://gbm.tanke756.top

[Q23] 分页
来源：http://juu.pengpengdd.cyou

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://uyx.vqdsnc.cn

[Q24] 去重
来源：http://osw.jinqigufen.top

SELECT DISTINCT city FROM users;
来源：http://lnp.hesvh.cn

[Q25] 只取前 N 条
来源：http://urk.gzhubu.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://bjp.haohaochexian.top

[Q26] 计数
来源：http://qow.yvedp.cn

SELECT COUNT(*) FROM users;
来源：http://upk.dianchejie.cn

[Q27] 条件计数
来源：http://kqe.gotoacloud.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://qjm.jinqigfzy.top

[Q28] 求和与平均
来源：http://jsh.52xcode.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://sca.zycfv.cn

[Q29] 最大最小值
来源：http://mgn.wangshuangyany.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://igh.sysykeji.top

[Q30] 分组统计
来源：http://vqd.zycfv.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mcc.sysykeji.top

[Q31] 分组后过滤
来源：http://yly.vqdsnc.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://vfv.shanyushiyangkeji.top

[Q32] 分组拼接字符串
来源：http://eow.birdmap.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://vaq.yueranfly.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://pgy.xuanzx.com

[Q33] 多列分组
来源：http://njl.chenzaomai.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://fmt.316326.xyz

[Q34] 每组取第一条
来源：http://xwv.ppjwa.cn

SELECT * FROM (
来源：http://dmc.chenzaomai.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://dea.yueranfly.top

) t WHERE rn = 1;
来源：http://hci.tanke756.top

[Q35] 内连接
来源：http://fze.shuidangran.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hsm.shanyushiyangtech.top

[Q36] 左连接
来源：http://bgy.ybcxt.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://aei.sjlbkw.cn

[Q37] 右连接
来源：http://bcb.jinyuanbaomall.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://nru.aibaodan.cn

[Q38] 全外连接（PostgreSQL）
来源：http://lra.zycfv.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://fzh.yangfankeji.com

[Q39] 自连接（查上下级）
来源：http://luv.pengpengdd.cyou

SELECT e.name, m.name AS manager FROM employees e
来源：http://ydx.jianghu66.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://teb.hcnkem.com

[Q40] 交叉连接（笛卡尔积）
来源：http://lnz.epnwcf.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ocz.tarul.cn

[Q41] 多表连接
来源：http://nse.316326.xyz

SELECT o.id, u.name, p.title FROM orders o
来源：http://qsg.ctjpmb.com

JOIN users u ON u.id = o.user_id
来源：http://gzw.daria6918.cn

JOIN products p ON p.id = o.product_id;
来源：http://laf.tianlin.xyz

[Q42] 连接条件附加过滤
来源：http://krw.hcnkem.com

SELECT u.name, o.amount FROM users u
来源：http://nch.yonumen.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wqw.vehdjk.com

[Q43] 标量子查询
来源：http://eao.tianlin.xyz

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://pzt.birdmap.top

[Q44] IN 子查询
来源：http://qwf.fzhhl.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://owt.0kj1m.cn

[Q45] EXISTS 判断存在
来源：http://zdq.pycfn.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wlf.sysykeji.top

[Q46] NOT EXISTS 判断不存在
来源：http://wva.cdnleiting.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fpy.jqgufenzy.top

[Q47] 与平均值比较
来源：http://sjl.smart0.xyz

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://fvn.tanke756.top

[Q48] CTE 公用表表达式
来源：http://alb.hnxiangtu.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wuc.zhongyouzk.top

SELECT * FROM t WHERE c > 5;
来源：http://cyv.xingfuxueyuan.xyz

[Q49] 更新单行
来源：http://vci.mhx1999.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mbl.jinqigufen.top

[Q50] 批量更新
来源：http://vgn.pengpengdd.cyou

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ock.wangshuangyany.cn

[Q51] 用子查询更新
来源：http://moz.yj202588.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://biu.wangshuangyany.cn

[Q52] 删除指定行
来源：http://aex.pengpengdd.cyou

DELETE FROM users WHERE id = 10;
来源：http://ixt.ppjwa.cn

[Q53] 按条件删除
来源：http://xvz.c1oappe.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://cnc.redwolf501.top

[Q54] 清空表
来源：http://lfm.zhengqikj.top

TRUNCATE TABLE logs;
来源：http://tdr.svipenyu.cn

[Q55] 排名（并列占位）
来源：http://xtk.guowangkeji.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://zxi.birdmap.top

[Q56] 密集排名（并列不占位）
来源：http://oyt.guannengcc.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mnt.hnqzz.top

[Q57] 行号
来源：http://hvq.yvedp.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://jzz.yuxming.cn

[Q58] 累计求和
来源：http://cys.daria6918.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://aez.fanxiaobao.xyz

[Q59] 分组内累计
来源：http://ram.tarul.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://oox.chenjidiqi.icu

[Q60] 取上一行 / 下一行
来源：http://nlh.yueranfly.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ers.yfazqb.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://qex.gotoacloud.top

[Q61] 移动平均
来源：http://fxt.svipenyu.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://nye.ybcxt.top

[Q62] 分组占比
来源：http://dcq.pengpengdd.cyou

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://cox.nanxuanxn.top

[Q63] 开启事务
来源：http://oom.tarul.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://yto.birdmap.top

[Q64] 提交事务
来源：http://fub.cheryme.top

COMMIT;
来源：http://gto.xylfe.cn

[Q65] 回滚事务
来源：http://acs.haohaochexian.top

ROLLBACK;
来源：http://vlf.fanxiaobao.xyz

[Q66] 行锁查询
来源：http://ifz.yuanzhike.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://fev.yvedp.cn

[Q67] 设置隔离级别
来源：http://wnt.hnqzz.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://loq.mhx1999.top

[Q68] 保存点
来源：http://ger.9152youxi.cn

SAVEPOINT sp1;
来源：http://qmm.yj202588.top

ROLLBACK TO sp1;
来源：http://xca.xylfe.cn

[Q69] 查看执行计划
来源：http://kfq.gzhubu.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://fbc.chenzaomai.com

[Q70] 更新统计信息
来源：http://kew.jyoumei.cn

ANALYZE TABLE users;
来源：http://ybt.yvedp.cn

[Q71] 查看建表语句
来源：http://dot.jinqigufen.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://zun.havefunace.top

[Q72] 查看索引
来源：http://xdx.ydzc1.top

SHOW INDEX FROM users;
来源：http://nea.shanyushiyangkeji.top

[Q73] 查看表状态
来源：http://myp.shzxlz.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://skf.yongpay.top

[Q74] 强制使用索引
来源：http://dst.shanyushiyangkeji.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://xls.yangfankeji.com

[Q75] 日期格式化
来源：http://ifg.jinghuilouyu.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://fvd.yueranfly.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ufg.snrcjt.cn

[Q76] 按天统计
来源：http://lkw.guannengcc.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ksd.fengsongda.top

[Q77] 时间加减
来源：http://rzr.zhengqikj.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://qhr.316326.xyz

[Q78] 当前时间
来源：http://krz.ywan-chungtsiang.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://het.jianghu66.top

[Q79] 字符串拼接
来源：http://cfu.fengsongda.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://utg.hongshengwenyu.top

[Q80] 字符串截取
来源：http://okb.cucudq.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://bwn.ehwqpu.com

[Q81] 字符串替换
来源：http://aoa.bbcook.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://xnp.birdmap.top

[Q82] 字符长度与字节长度
来源：http://ufx.tanke756.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://rll.hongshengwenyu.top

[Q83] 大小写转换
来源：http://abr.c1oappe.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://jnu.hnqzz.top

[Q84] 去除首尾空格
来源：http://wfx.ctjpmb.com

SELECT TRIM(name) FROM users;
来源：http://yei.snrcjt.cn

[Q85] 数值取整
来源：http://bmw.feifeiyinyue.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://cpt.snrcjt.cn

[Q86] 读取 JSON 字段
来源：http://jhp.hongshengwenyu.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://nnp.guowangkeji.top

[Q87] JSON 字段做条件
来源：http://itu.aizwys.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://zqb.pengpengdd.cyou

[Q88] 行转列（条件聚合）
来源：http://qco.hcnkem.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://qnj.shzxlz.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ube.wangshuangyany.cn

[Q89] 判断表是否存在
来源：http://szp.fanxiaobao.xyz

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://tew.fengsongda.top

[Q90] 生成序号列
来源：http://wxg.xinyue.icu

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://kha.jinqigufen.top

================================================================================
来源：http://uho.wangshuangyany.cn

R. Bash 专题
来源：http://mmd.andypj.xyz

================================================================================
来源：http://gfg.hnqzz.top

[R01] shebang 与严格模式
来源：http://loo.0kj1m.cn

#!/usr/bin/env bash
来源：http://rqk.cashguo.top

set -euo pipefail
来源：http://byy.shuidangran.top

[R02] 变量赋值与使用
来源：http://vtf.svipenyu.cn

name="Tom"; echo "$name"
来源：http://ukn.iojbl.cn

[R03] 只读变量
来源：http://bbx.iojbl.cn

readonly PI=3.14
来源：http://ath.xingfuxueyuan.xyz

[R04] 位置参数
来源：http://pfb.shuidangran.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://xcs.tianlin.xyz

[R05] 参数默认值
来源：http://rnb.yuxming.cn

name="${1:-default}"
来源：http://gyo.hesvh.cn

[R06] 判断命令是否存在
来源：http://mxh.xinyue.icu

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://zjg.sxryk.cn

[R07] if 判断文件
来源：http://cyc.c1oappe.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://uyd.meibo888.top

[R08] 数值比较
来源：http://cuz.fzhhl.top

if (( a > b )); then echo "a 更大"; fi
来源：http://znq.pycfn.com

[R09] 字符串比较
来源：http://ajf.shanyushiyangtech.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://bcq.sysykeji.top

[R10] 正则匹配
来源：http://stq.c1oappe.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ngh.hnqzz.top

[R11] case 多分支
来源：http://tyf.yvedp.cn

case "$1" in
来源：http://xqk.xuetiantiany.cn

start) echo "启动" ;;
来源：http://yfo.xylfe.cn

stop)  echo "停止" ;;
来源：http://qza.dianchejie.cn

*)     echo "未知命令" ;;
来源：http://tun.epnwcf.com

esac
来源：http://ypn.smart0.xyz

[R12] for 遍历文件
来源：http://jrv.pengpengdd.cyou

for f in *.txt; do echo "$f"; done
来源：http://ycn.ctjpmb.com

[R13] for 计数循环
来源：http://jgz.yj20258888.top

for i in {1..10}; do echo "$i"; done
来源：http://nwk.yanxiufei.cn

[R14] C 风格 for
来源：http://vqa.hammf.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ycm.pycfn.com

[R15] while 逐行读文件
来源：http://gxi.jinyuanbaomall.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://gfd.chenzaomai.com

[R16] until 等待条件
来源：http://wun.svipenyu.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://xat.yanxiufei.cn

[R17] 数组定义与取值
来源：http://yrt.yj20258888.top

arr=(a b c); echo "${arr[0]}"
来源：http://tms.ybcxt.top

[R18] 遍历数组
来源：http://luv.ehwqpu.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mid.nwbrower.top

[R19] 数组长度
来源：http://nwr.gzhubu.top

echo "${#arr[@]}"
来源：http://uyh.ydzc1.top

[R20] 关联数组（字典）
来源：http://oxj.yj20258888.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://iqy.shangyingyoupin.top

[R21] 字符串长度
来源：http://hpl.xylfe.cn

echo "${#s}"
来源：http://det.hysaishi.cn

[R22] 截取子串
来源：http://icl.jinqigufen.top

echo "${s:0:5}"
来源：http://unv.hammf.cn

[R23] 字符串替换
来源：http://qfy.cashguo.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://jhj.yuanzhike.top

[R24] 大小写转换
来源：http://oce.hnqzz.top

echo "${s^^}"; echo "${s,,}"
来源：http://oum.nwbrower.top

[R25] 去后缀 / 去前缀
来源：http://tjp.kuanghao11.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://vyb.hnqzz.top

[R26] 命令替换
来源：http://gwv.jqgufenzy.top

now=$(date +%F); echo "$now"
来源：http://tvz.fzhhl.top

[R27] 算术展开
来源：http://chm.yvedp.cn


<!-- 参考信息 -->