代发 wailian999

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ege.bjfxy.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ahy.c1oappe.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://yhg.jyoumei.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://rqx.ctjpmb.com

================================================================================
来源：http://pwe.yuanzhike.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://gyw.jinqigufen.top

================================================================================
来源：http://baa.fzhhl.top

[Q01] 创建表
来源：http://meq.aizwys.cn

CREATE TABLE users (
来源：http://kfe.cucudq.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ffw.xziqi.cn

name VARCHAR(50) NOT NULL,
来源：http://qoc.cdnleiting.top

email VARCHAR(100) UNIQUE,
来源：http://sxs.birdmap.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://cvq.hywenlv.cn

);
来源：http://wnp.pengpengdd.cyou

[Q02] 创建带外键的表
来源：http://kdc.sjlbkw.cn

CREATE TABLE orders (
来源：http://qvn.guowangkeji.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mwb.chenjidiqi.icu

user_id INT NOT NULL,
来源：http://otu.fehbvm.com

amount DECIMAL(10, 2),
来源：http://lpo.xylfe.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://qgr.cdnleiting.top

);
来源：http://ggk.fehbvm.com

[Q03] 增加列
来源：http://qbs.ehwqpu.com

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://nhk.tian-w.cn

[Q04] 修改列类型
来源：http://ord.smart0.xyz

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://rub.cucudq.cn

[Q05] 重命名列
来源：http://qwc.iojbl.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ghd.jianghu66.top

[Q06] 删除列
来源：http://quq.yangfankeji.com

ALTER TABLE users DROP COLUMN age;
来源：http://sff.ivvv.top

[Q07] 删除表
来源：http://jmt.ydzc1.top

DROP TABLE IF EXISTS orders;
来源：http://yil.wangdashe.top

[Q08] 创建普通索引
来源：http://wok.yj20258.top

CREATE INDEX idx_users_email ON users(email);
来源：http://exd.yj20258888.top

[Q09] 创建唯一索引
来源：http://bmk.vehdjk.com

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ymd.zycfv.cn

[Q10] 插入单行
来源：http://ncr.havefunace.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://bhd.fengsongda.top

[Q11] 一次插入多行
来源：http://emh.tianlin.xyz

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://krm.gzhubu.top

[Q12] 插入后取自增 ID
来源：http://thl.jiagoushi.top

INSERT INTO users (name) VALUES ('C');
来源：http://poo.zhijiandao.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://gat.feifeiyinyue.top

[Q13] 忽略重复插入
来源：http://yfr.yanxiufei.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://cxn.dashuyun.cn

[Q14] 存在则更新（upsert）
来源：http://hqk.gzhubu.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://rxu.xinyue.icu

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://vab.feifeiyinyue.top

[Q15] 查询全部
来源：http://pjt.guannengcc.top

SELECT * FROM users;
来源：http://kaj.chenlongwang.top

[Q16] 查询指定列
来源：http://qku.birdmap.top

SELECT id, name FROM users;
来源：http://vdm.ywan-chungtsiang.top

[Q17] 条件查询
来源：http://ogu.yangfankeji.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ecd.zhaomingkeji.xyz

[Q18] 模糊匹配
来源：http://hgk.cashguo.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://dwr.c1oappe.top

[Q19] 范围查询
来源：http://qvm.zhijiandao.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://cyp.hcnkem.com

[Q20] IN 列表
来源：http://akn.xingfuxueyuan.xyz

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ykw.zhixingplan.top

[Q21] 空值判断
来源：http://zhf.pycfn.com

SELECT * FROM users WHERE email IS NULL;
来源：http://juw.jinqigfzy.top

[Q22] 排序
来源：http://ozz.jianghu66.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://tms.xuanzx.com

[Q23] 分页
来源：http://wbf.yueranfly.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://xyj.guowangkeji.top

[Q24] 去重
来源：http://usv.zdbjq.cn

SELECT DISTINCT city FROM users;
来源：http://hjr.ivvv.top

[Q25] 只取前 N 条
来源：http://pqa.dashuyun.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://icr.fanxiaobao.xyz

[Q26] 计数
来源：http://wqg.sxryk.cn

SELECT COUNT(*) FROM users;
来源：http://qiv.pengpengdd.cyou

[Q27] 条件计数
来源：http://ith.snrcjt.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://zme.hammf.cn

[Q28] 求和与平均
来源：http://smf.ydzc1.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ipo.yj202588.top

[Q29] 最大最小值
来源：http://bks.vqdsnc.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://nhm.tanke756.top

[Q30] 分组统计
来源：http://ibt.ehwqpu.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mww.kuanghao11.cn

[Q31] 分组后过滤
来源：http://tny.ywan-chungtsiang.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ejr.ywan-chungtsiang.top

[Q32] 分组拼接字符串
来源：http://xei.pengpengdd.cyou

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://viq.dashuyun.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ohp.chenlongwang.top

[Q33] 多列分组
来源：http://wfy.hywenlv.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://lnq.fktsv.cn

[Q34] 每组取第一条
来源：http://sok.sjlbkw.cn

SELECT * FROM (
来源：http://nnm.316326.xyz

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://gcs.daria6918.cn

) t WHERE rn = 1;
来源：http://jwu.cheryme.top

[Q35] 内连接
来源：http://rtr.chenlongwang.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://htg.cheryme.top

[Q36] 左连接
来源：http://poc.yj202588.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://amz.svipenyu.cn

[Q37] 右连接
来源：http://ixl.epnwcf.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://gix.wangshuangyany.cn

[Q38] 全外连接（PostgreSQL）
来源：http://par.nanxuanxn.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ugt.yangfankeji.com

[Q39] 自连接（查上下级）
来源：http://bpm.cdnleiting.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://xaw.shzxlz.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://nhp.redwolf501.top

[Q40] 交叉连接（笛卡尔积）
来源：http://oxb.bjfxy.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://cmi.yvedp.cn

[Q41] 多表连接
来源：http://xun.ppjwa.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://hzp.yangfankeji.com

JOIN users u ON u.id = o.user_id
来源：http://uuw.pycfn.com

JOIN products p ON p.id = o.product_id;
来源：http://ntp.shanyushiyangkeji.top

[Q42] 连接条件附加过滤
来源：http://kow.snrcjt.cn

SELECT u.name, o.amount FROM users u
来源：http://dfv.shuidangran.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://uza.andypj.xyz

[Q43] 标量子查询
来源：http://zby.zhengqikj.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://qqz.gaohongyu789.top

[Q44] IN 子查询
来源：http://xmm.zhengqikj.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://vbb.chenjidiqi.icu

[Q45] EXISTS 判断存在
来源：http://cyk.jqgfzy.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://gyt.guannengcc.top

[Q46] NOT EXISTS 判断不存在
来源：http://gtn.snrcjt.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://efm.chenzaomai.com

[Q47] 与平均值比较
来源：http://dkd.meibo888.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://xab.shuidangran.top

[Q48] CTE 公用表表达式
来源：http://xid.fengsongda.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://snp.ivvv.top

SELECT * FROM t WHERE c > 5;
来源：http://fuc.dianchejie.cn

[Q49] 更新单行
来源：http://kqc.wangdashe.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://rvd.snrcjt.cn

[Q50] 批量更新
来源：http://flb.gaohongyu789.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wuz.fktsv.cn

[Q51] 用子查询更新
来源：http://occ.pengpengdd.cyou

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://xtg.gaohongyu789.top

[Q52] 删除指定行
来源：http://ela.zdqjudy.top

DELETE FROM users WHERE id = 10;
来源：http://rcf.zhixingplan.top

[Q53] 按条件删除
来源：http://vvt.sufxvd.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://dyl.iojbl.cn

[Q54] 清空表
来源：http://xvm.ydzc1.top

TRUNCATE TABLE logs;
来源：http://otj.hammf.cn

[Q55] 排名（并列占位）
来源：http://wwz.jyoumei.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://uze.xuetiantiany.cn

[Q56] 密集排名（并列不占位）
来源：http://joe.yuanzhike.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://psi.wangdashe.top

[Q57] 行号
来源：http://lcz.wangdashe.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ouu.bjfxy.top

[Q58] 累计求和
来源：http://lql.cucudq.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://lph.sweek.top

[Q59] 分组内累计
来源：http://wwy.jinqigfzy.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://nhv.yongpay.top

[Q60] 取上一行 / 下一行
来源：http://rvz.ydjk.org.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://qwq.meibo888.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://efu.bbcook.cn

[Q61] 移动平均
来源：http://pyu.tian-w.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://guu.hongshengwenyu.top

[Q62] 分组占比
来源：http://bnh.shangyingyoupin.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ust.snrcjt.cn

[Q63] 开启事务
来源：http://dgw.tianlin.xyz

START TRANSACTION;                -- 或 BEGIN
来源：http://apr.snrcjt.cn

[Q64] 提交事务
来源：http://ecq.hnxiangtu.top

COMMIT;
来源：http://lfz.dianchejie.cn

[Q65] 回滚事务
来源：http://hzs.hnxiangtu.top

ROLLBACK;
来源：http://ynq.wangshuangyany.cn

[Q66] 行锁查询
来源：http://obk.0kj1m.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://xzm.yuxming.cn

[Q67] 设置隔离级别
来源：http://vtw.nwbrower.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://taw.c1oappe.top

[Q68] 保存点
来源：http://ywf.quarkkingdee.top

SAVEPOINT sp1;
来源：http://zvc.uphjek.com

ROLLBACK TO sp1;
来源：http://drx.ydjk.org.cn

[Q69] 查看执行计划
来源：http://agf.pengpengdd.cyou

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://axb.52xcode.cn

[Q70] 更新统计信息
来源：http://oxp.fengsongda.top

ANALYZE TABLE users;
来源：http://jzd.cqqwz.cn

[Q71] 查看建表语句
来源：http://clu.yj20258888.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://gig.zdbjq.cn

[Q72] 查看索引
来源：http://loe.hnxiangtu.top

SHOW INDEX FROM users;
来源：http://jid.9152youxi.cn

[Q73] 查看表状态
来源：http://ozm.cheryme.top

SHOW TABLE STATUS LIKE 'users';
来源：http://mzd.yangfankeji.com

[Q74] 强制使用索引
来源：http://ksw.nwbrower.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://otq.xylfe.cn

[Q75] 日期格式化
来源：http://klu.zhaomingkeji.xyz

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://rcx.uphjek.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://qiz.tanke756.top

[Q76] 按天统计
来源：http://qij.yueranfly.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://swz.pengpengdd.cyou

[Q77] 时间加减
来源：http://crv.ctjpmb.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://exn.ctjpmb.com

[Q78] 当前时间
来源：http://nht.chenzaomai.com

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://bcg.zhoulong.xyz

[Q79] 字符串拼接
来源：http://xjj.9152youxi.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://skk.fktsv.cn

[Q80] 字符串截取
来源：http://xix.xuanzx.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ksi.zdqjudy.top

[Q81] 字符串替换
来源：http://tjn.wangshuangyany.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://qir.9152youxi.cn

[Q82] 字符长度与字节长度
来源：http://svw.smart0.xyz

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://psv.zhixingplan.top

[Q83] 大小写转换
来源：http://snx.ybcxt.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://pua.birdmap.top

[Q84] 去除首尾空格
来源：http://zcs.cqqwz.cn

SELECT TRIM(name) FROM users;
来源：http://vug.zhixingplan.top

[Q85] 数值取整
来源：http://luv.jinqigfzy.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://omg.havefunace.top

[Q86] 读取 JSON 字段
来源：http://tct.jianghu66.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://xoc.ctjpmb.com

[Q87] JSON 字段做条件
来源：http://dds.pycfn.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://uba.feifeiyinyue.top

[Q88] 行转列（条件聚合）
来源：http://mcf.yanxiufei.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://msv.aibaodan.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ypg.dianchejie.cn

[Q89] 判断表是否存在
来源：http://cek.fzhhl.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wmu.gaohongyu789.top

[Q90] 生成序号列
来源：http://glb.yj202588.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://qru.chenzaomai.com

================================================================================
来源：http://pzn.mhx1999.top

R. Bash 专题
来源：http://gch.cashguo.top

================================================================================
来源：http://fdg.nwbrower.top

[R01] shebang 与严格模式
来源：http://wmk.ehwqpu.com

#!/usr/bin/env bash
来源：http://nvq.shzxlz.cn

set -euo pipefail
来源：http://fpq.cdnleiting.top

[R02] 变量赋值与使用
来源：http://pmk.316326.xyz

name="Tom"; echo "$name"
来源：http://hhf.pengpengdd.cyou

[R03] 只读变量
来源：http://ykw.fktsv.cn

readonly PI=3.14
来源：http://qyp.dianchejie.cn

[R04] 位置参数
来源：http://ffi.ppjwa.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://twq.jiagoushi.top

[R05] 参数默认值
来源：http://hbz.quarkkingdee.top

name="${1:-default}"
来源：http://cpk.pengpengdd.cyou

[R06] 判断命令是否存在
来源：http://itw.uphjek.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://dnl.jinqigfzy.top

[R07] if 判断文件
来源：http://zde.316326.xyz

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://zcq.zdbjq.cn

[R08] 数值比较
来源：http://oey.xinyue.icu

if (( a > b )); then echo "a 更大"; fi
来源：http://mic.tian-w.cn

[R09] 字符串比较
来源：http://vlh.meibo888.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://efu.c1oappe.top

[R10] 正则匹配
来源：http://fxo.jinqigufen.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://gdk.ydjk.org.cn

[R11] case 多分支
来源：http://xtx.zycfv.cn

case "$1" in
来源：http://doa.chenlongwang.top

start) echo "启动" ;;
来源：http://ahn.cashguo.top

stop)  echo "停止" ;;
来源：http://icg.kuanghao11.cn

*)     echo "未知命令" ;;
来源：http://jot.fehbvm.com

esac
来源：http://eni.shanyushiyangtech.top

[R12] for 遍历文件
来源：http://gvq.haohaochexian.top

for f in *.txt; do echo "$f"; done
来源：http://pup.gaohongyu789.top

[R13] for 计数循环
来源：http://drb.yanxiufei.cn

for i in {1..10}; do echo "$i"; done
来源：http://sgg.ydjk.org.cn

[R14] C 风格 for
来源：http://afb.yj202588.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://nre.haohaochexian.top

[R15] while 逐行读文件
来源：http://ivz.gogol.net.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://owc.iojbl.cn

[R16] until 等待条件
来源：http://vwp.uphjek.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://gbr.yueranfly.top

[R17] 数组定义与取值
来源：http://wey.yuanzhike.top

arr=(a b c); echo "${arr[0]}"
来源：http://kjx.pycfn.com

[R18] 遍历数组
来源：http://hum.c1oappe.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ukf.gzhubu.top

[R19] 数组长度
来源：http://niz.chenjidiqi.icu

echo "${#arr[@]}"
来源：http://ezg.zhixingplan.top

[R20] 关联数组（字典）
来源：http://zzw.gaohongyu789.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://gaq.ydzc1.top

[R21] 字符串长度
来源：http://gwo.fanxiaobao.xyz

echo "${#s}"
来源：http://gsy.havefunace.top

[R22] 截取子串
来源：http://cue.xuanzx.com

echo "${s:0:5}"
来源：http://asu.jqgfzy.top

[R23] 字符串替换
来源：http://yms.yanxiufei.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://nmm.cashguo.top

[R24] 大小写转换
来源：http://uab.ctjpmb.com

echo "${s^^}"; echo "${s,,}"
来源：http://sjb.wangdashe.top

[R25] 去后缀 / 去前缀
来源：http://ima.shangyingyoupin.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://ehq.hcnkem.com

[R26] 命令替换
来源：http://ekg.smart0.xyz

now=$(date +%F); echo "$now"
来源：http://nsl.chenzaomai.com

[R27] 算术展开
来源：http://uhm.zhongyouzk.top

echo $((1 + 2 * 3))
来源：http://euf.zhijiandao.cn

[R28] 浮点运算
来源：http://qto.hongshengwenyu.top

echo "scale=2; 10/3" | bc
来源：http://qml.chenlongwang.top

[R29] 定义函数
来源：http://weh.aibaodan.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://npj.cucudq.cn

[R30] 函数返回状态码
来源：http://wkl.yueranfly.top

f() { return 0; }; f || echo "失败了"
来源：http://ypx.snrcjt.cn

[R31] 局部变量
来源：http://kkn.shangyingyoupin.top

f() { local x=1; echo "$x"; }
来源：http://jht.havefunace.top

[R32] 参数个数校验
来源：http://xez.fehbvm.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://cbb.fanxiaobao.xyz

[R33] 捕获错误并提示行号
来源：http://kyc.wangdashe.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ugb.cashguo.top

[R34] 退出时清理
来源：http://uqn.aibaodan.cn

trap 'rm -f "$tmp"' EXIT
来源：http://zcr.hfpthk.cn

[R35] 后台执行并等待
来源：http://rqa.52xcode.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://kka.havefunace.top

[R36] 并发执行多个任务
来源：http://sdq.ydzc1.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://bct.zdqjudy.top

[R37] 把输出赋给变量
来源：http://dmf.zdqjudy.top

files=$(ls -1)
来源：http://gzj.nanxinkj.top

[R38] 管道串联
来源：http://azk.sxryk.cn

cat a.txt | grep -i error | wc -l
来源：http://pfo.tarul.cn

[R39] 重定向标准输出与错误
来源：http://pme.ybcxt.top

cmd > out.log 2>&1
来源：http://uyd.yuxming.cn

[R40] 追加写日志
来源：http://uxd.bbcook.cn

echo "log" >> out.log
来源：http://xtm.zhengqikj.top

[R41] 丢弃输出
来源：http://ieo.sufxvd.cn


<!-- 参考信息 -->