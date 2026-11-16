代发 wailian999

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://xai.iojbl.cn

TS:   if (x == null) {}
来源：http://stn.xuanzx.com

Java: if (x == null || x.isEmpty()) {}
来源：http://xdf.tianlin.xyz

Go:   if x == nil {}
来源：http://oyd.shuidangran.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://owk.fengsongda.top

C#:   if (x is null) {}
来源：http://huj.yongpay.top

[P07] 防抖与节流
来源：http://qte.wangdashe.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ohc.tanke756.top

PHP:  // 手写时间戳比较
来源：http://sdu.kuanghao11.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fun.hywenlv.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://szy.hongshengwenyu.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://atp.gzhubu.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://eoz.hesvh.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://tcz.tianlin.xyz

C#:   // 用 System.Timers.Timer 重置实现
来源：http://vdg.9152youxi.cn

[P08] 处理浮点精度问题
来源：http://vpq.xinyue.icu

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mwu.ybcxt.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://fvd.chenlongwang.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ecl.fengsongda.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://tnl.zdqjudy.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://bnw.ehwqpu.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://beb.shangyingyoupin.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://fsu.hfpthk.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://rng.hammf.cn

================================================================================
来源：http://hso.zycfv.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://rxk.hywenlv.cn

================================================================================
来源：http://fyb.jianghu66.top

[Q01] 创建表
来源：http://xvg.gotoacloud.top

CREATE TABLE users (
来源：http://yxd.0kj1m.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://tbf.hnxiangtu.top

name VARCHAR(50) NOT NULL,
来源：http://ubx.cucudq.cn

email VARCHAR(100) UNIQUE,
来源：http://hcu.xziqi.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://vhz.dianchejie.cn

);
来源：http://gav.gaohongyu789.top

[Q02] 创建带外键的表
来源：http://ffs.yj20258.top

CREATE TABLE orders (
来源：http://icr.xuanzx.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://jko.quarkkingdee.top

user_id INT NOT NULL,
来源：http://uyc.chenzaomai.com

amount DECIMAL(10, 2),
来源：http://pdo.yueranfly.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://apc.quarkkingdee.top

);
来源：http://lun.yuanzhike.top

[Q03] 增加列
来源：http://sti.gotoacloud.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://qyf.yuanzhike.top

[Q04] 修改列类型
来源：http://mkh.9152youxi.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wnf.cheryme.top

[Q05] 重命名列
来源：http://ivr.nwbrower.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://lwb.meibo888.top

[Q06] 删除列
来源：http://pqb.shuidangran.top

ALTER TABLE users DROP COLUMN age;
来源：http://kwr.zhijiandao.cn

[Q07] 删除表
来源：http://eyz.tarul.cn

DROP TABLE IF EXISTS orders;
来源：http://yrg.jianghu66.top

[Q08] 创建普通索引
来源：http://dfj.guowangkeji.top

CREATE INDEX idx_users_email ON users(email);
来源：http://unu.jiagoushi.top

[Q09] 创建唯一索引
来源：http://ucs.bjfxy.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://owk.hysaishi.cn

[Q10] 插入单行
来源：http://bfl.redwolf501.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://xrz.jinyuanbaomall.cn

[Q11] 一次插入多行
来源：http://koa.aibaodan.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://avn.hfpthk.cn

[Q12] 插入后取自增 ID
来源：http://kuh.hammf.cn

INSERT INTO users (name) VALUES ('C');
来源：http://crt.316326.xyz

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mty.yonumen.top

[Q13] 忽略重复插入
来源：http://gep.quarkkingdee.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://tod.52xcode.cn

[Q14] 存在则更新（upsert）
来源：http://pbu.sufxvd.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://csy.uphjek.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ydi.ppjwa.cn

[Q15] 查询全部
来源：http://oio.chenlongwang.top

SELECT * FROM users;
来源：http://zog.ehwqpu.com

[Q16] 查询指定列
来源：http://bdm.hammf.cn

SELECT id, name FROM users;
来源：http://qsh.xinyue.icu

[Q17] 条件查询
来源：http://iri.cashguo.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://tsp.andypj.xyz

[Q18] 模糊匹配
来源：http://xlo.daria6918.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://dtf.hongshengwenyu.top

[Q19] 范围查询
来源：http://dlj.zhengqikj.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hkd.gzhubu.top

[Q20] IN 列表
来源：http://pfj.ctjpmb.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://yhc.chenzaomai.com

[Q21] 空值判断
来源：http://wqz.guowangkeji.top

SELECT * FROM users WHERE email IS NULL;
来源：http://smd.jinqigfzy.top

[Q22] 排序
来源：http://nni.c1oappe.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://gnm.tian-w.cn

[Q23] 分页
来源：http://vmd.zhongyouzk.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://bpa.gotoacloud.top

[Q24] 去重
来源：http://kqk.yuanzhike.top

SELECT DISTINCT city FROM users;
来源：http://utw.tanke756.top

[Q25] 只取前 N 条
来源：http://dno.hfpthk.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://xse.zhoulong.xyz

[Q26] 计数
来源：http://zcv.epnwcf.com

SELECT COUNT(*) FROM users;
来源：http://vga.yuxming.cn

[Q27] 条件计数
来源：http://oqf.ivvv.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://tol.cdnleiting.top

[Q28] 求和与平均
来源：http://nxz.wangshuangyany.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hko.shanyushiyangkeji.top

[Q29] 最大最小值
来源：http://uyp.cdnleiting.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://zla.hnqzz.top

[Q30] 分组统计
来源：http://esh.cqqwz.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://cvp.nwbrower.top

[Q31] 分组后过滤
来源：http://tgj.chenjidiqi.icu

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://icm.havefunace.top

[Q32] 分组拼接字符串
来源：http://bfv.ybcxt.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ygk.cheryme.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://lmt.xuanzx.com

[Q33] 多列分组
来源：http://lxn.bbcook.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://bsl.epnwcf.com

[Q34] 每组取第一条
来源：http://rxo.chenzaomai.com

SELECT * FROM (
来源：http://xyg.guowangkeji.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://uzw.yanxiufei.cn

) t WHERE rn = 1;
来源：http://ouu.0kj1m.cn

[Q35] 内连接
来源：http://iwa.birdmap.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://rvj.ctjpmb.com

[Q36] 左连接
来源：http://elb.yj202588.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://gcq.tanke756.top

[Q37] 右连接
来源：http://kuv.bjfxy.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://gjn.sxryk.cn

[Q38] 全外连接（PostgreSQL）
来源：http://uue.shzxlz.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://tqn.nwbrower.top

[Q39] 自连接（查上下级）
来源：http://sco.sysykeji.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://ufe.ybcxt.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ahf.guannengcc.top

[Q40] 交叉连接（笛卡尔积）
来源：http://raq.jiagoushi.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://bmn.svipenyu.cn

[Q41] 多表连接
来源：http://yfw.jianghu66.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://snd.xziqi.cn

JOIN users u ON u.id = o.user_id
来源：http://jre.316326.xyz

JOIN products p ON p.id = o.product_id;
来源：http://upc.shanyushiyangtech.top

[Q42] 连接条件附加过滤
来源：http://xpl.havefunace.top

SELECT u.name, o.amount FROM users u
来源：http://sny.jianghu66.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://gwl.jinqigfzy.top

[Q43] 标量子查询
来源：http://ind.ctjpmb.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://znq.yuanzhike.top

[Q44] IN 子查询
来源：http://vjf.chenlongwang.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ycf.dianchejie.cn

[Q45] EXISTS 判断存在
来源：http://tjs.aizwys.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://yaw.redwolf501.top

[Q46] NOT EXISTS 判断不存在
来源：http://sdy.zhaomingkeji.xyz

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://gqs.zhongyouzk.top

[Q47] 与平均值比较
来源：http://dqq.nanxuanxn.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://pyv.pengpengdd.cyou

[Q48] CTE 公用表表达式
来源：http://cvi.zhiwuduotai.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://bcy.gaohongyu789.top

SELECT * FROM t WHERE c > 5;
来源：http://eiy.xingfuxueyuan.xyz

[Q49] 更新单行
来源：http://iqr.9152youxi.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://gdq.yuxming.cn

[Q50] 批量更新
来源：http://cex.chenzaomai.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://dby.ywan-chungtsiang.top

[Q51] 用子查询更新
来源：http://yog.iojbl.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://qev.pycfn.com

[Q52] 删除指定行
来源：http://wyt.nanxinkj.top

DELETE FROM users WHERE id = 10;
来源：http://kqq.yuxming.cn

[Q53] 按条件删除
来源：http://ump.guowangkeji.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://kqv.xuanzx.com

[Q54] 清空表
来源：http://lla.wangdashe.top

TRUNCATE TABLE logs;
来源：http://ean.zhengqikj.top

[Q55] 排名（并列占位）
来源：http://pdo.feifeiyinyue.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://pfn.cucudq.cn

[Q56] 密集排名（并列不占位）
来源：http://zlu.snrcjt.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://vbq.yj20258888.top

[Q57] 行号
来源：http://wda.yonumen.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ixh.yueranfly.top

[Q58] 累计求和
来源：http://wms.uphjek.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://nfv.feifeiyinyue.top

[Q59] 分组内累计
来源：http://dpa.zdbjq.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://gmg.zhongyouzk.top

[Q60] 取上一行 / 下一行
来源：http://xow.hongshengwenyu.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://npa.ehwqpu.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://lbc.daxiang520.top

[Q61] 移动平均
来源：http://dtz.havefunace.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://xwb.jinqigfzy.top

[Q62] 分组占比
来源：http://htm.dianchejie.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://agt.andypj.xyz

[Q63] 开启事务
来源：http://kfx.tanke756.top

START TRANSACTION;                -- 或 BEGIN
来源：http://bxe.yj20258888.top

[Q64] 提交事务
来源：http://fsj.haohaochexian.top

COMMIT;
来源：http://wqu.quarkkingdee.top

[Q65] 回滚事务
来源：http://ldn.yj202588.top

ROLLBACK;
来源：http://qib.dashuyun.cn

[Q66] 行锁查询
来源：http://tub.hfpthk.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://gof.ivvv.top

[Q67] 设置隔离级别
来源：http://vri.zhengqikj.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ipx.hnqzz.top

[Q68] 保存点
来源：http://exw.ivvv.top

SAVEPOINT sp1;
来源：http://zbm.nanxinkj.top

ROLLBACK TO sp1;
来源：http://pbg.0kj1m.cn

[Q69] 查看执行计划
来源：http://dux.sweek.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://eeb.cqqwz.cn

[Q70] 更新统计信息
来源：http://gng.jinghuilouyu.cn

ANALYZE TABLE users;
来源：http://yax.aibaodan.cn

[Q71] 查看建表语句
来源：http://vqe.316326.xyz

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ctc.chenzaomai.com

[Q72] 查看索引
来源：http://xry.jinyuanbaomall.cn

SHOW INDEX FROM users;
来源：http://vdp.cashguo.top

[Q73] 查看表状态
来源：http://ydj.uphjek.com

SHOW TABLE STATUS LIKE 'users';
来源：http://ugq.zhengqikj.top

[Q74] 强制使用索引
来源：http://kta.zdqjudy.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://xzp.yj202588.top

[Q75] 日期格式化
来源：http://vft.zhiwuduotai.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://jpk.sxryk.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ctv.fengsongda.top

[Q76] 按天统计
来源：http://hjw.dianchejie.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://yyq.yongpay.top

[Q77] 时间加减
来源：http://kof.sxryk.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://cqw.jqgfzy.top

[Q78] 当前时间
来源：http://lkh.jinqigfzy.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hea.daria6918.cn

[Q79] 字符串拼接
来源：http://dtw.ctjpmb.com

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://yeu.hfpthk.cn

[Q80] 字符串截取
来源：http://acq.ppjwa.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://qof.cashguo.top

[Q81] 字符串替换
来源：http://ldr.cashguo.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://qxs.cashguo.top

[Q82] 字符长度与字节长度
来源：http://kua.xziqi.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://irx.zhaomingkeji.xyz

[Q83] 大小写转换
来源：http://bts.feifeiyinyue.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://had.bbcook.cn

[Q84] 去除首尾空格
来源：http://plq.yj20258.top

SELECT TRIM(name) FROM users;
来源：http://els.fktsv.cn

[Q85] 数值取整
来源：http://psq.yfazqb.com

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://gsq.pycfn.com

[Q86] 读取 JSON 字段
来源：http://soz.birdmap.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://sjt.tianlin.xyz

[Q87] JSON 字段做条件
来源：http://akk.epnwcf.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://nkt.sysykeji.top

[Q88] 行转列（条件聚合）
来源：http://zjy.jinqigfzy.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://vfr.ywan-chungtsiang.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://qcj.yongpay.top

[Q89] 判断表是否存在
来源：http://xzf.wangdashe.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://pvk.yonumen.top

[Q90] 生成序号列
来源：http://fny.52xcode.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://len.jqgfzy.top

================================================================================
来源：http://pls.snrcjt.cn

R. Bash 专题
来源：http://qyl.yj20258.top

================================================================================
来源：http://ttl.uphjek.com

[R01] shebang 与严格模式
来源：http://qmy.jqgfzy.top

#!/usr/bin/env bash
来源：http://wtz.xuetiantiany.cn

set -euo pipefail
来源：http://bbd.pycfn.com

[R02] 变量赋值与使用
来源：http://yek.iojbl.cn

name="Tom"; echo "$name"
来源：http://kue.zycfv.cn

[R03] 只读变量
来源：http://urp.aibaodan.cn

readonly PI=3.14
来源：http://ddn.xingfuxueyuan.xyz

[R04] 位置参数
来源：http://apt.hnqzz.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://uks.zdqjudy.top

[R05] 参数默认值
来源：http://ycu.tanke756.top

name="${1:-default}"
来源：http://rmb.pengpengdd.cyou

[R06] 判断命令是否存在
来源：http://aza.c1oappe.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://dqq.iojbl.cn

[R07] if 判断文件
来源：http://kyo.jyoumei.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://bqn.cucudq.cn

[R08] 数值比较
来源：http://jvk.xuanzx.com

if (( a > b )); then echo "a 更大"; fi
来源：http://xnl.guannengcc.top

[R09] 字符串比较
来源：http://xbm.havefunace.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://jfu.c1oappe.top

[R10] 正则匹配
来源：http://hye.yonumen.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://kww.yj202588.top

[R11] case 多分支
来源：http://pui.sufxvd.cn

case "$1" in
来源：http://mlg.quarkkingdee.top

start) echo "启动" ;;
来源：http://aoh.epnwcf.com

stop)  echo "停止" ;;
来源：http://skj.316326.xyz

*)     echo "未知命令" ;;
来源：http://ygm.jyoumei.cn

esac
来源：http://xbc.nanxinkj.top

[R12] for 遍历文件
来源：http://mfn.chenjidiqi.icu

for f in *.txt; do echo "$f"; done
来源：http://ggp.hongshengwenyu.top

[R13] for 计数循环
来源：http://jjq.chenjidiqi.icu

for i in {1..10}; do echo "$i"; done
来源：http://kyr.ydzc1.top

[R14] C 风格 for
来源：http://bou.tian-w.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://gcr.jlsjyb.cn

[R15] while 逐行读文件
来源：http://yzu.nanxinkj.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://nkd.pengpengdd.cyou

[R16] until 等待条件
来源：http://rwu.vehdjk.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://tsg.zhongyouzk.top

[R17] 数组定义与取值
来源：http://ffp.jqgufenzy.top

arr=(a b c); echo "${arr[0]}"
来源：http://kar.zhijiandao.cn

[R18] 遍历数组
来源：http://lwt.wangshuangyany.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://cqb.sxryk.cn

[R19] 数组长度
来源：http://shk.fzhhl.top

echo "${#arr[@]}"
来源：http://eos.zycfv.cn

[R20] 关联数组（字典）
来源：http://brt.ehwqpu.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://rks.hongshengwenyu.top

[R21] 字符串长度
来源：http://jdf.shanyushiyangkeji.top

echo "${#s}"
来源：http://rsh.vqdsnc.cn

[R22] 截取子串
来源：http://inw.52xcode.cn

echo "${s:0:5}"
来源：http://edl.havefunace.top

[R23] 字符串替换
来源：http://yst.xziqi.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ksp.yanxiufei.cn

[R24] 大小写转换
来源：http://qqb.zhongyouzk.top

echo "${s^^}"; echo "${s,,}"
来源：http://qra.xingfuxueyuan.xyz

[R25] 去后缀 / 去前缀
来源：http://jld.vqdsnc.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://kmo.zhaomingkeji.xyz

[R26] 命令替换
来源：http://fwd.jinqigfzy.top

now=$(date +%F); echo "$now"
来源：http://tby.nwbrower.top

[R27] 算术展开
来源：http://dbr.vqdsnc.cn

echo $((1 + 2 * 3))
来源：http://xkc.yuanzhike.top

[R28] 浮点运算
来源：http://trf.yvedp.cn

echo "scale=2; 10/3" | bc
来源：http://klz.smart0.xyz

[R29] 定义函数
来源：http://exg.sjlbkw.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://lux.sufxvd.cn

[R30] 函数返回状态码
来源：http://vct.yvedp.cn

f() { return 0; }; f || echo "失败了"
来源：http://rtg.yanxiufei.cn

[R31] 局部变量
来源：http://ezb.cucudq.cn


<!-- 参考信息 -->