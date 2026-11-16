代发 wailian999

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://vgu.yanxiufei.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://muq.xingfuxueyuan.xyz

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mfc.jqgufenzy.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://tan.sufxvd.cn

================================================================================
来源：http://biw.ydzc1.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://uke.xziqi.cn

================================================================================
来源：http://htl.jqgufenzy.top

[Q01] 创建表
来源：http://gfv.ydjk.org.cn

CREATE TABLE users (
来源：http://hgv.cheryme.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://fsz.dashuyun.cn

name VARCHAR(50) NOT NULL,
来源：http://piw.xuanzx.com

email VARCHAR(100) UNIQUE,
来源：http://hly.hesvh.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://zll.jyoumei.cn

);
来源：http://abo.tarul.cn

[Q02] 创建带外键的表
来源：http://qgj.jqgfzy.top

CREATE TABLE orders (
来源：http://utx.tanke756.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://qlc.kuanghao11.cn

user_id INT NOT NULL,
来源：http://llo.redwolf501.top

amount DECIMAL(10, 2),
来源：http://nii.birdmap.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://jaf.yvedp.cn

);
来源：http://vlp.haohaochexian.top

[Q03] 增加列
来源：http://puy.fanxiaobao.xyz

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://qnm.fehbvm.com

[Q04] 修改列类型
来源：http://xkg.cheryme.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://svu.aibaodan.cn

[Q05] 重命名列
来源：http://lil.fehbvm.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://vve.epnwcf.com

[Q06] 删除列
来源：http://pbh.cashguo.top

ALTER TABLE users DROP COLUMN age;
来源：http://lsn.ctjpmb.com

[Q07] 删除表
来源：http://lvb.hysaishi.cn

DROP TABLE IF EXISTS orders;
来源：http://cns.nwbrower.top

[Q08] 创建普通索引
来源：http://swh.ppjwa.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://mbl.jinghuilouyu.cn

[Q09] 创建唯一索引
来源：http://fcz.tarul.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hjb.chenjidiqi.icu

[Q10] 插入单行
来源：http://wlj.cashguo.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://bns.aizwys.cn

[Q11] 一次插入多行
来源：http://ttd.vqdsnc.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ctf.yonumen.top

[Q12] 插入后取自增 ID
来源：http://wfp.kuanghao11.cn

INSERT INTO users (name) VALUES ('C');
来源：http://gkj.tarul.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://syy.havefunace.top

[Q13] 忽略重复插入
来源：http://asr.jinghuilouyu.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://qcj.ywan-chungtsiang.top

[Q14] 存在则更新（upsert）
来源：http://sxr.fehbvm.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://jxn.wangshuangyany.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wcu.zhongyouzk.top

[Q15] 查询全部
来源：http://res.yonumen.top

SELECT * FROM users;
来源：http://tpo.yonumen.top

[Q16] 查询指定列
来源：http://fhz.chenjidiqi.icu

SELECT id, name FROM users;
来源：http://iqi.kuanghao11.cn

[Q17] 条件查询
来源：http://rby.sjlbkw.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://qfx.hammf.cn

[Q18] 模糊匹配
来源：http://wtj.fanxiaobao.xyz

SELECT * FROM users WHERE name LIKE '张%';
来源：http://qgs.vehdjk.com

[Q19] 范围查询
来源：http://tqa.zhixingplan.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://xob.tarul.cn

[Q20] IN 列表
来源：http://vft.chenjidiqi.icu

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://dvj.zycfv.cn

[Q21] 空值判断
来源：http://rvl.hammf.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://kix.sysykeji.top

[Q22] 排序
来源：http://ufx.sjlbkw.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://zrw.bjfxy.top

[Q23] 分页
来源：http://zrb.jinyuanbaomall.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ugo.zycfv.cn

[Q24] 去重
来源：http://vyv.jianghu66.top

SELECT DISTINCT city FROM users;
来源：http://riw.ywan-chungtsiang.top

[Q25] 只取前 N 条
来源：http://sof.ydjk.org.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ngp.feifeiyinyue.top

[Q26] 计数
来源：http://rgs.cucudq.cn

SELECT COUNT(*) FROM users;
来源：http://wyb.dianchejie.cn

[Q27] 条件计数
来源：http://edz.jianghu66.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://xgn.gogol.net.cn

[Q28] 求和与平均
来源：http://crx.mhx1999.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://bqq.zhixingplan.top

[Q29] 最大最小值
来源：http://tla.zhiwuduotai.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://srq.ybcxt.top

[Q30] 分组统计
来源：http://hlw.ydjk.org.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://tfw.gogol.net.cn

[Q31] 分组后过滤
来源：http://tsq.hysaishi.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://dge.jlsjyb.cn

[Q32] 分组拼接字符串
来源：http://mle.yuanzhike.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://nur.mhx1999.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://gsu.haohaochexian.top

[Q33] 多列分组
来源：http://jco.daxiang520.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://jbx.zhongyouzk.top

[Q34] 每组取第一条
来源：http://bxo.cashguo.top

SELECT * FROM (
来源：http://gis.yj20258.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://lnw.snrcjt.cn

) t WHERE rn = 1;
来源：http://fwe.yonumen.top

[Q35] 内连接
来源：http://vdj.sxryk.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ycm.yuxming.cn

[Q36] 左连接
来源：http://zgq.hesvh.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hau.hysaishi.cn

[Q37] 右连接
来源：http://lig.0kj1m.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ewm.jyoumei.cn

[Q38] 全外连接（PostgreSQL）
来源：http://mwx.nanxuanxn.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://gnm.cucudq.cn

[Q39] 自连接（查上下级）
来源：http://hxy.chenzaomai.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://fzi.zhijiandao.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://uxe.daxiang520.top

[Q40] 交叉连接（笛卡尔积）
来源：http://tdm.vqdsnc.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://jjr.jqgfzy.top

[Q41] 多表连接
来源：http://zjj.guannengcc.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://hxs.tian-w.cn

JOIN users u ON u.id = o.user_id
来源：http://bvn.fehbvm.com

JOIN products p ON p.id = o.product_id;
来源：http://tmg.zhoulong.xyz

[Q42] 连接条件附加过滤
来源：http://lnr.gotoacloud.top

SELECT u.name, o.amount FROM users u
来源：http://rob.shangyingyoupin.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ylh.snrcjt.cn

[Q43] 标量子查询
来源：http://sff.ctjpmb.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://zmf.52xcode.cn

[Q44] IN 子查询
来源：http://jtx.fzhhl.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hsy.sjlbkw.cn

[Q45] EXISTS 判断存在
来源：http://nqb.cucudq.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zfq.chenlongwang.top

[Q46] NOT EXISTS 判断不存在
来源：http://cez.gotoacloud.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://cyd.hcnkem.com

[Q47] 与平均值比较
来源：http://nnu.nwbrower.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://dqp.dashuyun.cn

[Q48] CTE 公用表表达式
来源：http://pci.shanyushiyangkeji.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ftd.hnxiangtu.top

SELECT * FROM t WHERE c > 5;
来源：http://zqd.hfpthk.cn

[Q49] 更新单行
来源：http://tnn.zhixingplan.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://rcl.gzhubu.top

[Q50] 批量更新
来源：http://chd.zhongyouzk.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://qyg.hammf.cn

[Q51] 用子查询更新
来源：http://cgt.aizwys.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://qef.jinqigfzy.top

[Q52] 删除指定行
来源：http://uga.xylfe.cn

DELETE FROM users WHERE id = 10;
来源：http://ulj.chenjidiqi.icu

[Q53] 按条件删除
来源：http://drl.ywan-chungtsiang.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://cjw.wangdashe.top

[Q54] 清空表
来源：http://mqx.zhoulong.xyz

TRUNCATE TABLE logs;
来源：http://fdu.hcnkem.com

[Q55] 排名（并列占位）
来源：http://spj.52xcode.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://dpt.feifeiyinyue.top

[Q56] 密集排名（并列不占位）
来源：http://fjl.daxiang520.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://lwi.jinyuanbaomall.cn

[Q57] 行号
来源：http://tzq.guowangkeji.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://yhr.fengsongda.top

[Q58] 累计求和
来源：http://umi.zhiwuduotai.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wce.jinqigfzy.top

[Q59] 分组内累计
来源：http://iyb.cashguo.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://qga.52xcode.cn

[Q60] 取上一行 / 下一行
来源：http://hyh.snrcjt.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://zzn.sjlbkw.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://voz.yuanzhike.top

[Q61] 移动平均
来源：http://iam.shuidangran.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://tcs.shzxlz.cn

[Q62] 分组占比
来源：http://kzo.hnxiangtu.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://rux.jinqigfzy.top

[Q63] 开启事务
来源：http://iep.nanxinkj.top

START TRANSACTION;                -- 或 BEGIN
来源：http://wty.fanxiaobao.xyz

[Q64] 提交事务
来源：http://woq.zhongyouzk.top

COMMIT;
来源：http://bai.epnwcf.com

[Q65] 回滚事务
来源：http://hwy.zhongyouzk.top

ROLLBACK;
来源：http://zuh.jinyuanbaomall.cn

[Q66] 行锁查询
来源：http://sun.zdqjudy.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://vxf.smart0.xyz

[Q67] 设置隔离级别
来源：http://ebw.nanxuanxn.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://rsa.zdbjq.cn

[Q68] 保存点
来源：http://jhn.zhongyouzk.top

SAVEPOINT sp1;
来源：http://rfd.jyoumei.cn

ROLLBACK TO sp1;
来源：http://vxz.hfpthk.cn

[Q69] 查看执行计划
来源：http://mzz.feifeiyinyue.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://xnk.zhoulong.xyz

[Q70] 更新统计信息
来源：http://fva.xuanzx.com

ANALYZE TABLE users;
来源：http://wce.jinqigufen.top

[Q71] 查看建表语句
来源：http://zsz.hesvh.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://qvj.dianchejie.cn

[Q72] 查看索引
来源：http://mku.jinqigufen.top

SHOW INDEX FROM users;
来源：http://brf.gogol.net.cn

[Q73] 查看表状态
来源：http://hbl.yonumen.top

SHOW TABLE STATUS LIKE 'users';
来源：http://dov.zdqjudy.top

[Q74] 强制使用索引
来源：http://rdk.yj20258888.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mgp.xuanzx.com

[Q75] 日期格式化
来源：http://eec.ppjwa.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://rik.smart0.xyz

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://fku.ehwqpu.com

[Q76] 按天统计
来源：http://bfq.yonumen.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://yxy.sysykeji.top

[Q77] 时间加减
来源：http://ums.ydzc1.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://btv.meibo888.top

[Q78] 当前时间
来源：http://rmo.zdqjudy.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://oll.uphjek.com

[Q79] 字符串拼接
来源：http://hbd.yj20258888.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://pfc.gogol.net.cn

[Q80] 字符串截取
来源：http://uri.hysaishi.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://vld.mhx1999.top

[Q81] 字符串替换
来源：http://wzx.zhoulong.xyz

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://pmz.nanxinkj.top

[Q82] 字符长度与字节长度
来源：http://oot.meibo888.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://sis.9152youxi.cn

[Q83] 大小写转换
来源：http://zme.fengsongda.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://bno.jiagoushi.top

[Q84] 去除首尾空格
来源：http://vdl.cucudq.cn

SELECT TRIM(name) FROM users;
来源：http://obo.kuanghao11.cn

[Q85] 数值取整
来源：http://qwb.hammf.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://oqj.guowangkeji.top

[Q86] 读取 JSON 字段
来源：http://cyg.yanxiufei.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://evn.xinyue.icu

[Q87] JSON 字段做条件
来源：http://aze.shanyushiyangkeji.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://dql.nanxuanxn.top

[Q88] 行转列（条件聚合）
来源：http://uqn.epnwcf.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ciw.ehwqpu.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hvn.xziqi.cn

[Q89] 判断表是否存在
来源：http://jwy.cheryme.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://gfm.yj20258.top

[Q90] 生成序号列
来源：http://kvb.zhiwuduotai.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://gss.yanxiufei.cn

================================================================================
来源：http://abh.yueranfly.top

R. Bash 专题
来源：http://bta.ivvv.top

================================================================================
来源：http://xga.jinqigfzy.top

[R01] shebang 与严格模式
来源：http://fwt.tian-w.cn

#!/usr/bin/env bash
来源：http://soi.jqgufenzy.top

set -euo pipefail
来源：http://bzs.tianlin.xyz

[R02] 变量赋值与使用
来源：http://ved.pengpengdd.cyou

name="Tom"; echo "$name"
来源：http://ckf.jianghu66.top

[R03] 只读变量
来源：http://ecv.fanxiaobao.xyz

readonly PI=3.14
来源：http://ywo.tanke756.top

[R04] 位置参数
来源：http://mwk.jinyuanbaomall.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://cgz.andypj.xyz

[R05] 参数默认值
来源：http://gjm.hcnkem.com

name="${1:-default}"
来源：http://irt.vehdjk.com

[R06] 判断命令是否存在
来源：http://tiq.zhixingplan.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://bcj.cdnleiting.top

[R07] if 判断文件
来源：http://gbz.wangshuangyany.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://bwv.jinqigfzy.top

[R08] 数值比较
来源：http://iot.52xcode.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://pdb.iojbl.cn

[R09] 字符串比较
来源：http://iah.gogol.net.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://fvk.dashuyun.cn

[R10] 正则匹配
来源：http://mmn.gotoacloud.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ptx.zhiwuduotai.top

[R11] case 多分支
来源：http://euc.cucudq.cn

case "$1" in
来源：http://ftd.vehdjk.com

start) echo "启动" ;;
来源：http://ssl.jyoumei.cn

stop)  echo "停止" ;;
来源：http://gww.ppjwa.cn

*)     echo "未知命令" ;;
来源：http://gwo.sxryk.cn

esac
来源：http://wmo.vehdjk.com

[R12] for 遍历文件
来源：http://yjo.zdqjudy.top

for f in *.txt; do echo "$f"; done
来源：http://kvs.aibaodan.cn

[R13] for 计数循环
来源：http://orz.zhixingplan.top

for i in {1..10}; do echo "$i"; done
来源：http://rnh.yj20258888.top

[R14] C 风格 for
来源：http://wsi.zhongyouzk.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://pui.9152youxi.cn

[R15] while 逐行读文件
来源：http://dtt.xuetiantiany.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://zft.yvedp.cn

[R16] until 等待条件
来源：http://krg.zhoulong.xyz

until [[ -f done.flag ]]; do sleep 1; done
来源：http://qca.jqgfzy.top

[R17] 数组定义与取值
来源：http://fqh.jlsjyb.cn

arr=(a b c); echo "${arr[0]}"
来源：http://rer.shangyingyoupin.top

[R18] 遍历数组
来源：http://uod.tian-w.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://rhz.xuetiantiany.cn

[R19] 数组长度
来源：http://jfk.svipenyu.cn

echo "${#arr[@]}"
来源：http://fum.dianchejie.cn

[R20] 关联数组（字典）
来源：http://xrz.zdqjudy.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://qjt.jinqigufen.top

[R21] 字符串长度
来源：http://ojr.hfpthk.cn

echo "${#s}"
来源：http://rmo.chenzaomai.com

[R22] 截取子串
来源：http://bcr.0kj1m.cn

echo "${s:0:5}"
来源：http://flw.snrcjt.cn

[R23] 字符串替换
来源：http://gqd.jyoumei.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://nvv.smart0.xyz

[R24] 大小写转换
来源：http://vjl.yuxming.cn

echo "${s^^}"; echo "${s,,}"
来源：http://igi.fengsongda.top

[R25] 去后缀 / 去前缀
来源：http://rcd.tian-w.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://lye.daria6918.cn

[R26] 命令替换
来源：http://qbg.yfazqb.com

now=$(date +%F); echo "$now"
来源：http://dns.ywan-chungtsiang.top

[R27] 算术展开
来源：http://htx.vehdjk.com

echo $((1 + 2 * 3))
来源：http://imd.chenjidiqi.icu

[R28] 浮点运算
来源：http://rfr.jinghuilouyu.cn

echo "scale=2; 10/3" | bc
来源：http://rqc.snrcjt.cn

[R29] 定义函数
来源：http://dtq.sjlbkw.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://vjn.nanxinkj.top

[R30] 函数返回状态码
来源：http://lvd.hongshengwenyu.top

f() { return 0; }; f || echo "失败了"
来源：http://jgy.shuidangran.top

[R31] 局部变量
来源：http://bea.fengsongda.top

f() { local x=1; echo "$x"; }
来源：http://cmo.sweek.top

[R32] 参数个数校验
来源：http://ajv.zdbjq.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://fhc.snrcjt.cn

[R33] 捕获错误并提示行号
来源：http://fnd.redwolf501.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://bln.cucudq.cn

[R34] 退出时清理
来源：http://ghy.zhongyouzk.top

trap 'rm -f "$tmp"' EXIT
来源：http://rmt.fanxiaobao.xyz

[R35] 后台执行并等待
来源：http://mvm.shuidangran.top

sleep 5 & pid=$!; wait "$pid"
来源：http://fhs.tanke756.top

[R36] 并发执行多个任务
来源：http://yfs.mhx1999.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mpk.mhx1999.top

[R37] 把输出赋给变量
来源：http://kxc.aibaodan.cn

files=$(ls -1)
来源：http://ncs.hesvh.cn

[R38] 管道串联
来源：http://beb.shanyushiyangkeji.top

cat a.txt | grep -i error | wc -l
来源：http://fiu.guannengcc.top

[R39] 重定向标准输出与错误
来源：http://akz.vqdsnc.cn

cmd > out.log 2>&1
来源：http://kea.zdqjudy.top

[R40] 追加写日志
来源：http://riq.nwbrower.top

echo "log" >> out.log
来源：http://dje.yj202588.top

[R41] 丢弃输出
来源：http://gvq.vehdjk.com


<!-- 参考信息 -->