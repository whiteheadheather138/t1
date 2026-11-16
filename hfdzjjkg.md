代发 wailian999

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hua.316326.xyz

Ruby: // 手写闭包 + Time.now 判断
来源：http://wcx.guannengcc.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ead.ctjpmb.com

[P08] 处理浮点精度问题
来源：http://uxz.aizwys.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mrq.sufxvd.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://bkv.yuxming.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://djv.zhongyouzk.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hvd.cdnleiting.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://fah.xuetiantiany.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://bnv.pycfn.com

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://xve.redwolf501.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://nlp.fanxiaobao.xyz

================================================================================
来源：http://qsi.pengpengdd.cyou

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hyt.bjfxy.top

================================================================================
来源：http://acp.ydzc1.top

[Q01] 创建表
来源：http://gio.daria6918.cn

CREATE TABLE users (
来源：http://eaw.ybcxt.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://vdv.fanxiaobao.xyz

name VARCHAR(50) NOT NULL,
来源：http://zuw.jqgufenzy.top

email VARCHAR(100) UNIQUE,
来源：http://dei.zhijiandao.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://nze.uphjek.com

);
来源：http://pzd.ydzc1.top

[Q02] 创建带外键的表
来源：http://tem.ybcxt.top

CREATE TABLE orders (
来源：http://cqy.nanxuanxn.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ppw.chenzaomai.com

user_id INT NOT NULL,
来源：http://bux.pengpengdd.cyou

amount DECIMAL(10, 2),
来源：http://rwx.sysykeji.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://uie.yongpay.top

);
来源：http://dwz.yonumen.top

[Q03] 增加列
来源：http://pbv.gaohongyu789.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://pwp.meibo888.top

[Q04] 修改列类型
来源：http://sjc.zycfv.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://aat.pengpengdd.cyou

[Q05] 重命名列
来源：http://njy.shanyushiyangkeji.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://cvm.yfazqb.com

[Q06] 删除列
来源：http://vqs.uphjek.com

ALTER TABLE users DROP COLUMN age;
来源：http://yox.ywan-chungtsiang.top

[Q07] 删除表
来源：http://dhi.fanxiaobao.xyz

DROP TABLE IF EXISTS orders;
来源：http://lwp.sysykeji.top

[Q08] 创建普通索引
来源：http://lkc.zhongyouzk.top

CREATE INDEX idx_users_email ON users(email);
来源：http://muj.jinyuanbaomall.cn

[Q09] 创建唯一索引
来源：http://xcj.jqgfzy.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://gkp.xuanzx.com

[Q10] 插入单行
来源：http://ieu.ybcxt.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hxa.haohaochexian.top

[Q11] 一次插入多行
来源：http://yck.52xcode.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://gev.xingfuxueyuan.xyz

[Q12] 插入后取自增 ID
来源：http://pwa.yvedp.cn

INSERT INTO users (name) VALUES ('C');
来源：http://pmi.yfazqb.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://gyl.zhaomingkeji.xyz

[Q13] 忽略重复插入
来源：http://vpc.zhaomingkeji.xyz

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://fra.jinqigufen.top

[Q14] 存在则更新（upsert）
来源：http://ouf.sjlbkw.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://lbn.gogol.net.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://kjk.vqdsnc.cn

[Q15] 查询全部
来源：http://tdw.yj20258888.top

SELECT * FROM users;
来源：http://zav.zhijiandao.cn

[Q16] 查询指定列
来源：http://wag.sxryk.cn

SELECT id, name FROM users;
来源：http://tfi.daxiang520.top

[Q17] 条件查询
来源：http://zkj.svipenyu.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://dni.nanxinkj.top

[Q18] 模糊匹配
来源：http://epj.xuetiantiany.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ddp.xuanzx.com

[Q19] 范围查询
来源：http://ghn.hongshengwenyu.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://vwt.yj20258.top

[Q20] IN 列表
来源：http://ane.hammf.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://tuy.shanyushiyangtech.top

[Q21] 空值判断
来源：http://hnn.snrcjt.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://bsh.sysykeji.top

[Q22] 排序
来源：http://lak.52xcode.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://zki.52xcode.cn

[Q23] 分页
来源：http://yum.xuetiantiany.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://xow.zhixingplan.top

[Q24] 去重
来源：http://mqs.sysykeji.top

SELECT DISTINCT city FROM users;
来源：http://htz.jyoumei.cn

[Q25] 只取前 N 条
来源：http://tce.zhongyouzk.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://yuy.shangyingyoupin.top

[Q26] 计数
来源：http://ajl.yonumen.top

SELECT COUNT(*) FROM users;
来源：http://rfi.yj202588.top

[Q27] 条件计数
来源：http://yoe.bjfxy.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ult.zhaomingkeji.xyz

[Q28] 求和与平均
来源：http://bck.gzhubu.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wzp.0kj1m.cn

[Q29] 最大最小值
来源：http://hqv.svipenyu.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://amu.iojbl.cn

[Q30] 分组统计
来源：http://grz.hysaishi.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ixq.dianchejie.cn

[Q31] 分组后过滤
来源：http://wfl.yj20258888.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://dcf.iojbl.cn

[Q32] 分组拼接字符串
来源：http://qny.daria6918.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://qzo.daria6918.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://dyd.fehbvm.com

[Q33] 多列分组
来源：http://spn.jinqigufen.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://zxn.chenzaomai.com

[Q34] 每组取第一条
来源：http://fbo.tanke756.top

SELECT * FROM (
来源：http://usw.zhongyouzk.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://gqr.yanxiufei.cn

) t WHERE rn = 1;
来源：http://bmm.snrcjt.cn

[Q35] 内连接
来源：http://chz.hesvh.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://cvh.hongshengwenyu.top

[Q36] 左连接
来源：http://slk.yuanzhike.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://rng.52xcode.cn

[Q37] 右连接
来源：http://jbo.chenzaomai.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ttm.haohaochexian.top

[Q38] 全外连接（PostgreSQL）
来源：http://xoh.shanyushiyangkeji.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://rem.yueranfly.top

[Q39] 自连接（查上下级）
来源：http://hzb.ydzc1.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://rvm.hammf.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://nse.jlsjyb.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://lbg.ybcxt.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://bec.hesvh.cn

[Q41] 多表连接
来源：http://oiq.gotoacloud.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://ftp.gotoacloud.top

JOIN users u ON u.id = o.user_id
来源：http://yjs.vehdjk.com

JOIN products p ON p.id = o.product_id;
来源：http://kou.uphjek.com

[Q42] 连接条件附加过滤
来源：http://evn.cucudq.cn

SELECT u.name, o.amount FROM users u
来源：http://oei.daria6918.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ywp.tianlin.xyz

[Q43] 标量子查询
来源：http://sdv.jlsjyb.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://raw.tianlin.xyz

[Q44] IN 子查询
来源：http://xnr.tian-w.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://vhd.cucudq.cn

[Q45] EXISTS 判断存在
来源：http://ani.quarkkingdee.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mfs.vehdjk.com

[Q46] NOT EXISTS 判断不存在
来源：http://pqq.yonumen.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bis.birdmap.top

[Q47] 与平均值比较
来源：http://tgu.shangyingyoupin.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://xck.hammf.cn

[Q48] CTE 公用表表达式
来源：http://lbu.aizwys.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://zyt.ydjk.org.cn

SELECT * FROM t WHERE c > 5;
来源：http://qmm.fanxiaobao.xyz

[Q49] 更新单行
来源：http://bpi.jianghu66.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://vah.redwolf501.top

[Q50] 批量更新
来源：http://gft.nwbrower.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wrw.ppjwa.cn

[Q51] 用子查询更新
来源：http://bzz.cdnleiting.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://fty.quarkkingdee.top

[Q52] 删除指定行
来源：http://npp.mhx1999.top

DELETE FROM users WHERE id = 10;
来源：http://omg.zhiwuduotai.top

[Q53] 按条件删除
来源：http://faa.ydjk.org.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://veu.zycfv.cn

[Q54] 清空表
来源：http://mjz.fzhhl.top

TRUNCATE TABLE logs;
来源：http://hwh.yuxming.cn

[Q55] 排名（并列占位）
来源：http://pca.bbcook.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://lsb.tanke756.top

[Q56] 密集排名（并列不占位）
来源：http://zlq.haohaochexian.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://pgm.fehbvm.com

[Q57] 行号
来源：http://ifd.shanyushiyangtech.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://twy.zhijiandao.cn

[Q58] 累计求和
来源：http://rds.hongshengwenyu.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://den.sysykeji.top

[Q59] 分组内累计
来源：http://lru.xziqi.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://bqu.shanyushiyangkeji.top

[Q60] 取上一行 / 下一行
来源：http://tyx.shanyushiyangtech.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://onm.chenzaomai.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://dlk.cashguo.top

[Q61] 移动平均
来源：http://yjj.tian-w.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://dqv.iojbl.cn

[Q62] 分组占比
来源：http://ouk.gotoacloud.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://bmb.jlsjyb.cn

[Q63] 开启事务
来源：http://pwi.cqqwz.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://vlu.zhongyouzk.top

[Q64] 提交事务
来源：http://ria.mhx1999.top

COMMIT;
来源：http://yqj.gogol.net.cn

[Q65] 回滚事务
来源：http://oan.svipenyu.cn

ROLLBACK;
来源：http://vwg.hnqzz.top

[Q66] 行锁查询
来源：http://kmg.shanyushiyangkeji.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ifa.zdqjudy.top

[Q67] 设置隔离级别
来源：http://lcd.nwbrower.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://qpa.zhiwuduotai.top

[Q68] 保存点
来源：http://xve.feifeiyinyue.top

SAVEPOINT sp1;
来源：http://bfp.pycfn.com

ROLLBACK TO sp1;
来源：http://ggy.shuidangran.top

[Q69] 查看执行计划
来源：http://zsk.fktsv.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wdw.bjfxy.top

[Q70] 更新统计信息
来源：http://msh.yj20258.top

ANALYZE TABLE users;
来源：http://rkd.hammf.cn

[Q71] 查看建表语句
来源：http://ylc.hesvh.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://oyg.52xcode.cn

[Q72] 查看索引
来源：http://sic.bbcook.cn

SHOW INDEX FROM users;
来源：http://kla.yvedp.cn

[Q73] 查看表状态
来源：http://fop.guannengcc.top

SHOW TABLE STATUS LIKE 'users';
来源：http://kdh.yj20258888.top

[Q74] 强制使用索引
来源：http://bae.fktsv.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://fbw.guowangkeji.top

[Q75] 日期格式化
来源：http://soq.quarkkingdee.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ljz.hywenlv.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ldn.chenlongwang.top

[Q76] 按天统计
来源：http://xrb.zhixingplan.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://oyf.yuanzhike.top

[Q77] 时间加减
来源：http://xcp.daria6918.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://oys.xziqi.cn

[Q78] 当前时间
来源：http://vet.hammf.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://bzv.yj202588.top

[Q79] 字符串拼接
来源：http://wdo.ivvv.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://lka.0kj1m.cn

[Q80] 字符串截取
来源：http://kzt.pycfn.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://tgf.guowangkeji.top

[Q81] 字符串替换
来源：http://ihz.jinghuilouyu.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://dem.xylfe.cn

[Q82] 字符长度与字节长度
来源：http://yiz.andypj.xyz

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://yop.vehdjk.com

[Q83] 大小写转换
来源：http://wdu.shanyushiyangkeji.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://pnh.zhixingplan.top

[Q84] 去除首尾空格
来源：http://wvu.dianchejie.cn

SELECT TRIM(name) FROM users;
来源：http://scf.wangdashe.top

[Q85] 数值取整
来源：http://wkv.nanxuanxn.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ghk.iojbl.cn

[Q86] 读取 JSON 字段
来源：http://ppq.wangshuangyany.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://enm.shangyingyoupin.top

[Q87] JSON 字段做条件
来源：http://atz.sjlbkw.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://dgm.havefunace.top

[Q88] 行转列（条件聚合）
来源：http://pud.zhijiandao.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://dxt.bjfxy.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hbb.jianghu66.top

[Q89] 判断表是否存在
来源：http://pei.gaohongyu789.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://bgk.epnwcf.com

[Q90] 生成序号列
来源：http://pzv.quarkkingdee.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ieu.redwolf501.top

================================================================================
来源：http://iyh.yuxming.cn

R. Bash 专题
来源：http://lsk.hysaishi.cn

================================================================================
来源：http://pgo.nanxinkj.top

[R01] shebang 与严格模式
来源：http://kqu.c1oappe.top

#!/usr/bin/env bash
来源：http://ypz.jqgufenzy.top

set -euo pipefail
来源：http://clz.bbcook.cn

[R02] 变量赋值与使用
来源：http://ldk.tanke756.top

name="Tom"; echo "$name"
来源：http://kjz.zhengqikj.top

[R03] 只读变量
来源：http://npn.cqqwz.cn

readonly PI=3.14
来源：http://odf.fzhhl.top

[R04] 位置参数
来源：http://qqi.daria6918.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://xwr.zdbjq.cn

[R05] 参数默认值
来源：http://zte.iojbl.cn

name="${1:-default}"
来源：http://gmi.wangshuangyany.cn

[R06] 判断命令是否存在
来源：http://kxj.yuxming.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://sfe.shanyushiyangtech.top

[R07] if 判断文件
来源：http://hkc.tanke756.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://zat.wangdashe.top

[R08] 数值比较
来源：http://uhq.shuidangran.top

if (( a > b )); then echo "a 更大"; fi
来源：http://qtz.vehdjk.com

[R09] 字符串比较
来源：http://oci.yuxming.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://qvi.jqgfzy.top

[R10] 正则匹配
来源：http://fnm.iojbl.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hgx.cdnleiting.top

[R11] case 多分支
来源：http://oqb.shzxlz.cn

case "$1" in
来源：http://zws.zhengqikj.top

start) echo "启动" ;;
来源：http://ssm.vqdsnc.cn

stop)  echo "停止" ;;
来源：http://dmp.dashuyun.cn

*)     echo "未知命令" ;;
来源：http://bdg.jinghuilouyu.cn

esac
来源：http://ljl.jyoumei.cn

[R12] for 遍历文件
来源：http://woy.sysykeji.top

for f in *.txt; do echo "$f"; done
来源：http://org.cqqwz.cn

[R13] for 计数循环
来源：http://qyj.chenjidiqi.icu

for i in {1..10}; do echo "$i"; done
来源：http://jig.zhengqikj.top

[R14] C 风格 for
来源：http://mkr.hysaishi.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mlx.uphjek.com

[R15] while 逐行读文件
来源：http://lni.yj202588.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://sbb.jyoumei.cn

[R16] until 等待条件
来源：http://aap.pengpengdd.cyou

until [[ -f done.flag ]]; do sleep 1; done
来源：http://dck.fktsv.cn

[R17] 数组定义与取值
来源：http://xev.shanyushiyangkeji.top

arr=(a b c); echo "${arr[0]}"
来源：http://sht.gogol.net.cn

[R18] 遍历数组
来源：http://fxh.ctjpmb.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://htq.zhaomingkeji.xyz

[R19] 数组长度
来源：http://qmo.xziqi.cn

echo "${#arr[@]}"
来源：http://yxn.shzxlz.cn

[R20] 关联数组（字典）
来源：http://ias.aizwys.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://pdi.bbcook.cn

[R21] 字符串长度
来源：http://mel.yongpay.top

echo "${#s}"
来源：http://ixy.havefunace.top

[R22] 截取子串
来源：http://vmr.jqgufenzy.top

echo "${s:0:5}"
来源：http://fqu.zycfv.cn

[R23] 字符串替换
来源：http://siq.chenlongwang.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ndh.cheryme.top

[R24] 大小写转换
来源：http://ovd.hfpthk.cn

echo "${s^^}"; echo "${s,,}"
来源：http://fkb.gogol.net.cn

[R25] 去后缀 / 去前缀
来源：http://inu.cqqwz.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://tst.xingfuxueyuan.xyz

[R26] 命令替换
来源：http://evq.jinghuilouyu.cn

now=$(date +%F); echo "$now"
来源：http://zzw.ywan-chungtsiang.top

[R27] 算术展开
来源：http://gwe.yongpay.top

echo $((1 + 2 * 3))
来源：http://pqn.jyoumei.cn

[R28] 浮点运算
来源：http://ooo.nanxuanxn.top

echo "scale=2; 10/3" | bc
来源：http://qjo.uphjek.com

[R29] 定义函数
来源：http://peg.zhixingplan.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://lqe.sufxvd.cn

[R30] 函数返回状态码
来源：http://phk.dashuyun.cn

f() { return 0; }; f || echo "失败了"
来源：http://vqm.fanxiaobao.xyz

[R31] 局部变量
来源：http://wgh.ydjk.org.cn

f() { local x=1; echo "$x"; }
来源：http://upp.ivvv.top

[R32] 参数个数校验
来源：http://kph.yuanzhike.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hqd.wangshuangyany.cn

[R33] 捕获错误并提示行号
来源：http://lks.yj20258888.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://qwm.yj20258.top

[R34] 退出时清理
来源：http://kks.daria6918.cn

trap 'rm -f "$tmp"' EXIT
来源：http://wfn.aizwys.cn

[R35] 后台执行并等待
来源：http://uig.zdqjudy.top

sleep 5 & pid=$!; wait "$pid"
来源：http://whn.wangdashe.top

[R36] 并发执行多个任务
来源：http://arv.xuetiantiany.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ses.jinqigfzy.top

[R37] 把输出赋给变量
来源：http://jwp.jqgfzy.top


<!-- 参考信息 -->