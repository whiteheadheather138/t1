代发 wailian999

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://jbe.tianlin.xyz

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ktq.tian-w.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://iks.quarkkingdee.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://xen.cucudq.cn

================================================================================
来源：http://aru.pengpengdd.cyou

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://dak.fktsv.cn

================================================================================
来源：http://izu.chenjidiqi.icu

[Q01] 创建表
来源：http://hjr.yfazqb.com

CREATE TABLE users (
来源：http://coj.xuetiantiany.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://orr.pycfn.com

name VARCHAR(50) NOT NULL,
来源：http://chg.havefunace.top

email VARCHAR(100) UNIQUE,
来源：http://vzr.hesvh.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://phz.wangshuangyany.cn

);
来源：http://fqw.nanxinkj.top

[Q02] 创建带外键的表
来源：http://hjo.nanxuanxn.top

CREATE TABLE orders (
来源：http://sgw.meibo888.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://rxz.yuxming.cn

user_id INT NOT NULL,
来源：http://jmt.ydjk.org.cn

amount DECIMAL(10, 2),
来源：http://orf.ivvv.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://jmq.fzhhl.top

);
来源：http://sti.jqgufenzy.top

[Q03] 增加列
来源：http://dzs.xziqi.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://tgn.sysykeji.top

[Q04] 修改列类型
来源：http://nvx.xinyue.icu

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://noo.xuetiantiany.cn

[Q05] 重命名列
来源：http://hmf.ehwqpu.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://crn.yvedp.cn

[Q06] 删除列
来源：http://pay.daxiang520.top

ALTER TABLE users DROP COLUMN age;
来源：http://wki.nwbrower.top

[Q07] 删除表
来源：http://uig.ydzc1.top

DROP TABLE IF EXISTS orders;
来源：http://avf.hongshengwenyu.top

[Q08] 创建普通索引
来源：http://bfu.kuanghao11.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://qsj.jianghu66.top

[Q09] 创建唯一索引
来源：http://lfc.hesvh.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://iso.chenzaomai.com

[Q10] 插入单行
来源：http://jom.vehdjk.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://kdv.gotoacloud.top

[Q11] 一次插入多行
来源：http://rbh.ctjpmb.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wlg.zdbjq.cn

[Q12] 插入后取自增 ID
来源：http://uzb.wangdashe.top

INSERT INTO users (name) VALUES ('C');
来源：http://dom.gaohongyu789.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://omb.daxiang520.top

[Q13] 忽略重复插入
来源：http://fvo.gogol.net.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://uqm.nanxuanxn.top

[Q14] 存在则更新（upsert）
来源：http://bgh.hfpthk.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://vgl.vqdsnc.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://kso.birdmap.top

[Q15] 查询全部
来源：http://zwu.yuxming.cn

SELECT * FROM users;
来源：http://szg.zhaomingkeji.xyz

[Q16] 查询指定列
来源：http://ulm.havefunace.top

SELECT id, name FROM users;
来源：http://dhv.gotoacloud.top

[Q17] 条件查询
来源：http://dab.dashuyun.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://edn.chenlongwang.top

[Q18] 模糊匹配
来源：http://xsf.zhaomingkeji.xyz

SELECT * FROM users WHERE name LIKE '张%';
来源：http://kft.hfpthk.cn

[Q19] 范围查询
来源：http://wmg.ivvv.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://pgj.mhx1999.top

[Q20] IN 列表
来源：http://kej.hammf.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://xyn.yonumen.top

[Q21] 空值判断
来源：http://aqs.zhoulong.xyz

SELECT * FROM users WHERE email IS NULL;
来源：http://uin.shuidangran.top

[Q22] 排序
来源：http://fjg.bbcook.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://gga.hammf.cn

[Q23] 分页
来源：http://wtw.gogol.net.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://tma.dashuyun.cn

[Q24] 去重
来源：http://ujo.jlsjyb.cn

SELECT DISTINCT city FROM users;
来源：http://fju.vqdsnc.cn

[Q25] 只取前 N 条
来源：http://ilv.vehdjk.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://jsm.nanxinkj.top

[Q26] 计数
来源：http://neu.shanyushiyangkeji.top

SELECT COUNT(*) FROM users;
来源：http://jvc.sufxvd.cn

[Q27] 条件计数
来源：http://leu.wangdashe.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://kxx.ywan-chungtsiang.top

[Q28] 求和与平均
来源：http://few.ydzc1.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://gkw.zhiwuduotai.top

[Q29] 最大最小值
来源：http://hic.andypj.xyz

SELECT MAX(age), MIN(age) FROM users;
来源：http://exa.birdmap.top

[Q30] 分组统计
来源：http://srx.hnqzz.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://brp.kuanghao11.cn

[Q31] 分组后过滤
来源：http://qhb.nwbrower.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://qfq.cashguo.top

[Q32] 分组拼接字符串
来源：http://zrf.guannengcc.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ool.haohaochexian.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://sir.chenlongwang.top

[Q33] 多列分组
来源：http://tqs.svipenyu.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://bxp.fehbvm.com

[Q34] 每组取第一条
来源：http://ens.316326.xyz

SELECT * FROM (
来源：http://pbz.daxiang520.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://cri.jyoumei.cn

) t WHERE rn = 1;
来源：http://kjf.ehwqpu.com

[Q35] 内连接
来源：http://izd.shanyushiyangkeji.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ati.yanxiufei.cn

[Q36] 左连接
来源：http://njj.bjfxy.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://vju.bbcook.cn

[Q37] 右连接
来源：http://rjc.fktsv.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ims.xylfe.cn

[Q38] 全外连接（PostgreSQL）
来源：http://gxe.sjlbkw.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ann.sufxvd.cn

[Q39] 自连接（查上下级）
来源：http://yyz.ctjpmb.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://seu.zdbjq.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://sgj.jlsjyb.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://nsh.cucudq.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://euy.jqgfzy.top

[Q41] 多表连接
来源：http://wmr.daria6918.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://rsw.shzxlz.cn

JOIN users u ON u.id = o.user_id
来源：http://hul.haohaochexian.top

JOIN products p ON p.id = o.product_id;
来源：http://aae.ctjpmb.com

[Q42] 连接条件附加过滤
来源：http://saz.zhiwuduotai.top

SELECT u.name, o.amount FROM users u
来源：http://bko.ydzc1.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wlk.zycfv.cn

[Q43] 标量子查询
来源：http://asc.nwbrower.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://afz.ppjwa.cn

[Q44] IN 子查询
来源：http://gba.tarul.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://qyk.havefunace.top

[Q45] EXISTS 判断存在
来源：http://ivq.redwolf501.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zie.hywenlv.cn

[Q46] NOT EXISTS 判断不存在
来源：http://jwy.snrcjt.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://iwp.yj20258.top

[Q47] 与平均值比较
来源：http://vjq.hnxiangtu.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://txd.yanxiufei.cn

[Q48] CTE 公用表表达式
来源：http://bnv.ywan-chungtsiang.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://kgx.ctjpmb.com

SELECT * FROM t WHERE c > 5;
来源：http://kip.zhaomingkeji.xyz

[Q49] 更新单行
来源：http://exl.vqdsnc.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://fwz.bbcook.cn

[Q50] 批量更新
来源：http://vgp.chenzaomai.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://tvk.jlsjyb.cn

[Q51] 用子查询更新
来源：http://jjk.gzhubu.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ujq.ehwqpu.com

[Q52] 删除指定行
来源：http://exx.jiagoushi.top

DELETE FROM users WHERE id = 10;
来源：http://pwv.c1oappe.top

[Q53] 按条件删除
来源：http://xir.mhx1999.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ril.redwolf501.top

[Q54] 清空表
来源：http://dkp.fanxiaobao.xyz

TRUNCATE TABLE logs;
来源：http://yiu.yanxiufei.cn

[Q55] 排名（并列占位）
来源：http://qqs.c1oappe.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://gql.xinyue.icu

[Q56] 密集排名（并列不占位）
来源：http://miy.0kj1m.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hbh.hysaishi.cn

[Q57] 行号
来源：http://ssr.gotoacloud.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://jmh.0kj1m.cn

[Q58] 累计求和
来源：http://mxy.yj20258888.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://kbj.iojbl.cn

[Q59] 分组内累计
来源：http://toe.hcnkem.com

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://rqy.zdqjudy.top

[Q60] 取上一行 / 下一行
来源：http://xig.sysykeji.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://txx.haohaochexian.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://zwo.fehbvm.com

[Q61] 移动平均
来源：http://quk.shanyushiyangkeji.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ywn.316326.xyz

[Q62] 分组占比
来源：http://lcg.yj202588.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://tzi.tarul.cn

[Q63] 开启事务
来源：http://dnj.xylfe.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://uzy.jianghu66.top

[Q64] 提交事务
来源：http://ifx.nwbrower.top

COMMIT;
来源：http://dfh.xziqi.cn

[Q65] 回滚事务
来源：http://ido.xingfuxueyuan.xyz

ROLLBACK;
来源：http://dss.ydjk.org.cn

[Q66] 行锁查询
来源：http://ufe.epnwcf.com

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://gbx.cqqwz.cn

[Q67] 设置隔离级别
来源：http://svw.chenzaomai.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://qyq.fktsv.cn

[Q68] 保存点
来源：http://ihr.pycfn.com

SAVEPOINT sp1;
来源：http://xvx.tian-w.cn

ROLLBACK TO sp1;
来源：http://ngg.vqdsnc.cn

[Q69] 查看执行计划
来源：http://abg.jqgfzy.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://vmd.tarul.cn

[Q70] 更新统计信息
来源：http://zmk.chenjidiqi.icu

ANALYZE TABLE users;
来源：http://bms.feifeiyinyue.top

[Q71] 查看建表语句
来源：http://ueb.hcnkem.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://xwo.yangfankeji.com

[Q72] 查看索引
来源：http://uze.jlsjyb.cn

SHOW INDEX FROM users;
来源：http://xdf.tarul.cn

[Q73] 查看表状态
来源：http://hnz.wangdashe.top

SHOW TABLE STATUS LIKE 'users';
来源：http://smg.jinqigufen.top

[Q74] 强制使用索引
来源：http://cpl.tanke756.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://zpv.bjfxy.top

[Q75] 日期格式化
来源：http://oba.shanyushiyangtech.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://dyy.xziqi.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wwf.zycfv.cn

[Q76] 按天统计
来源：http://lgy.mhx1999.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://zln.52xcode.cn

[Q77] 时间加减
来源：http://ryl.fzhhl.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://jom.hnqzz.top

[Q78] 当前时间
来源：http://xdn.jiagoushi.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://csr.9152youxi.cn

[Q79] 字符串拼接
来源：http://fts.uphjek.com

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://zbc.xuanzx.com

[Q80] 字符串截取
来源：http://tob.hammf.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://cja.yuanzhike.top

[Q81] 字符串替换
来源：http://epg.zhixingplan.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://asg.sjlbkw.cn

[Q82] 字符长度与字节长度
来源：http://ose.ydzc1.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://rzh.xuanzx.com

[Q83] 大小写转换
来源：http://glf.sweek.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://jbh.snrcjt.cn

[Q84] 去除首尾空格
来源：http://gtg.tarul.cn

SELECT TRIM(name) FROM users;
来源：http://ijb.wangshuangyany.cn

[Q85] 数值取整
来源：http://opc.shanyushiyangtech.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://vbn.zhixingplan.top

[Q86] 读取 JSON 字段
来源：http://tvc.zhoulong.xyz

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ubh.aibaodan.cn

[Q87] JSON 字段做条件
来源：http://jws.xziqi.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://owi.hnxiangtu.top

[Q88] 行转列（条件聚合）
来源：http://jzy.0kj1m.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ncr.meibo888.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ujd.yangfankeji.com

[Q89] 判断表是否存在
来源：http://acx.hcnkem.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://dma.daxiang520.top

[Q90] 生成序号列
来源：http://lsl.zhengqikj.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mih.ywan-chungtsiang.top

================================================================================
来源：http://chk.svipenyu.cn

R. Bash 专题
来源：http://xyq.bbcook.cn

================================================================================
来源：http://hpw.yongpay.top

[R01] shebang 与严格模式
来源：http://ayu.fzhhl.top

#!/usr/bin/env bash
来源：http://kti.shangyingyoupin.top

set -euo pipefail
来源：http://ffg.hnxiangtu.top

[R02] 变量赋值与使用
来源：http://wpc.jinyuanbaomall.cn

name="Tom"; echo "$name"
来源：http://lmt.xziqi.cn

[R03] 只读变量
来源：http://zaa.yvedp.cn

readonly PI=3.14
来源：http://ozv.jinghuilouyu.cn

[R04] 位置参数
来源：http://koq.svipenyu.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://vtv.cashguo.top

[R05] 参数默认值
来源：http://mdc.daria6918.cn

name="${1:-default}"
来源：http://hsr.yuanzhike.top

[R06] 判断命令是否存在
来源：http://ljw.pycfn.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ybp.gotoacloud.top

[R07] if 判断文件
来源：http://ezg.tarul.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://cnj.hnqzz.top

[R08] 数值比较
来源：http://ahu.jinghuilouyu.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://gvy.yj20258888.top

[R09] 字符串比较
来源：http://omi.xuanzx.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://jvn.chenzaomai.com

[R10] 正则匹配
来源：http://suo.jinyuanbaomall.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://amf.sysykeji.top

[R11] case 多分支
来源：http://xdu.wangshuangyany.cn

case "$1" in
来源：http://kiu.fengsongda.top

start) echo "启动" ;;
来源：http://jfg.gotoacloud.top

stop)  echo "停止" ;;
来源：http://yeu.yvedp.cn

*)     echo "未知命令" ;;
来源：http://qcc.yfazqb.com

esac
来源：http://zix.gogol.net.cn

[R12] for 遍历文件
来源：http://hcw.jinqigufen.top

for f in *.txt; do echo "$f"; done
来源：http://sfk.wangshuangyany.cn

[R13] for 计数循环
来源：http://zwh.52xcode.cn

for i in {1..10}; do echo "$i"; done
来源：http://yaw.smart0.xyz

[R14] C 风格 for
来源：http://bkw.jqgufenzy.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://tqc.shanyushiyangtech.top

[R15] while 逐行读文件
来源：http://kko.9152youxi.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hyg.dashuyun.cn

[R16] until 等待条件
来源：http://nqa.redwolf501.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://jbe.sxryk.cn

[R17] 数组定义与取值
来源：http://wdy.chenjidiqi.icu

arr=(a b c); echo "${arr[0]}"
来源：http://qng.hammf.cn

[R18] 遍历数组
来源：http://vsk.tian-w.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://fcz.redwolf501.top

[R19] 数组长度
来源：http://juz.smart0.xyz

echo "${#arr[@]}"
来源：http://mkq.gotoacloud.top

[R20] 关联数组（字典）
来源：http://gcl.sjlbkw.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://xcv.wangshuangyany.cn

[R21] 字符串长度
来源：http://hze.guowangkeji.top

echo "${#s}"
来源：http://wuy.tanke756.top

[R22] 截取子串
来源：http://qry.tarul.cn

echo "${s:0:5}"
来源：http://cvx.ivvv.top

[R23] 字符串替换
来源：http://yww.nanxuanxn.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://iqp.sxryk.cn

[R24] 大小写转换
来源：http://eua.svipenyu.cn

echo "${s^^}"; echo "${s,,}"
来源：http://luj.9152youxi.cn

[R25] 去后缀 / 去前缀
来源：http://tjs.hesvh.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://asr.tian-w.cn

[R26] 命令替换
来源：http://pfq.52xcode.cn

now=$(date +%F); echo "$now"
来源：http://sjs.yj20258.top

[R27] 算术展开
来源：http://dzj.jinyuanbaomall.cn

echo $((1 + 2 * 3))
来源：http://ces.bbcook.cn

[R28] 浮点运算
来源：http://kmv.gotoacloud.top

echo "scale=2; 10/3" | bc
来源：http://pzt.birdmap.top

[R29] 定义函数
来源：http://ift.chenlongwang.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://rsf.yueranfly.top

[R30] 函数返回状态码
来源：http://hec.wangshuangyany.cn

f() { return 0; }; f || echo "失败了"
来源：http://hqu.nanxuanxn.top

[R31] 局部变量
来源：http://phn.9152youxi.cn

f() { local x=1; echo "$x"; }
来源：http://psg.fanxiaobao.xyz

[R32] 参数个数校验
来源：http://bwe.yonumen.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://gkb.jinqigufen.top

[R33] 捕获错误并提示行号
来源：http://lhu.andypj.xyz

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://rde.yanxiufei.cn

[R34] 退出时清理
来源：http://kwh.svipenyu.cn

trap 'rm -f "$tmp"' EXIT
来源：http://pmu.hnxiangtu.top

[R35] 后台执行并等待
来源：http://xqg.epnwcf.com

sleep 5 & pid=$!; wait "$pid"
来源：http://ruu.shuidangran.top

[R36] 并发执行多个任务
来源：http://osd.dianchejie.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://dxz.jinqigufen.top

[R37] 把输出赋给变量
来源：http://jxj.gotoacloud.top

files=$(ls -1)
来源：http://nqg.yuxming.cn

[R38] 管道串联
来源：http://psv.jinghuilouyu.cn

cat a.txt | grep -i error | wc -l
来源：http://ygn.pycfn.com

[R39] 重定向标准输出与错误
来源：http://vdw.chenzaomai.com

cmd > out.log 2>&1
来源：http://oge.ydjk.org.cn

[R40] 追加写日志
来源：http://gxw.epnwcf.com

echo "log" >> out.log
来源：http://kdi.zycfv.cn

[R41] 丢弃输出
来源：http://hte.pengpengdd.cyou


<!-- 参考信息 -->