代发 wailian999

PHP:  // 手写时间戳比较
来源：http://sji.52xcode.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yvj.iojbl.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wyk.shanyushiyangtech.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://uzv.wangdashe.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://clf.yueranfly.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://plp.nanxuanxn.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://cyg.shuidangran.top

[P08] 处理浮点精度问题
来源：http://vrh.tarul.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wiw.daxiang520.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://zvp.cashguo.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://zdo.jinyuanbaomall.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://zia.svipenyu.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://nuw.chenlongwang.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://znm.haohaochexian.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://dpu.shuidangran.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://gik.yj20258.top

================================================================================
来源：http://dia.wangshuangyany.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://lii.iojbl.cn

================================================================================
来源：http://uei.ppjwa.cn

[Q01] 创建表
来源：http://sxi.gzhubu.top

CREATE TABLE users (
来源：http://ipg.yj20258.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mkp.ctjpmb.com

name VARCHAR(50) NOT NULL,
来源：http://ccd.hysaishi.cn

email VARCHAR(100) UNIQUE,
来源：http://kvk.xuetiantiany.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mkd.redwolf501.top

);
来源：http://ugb.bbcook.cn

[Q02] 创建带外键的表
来源：http://xey.yueranfly.top

CREATE TABLE orders (
来源：http://poy.bbcook.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://dcq.ydjk.org.cn

user_id INT NOT NULL,
来源：http://foq.yueranfly.top

amount DECIMAL(10, 2),
来源：http://nef.shanyushiyangkeji.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ogi.hywenlv.cn

);
来源：http://oxn.jqgfzy.top

[Q03] 增加列
来源：http://hvc.ywan-chungtsiang.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://nup.shanyushiyangkeji.top

[Q04] 修改列类型
来源：http://llg.xylfe.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://oqw.yongpay.top

[Q05] 重命名列
来源：http://zjo.sufxvd.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://niy.gzhubu.top

[Q06] 删除列
来源：http://bmd.shzxlz.cn

ALTER TABLE users DROP COLUMN age;
来源：http://oys.havefunace.top

[Q07] 删除表
来源：http://yaz.zhaomingkeji.xyz

DROP TABLE IF EXISTS orders;
来源：http://gfm.haohaochexian.top

[Q08] 创建普通索引
来源：http://qdb.tanke756.top

CREATE INDEX idx_users_email ON users(email);
来源：http://tsh.tian-w.cn

[Q09] 创建唯一索引
来源：http://kdu.aibaodan.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://rsw.epnwcf.com

[Q10] 插入单行
来源：http://clr.tanke756.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://tmn.cashguo.top

[Q11] 一次插入多行
来源：http://uvs.bjfxy.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mdm.uphjek.com

[Q12] 插入后取自增 ID
来源：http://fxe.sweek.top

INSERT INTO users (name) VALUES ('C');
来源：http://oxk.zhiwuduotai.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://yun.pycfn.com

[Q13] 忽略重复插入
来源：http://wrg.cheryme.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ycg.ybcxt.top

[Q14] 存在则更新（upsert）
来源：http://hns.gzhubu.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://pib.hfpthk.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://fum.shangyingyoupin.top

[Q15] 查询全部
来源：http://sxa.zhaomingkeji.xyz

SELECT * FROM users;
来源：http://bss.daxiang520.top

[Q16] 查询指定列
来源：http://tni.yvedp.cn

SELECT id, name FROM users;
来源：http://pqn.hesvh.cn

[Q17] 条件查询
来源：http://qoz.aizwys.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ljg.andypj.xyz

[Q18] 模糊匹配
来源：http://njd.ydzc1.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://vct.feifeiyinyue.top

[Q19] 范围查询
来源：http://vqi.dianchejie.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://tnu.shanyushiyangkeji.top

[Q20] IN 列表
来源：http://lem.cucudq.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://lac.tanke756.top

[Q21] 空值判断
来源：http://ibo.tarul.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://tup.sjlbkw.cn

[Q22] 排序
来源：http://mqw.jinqigfzy.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://xeh.ydjk.org.cn

[Q23] 分页
来源：http://vyx.aizwys.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://kom.mhx1999.top

[Q24] 去重
来源：http://zsn.jqgfzy.top

SELECT DISTINCT city FROM users;
来源：http://mda.jlsjyb.cn

[Q25] 只取前 N 条
来源：http://spn.zhongyouzk.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mpv.hfpthk.cn

[Q26] 计数
来源：http://nub.yongpay.top

SELECT COUNT(*) FROM users;
来源：http://joh.andypj.xyz

[Q27] 条件计数
来源：http://hgi.52xcode.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://kak.chenzaomai.com

[Q28] 求和与平均
来源：http://cnp.vqdsnc.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://peo.xylfe.cn

[Q29] 最大最小值
来源：http://gfj.smart0.xyz

SELECT MAX(age), MIN(age) FROM users;
来源：http://iwn.xziqi.cn

[Q30] 分组统计
来源：http://zay.bbcook.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://vsm.snrcjt.cn

[Q31] 分组后过滤
来源：http://lil.shanyushiyangtech.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://kij.daria6918.cn

[Q32] 分组拼接字符串
来源：http://qtu.hnqzz.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hnb.zhongyouzk.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://rrh.wangdashe.top

[Q33] 多列分组
来源：http://fal.hnqzz.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://qgs.nwbrower.top

[Q34] 每组取第一条
来源：http://lzc.zdqjudy.top

SELECT * FROM (
来源：http://llv.dianchejie.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://yfj.shuidangran.top

) t WHERE rn = 1;
来源：http://amk.hcnkem.com

[Q35] 内连接
来源：http://biw.svipenyu.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://jei.zhixingplan.top

[Q36] 左连接
来源：http://eyp.fanxiaobao.xyz

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://nqf.ydzc1.top

[Q37] 右连接
来源：http://myb.vqdsnc.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://glb.aizwys.cn

[Q38] 全外连接（PostgreSQL）
来源：http://nuw.fengsongda.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://rif.meibo888.top

[Q39] 自连接（查上下级）
来源：http://adf.daria6918.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ryw.zycfv.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://dyp.mhx1999.top

[Q40] 交叉连接（笛卡尔积）
来源：http://wwb.cucudq.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://zbv.andypj.xyz

[Q41] 多表连接
来源：http://iif.fzhhl.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://aqi.ybcxt.top

JOIN users u ON u.id = o.user_id
来源：http://hyg.snrcjt.cn

JOIN products p ON p.id = o.product_id;
来源：http://uzz.gaohongyu789.top

[Q42] 连接条件附加过滤
来源：http://ztf.yangfankeji.com

SELECT u.name, o.amount FROM users u
来源：http://gwo.jianghu66.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://kzh.feifeiyinyue.top

[Q43] 标量子查询
来源：http://qdh.smart0.xyz

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://teb.chenjidiqi.icu

[Q44] IN 子查询
来源：http://zng.zdqjudy.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://xpt.uphjek.com

[Q45] EXISTS 判断存在
来源：http://spv.chenzaomai.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://pwz.bjfxy.top

[Q46] NOT EXISTS 判断不存在
来源：http://zyd.chenlongwang.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://inj.zhengqikj.top

[Q47] 与平均值比较
来源：http://ppg.hcnkem.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://fht.vehdjk.com

[Q48] CTE 公用表表达式
来源：http://cin.gaohongyu789.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mon.ydzc1.top

SELECT * FROM t WHERE c > 5;
来源：http://hmf.jqgfzy.top

[Q49] 更新单行
来源：http://uol.sweek.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://vzp.iojbl.cn

[Q50] 批量更新
来源：http://wfr.fktsv.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://pfe.xziqi.cn

[Q51] 用子查询更新
来源：http://xeg.quarkkingdee.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://xyp.ehwqpu.com

[Q52] 删除指定行
来源：http://izp.meibo888.top

DELETE FROM users WHERE id = 10;
来源：http://lqf.chenlongwang.top

[Q53] 按条件删除
来源：http://rum.shanyushiyangtech.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://caw.epnwcf.com

[Q54] 清空表
来源：http://vnb.hnxiangtu.top

TRUNCATE TABLE logs;
来源：http://pkd.jlsjyb.cn

[Q55] 排名（并列占位）
来源：http://spq.hesvh.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://fvj.yanxiufei.cn

[Q56] 密集排名（并列不占位）
来源：http://fdf.cheryme.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://gvc.zycfv.cn

[Q57] 行号
来源：http://way.sjlbkw.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wle.fktsv.cn

[Q58] 累计求和
来源：http://cqh.ehwqpu.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://zos.tianlin.xyz

[Q59] 分组内累计
来源：http://rbs.mhx1999.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://zlu.zhixingplan.top

[Q60] 取上一行 / 下一行
来源：http://put.0kj1m.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hpc.bjfxy.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://syg.yongpay.top

[Q61] 移动平均
来源：http://psh.hammf.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://egn.yongpay.top

[Q62] 分组占比
来源：http://ifx.shanyushiyangkeji.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://zow.gogol.net.cn

[Q63] 开启事务
来源：http://pmk.cashguo.top

START TRANSACTION;                -- 或 BEGIN
来源：http://tkr.fehbvm.com

[Q64] 提交事务
来源：http://rpg.meibo888.top

COMMIT;
来源：http://wsv.chenjidiqi.icu

[Q65] 回滚事务
来源：http://cra.pengpengdd.cyou

ROLLBACK;
来源：http://ioi.epnwcf.com

[Q66] 行锁查询
来源：http://ngg.nanxinkj.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://gma.sufxvd.cn

[Q67] 设置隔离级别
来源：http://ecf.jinghuilouyu.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://lhy.mhx1999.top

[Q68] 保存点
来源：http://ell.hesvh.cn

SAVEPOINT sp1;
来源：http://emj.shanyushiyangkeji.top

ROLLBACK TO sp1;
来源：http://zhj.yongpay.top

[Q69] 查看执行计划
来源：http://sri.sxryk.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://vml.zdbjq.cn

[Q70] 更新统计信息
来源：http://nhh.uphjek.com

ANALYZE TABLE users;
来源：http://hlo.0kj1m.cn

[Q71] 查看建表语句
来源：http://zzr.yj202588.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mhs.zhaomingkeji.xyz

[Q72] 查看索引
来源：http://gyk.shangyingyoupin.top

SHOW INDEX FROM users;
来源：http://vtv.hammf.cn

[Q73] 查看表状态
来源：http://ute.tanke756.top

SHOW TABLE STATUS LIKE 'users';
来源：http://rig.tianlin.xyz

[Q74] 强制使用索引
来源：http://cnl.jinqigfzy.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ezm.hammf.cn

[Q75] 日期格式化
来源：http://uvd.0kj1m.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://vqu.zhengqikj.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://frg.birdmap.top

[Q76] 按天统计
来源：http://oik.smart0.xyz

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://qnb.hesvh.cn

[Q77] 时间加减
来源：http://vlp.yangfankeji.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://lxb.jinqigfzy.top

[Q78] 当前时间
来源：http://hvs.shangyingyoupin.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wax.ppjwa.cn

[Q79] 字符串拼接
来源：http://rtb.cheryme.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://bku.sxryk.cn

[Q80] 字符串截取
来源：http://ndw.bjfxy.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wtb.cucudq.cn

[Q81] 字符串替换
来源：http://wft.nanxinkj.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://yyd.hongshengwenyu.top

[Q82] 字符长度与字节长度
来源：http://ywe.shanyushiyangtech.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://jlp.zhixingplan.top

[Q83] 大小写转换
来源：http://ygw.zhengqikj.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://rfe.jlsjyb.cn

[Q84] 去除首尾空格
来源：http://qlr.zhengqikj.top

SELECT TRIM(name) FROM users;
来源：http://ayj.ctjpmb.com

[Q85] 数值取整
来源：http://zbc.gogol.net.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ndz.jinqigfzy.top

[Q86] 读取 JSON 字段
来源：http://vej.yueranfly.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://eni.kuanghao11.cn

[Q87] JSON 字段做条件
来源：http://myt.jinyuanbaomall.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ztv.guannengcc.top

[Q88] 行转列（条件聚合）
来源：http://ewj.meibo888.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ibi.xingfuxueyuan.xyz

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://bes.sweek.top

[Q89] 判断表是否存在
来源：http://ajg.xylfe.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://xmx.hammf.cn

[Q90] 生成序号列
来源：http://zqu.yonumen.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://xwn.cdnleiting.top

================================================================================
来源：http://ylz.mhx1999.top

R. Bash 专题
来源：http://xxg.yj202588.top

================================================================================
来源：http://rvf.shangyingyoupin.top

[R01] shebang 与严格模式
来源：http://qlz.gaohongyu789.top

#!/usr/bin/env bash
来源：http://gud.zdbjq.cn

set -euo pipefail
来源：http://fgh.bjfxy.top

[R02] 变量赋值与使用
来源：http://ehz.xingfuxueyuan.xyz

name="Tom"; echo "$name"
来源：http://ggu.gotoacloud.top

[R03] 只读变量
来源：http://fpd.jinqigfzy.top

readonly PI=3.14
来源：http://qpe.hysaishi.cn

[R04] 位置参数
来源：http://osy.fzhhl.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://xmw.cashguo.top

[R05] 参数默认值
来源：http://hnd.zdbjq.cn

name="${1:-default}"
来源：http://rsl.yongpay.top

[R06] 判断命令是否存在
来源：http://bbu.jinqigufen.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://jhq.xingfuxueyuan.xyz

[R07] if 判断文件
来源：http://agg.birdmap.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://tux.shangyingyoupin.top

[R08] 数值比较
来源：http://tir.haohaochexian.top

if (( a > b )); then echo "a 更大"; fi
来源：http://mqh.gotoacloud.top

[R09] 字符串比较
来源：http://qpk.gzhubu.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ybv.zhongyouzk.top

[R10] 正则匹配
来源：http://nip.yuxming.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://pxy.havefunace.top

[R11] case 多分支
来源：http://xfd.ppjwa.cn

case "$1" in
来源：http://tak.svipenyu.cn

start) echo "启动" ;;
来源：http://ipd.pengpengdd.cyou

stop)  echo "停止" ;;
来源：http://rlm.hammf.cn

*)     echo "未知命令" ;;
来源：http://jde.hesvh.cn

esac
来源：http://ejt.guannengcc.top

[R12] for 遍历文件
来源：http://hgg.0kj1m.cn

for f in *.txt; do echo "$f"; done
来源：http://dsn.kuanghao11.cn

[R13] for 计数循环
来源：http://igw.xuanzx.com

for i in {1..10}; do echo "$i"; done
来源：http://hhv.ctjpmb.com

[R14] C 风格 for
来源：http://fbf.hongshengwenyu.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://axj.dianchejie.cn

[R15] while 逐行读文件
来源：http://cpu.yj202588.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hif.chenzaomai.com

[R16] until 等待条件
来源：http://awc.redwolf501.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://pry.yonumen.top

[R17] 数组定义与取值
来源：http://idk.shzxlz.cn

arr=(a b c); echo "${arr[0]}"
来源：http://vbd.daria6918.cn

[R18] 遍历数组
来源：http://fxx.xuanzx.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://tcx.gotoacloud.top

[R19] 数组长度
来源：http://rxg.shuidangran.top

echo "${#arr[@]}"
来源：http://qxp.cqqwz.cn

[R20] 关联数组（字典）
来源：http://bhl.nwbrower.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://unl.hysaishi.cn

[R21] 字符串长度
来源：http://jkj.wangshuangyany.cn

echo "${#s}"
来源：http://zhk.jiagoushi.top

[R22] 截取子串
来源：http://ywz.hywenlv.cn

echo "${s:0:5}"
来源：http://bml.cucudq.cn

[R23] 字符串替换
来源：http://tdi.svipenyu.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://nmo.tanke756.top

[R24] 大小写转换
来源：http://mar.andypj.xyz

echo "${s^^}"; echo "${s,,}"
来源：http://jea.nanxuanxn.top

[R25] 去后缀 / 去前缀
来源：http://szt.gogol.net.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://rqu.c1oappe.top

[R26] 命令替换
来源：http://luc.xingfuxueyuan.xyz

now=$(date +%F); echo "$now"
来源：http://kir.hysaishi.cn

[R27] 算术展开
来源：http://wec.nanxinkj.top

echo $((1 + 2 * 3))
来源：http://iof.hfpthk.cn

[R28] 浮点运算
来源：http://jtx.yangfankeji.com

echo "scale=2; 10/3" | bc
来源：http://kci.yj202588.top

[R29] 定义函数
来源：http://kka.fanxiaobao.xyz

add() { echo $(($1 + $2)); }; add 1 2
来源：http://tcn.jinyuanbaomall.cn

[R30] 函数返回状态码
来源：http://oxo.daria6918.cn

f() { return 0; }; f || echo "失败了"
来源：http://hgr.pycfn.com

[R31] 局部变量
来源：http://wkq.meibo888.top

f() { local x=1; echo "$x"; }
来源：http://opr.shanyushiyangtech.top

[R32] 参数个数校验
来源：http://zoq.uphjek.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://okq.zhijiandao.cn

[R33] 捕获错误并提示行号
来源：http://qdk.shanyushiyangtech.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://xyx.dashuyun.cn

[R34] 退出时清理
来源：http://tyj.guowangkeji.top

trap 'rm -f "$tmp"' EXIT
来源：http://gik.bbcook.cn

[R35] 后台执行并等待
来源：http://azh.quarkkingdee.top


<!-- 参考信息 -->