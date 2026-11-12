代发 wailian999

PHP:  // 手写时间戳比较
来源：http://wam.tian-w.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://atv.chenjidiqi.icu

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vpw.meibo888.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://nco.cashguo.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://lgl.wangshuangyany.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://yri.xuanzx.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://tqg.pengpengdd.cyou

[P08] 处理浮点精度问题
来源：http://tcn.hnxiangtu.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://vkj.iojbl.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://vvm.gotoacloud.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://nbo.hammf.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hlj.yj20258888.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://yyv.jiagoushi.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://nps.chenlongwang.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://lje.cheryme.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://bvm.zhijiandao.cn

================================================================================
来源：http://tvd.iojbl.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://dfn.gogol.net.cn

================================================================================
来源：http://aie.xuetiantiany.cn

[Q01] 创建表
来源：http://kkb.yj20258888.top

CREATE TABLE users (
来源：http://lyr.hongshengwenyu.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ygj.fanxiaobao.xyz

name VARCHAR(50) NOT NULL,
来源：http://kjq.zhoulong.xyz

email VARCHAR(100) UNIQUE,
来源：http://ded.sxryk.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://xuz.yvedp.cn

);
来源：http://nue.shanyushiyangtech.top

[Q02] 创建带外键的表
来源：http://oeo.ywan-chungtsiang.top

CREATE TABLE orders (
来源：http://fwg.cdnleiting.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://gli.sysykeji.top

user_id INT NOT NULL,
来源：http://lag.snrcjt.cn

amount DECIMAL(10, 2),
来源：http://qfh.bbcook.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://jwz.sysykeji.top

);
来源：http://cfb.daxiang520.top

[Q03] 增加列
来源：http://uuo.snrcjt.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ues.iojbl.cn

[Q04] 修改列类型
来源：http://zxz.hesvh.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://lqz.zdbjq.cn

[Q05] 重命名列
来源：http://npm.yj20258.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://fct.zhijiandao.cn

[Q06] 删除列
来源：http://uei.chenjidiqi.icu

ALTER TABLE users DROP COLUMN age;
来源：http://fek.kuanghao11.cn

[Q07] 删除表
来源：http://jcc.dashuyun.cn

DROP TABLE IF EXISTS orders;
来源：http://nuh.shanyushiyangkeji.top

[Q08] 创建普通索引
来源：http://ayi.zhengqikj.top

CREATE INDEX idx_users_email ON users(email);
来源：http://aji.haohaochexian.top

[Q09] 创建唯一索引
来源：http://pdm.xuanzx.com

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ohp.yvedp.cn

[Q10] 插入单行
来源：http://ixq.ehwqpu.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://fom.aizwys.cn

[Q11] 一次插入多行
来源：http://yto.aibaodan.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://fuu.sysykeji.top

[Q12] 插入后取自增 ID
来源：http://yuz.nwbrower.top

INSERT INTO users (name) VALUES ('C');
来源：http://snh.jlsjyb.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://zqx.fengsongda.top

[Q13] 忽略重复插入
来源：http://mmv.jlsjyb.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://qvc.yvedp.cn

[Q14] 存在则更新（upsert）
来源：http://ley.ydzc1.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://aec.havefunace.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://zzp.jqgufenzy.top

[Q15] 查询全部
来源：http://qnr.bbcook.cn

SELECT * FROM users;
来源：http://tfy.tian-w.cn

[Q16] 查询指定列
来源：http://phi.havefunace.top

SELECT id, name FROM users;
来源：http://pzw.hysaishi.cn

[Q17] 条件查询
来源：http://rco.zycfv.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://glf.yongpay.top

[Q18] 模糊匹配
来源：http://ill.mhx1999.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://cdq.quarkkingdee.top

[Q19] 范围查询
来源：http://vka.aizwys.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://bar.haohaochexian.top

[Q20] IN 列表
来源：http://iuk.jinqigufen.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://jjw.jianghu66.top

[Q21] 空值判断
来源：http://pqv.ctjpmb.com

SELECT * FROM users WHERE email IS NULL;
来源：http://gen.yonumen.top

[Q22] 排序
来源：http://odl.cucudq.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://fqx.epnwcf.com

[Q23] 分页
来源：http://rkx.havefunace.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://jhx.yfazqb.com

[Q24] 去重
来源：http://vjv.chenlongwang.top

SELECT DISTINCT city FROM users;
来源：http://fgh.ybcxt.top

[Q25] 只取前 N 条
来源：http://syc.hfpthk.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://vep.c1oappe.top

[Q26] 计数
来源：http://jom.xingfuxueyuan.xyz

SELECT COUNT(*) FROM users;
来源：http://hef.aibaodan.cn

[Q27] 条件计数
来源：http://mrv.52xcode.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://yci.ybcxt.top

[Q28] 求和与平均
来源：http://jtq.ybcxt.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ltm.andypj.xyz

[Q29] 最大最小值
来源：http://nid.haohaochexian.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://uhx.meibo888.top

[Q30] 分组统计
来源：http://lfr.yvedp.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://tnz.gaohongyu789.top

[Q31] 分组后过滤
来源：http://fwg.hywenlv.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wwx.yj20258.top

[Q32] 分组拼接字符串
来源：http://izb.mhx1999.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wgf.hesvh.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://rpq.cucudq.cn

[Q33] 多列分组
来源：http://uyo.sufxvd.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://qir.ydzc1.top

[Q34] 每组取第一条
来源：http://vuj.pengpengdd.cyou

SELECT * FROM (
来源：http://fgn.9152youxi.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://pff.dianchejie.cn

) t WHERE rn = 1;
来源：http://tzi.chenzaomai.com

[Q35] 内连接
来源：http://jcy.fktsv.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://lrn.xingfuxueyuan.xyz

[Q36] 左连接
来源：http://gli.yfazqb.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://cdo.chenlongwang.top

[Q37] 右连接
来源：http://oqp.yonumen.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://uge.ybcxt.top

[Q38] 全外连接（PostgreSQL）
来源：http://vsb.xylfe.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://fxu.zhongyouzk.top

[Q39] 自连接（查上下级）
来源：http://ncy.jyoumei.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://bjx.chenlongwang.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://qyk.yueranfly.top

[Q40] 交叉连接（笛卡尔积）
来源：http://hhf.bbcook.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://kzt.shuidangran.top

[Q41] 多表连接
来源：http://lnp.yueranfly.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://oql.fzhhl.top

JOIN users u ON u.id = o.user_id
来源：http://fut.quarkkingdee.top

JOIN products p ON p.id = o.product_id;
来源：http://wdc.nwbrower.top

[Q42] 连接条件附加过滤
来源：http://ggq.tanke756.top

SELECT u.name, o.amount FROM users u
来源：http://jge.sufxvd.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://nbx.gzhubu.top

[Q43] 标量子查询
来源：http://vmy.hongshengwenyu.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://yep.yj20258.top

[Q44] IN 子查询
来源：http://rqe.cheryme.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://eif.jinqigfzy.top

[Q45] EXISTS 判断存在
来源：http://tzn.andypj.xyz

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wza.sufxvd.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ibi.fengsongda.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://nbt.zhixingplan.top

[Q47] 与平均值比较
来源：http://mow.wangshuangyany.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ink.yongpay.top

[Q48] CTE 公用表表达式
来源：http://dmu.dianchejie.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://lnn.chenjidiqi.icu

SELECT * FROM t WHERE c > 5;
来源：http://eov.sysykeji.top

[Q49] 更新单行
来源：http://aze.quarkkingdee.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://xjv.zhixingplan.top

[Q50] 批量更新
来源：http://wof.fehbvm.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://huk.ydjk.org.cn

[Q51] 用子查询更新
来源：http://jcf.sufxvd.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://xsq.jiagoushi.top

[Q52] 删除指定行
来源：http://ybs.jyoumei.cn

DELETE FROM users WHERE id = 10;
来源：http://say.jinghuilouyu.cn

[Q53] 按条件删除
来源：http://tkn.jinyuanbaomall.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://vmg.shuidangran.top

[Q54] 清空表
来源：http://yke.pycfn.com

TRUNCATE TABLE logs;
来源：http://foe.aizwys.cn

[Q55] 排名（并列占位）
来源：http://jex.hongshengwenyu.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://xmn.bbcook.cn

[Q56] 密集排名（并列不占位）
来源：http://vvz.xziqi.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wcr.cashguo.top

[Q57] 行号
来源：http://exw.ydzc1.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://nwu.zhoulong.xyz

[Q58] 累计求和
来源：http://oox.vqdsnc.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ahe.tianlin.xyz

[Q59] 分组内累计
来源：http://pya.daxiang520.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ucf.ydjk.org.cn

[Q60] 取上一行 / 下一行
来源：http://ncv.xingfuxueyuan.xyz

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ojr.hywenlv.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mdt.jinqigfzy.top

[Q61] 移动平均
来源：http://adj.yj202588.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wfz.kuanghao11.cn

[Q62] 分组占比
来源：http://yxw.yuxming.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mry.yonumen.top

[Q63] 开启事务
来源：http://hfn.jiagoushi.top

START TRANSACTION;                -- 或 BEGIN
来源：http://qhu.wangshuangyany.cn

[Q64] 提交事务
来源：http://cfg.shuidangran.top

COMMIT;
来源：http://vfq.jinghuilouyu.cn

[Q65] 回滚事务
来源：http://bme.jqgufenzy.top

ROLLBACK;
来源：http://yrg.svipenyu.cn

[Q66] 行锁查询
来源：http://jzk.xylfe.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://lul.xinyue.icu

[Q67] 设置隔离级别
来源：http://pyf.c1oappe.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://kbt.sjlbkw.cn

[Q68] 保存点
来源：http://bao.316326.xyz

SAVEPOINT sp1;
来源：http://jza.zhiwuduotai.top

ROLLBACK TO sp1;
来源：http://btq.kuanghao11.cn

[Q69] 查看执行计划
来源：http://lfa.zhongyouzk.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hea.xylfe.cn

[Q70] 更新统计信息
来源：http://plc.xylfe.cn

ANALYZE TABLE users;
来源：http://vpq.cqqwz.cn

[Q71] 查看建表语句
来源：http://uxd.xinyue.icu

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ruw.zycfv.cn

[Q72] 查看索引
来源：http://vyh.cucudq.cn

SHOW INDEX FROM users;
来源：http://tfp.andypj.xyz

[Q73] 查看表状态
来源：http://ass.hcnkem.com

SHOW TABLE STATUS LIKE 'users';
来源：http://kww.quarkkingdee.top

[Q74] 强制使用索引
来源：http://uaj.316326.xyz

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://lka.jinqigfzy.top

[Q75] 日期格式化
来源：http://qvh.ppjwa.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hjb.daria6918.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://pas.feifeiyinyue.top

[Q76] 按天统计
来源：http://hvw.jiagoushi.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://azf.9152youxi.cn

[Q77] 时间加减
来源：http://hvm.hesvh.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://jam.ybcxt.top

[Q78] 当前时间
来源：http://ntv.yongpay.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://uhb.yfazqb.com

[Q79] 字符串拼接
来源：http://fvq.shanyushiyangkeji.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://bjv.jinqigufen.top

[Q80] 字符串截取
来源：http://mrp.dashuyun.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wyh.andypj.xyz

[Q81] 字符串替换
来源：http://hpg.bjfxy.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hcz.fzhhl.top

[Q82] 字符长度与字节长度
来源：http://eit.hywenlv.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mxr.yvedp.cn

[Q83] 大小写转换
来源：http://xld.shangyingyoupin.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ojx.jinqigufen.top

[Q84] 去除首尾空格
来源：http://ppj.yuanzhike.top

SELECT TRIM(name) FROM users;
来源：http://qwu.chenjidiqi.icu

[Q85] 数值取整
来源：http://jld.0kj1m.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://jfj.nanxuanxn.top

[Q86] 读取 JSON 字段
来源：http://cpe.tian-w.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://dvh.hammf.cn

[Q87] JSON 字段做条件
来源：http://ram.vehdjk.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://oet.fehbvm.com

[Q88] 行转列（条件聚合）
来源：http://ezs.guowangkeji.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://tgm.shanyushiyangtech.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://sxg.shanyushiyangkeji.top

[Q89] 判断表是否存在
来源：http://lfk.shuidangran.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://anm.chenlongwang.top

[Q90] 生成序号列
来源：http://kyt.havefunace.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://tki.haohaochexian.top

================================================================================
来源：http://dkd.hysaishi.cn

R. Bash 专题
来源：http://dkn.gzhubu.top

================================================================================
来源：http://jar.ehwqpu.com

[R01] shebang 与严格模式
来源：http://rbz.yfazqb.com

#!/usr/bin/env bash
来源：http://six.dianchejie.cn

set -euo pipefail
来源：http://xdm.tian-w.cn

[R02] 变量赋值与使用
来源：http://juw.sysykeji.top

name="Tom"; echo "$name"
来源：http://egx.hammf.cn

[R03] 只读变量
来源：http://qbh.yangfankeji.com

readonly PI=3.14
来源：http://sic.yueranfly.top

[R04] 位置参数
来源：http://rzv.xziqi.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ojw.dianchejie.cn

[R05] 参数默认值
来源：http://sop.ydjk.org.cn

name="${1:-default}"
来源：http://gcd.sufxvd.cn

[R06] 判断命令是否存在
来源：http://kvv.bbcook.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://eim.cheryme.top

[R07] if 判断文件
来源：http://kbm.nanxinkj.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://jrv.aizwys.cn

[R08] 数值比较
来源：http://ulm.daria6918.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://drw.daxiang520.top

[R09] 字符串比较
来源：http://nbp.fanxiaobao.xyz

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://qrn.0kj1m.cn

[R10] 正则匹配
来源：http://fpm.feifeiyinyue.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://inu.sysykeji.top

[R11] case 多分支
来源：http://hhf.nwbrower.top

case "$1" in
来源：http://wpj.vqdsnc.cn

start) echo "启动" ;;
来源：http://jpp.cheryme.top

stop)  echo "停止" ;;
来源：http://dqf.sweek.top

*)     echo "未知命令" ;;
来源：http://yoo.vehdjk.com

esac
来源：http://ygj.yuxming.cn

[R12] for 遍历文件
来源：http://szo.hammf.cn

for f in *.txt; do echo "$f"; done
来源：http://qhy.epnwcf.com

[R13] for 计数循环
来源：http://snn.svipenyu.cn

for i in {1..10}; do echo "$i"; done
来源：http://edt.hesvh.cn

[R14] C 风格 for
来源：http://kcd.yvedp.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ksg.chenlongwang.top

[R15] while 逐行读文件
来源：http://dcg.ydzc1.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://znm.xingfuxueyuan.xyz

[R16] until 等待条件
来源：http://sim.bbcook.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://vcd.pycfn.com

[R17] 数组定义与取值
来源：http://ent.sysykeji.top

arr=(a b c); echo "${arr[0]}"
来源：http://poe.daxiang520.top

[R18] 遍历数组
来源：http://cnq.gotoacloud.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://xfz.vehdjk.com

[R19] 数组长度
来源：http://kmz.shanyushiyangkeji.top

echo "${#arr[@]}"
来源：http://qjd.iojbl.cn

[R20] 关联数组（字典）
来源：http://dep.yvedp.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://bas.c1oappe.top

[R21] 字符串长度
来源：http://fha.pengpengdd.cyou

echo "${#s}"
来源：http://eot.bbcook.cn

[R22] 截取子串
来源：http://ptr.jyoumei.cn

echo "${s:0:5}"
来源：http://uzv.52xcode.cn

[R23] 字符串替换
来源：http://onf.svipenyu.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://iiq.ywan-chungtsiang.top

[R24] 大小写转换
来源：http://hra.chenlongwang.top

echo "${s^^}"; echo "${s,,}"
来源：http://clr.redwolf501.top

[R25] 去后缀 / 去前缀
来源：http://zer.yj20258888.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://xhw.tanke756.top

[R26] 命令替换
来源：http://xcz.ehwqpu.com

now=$(date +%F); echo "$now"
来源：http://dwd.yuxming.cn

[R27] 算术展开
来源：http://iwy.chenlongwang.top

echo $((1 + 2 * 3))
来源：http://anf.gogol.net.cn

[R28] 浮点运算
来源：http://otm.zhoulong.xyz

echo "scale=2; 10/3" | bc
来源：http://awj.0kj1m.cn

[R29] 定义函数
来源：http://ood.meibo888.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://rtg.ctjpmb.com

[R30] 函数返回状态码
来源：http://qcd.ctjpmb.com

f() { return 0; }; f || echo "失败了"
来源：http://vxv.pengpengdd.cyou

[R31] 局部变量
来源：http://bol.tarul.cn

f() { local x=1; echo "$x"; }
来源：http://wnq.wangshuangyany.cn

[R32] 参数个数校验
来源：http://yzp.zycfv.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://gix.yuxming.cn

[R33] 捕获错误并提示行号
来源：http://gmj.sjlbkw.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://vll.aibaodan.cn

[R34] 退出时清理
来源：http://zoa.kuanghao11.cn

trap 'rm -f "$tmp"' EXIT
来源：http://qbq.yuxming.cn

[R35] 后台执行并等待
来源：http://bbs.jqgfzy.top


<!-- 参考信息 -->