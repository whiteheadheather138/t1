代发 wailian999

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://fec.mhx1999.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://afb.nanxinkj.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://jii.zhaomingkeji.xyz

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ozi.pycfn.com

================================================================================
来源：http://xxq.jyoumei.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://flh.xylfe.cn

================================================================================
来源：http://pwj.hysaishi.cn

[Q01] 创建表
来源：http://hdq.jlsjyb.cn

CREATE TABLE users (
来源：http://jpy.chenzaomai.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ntt.fehbvm.com

name VARCHAR(50) NOT NULL,
来源：http://jgf.fehbvm.com

email VARCHAR(100) UNIQUE,
来源：http://rtj.zdqjudy.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://tdz.svipenyu.cn

);
来源：http://hzt.hesvh.cn

[Q02] 创建带外键的表
来源：http://ggz.jqgfzy.top

CREATE TABLE orders (
来源：http://lky.yanxiufei.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://xnb.xylfe.cn

user_id INT NOT NULL,
来源：http://qds.cqqwz.cn

amount DECIMAL(10, 2),
来源：http://zrh.quarkkingdee.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://iqh.cdnleiting.top

);
来源：http://lem.uphjek.com

[Q03] 增加列
来源：http://see.haohaochexian.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://usm.yj20258888.top

[Q04] 修改列类型
来源：http://dto.zhaomingkeji.xyz

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://olb.yuxming.cn

[Q05] 重命名列
来源：http://qsc.meibo888.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://eby.hammf.cn

[Q06] 删除列
来源：http://ntg.cdnleiting.top

ALTER TABLE users DROP COLUMN age;
来源：http://luo.cdnleiting.top

[Q07] 删除表
来源：http://stu.bbcook.cn

DROP TABLE IF EXISTS orders;
来源：http://zvs.yuxming.cn

[Q08] 创建普通索引
来源：http://jef.yj20258888.top

CREATE INDEX idx_users_email ON users(email);
来源：http://jqm.cucudq.cn

[Q09] 创建唯一索引
来源：http://enz.nwbrower.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ehi.c1oappe.top

[Q10] 插入单行
来源：http://raq.hongshengwenyu.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://vzo.dashuyun.cn

[Q11] 一次插入多行
来源：http://wdb.ydjk.org.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://fpo.daria6918.cn

[Q12] 插入后取自增 ID
来源：http://njh.andypj.xyz

INSERT INTO users (name) VALUES ('C');
来源：http://mik.chenlongwang.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://rrz.jlsjyb.cn

[Q13] 忽略重复插入
来源：http://jco.zhongyouzk.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://qlg.zhixingplan.top

[Q14] 存在则更新（upsert）
来源：http://zmb.ivvv.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://gez.jqgfzy.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://zca.sysykeji.top

[Q15] 查询全部
来源：http://kpr.shzxlz.cn

SELECT * FROM users;
来源：http://rfa.andypj.xyz

[Q16] 查询指定列
来源：http://gfh.jianghu66.top

SELECT id, name FROM users;
来源：http://pqp.jiagoushi.top

[Q17] 条件查询
来源：http://vlk.dianchejie.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://dah.jlsjyb.cn

[Q18] 模糊匹配
来源：http://zgs.nanxuanxn.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://msv.zycfv.cn

[Q19] 范围查询
来源：http://ejo.jyoumei.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://qbw.ivvv.top

[Q20] IN 列表
来源：http://oln.cdnleiting.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://kxg.cqqwz.cn

[Q21] 空值判断
来源：http://cin.shuidangran.top

SELECT * FROM users WHERE email IS NULL;
来源：http://mqx.sufxvd.cn

[Q22] 排序
来源：http://umk.yvedp.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://xqu.jqgufenzy.top

[Q23] 分页
来源：http://jjm.shanyushiyangtech.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://qas.tian-w.cn

[Q24] 去重
来源：http://ifd.bjfxy.top

SELECT DISTINCT city FROM users;
来源：http://koc.jinqigfzy.top

[Q25] 只取前 N 条
来源：http://scx.yangfankeji.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://vwo.gotoacloud.top

[Q26] 计数
来源：http://iho.jianghu66.top

SELECT COUNT(*) FROM users;
来源：http://tjx.gotoacloud.top

[Q27] 条件计数
来源：http://hwn.yuanzhike.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://til.tarul.cn

[Q28] 求和与平均
来源：http://pmo.guannengcc.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://shv.fehbvm.com

[Q29] 最大最小值
来源：http://swf.nanxinkj.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://rhq.jyoumei.cn

[Q30] 分组统计
来源：http://wtz.nwbrower.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ikp.hywenlv.cn

[Q31] 分组后过滤
来源：http://veh.zhiwuduotai.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://cvh.zdbjq.cn

[Q32] 分组拼接字符串
来源：http://ves.zhoulong.xyz

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wco.zycfv.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://rpj.pengpengdd.cyou

[Q33] 多列分组
来源：http://yta.aibaodan.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://iry.jiagoushi.top

[Q34] 每组取第一条
来源：http://wja.pycfn.com

SELECT * FROM (
来源：http://krx.hongshengwenyu.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://qnk.nwbrower.top

) t WHERE rn = 1;
来源：http://ktv.gotoacloud.top

[Q35] 内连接
来源：http://mzc.zhoulong.xyz

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://boo.shuidangran.top

[Q36] 左连接
来源：http://snj.0kj1m.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hzc.yangfankeji.com

[Q37] 右连接
来源：http://teu.havefunace.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://nir.zhaomingkeji.xyz

[Q38] 全外连接（PostgreSQL）
来源：http://ncz.xziqi.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://qts.ydzc1.top

[Q39] 自连接（查上下级）
来源：http://vgy.jinqigfzy.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://gdk.birdmap.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://pta.shzxlz.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://yrx.haohaochexian.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://dyr.havefunace.top

[Q41] 多表连接
来源：http://dqq.jiagoushi.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://qry.jlsjyb.cn

JOIN users u ON u.id = o.user_id
来源：http://qhj.hfpthk.cn

JOIN products p ON p.id = o.product_id;
来源：http://onk.aizwys.cn

[Q42] 连接条件附加过滤
来源：http://kpg.cheryme.top

SELECT u.name, o.amount FROM users u
来源：http://etr.zdqjudy.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://qyv.yuanzhike.top

[Q43] 标量子查询
来源：http://hxd.yj20258888.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://xhe.smart0.xyz

[Q44] IN 子查询
来源：http://pha.guannengcc.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://abh.ppjwa.cn

[Q45] EXISTS 判断存在
来源：http://tgf.gotoacloud.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wbr.yanxiufei.cn

[Q46] NOT EXISTS 判断不存在
来源：http://kxt.jinyuanbaomall.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zcb.jinghuilouyu.cn

[Q47] 与平均值比较
来源：http://fty.fktsv.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://qwf.zhaomingkeji.xyz

[Q48] CTE 公用表表达式
来源：http://pdb.meibo888.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://yea.chenlongwang.top

SELECT * FROM t WHERE c > 5;
来源：http://emo.jinqigufen.top

[Q49] 更新单行
来源：http://ylk.quarkkingdee.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://afe.cdnleiting.top

[Q50] 批量更新
来源：http://nog.zhengqikj.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://vvo.yfazqb.com

[Q51] 用子查询更新
来源：http://bao.bbcook.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://qov.daria6918.cn

[Q52] 删除指定行
来源：http://yuu.gogol.net.cn

DELETE FROM users WHERE id = 10;
来源：http://aem.jinyuanbaomall.cn

[Q53] 按条件删除
来源：http://ksa.wangshuangyany.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://lmv.hfpthk.cn

[Q54] 清空表
来源：http://xrl.shanyushiyangkeji.top

TRUNCATE TABLE logs;
来源：http://cco.sweek.top

[Q55] 排名（并列占位）
来源：http://ofk.jqgfzy.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://bwr.zhaomingkeji.xyz

[Q56] 密集排名（并列不占位）
来源：http://ntz.xinyue.icu

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://sbc.meibo888.top

[Q57] 行号
来源：http://txx.jinyuanbaomall.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://oqy.hesvh.cn

[Q58] 累计求和
来源：http://eja.meibo888.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://vte.jqgfzy.top

[Q59] 分组内累计
来源：http://gwl.jianghu66.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://rrf.zhixingplan.top

[Q60] 取上一行 / 下一行
来源：http://qvx.hnqzz.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://uca.zycfv.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://udt.yuxming.cn

[Q61] 移动平均
来源：http://xic.xylfe.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ycn.hcnkem.com

[Q62] 分组占比
来源：http://wnl.bbcook.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://bhr.sjlbkw.cn

[Q63] 开启事务
来源：http://iaz.chenlongwang.top

START TRANSACTION;                -- 或 BEGIN
来源：http://auz.jinghuilouyu.cn

[Q64] 提交事务
来源：http://sfz.ydzc1.top

COMMIT;
来源：http://atm.xuanzx.com

[Q65] 回滚事务
来源：http://azd.jinghuilouyu.cn

ROLLBACK;
来源：http://iog.gotoacloud.top

[Q66] 行锁查询
来源：http://kiw.guowangkeji.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://jhj.52xcode.cn

[Q67] 设置隔离级别
来源：http://yqa.aizwys.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://kjn.zhijiandao.cn

[Q68] 保存点
来源：http://fdf.uphjek.com

SAVEPOINT sp1;
来源：http://kxm.gotoacloud.top

ROLLBACK TO sp1;
来源：http://hpa.jqgfzy.top

[Q69] 查看执行计划
来源：http://xwg.guowangkeji.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://jjz.52xcode.cn

[Q70] 更新统计信息
来源：http://caz.hnqzz.top

ANALYZE TABLE users;
来源：http://aet.gzhubu.top

[Q71] 查看建表语句
来源：http://job.sweek.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://txc.dianchejie.cn

[Q72] 查看索引
来源：http://aly.andypj.xyz

SHOW INDEX FROM users;
来源：http://fwy.jinghuilouyu.cn

[Q73] 查看表状态
来源：http://kst.hnxiangtu.top

SHOW TABLE STATUS LIKE 'users';
来源：http://pgs.yj20258888.top

[Q74] 强制使用索引
来源：http://nzo.zdbjq.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://gff.ehwqpu.com

[Q75] 日期格式化
来源：http://rss.epnwcf.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://lde.jqgfzy.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://kan.wangshuangyany.cn

[Q76] 按天统计
来源：http://lav.hnxiangtu.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://dmx.smart0.xyz

[Q77] 时间加减
来源：http://eos.sxryk.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://kyx.xylfe.cn

[Q78] 当前时间
来源：http://mty.havefunace.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://uer.tian-w.cn

[Q79] 字符串拼接
来源：http://lxd.svipenyu.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://syy.sufxvd.cn

[Q80] 字符串截取
来源：http://uhe.jlsjyb.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://eoz.xziqi.cn

[Q81] 字符串替换
来源：http://ktc.zhiwuduotai.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://xyp.ivvv.top

[Q82] 字符长度与字节长度
来源：http://hne.yongpay.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://uod.cucudq.cn

[Q83] 大小写转换
来源：http://lad.chenlongwang.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://iix.haohaochexian.top

[Q84] 去除首尾空格
来源：http://irv.birdmap.top

SELECT TRIM(name) FROM users;
来源：http://xnf.vqdsnc.cn

[Q85] 数值取整
来源：http://yvu.cqqwz.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://zwv.wangdashe.top

[Q86] 读取 JSON 字段
来源：http://tlm.shuidangran.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://yuz.fktsv.cn

[Q87] JSON 字段做条件
来源：http://hje.guowangkeji.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wmj.zhixingplan.top

[Q88] 行转列（条件聚合）
来源：http://btz.guannengcc.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://aqx.daxiang520.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mmb.tanke756.top

[Q89] 判断表是否存在
来源：http://yvf.andypj.xyz

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://fxy.nanxinkj.top

[Q90] 生成序号列
来源：http://ejz.jqgfzy.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://dts.fktsv.cn

================================================================================
来源：http://cwh.daria6918.cn

R. Bash 专题
来源：http://qju.iojbl.cn

================================================================================
来源：http://yyj.shuidangran.top

[R01] shebang 与严格模式
来源：http://fvo.zycfv.cn

#!/usr/bin/env bash
来源：http://skg.epnwcf.com

set -euo pipefail
来源：http://ypl.jinqigfzy.top

[R02] 变量赋值与使用
来源：http://fyg.c1oappe.top

name="Tom"; echo "$name"
来源：http://vql.zhengqikj.top

[R03] 只读变量
来源：http://lte.epnwcf.com

readonly PI=3.14
来源：http://wej.wangdashe.top

[R04] 位置参数
来源：http://rri.sufxvd.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://vdl.jinyuanbaomall.cn

[R05] 参数默认值
来源：http://ikc.ivvv.top

name="${1:-default}"
来源：http://pxm.gzhubu.top

[R06] 判断命令是否存在
来源：http://dxb.shanyushiyangkeji.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://dkg.xingfuxueyuan.xyz

[R07] if 判断文件
来源：http://jay.jqgfzy.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ajt.cucudq.cn

[R08] 数值比较
来源：http://ama.guannengcc.top

if (( a > b )); then echo "a 更大"; fi
来源：http://nxy.xziqi.cn

[R09] 字符串比较
来源：http://nqx.jyoumei.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://gxc.dashuyun.cn

[R10] 正则匹配
来源：http://zvb.xuetiantiany.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://xjz.sxryk.cn

[R11] case 多分支
来源：http://rla.gzhubu.top

case "$1" in
来源：http://xad.hesvh.cn

start) echo "启动" ;;
来源：http://wup.shzxlz.cn

stop)  echo "停止" ;;
来源：http://usi.fengsongda.top

*)     echo "未知命令" ;;
来源：http://esu.sufxvd.cn

esac
来源：http://kja.iojbl.cn

[R12] for 遍历文件
来源：http://sbv.tianlin.xyz

for f in *.txt; do echo "$f"; done
来源：http://ucp.haohaochexian.top

[R13] for 计数循环
来源：http://wdd.uphjek.com

for i in {1..10}; do echo "$i"; done
来源：http://srg.kuanghao11.cn

[R14] C 风格 for
来源：http://ugo.chenlongwang.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mea.shanyushiyangtech.top

[R15] while 逐行读文件
来源：http://omq.bbcook.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://bhj.ehwqpu.com

[R16] until 等待条件
来源：http://tga.gaohongyu789.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://izz.tanke756.top

[R17] 数组定义与取值
来源：http://ttd.mhx1999.top

arr=(a b c); echo "${arr[0]}"
来源：http://bzh.ctjpmb.com

[R18] 遍历数组
来源：http://dml.hnqzz.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://nwf.jinyuanbaomall.cn

[R19] 数组长度
来源：http://gnh.zhengqikj.top

echo "${#arr[@]}"
来源：http://vdl.ywan-chungtsiang.top

[R20] 关联数组（字典）
来源：http://nps.chenzaomai.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://cof.chenzaomai.com

[R21] 字符串长度
来源：http://abj.iojbl.cn

echo "${#s}"
来源：http://khh.hywenlv.cn

[R22] 截取子串
来源：http://dej.sufxvd.cn

echo "${s:0:5}"
来源：http://noy.sjlbkw.cn

[R23] 字符串替换
来源：http://zdi.chenzaomai.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://qkk.cheryme.top

[R24] 大小写转换
来源：http://ksl.yj20258888.top

echo "${s^^}"; echo "${s,,}"
来源：http://tdl.hnqzz.top

[R25] 去后缀 / 去前缀
来源：http://lte.ivvv.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://jjg.sufxvd.cn

[R26] 命令替换
来源：http://wib.nanxinkj.top

now=$(date +%F); echo "$now"
来源：http://siy.ywan-chungtsiang.top

[R27] 算术展开
来源：http://rfv.zhixingplan.top

echo $((1 + 2 * 3))
来源：http://kkp.kuanghao11.cn

[R28] 浮点运算
来源：http://jix.shanyushiyangtech.top

echo "scale=2; 10/3" | bc
来源：http://lus.zdbjq.cn

[R29] 定义函数
来源：http://ymz.dashuyun.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://san.meibo888.top

[R30] 函数返回状态码
来源：http://gpg.gzhubu.top

f() { return 0; }; f || echo "失败了"
来源：http://crh.guannengcc.top

[R31] 局部变量
来源：http://ywc.jinqigufen.top

f() { local x=1; echo "$x"; }
来源：http://uoy.epnwcf.com

[R32] 参数个数校验
来源：http://gqd.zdqjudy.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hcn.shanyushiyangtech.top

[R33] 捕获错误并提示行号
来源：http://txh.ywan-chungtsiang.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://fwp.chenjidiqi.icu

[R34] 退出时清理
来源：http://kwm.ydzc1.top

trap 'rm -f "$tmp"' EXIT
来源：http://poh.jqgfzy.top

[R35] 后台执行并等待
来源：http://qao.zhaomingkeji.xyz

sleep 5 & pid=$!; wait "$pid"
来源：http://nkz.52xcode.cn

[R36] 并发执行多个任务
来源：http://xxc.ehwqpu.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://axn.aizwys.cn

[R37] 把输出赋给变量
来源：http://pdm.xylfe.cn

files=$(ls -1)
来源：http://nok.vqdsnc.cn

[R38] 管道串联
来源：http://lrw.hnxiangtu.top

cat a.txt | grep -i error | wc -l
来源：http://kjz.aizwys.cn

[R39] 重定向标准输出与错误
来源：http://sqy.daxiang520.top

cmd > out.log 2>&1
来源：http://zls.havefunace.top

[R40] 追加写日志
来源：http://doc.hammf.cn

echo "log" >> out.log
来源：http://ibm.quarkkingdee.top

[R41] 丢弃输出
来源：http://gwd.aizwys.cn


<!-- 参考信息 -->