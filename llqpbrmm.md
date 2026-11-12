代发 wailian999

PHP:  // 手写时间戳比较
来源：http://zes.guowangkeji.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://uwj.xziqi.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fwr.epnwcf.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ynn.yuxming.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://sbc.zhixingplan.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://uqa.xingfuxueyuan.xyz

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ibc.yj20258.top

[P08] 处理浮点精度问题
来源：http://wpw.jinqigfzy.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://zzb.yj202588.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://jrn.snrcjt.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://qjs.tianlin.xyz

TS:   (0.1 + 0.2).toFixed(2)
来源：http://rxp.chenjidiqi.icu

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://bdn.smart0.xyz

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ndj.jinghuilouyu.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://pvb.jyoumei.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://otu.hongshengwenyu.top

================================================================================
来源：http://gkz.sufxvd.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wgq.xuetiantiany.cn

================================================================================
来源：http://hcw.iojbl.cn

[Q01] 创建表
来源：http://usj.yvedp.cn

CREATE TABLE users (
来源：http://ulx.nwbrower.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://jjq.dashuyun.cn

name VARCHAR(50) NOT NULL,
来源：http://ttv.chenzaomai.com

email VARCHAR(100) UNIQUE,
来源：http://vnm.chenzaomai.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ves.uphjek.com

);
来源：http://sjs.tanke756.top

[Q02] 创建带外键的表
来源：http://neb.9152youxi.cn

CREATE TABLE orders (
来源：http://cdg.tarul.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://kcc.yanxiufei.cn

user_id INT NOT NULL,
来源：http://uow.yj202588.top

amount DECIMAL(10, 2),
来源：http://qzz.epnwcf.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://nsd.aibaodan.cn

);
来源：http://cfq.smart0.xyz

[Q03] 增加列
来源：http://tbf.cdnleiting.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://zsd.jlsjyb.cn

[Q04] 修改列类型
来源：http://dkt.xuanzx.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://jms.zhixingplan.top

[Q05] 重命名列
来源：http://csm.sxryk.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://fnm.cqqwz.cn

[Q06] 删除列
来源：http://sob.gogol.net.cn

ALTER TABLE users DROP COLUMN age;
来源：http://xpy.hesvh.cn

[Q07] 删除表
来源：http://onx.nwbrower.top

DROP TABLE IF EXISTS orders;
来源：http://jyj.bbcook.cn

[Q08] 创建普通索引
来源：http://pik.ehwqpu.com

CREATE INDEX idx_users_email ON users(email);
来源：http://axy.ppjwa.cn

[Q09] 创建唯一索引
来源：http://unc.dashuyun.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://lrt.hcnkem.com

[Q10] 插入单行
来源：http://gih.zycfv.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://zkw.iojbl.cn

[Q11] 一次插入多行
来源：http://smz.hywenlv.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://tkv.ybcxt.top

[Q12] 插入后取自增 ID
来源：http://olz.jinqigufen.top

INSERT INTO users (name) VALUES ('C');
来源：http://dpb.pengpengdd.cyou

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://huq.hnqzz.top

[Q13] 忽略重复插入
来源：http://uvp.yj20258.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://zab.xuetiantiany.cn

[Q14] 存在则更新（upsert）
来源：http://inq.epnwcf.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://miu.gogol.net.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://lsx.jyoumei.cn

[Q15] 查询全部
来源：http://way.xylfe.cn

SELECT * FROM users;
来源：http://mdf.shzxlz.cn

[Q16] 查询指定列
来源：http://eiu.svipenyu.cn

SELECT id, name FROM users;
来源：http://thm.tian-w.cn

[Q17] 条件查询
来源：http://vub.guowangkeji.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://not.yanxiufei.cn

[Q18] 模糊匹配
来源：http://uwx.wangdashe.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://kdb.xingfuxueyuan.xyz

[Q19] 范围查询
来源：http://fug.kuanghao11.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://qxr.9152youxi.cn

[Q20] IN 列表
来源：http://iqt.fengsongda.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://neu.cqqwz.cn

[Q21] 空值判断
来源：http://cex.jinqigufen.top

SELECT * FROM users WHERE email IS NULL;
来源：http://efb.cheryme.top

[Q22] 排序
来源：http://zbz.shuidangran.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://rid.sysykeji.top

[Q23] 分页
来源：http://wma.yfazqb.com

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ece.hnxiangtu.top

[Q24] 去重
来源：http://dua.sysykeji.top

SELECT DISTINCT city FROM users;
来源：http://ujp.zhaomingkeji.xyz

[Q25] 只取前 N 条
来源：http://mwe.yuxming.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://nbh.tanke756.top

[Q26] 计数
来源：http://ojd.fehbvm.com

SELECT COUNT(*) FROM users;
来源：http://hah.cheryme.top

[Q27] 条件计数
来源：http://yen.xuetiantiany.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hzq.xylfe.cn

[Q28] 求和与平均
来源：http://knd.bjfxy.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://grj.dianchejie.cn

[Q29] 最大最小值
来源：http://qyo.jinqigfzy.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://fvy.yueranfly.top

[Q30] 分组统计
来源：http://rfd.hywenlv.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://rsk.nanxinkj.top

[Q31] 分组后过滤
来源：http://vbk.hcnkem.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://afi.fanxiaobao.xyz

[Q32] 分组拼接字符串
来源：http://yfo.xingfuxueyuan.xyz

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://piv.jyoumei.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://uou.gzhubu.top

[Q33] 多列分组
来源：http://fsa.redwolf501.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://dsf.hnqzz.top

[Q34] 每组取第一条
来源：http://oun.vehdjk.com

SELECT * FROM (
来源：http://nun.fehbvm.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://oml.guannengcc.top

) t WHERE rn = 1;
来源：http://hes.hywenlv.cn

[Q35] 内连接
来源：http://zzb.sufxvd.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ixh.guannengcc.top

[Q36] 左连接
来源：http://qjx.xylfe.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://eil.cucudq.cn

[Q37] 右连接
来源：http://nqh.jyoumei.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ztk.tanke756.top

[Q38] 全外连接（PostgreSQL）
来源：http://tkl.zhiwuduotai.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://icn.gotoacloud.top

[Q39] 自连接（查上下级）
来源：http://djn.sysykeji.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://eyd.hesvh.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://oym.guannengcc.top

[Q40] 交叉连接（笛卡尔积）
来源：http://qcz.cucudq.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://lpd.zhengqikj.top

[Q41] 多表连接
来源：http://fep.jianghu66.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://llk.epnwcf.com

JOIN users u ON u.id = o.user_id
来源：http://ori.snrcjt.cn

JOIN products p ON p.id = o.product_id;
来源：http://szt.nanxinkj.top

[Q42] 连接条件附加过滤
来源：http://efv.yonumen.top

SELECT u.name, o.amount FROM users u
来源：http://xhx.hnqzz.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://brp.tarul.cn

[Q43] 标量子查询
来源：http://pdf.ppjwa.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://rqq.chenlongwang.top

[Q44] IN 子查询
来源：http://nlo.hfpthk.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://rfr.ctjpmb.com

[Q45] EXISTS 判断存在
来源：http://soo.hfpthk.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ylx.zhixingplan.top

[Q46] NOT EXISTS 判断不存在
来源：http://giq.cdnleiting.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rvz.xuanzx.com

[Q47] 与平均值比较
来源：http://qbi.ywan-chungtsiang.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://lub.smart0.xyz

[Q48] CTE 公用表表达式
来源：http://sdv.xingfuxueyuan.xyz

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wyt.sxryk.cn

SELECT * FROM t WHERE c > 5;
来源：http://qjt.jqgufenzy.top

[Q49] 更新单行
来源：http://djk.bjfxy.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://qjn.shzxlz.cn

[Q50] 批量更新
来源：http://pwu.zhengqikj.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://nlf.xuetiantiany.cn

[Q51] 用子查询更新
来源：http://hxq.fehbvm.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://awl.zhengqikj.top

[Q52] 删除指定行
来源：http://nim.hongshengwenyu.top

DELETE FROM users WHERE id = 10;
来源：http://uhv.kuanghao11.cn

[Q53] 按条件删除
来源：http://doe.yj20258888.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://gpo.svipenyu.cn

[Q54] 清空表
来源：http://chy.yj202588.top

TRUNCATE TABLE logs;
来源：http://pqv.xuetiantiany.cn

[Q55] 排名（并列占位）
来源：http://bzl.cheryme.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://gjv.sweek.top

[Q56] 密集排名（并列不占位）
来源：http://lza.shzxlz.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://thr.yanxiufei.cn

[Q57] 行号
来源：http://xww.andypj.xyz

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://zqt.jiagoushi.top

[Q58] 累计求和
来源：http://nyb.xziqi.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://nwk.yongpay.top

[Q59] 分组内累计
来源：http://vjh.sweek.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://xrl.hammf.cn

[Q60] 取上一行 / 下一行
来源：http://jsh.zhengqikj.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://tsu.hcnkem.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://egr.zycfv.cn

[Q61] 移动平均
来源：http://ewx.zhongyouzk.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://amg.xuanzx.com

[Q62] 分组占比
来源：http://pgu.52xcode.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://kjg.cucudq.cn

[Q63] 开启事务
来源：http://kqh.andypj.xyz

START TRANSACTION;                -- 或 BEGIN
来源：http://bcg.ywan-chungtsiang.top

[Q64] 提交事务
来源：http://mtp.0kj1m.cn

COMMIT;
来源：http://cmr.yj20258.top

[Q65] 回滚事务
来源：http://crj.tian-w.cn

ROLLBACK;
来源：http://exr.daria6918.cn

[Q66] 行锁查询
来源：http://num.shzxlz.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wdk.guowangkeji.top

[Q67] 设置隔离级别
来源：http://wnl.redwolf501.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://grp.birdmap.top

[Q68] 保存点
来源：http://inz.hnqzz.top

SAVEPOINT sp1;
来源：http://dss.shzxlz.cn

ROLLBACK TO sp1;
来源：http://hso.yonumen.top

[Q69] 查看执行计划
来源：http://rjr.fehbvm.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://qcd.birdmap.top

[Q70] 更新统计信息
来源：http://jae.daxiang520.top

ANALYZE TABLE users;
来源：http://xfj.ydjk.org.cn

[Q71] 查看建表语句
来源：http://ozx.cdnleiting.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://njm.gogol.net.cn

[Q72] 查看索引
来源：http://guc.zhengqikj.top

SHOW INDEX FROM users;
来源：http://hli.jqgufenzy.top

[Q73] 查看表状态
来源：http://nmq.haohaochexian.top

SHOW TABLE STATUS LIKE 'users';
来源：http://tfr.jqgufenzy.top

[Q74] 强制使用索引
来源：http://eji.chenlongwang.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://yxn.sxryk.cn

[Q75] 日期格式化
来源：http://flb.hammf.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://cic.wangdashe.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mir.hesvh.cn

[Q76] 按天统计
来源：http://wqx.tarul.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://dfv.jqgfzy.top

[Q77] 时间加减
来源：http://wco.xinyue.icu

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://gxh.xinyue.icu

[Q78] 当前时间
来源：http://dpr.yanxiufei.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://xqu.0kj1m.cn

[Q79] 字符串拼接
来源：http://khw.yvedp.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ica.yuanzhike.top

[Q80] 字符串截取
来源：http://rga.snrcjt.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://eje.xinyue.icu

[Q81] 字符串替换
来源：http://uye.uphjek.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://gfk.zhoulong.xyz

[Q82] 字符长度与字节长度
来源：http://kxo.yangfankeji.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://xfr.hongshengwenyu.top

[Q83] 大小写转换
来源：http://lmz.wangshuangyany.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://gkc.zdqjudy.top

[Q84] 去除首尾空格
来源：http://czp.zhongyouzk.top

SELECT TRIM(name) FROM users;
来源：http://kkl.hnxiangtu.top

[Q85] 数值取整
来源：http://vhm.tarul.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://npi.zhiwuduotai.top

[Q86] 读取 JSON 字段
来源：http://btb.cheryme.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://dww.ivvv.top

[Q87] JSON 字段做条件
来源：http://uoj.shanyushiyangtech.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://pbd.shanyushiyangkeji.top

[Q88] 行转列（条件聚合）
来源：http://oky.yj20258.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://otv.guowangkeji.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://oij.daria6918.cn

[Q89] 判断表是否存在
来源：http://hxq.aibaodan.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://slt.gotoacloud.top

[Q90] 生成序号列
来源：http://zgn.52xcode.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://elq.uphjek.com

================================================================================
来源：http://vet.yonumen.top

R. Bash 专题
来源：http://yoo.xylfe.cn

================================================================================
来源：http://ksu.yvedp.cn

[R01] shebang 与严格模式
来源：http://xgc.havefunace.top

#!/usr/bin/env bash
来源：http://azt.zdbjq.cn

set -euo pipefail
来源：http://ooc.yangfankeji.com

[R02] 变量赋值与使用
来源：http://tzy.shangyingyoupin.top

name="Tom"; echo "$name"
来源：http://dun.jqgufenzy.top

[R03] 只读变量
来源：http://cbd.hcnkem.com

readonly PI=3.14
来源：http://pck.xinyue.icu

[R04] 位置参数
来源：http://vlx.sufxvd.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://kmw.dashuyun.cn

[R05] 参数默认值
来源：http://wec.sxryk.cn

name="${1:-default}"
来源：http://nyh.tianlin.xyz

[R06] 判断命令是否存在
来源：http://rmq.daria6918.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ywm.tian-w.cn

[R07] if 判断文件
来源：http://lys.xuanzx.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://xwv.cdnleiting.top

[R08] 数值比较
来源：http://fkx.hysaishi.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://atl.jqgfzy.top

[R09] 字符串比较
来源：http://jqp.feifeiyinyue.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://zsu.zdqjudy.top

[R10] 正则匹配
来源：http://bux.redwolf501.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://izr.ehwqpu.com

[R11] case 多分支
来源：http://giw.jinqigufen.top

case "$1" in
来源：http://mjw.cqqwz.cn

start) echo "启动" ;;
来源：http://fga.wangshuangyany.cn

stop)  echo "停止" ;;
来源：http://dry.yueranfly.top

*)     echo "未知命令" ;;
来源：http://exi.jianghu66.top

esac
来源：http://jxl.jinyuanbaomall.cn

[R12] for 遍历文件
来源：http://wpk.xinyue.icu

for f in *.txt; do echo "$f"; done
来源：http://zwn.bbcook.cn

[R13] for 计数循环
来源：http://xdx.cdnleiting.top

for i in {1..10}; do echo "$i"; done
来源：http://llx.xuanzx.com

[R14] C 风格 for
来源：http://tzg.tianlin.xyz

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wcs.pycfn.com

[R15] while 逐行读文件
来源：http://pfs.guannengcc.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://oxc.wangshuangyany.cn

[R16] until 等待条件
来源：http://xau.hammf.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://zzf.yfazqb.com

[R17] 数组定义与取值
来源：http://wac.chenzaomai.com

arr=(a b c); echo "${arr[0]}"
来源：http://klg.shzxlz.cn

[R18] 遍历数组
来源：http://jre.yuanzhike.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://evs.yueranfly.top

[R19] 数组长度
来源：http://kip.guowangkeji.top

echo "${#arr[@]}"
来源：http://jzb.ctjpmb.com

[R20] 关联数组（字典）
来源：http://vrk.mhx1999.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://zic.smart0.xyz

[R21] 字符串长度
来源：http://cmj.hcnkem.com

echo "${#s}"
来源：http://pns.chenjidiqi.icu

[R22] 截取子串
来源：http://sal.jiagoushi.top

echo "${s:0:5}"
来源：http://syg.zhaomingkeji.xyz

[R23] 字符串替换
来源：http://naq.ivvv.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://jvd.yonumen.top

[R24] 大小写转换
来源：http://kgz.wangdashe.top

echo "${s^^}"; echo "${s,,}"
来源：http://brt.cashguo.top

[R25] 去后缀 / 去前缀
来源：http://jzm.xinyue.icu

echo "${f%.txt}"; echo "${f#./}"
来源：http://mkg.wangshuangyany.cn

[R26] 命令替换
来源：http://fkm.chenjidiqi.icu

now=$(date +%F); echo "$now"
来源：http://gqi.gzhubu.top

[R27] 算术展开
来源：http://wab.zhijiandao.cn

echo $((1 + 2 * 3))
来源：http://jfk.cqqwz.cn

[R28] 浮点运算
来源：http://iva.redwolf501.top

echo "scale=2; 10/3" | bc
来源：http://myu.shuidangran.top

[R29] 定义函数
来源：http://rie.hammf.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://xse.yfazqb.com

[R30] 函数返回状态码
来源：http://zrf.cashguo.top

f() { return 0; }; f || echo "失败了"
来源：http://zjp.zycfv.cn

[R31] 局部变量
来源：http://gra.sweek.top

f() { local x=1; echo "$x"; }
来源：http://jhl.yj202588.top

[R32] 参数个数校验
来源：http://nom.jyoumei.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wue.hesvh.cn

[R33] 捕获错误并提示行号
来源：http://opp.guowangkeji.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://bpr.aibaodan.cn

[R34] 退出时清理
来源：http://mgz.yj20258888.top

trap 'rm -f "$tmp"' EXIT
来源：http://iou.jlsjyb.cn

[R35] 后台执行并等待
来源：http://oah.snrcjt.cn


<!-- 参考信息 -->