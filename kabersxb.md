代发 wailian999

PHP:  // 手写时间戳比较
来源：http://cpr.xylfe.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jrr.yangfankeji.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tam.zhixingplan.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mix.vqdsnc.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://moa.sweek.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://pfi.ehwqpu.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://noy.andypj.xyz

[P08] 处理浮点精度问题
来源：http://fik.guannengcc.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://sfg.vqdsnc.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://rsg.pengpengdd.cyou

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wau.gogol.net.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mbc.andypj.xyz

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://kty.yuxming.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wvn.hnxiangtu.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://vlr.gzhubu.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://zpr.yuxming.cn

================================================================================
来源：http://sef.hnqzz.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://kgo.yueranfly.top

================================================================================
来源：http://der.sxryk.cn

[Q01] 创建表
来源：http://fjd.gaohongyu789.top

CREATE TABLE users (
来源：http://xgb.xingfuxueyuan.xyz

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://oxk.tarul.cn

name VARCHAR(50) NOT NULL,
来源：http://hbv.guowangkeji.top

email VARCHAR(100) UNIQUE,
来源：http://kph.bbcook.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://uxi.yvedp.cn

);
来源：http://gcn.redwolf501.top

[Q02] 创建带外键的表
来源：http://vqf.zhaomingkeji.xyz

CREATE TABLE orders (
来源：http://pca.yongpay.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://tle.xuanzx.com

user_id INT NOT NULL,
来源：http://bij.tian-w.cn

amount DECIMAL(10, 2),
来源：http://gex.cheryme.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wth.jqgfzy.top

);
来源：http://iyg.yj202588.top

[Q03] 增加列
来源：http://uto.wangdashe.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mgd.jinghuilouyu.cn

[Q04] 修改列类型
来源：http://lly.zdqjudy.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://fwr.bbcook.cn

[Q05] 重命名列
来源：http://zyb.mhx1999.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://gao.yj20258.top

[Q06] 删除列
来源：http://buh.jinqigufen.top

ALTER TABLE users DROP COLUMN age;
来源：http://ilj.guowangkeji.top

[Q07] 删除表
来源：http://rug.zhijiandao.cn

DROP TABLE IF EXISTS orders;
来源：http://sct.xuetiantiany.cn

[Q08] 创建普通索引
来源：http://znz.gaohongyu789.top

CREATE INDEX idx_users_email ON users(email);
来源：http://avx.zhiwuduotai.top

[Q09] 创建唯一索引
来源：http://bow.andypj.xyz

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mrg.0kj1m.cn

[Q10] 插入单行
来源：http://qvs.jinqigfzy.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://kpb.sjlbkw.cn

[Q11] 一次插入多行
来源：http://zwb.fktsv.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://zny.uphjek.com

[Q12] 插入后取自增 ID
来源：http://bqn.wangdashe.top

INSERT INTO users (name) VALUES ('C');
来源：http://wbf.52xcode.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://sin.hnxiangtu.top

[Q13] 忽略重复插入
来源：http://bgu.xinyue.icu

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ucf.zhijiandao.cn

[Q14] 存在则更新（upsert）
来源：http://uiw.xingfuxueyuan.xyz

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://dep.jiagoushi.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://uda.kuanghao11.cn

[Q15] 查询全部
来源：http://yhi.vqdsnc.cn

SELECT * FROM users;
来源：http://wkd.316326.xyz

[Q16] 查询指定列
来源：http://lgo.ppjwa.cn

SELECT id, name FROM users;
来源：http://sfw.snrcjt.cn

[Q17] 条件查询
来源：http://nio.jqgufenzy.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://kda.yj20258888.top

[Q18] 模糊匹配
来源：http://mtz.0kj1m.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://uec.hcnkem.com

[Q19] 范围查询
来源：http://kwa.xylfe.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://lfb.zhiwuduotai.top

[Q20] IN 列表
来源：http://qjx.shanyushiyangkeji.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://qdm.zhongyouzk.top

[Q21] 空值判断
来源：http://teq.svipenyu.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://bwo.cqqwz.cn

[Q22] 排序
来源：http://leg.fzhhl.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://aul.sjlbkw.cn

[Q23] 分页
来源：http://vdu.ydzc1.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ori.yfazqb.com

[Q24] 去重
来源：http://anr.redwolf501.top

SELECT DISTINCT city FROM users;
来源：http://ioh.shanyushiyangtech.top

[Q25] 只取前 N 条
来源：http://rmt.yuxming.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://uek.xinyue.icu

[Q26] 计数
来源：http://gkg.mhx1999.top

SELECT COUNT(*) FROM users;
来源：http://jum.xylfe.cn

[Q27] 条件计数
来源：http://kpb.cheryme.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://oov.havefunace.top

[Q28] 求和与平均
来源：http://ixz.xziqi.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://zyh.yonumen.top

[Q29] 最大最小值
来源：http://niz.vehdjk.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://seq.chenlongwang.top

[Q30] 分组统计
来源：http://mfq.gzhubu.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ceu.iojbl.cn

[Q31] 分组后过滤
来源：http://mmz.epnwcf.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ipe.52xcode.cn

[Q32] 分组拼接字符串
来源：http://dol.yfazqb.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://dia.cqqwz.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ggh.zdqjudy.top

[Q33] 多列分组
来源：http://klt.zdbjq.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://loh.ppjwa.cn

[Q34] 每组取第一条
来源：http://prb.ydzc1.top

SELECT * FROM (
来源：http://awa.hfpthk.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://yiu.svipenyu.cn

) t WHERE rn = 1;
来源：http://wri.zhengqikj.top

[Q35] 内连接
来源：http://uqc.iojbl.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ucm.redwolf501.top

[Q36] 左连接
来源：http://cfc.hnqzz.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://qln.ydzc1.top

[Q37] 右连接
来源：http://qle.redwolf501.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ryi.birdmap.top

[Q38] 全外连接（PostgreSQL）
来源：http://ehg.yongpay.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://zcl.hysaishi.cn

[Q39] 自连接（查上下级）
来源：http://emw.uphjek.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://jqs.aizwys.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wiq.havefunace.top

[Q40] 交叉连接（笛卡尔积）
来源：http://fij.jinghuilouyu.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://rzg.birdmap.top

[Q41] 多表连接
来源：http://uvc.tianlin.xyz

SELECT o.id, u.name, p.title FROM orders o
来源：http://ikf.shanyushiyangkeji.top

JOIN users u ON u.id = o.user_id
来源：http://uqk.zdbjq.cn

JOIN products p ON p.id = o.product_id;
来源：http://luu.shuidangran.top

[Q42] 连接条件附加过滤
来源：http://iik.hnqzz.top

SELECT u.name, o.amount FROM users u
来源：http://csu.ydzc1.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ehh.nwbrower.top

[Q43] 标量子查询
来源：http://jgd.jinghuilouyu.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://rmm.hysaishi.cn

[Q44] IN 子查询
来源：http://zyv.zhongyouzk.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://syq.fanxiaobao.xyz

[Q45] EXISTS 判断存在
来源：http://gyz.shuidangran.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://twx.fzhhl.top

[Q46] NOT EXISTS 判断不存在
来源：http://oxg.c1oappe.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://grv.sysykeji.top

[Q47] 与平均值比较
来源：http://tyx.yangfankeji.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ung.gzhubu.top

[Q48] CTE 公用表表达式
来源：http://fbn.jianghu66.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://puw.yj202588.top

SELECT * FROM t WHERE c > 5;
来源：http://lou.hesvh.cn

[Q49] 更新单行
来源：http://pmz.epnwcf.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://xfl.hysaishi.cn

[Q50] 批量更新
来源：http://ygf.uphjek.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://pfv.shuidangran.top

[Q51] 用子查询更新
来源：http://wro.316326.xyz

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://qds.svipenyu.cn

[Q52] 删除指定行
来源：http://lbd.hfpthk.cn

DELETE FROM users WHERE id = 10;
来源：http://lzy.yueranfly.top

[Q53] 按条件删除
来源：http://rgr.yj20258.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://zdp.gzhubu.top

[Q54] 清空表
来源：http://dat.snrcjt.cn

TRUNCATE TABLE logs;
来源：http://cig.zhoulong.xyz

[Q55] 排名（并列占位）
来源：http://mhi.gzhubu.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://cgb.shanyushiyangtech.top

[Q56] 密集排名（并列不占位）
来源：http://pdc.zhengqikj.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ysi.svipenyu.cn

[Q57] 行号
来源：http://sdy.sufxvd.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://nbm.aibaodan.cn

[Q58] 累计求和
来源：http://noj.sufxvd.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://owb.mhx1999.top

[Q59] 分组内累计
来源：http://dda.redwolf501.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://efx.yongpay.top

[Q60] 取上一行 / 下一行
来源：http://xkw.kuanghao11.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://eja.dianchejie.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://woc.yuxming.cn

[Q61] 移动平均
来源：http://lgl.shangyingyoupin.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://uhq.zhongyouzk.top

[Q62] 分组占比
来源：http://rsa.zycfv.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://lqx.aibaodan.cn

[Q63] 开启事务
来源：http://dii.dianchejie.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://gwn.hysaishi.cn

[Q64] 提交事务
来源：http://gth.tian-w.cn

COMMIT;
来源：http://qua.sxryk.cn

[Q65] 回滚事务
来源：http://rvk.xylfe.cn

ROLLBACK;
来源：http://voh.hcnkem.com

[Q66] 行锁查询
来源：http://ljt.yj202588.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://oud.havefunace.top

[Q67] 设置隔离级别
来源：http://ept.cheryme.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://nqg.shanyushiyangtech.top

[Q68] 保存点
来源：http://mrc.jiagoushi.top

SAVEPOINT sp1;
来源：http://tlg.snrcjt.cn

ROLLBACK TO sp1;
来源：http://ppu.cdnleiting.top

[Q69] 查看执行计划
来源：http://kyc.xuanzx.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ozh.sysykeji.top

[Q70] 更新统计信息
来源：http://iuo.tanke756.top

ANALYZE TABLE users;
来源：http://riv.yangfankeji.com

[Q71] 查看建表语句
来源：http://fvv.daxiang520.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://byh.gzhubu.top

[Q72] 查看索引
来源：http://amw.gzhubu.top

SHOW INDEX FROM users;
来源：http://dgb.mhx1999.top

[Q73] 查看表状态
来源：http://smu.pengpengdd.cyou

SHOW TABLE STATUS LIKE 'users';
来源：http://mkw.zhiwuduotai.top

[Q74] 强制使用索引
来源：http://ggh.daria6918.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ioa.jinghuilouyu.cn

[Q75] 日期格式化
来源：http://vqw.hysaishi.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ueh.yvedp.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://owv.kuanghao11.cn

[Q76] 按天统计
来源：http://qss.chenlongwang.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://uiy.yongpay.top

[Q77] 时间加减
来源：http://ama.nanxuanxn.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://jve.chenjidiqi.icu

[Q78] 当前时间
来源：http://bkh.yueranfly.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://vvg.fanxiaobao.xyz

[Q79] 字符串拼接
来源：http://dzs.hesvh.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://yns.tianlin.xyz

[Q80] 字符串截取
来源：http://rdw.zhijiandao.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://khn.xuanzx.com

[Q81] 字符串替换
来源：http://fhd.guannengcc.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://igd.fehbvm.com

[Q82] 字符长度与字节长度
来源：http://qbg.0kj1m.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ohn.jinyuanbaomall.cn

[Q83] 大小写转换
来源：http://fpf.yangfankeji.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://xyj.chenjidiqi.icu

[Q84] 去除首尾空格
来源：http://aoz.sjlbkw.cn

SELECT TRIM(name) FROM users;
来源：http://nos.quarkkingdee.top

[Q85] 数值取整
来源：http://mgm.jianghu66.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://khb.xylfe.cn

[Q86] 读取 JSON 字段
来源：http://bbl.yonumen.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://usn.sxryk.cn

[Q87] JSON 字段做条件
来源：http://oci.zhaomingkeji.xyz

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mge.zdbjq.cn

[Q88] 行转列（条件聚合）
来源：http://kue.iojbl.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://tig.zhiwuduotai.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://lhh.gzhubu.top

[Q89] 判断表是否存在
来源：http://zot.kuanghao11.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://utv.nanxuanxn.top

[Q90] 生成序号列
来源：http://gnx.jinghuilouyu.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://gft.hongshengwenyu.top

================================================================================
来源：http://lid.nanxuanxn.top

R. Bash 专题
来源：http://ugk.c1oappe.top

================================================================================
来源：http://her.dashuyun.cn

[R01] shebang 与严格模式
来源：http://dnr.dianchejie.cn

#!/usr/bin/env bash
来源：http://lcw.sweek.top

set -euo pipefail
来源：http://uiw.ppjwa.cn

[R02] 变量赋值与使用
来源：http://jpb.mhx1999.top

name="Tom"; echo "$name"
来源：http://bvq.xuetiantiany.cn

[R03] 只读变量
来源：http://xkn.yonumen.top

readonly PI=3.14
来源：http://nwh.xuetiantiany.cn

[R04] 位置参数
来源：http://lbo.jqgfzy.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://pjn.gzhubu.top

[R05] 参数默认值
来源：http://idl.gaohongyu789.top

name="${1:-default}"
来源：http://qdn.jinghuilouyu.cn

[R06] 判断命令是否存在
来源：http://kxf.hammf.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://cbv.jianghu66.top

[R07] if 判断文件
来源：http://pvr.tanke756.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://fny.ehwqpu.com

[R08] 数值比较
来源：http://ego.dianchejie.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://kue.hysaishi.cn

[R09] 字符串比较
来源：http://rkq.nanxuanxn.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://vem.guowangkeji.top

[R10] 正则匹配
来源：http://nme.sxryk.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://haz.vehdjk.com

[R11] case 多分支
来源：http://qsx.zhiwuduotai.top

case "$1" in
来源：http://ldd.shuidangran.top

start) echo "启动" ;;
来源：http://lbl.yuxming.cn

stop)  echo "停止" ;;
来源：http://vuo.yfazqb.com

*)     echo "未知命令" ;;
来源：http://lom.jinqigufen.top

esac
来源：http://zzs.aibaodan.cn

[R12] for 遍历文件
来源：http://bgw.birdmap.top

for f in *.txt; do echo "$f"; done
来源：http://qbz.fzhhl.top

[R13] for 计数循环
来源：http://wcn.chenzaomai.com

for i in {1..10}; do echo "$i"; done
来源：http://zqn.zdbjq.cn

[R14] C 风格 for
来源：http://nrd.bjfxy.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://gtm.sjlbkw.cn

[R15] while 逐行读文件
来源：http://tru.xylfe.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://twt.uphjek.com

[R16] until 等待条件
来源：http://pob.ehwqpu.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://qwu.jlsjyb.cn

[R17] 数组定义与取值
来源：http://qgu.fanxiaobao.xyz

arr=(a b c); echo "${arr[0]}"
来源：http://edj.dashuyun.cn

[R18] 遍历数组
来源：http://pne.yuxming.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ybi.jiagoushi.top

[R19] 数组长度
来源：http://ruh.cdnleiting.top

echo "${#arr[@]}"
来源：http://zdb.birdmap.top

[R20] 关联数组（字典）
来源：http://thj.jinghuilouyu.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://gxr.jianghu66.top

[R21] 字符串长度
来源：http://acb.hysaishi.cn

echo "${#s}"
来源：http://adi.feifeiyinyue.top

[R22] 截取子串
来源：http://lyx.sweek.top

echo "${s:0:5}"
来源：http://nsh.guannengcc.top

[R23] 字符串替换
来源：http://cht.shuidangran.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://bse.wangshuangyany.cn

[R24] 大小写转换
来源：http://fur.fanxiaobao.xyz

echo "${s^^}"; echo "${s,,}"
来源：http://mjz.gotoacloud.top

[R25] 去后缀 / 去前缀
来源：http://qtj.vehdjk.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://vvd.havefunace.top

[R26] 命令替换
来源：http://ufm.chenzaomai.com

now=$(date +%F); echo "$now"
来源：http://sdm.havefunace.top

[R27] 算术展开
来源：http://hxd.cashguo.top

echo $((1 + 2 * 3))
来源：http://rwz.bbcook.cn

[R28] 浮点运算
来源：http://vwo.vqdsnc.cn

echo "scale=2; 10/3" | bc
来源：http://otg.ydjk.org.cn

[R29] 定义函数
来源：http://obt.jianghu66.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mie.redwolf501.top

[R30] 函数返回状态码
来源：http://zdq.jlsjyb.cn

f() { return 0; }; f || echo "失败了"
来源：http://eot.sweek.top

[R31] 局部变量
来源：http://ngu.yanxiufei.cn

f() { local x=1; echo "$x"; }
来源：http://olb.xziqi.cn

[R32] 参数个数校验
来源：http://wgp.c1oappe.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://jam.sysykeji.top

[R33] 捕获错误并提示行号
来源：http://nxy.daria6918.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://gqv.gotoacloud.top

[R34] 退出时清理
来源：http://qqq.havefunace.top

trap 'rm -f "$tmp"' EXIT
来源：http://xkn.hongshengwenyu.top

[R35] 后台执行并等待
来源：http://gff.bbcook.cn


<!-- 参考信息 -->