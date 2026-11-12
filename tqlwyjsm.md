代发 wailian999

CREATE TABLE users (
来源：http://lfv.hnqzz.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://yhd.zhixingplan.top

name VARCHAR(50) NOT NULL,
来源：http://cxj.shanyushiyangtech.top

email VARCHAR(100) UNIQUE,
来源：http://way.yj20258.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://zlz.tianlin.xyz

);
来源：http://prs.smart0.xyz

[Q02] 创建带外键的表
来源：http://kyk.hcnkem.com

CREATE TABLE orders (
来源：http://ukx.chenzaomai.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://qki.xuetiantiany.cn

user_id INT NOT NULL,
来源：http://vaj.hammf.cn

amount DECIMAL(10, 2),
来源：http://uut.fktsv.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://iwp.52xcode.cn

);
来源：http://owf.shangyingyoupin.top

[Q03] 增加列
来源：http://lms.0kj1m.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mye.sufxvd.cn

[Q04] 修改列类型
来源：http://vss.hesvh.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://jdn.yongpay.top

[Q05] 重命名列
来源：http://jsm.dashuyun.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ahm.shzxlz.cn

[Q06] 删除列
来源：http://rpq.snrcjt.cn

ALTER TABLE users DROP COLUMN age;
来源：http://blu.zhiwuduotai.top

[Q07] 删除表
来源：http://hjp.aizwys.cn

DROP TABLE IF EXISTS orders;
来源：http://fhk.ybcxt.top

[Q08] 创建普通索引
来源：http://roh.jyoumei.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://car.redwolf501.top

[Q09] 创建唯一索引
来源：http://xxb.yfazqb.com

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://bfm.chenzaomai.com

[Q10] 插入单行
来源：http://dbf.ybcxt.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mqn.uphjek.com

[Q11] 一次插入多行
来源：http://exc.nanxinkj.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://agz.zdqjudy.top

[Q12] 插入后取自增 ID
来源：http://afb.gotoacloud.top

INSERT INTO users (name) VALUES ('C');
来源：http://ttn.feifeiyinyue.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://tdg.sjlbkw.cn

[Q13] 忽略重复插入
来源：http://tyg.shzxlz.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://npy.jinqigufen.top

[Q14] 存在则更新（upsert）
来源：http://jvs.daria6918.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://xdr.ctjpmb.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://rqs.redwolf501.top

[Q15] 查询全部
来源：http://xbb.svipenyu.cn

SELECT * FROM users;
来源：http://kaw.redwolf501.top

[Q16] 查询指定列
来源：http://pap.hongshengwenyu.top

SELECT id, name FROM users;
来源：http://lho.aizwys.cn

[Q17] 条件查询
来源：http://ylg.jlsjyb.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://kjg.vqdsnc.cn

[Q18] 模糊匹配
来源：http://jge.hcnkem.com

SELECT * FROM users WHERE name LIKE '张%';
来源：http://cki.snrcjt.cn

[Q19] 范围查询
来源：http://zyw.c1oappe.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://zbm.c1oappe.top

[Q20] IN 列表
来源：http://dlv.bjfxy.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://kgw.wangshuangyany.cn

[Q21] 空值判断
来源：http://nub.hywenlv.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://pkw.meibo888.top

[Q22] 排序
来源：http://nlr.meibo888.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://vzi.c1oappe.top

[Q23] 分页
来源：http://wck.ivvv.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://vqc.xinyue.icu

[Q24] 去重
来源：http://jad.ivvv.top

SELECT DISTINCT city FROM users;
来源：http://owj.uphjek.com

[Q25] 只取前 N 条
来源：http://wur.hfpthk.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://pcp.dianchejie.cn

[Q26] 计数
来源：http://pht.yonumen.top

SELECT COUNT(*) FROM users;
来源：http://lvt.nanxinkj.top

[Q27] 条件计数
来源：http://xuf.jqgfzy.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://aqv.xingfuxueyuan.xyz

[Q28] 求和与平均
来源：http://hni.fengsongda.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://pyj.tarul.cn

[Q29] 最大最小值
来源：http://gjy.dashuyun.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://mgd.dashuyun.cn

[Q30] 分组统计
来源：http://odh.zhoulong.xyz

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://etn.tianlin.xyz

[Q31] 分组后过滤
来源：http://jxw.shanyushiyangtech.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ppn.shangyingyoupin.top

[Q32] 分组拼接字符串
来源：http://sbe.52xcode.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://pkt.hnxiangtu.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://yuv.redwolf501.top

[Q33] 多列分组
来源：http://exl.shangyingyoupin.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://aih.ydzc1.top

[Q34] 每组取第一条
来源：http://tyo.ybcxt.top

SELECT * FROM (
来源：http://gdu.hammf.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://oui.jinyuanbaomall.cn

) t WHERE rn = 1;
来源：http://dfn.hammf.cn

[Q35] 内连接
来源：http://bce.sjlbkw.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://tdw.zhiwuduotai.top

[Q36] 左连接
来源：http://jpc.chenzaomai.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://lsc.zhoulong.xyz

[Q37] 右连接
来源：http://zwg.smart0.xyz

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://xuy.jqgfzy.top

[Q38] 全外连接（PostgreSQL）
来源：http://krj.yvedp.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://cyl.xylfe.cn

[Q39] 自连接（查上下级）
来源：http://dci.fzhhl.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://kba.gotoacloud.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ycn.xuanzx.com

[Q40] 交叉连接（笛卡尔积）
来源：http://red.hywenlv.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://vrj.fktsv.cn

[Q41] 多表连接
来源：http://jim.shuidangran.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://egj.ehwqpu.com

JOIN users u ON u.id = o.user_id
来源：http://iik.jinyuanbaomall.cn

JOIN products p ON p.id = o.product_id;
来源：http://jfr.jlsjyb.cn

[Q42] 连接条件附加过滤
来源：http://uop.jlsjyb.cn

SELECT u.name, o.amount FROM users u
来源：http://yat.zhoulong.xyz

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://iuo.hfpthk.cn

[Q43] 标量子查询
来源：http://fcg.hcnkem.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://fwj.sxryk.cn

[Q44] IN 子查询
来源：http://mjn.kuanghao11.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://zyi.daria6918.cn

[Q45] EXISTS 判断存在
来源：http://upz.yonumen.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://dwx.tianlin.xyz

[Q46] NOT EXISTS 判断不存在
来源：http://oup.hongshengwenyu.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://yhd.c1oappe.top

[Q47] 与平均值比较
来源：http://nay.xuetiantiany.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ydi.daria6918.cn

[Q48] CTE 公用表表达式
来源：http://ukv.dashuyun.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://vvp.vehdjk.com

SELECT * FROM t WHERE c > 5;
来源：http://ebo.hnxiangtu.top

[Q49] 更新单行
来源：http://qld.smart0.xyz

UPDATE users SET status = 1 WHERE id = 10;
来源：http://fcp.sysykeji.top

[Q50] 批量更新
来源：http://pdt.feifeiyinyue.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://vho.hysaishi.cn

[Q51] 用子查询更新
来源：http://wob.ivvv.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://tkt.jinqigufen.top

[Q52] 删除指定行
来源：http://wzx.birdmap.top

DELETE FROM users WHERE id = 10;
来源：http://bkp.gogol.net.cn

[Q53] 按条件删除
来源：http://wuc.jqgfzy.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://pki.guannengcc.top

[Q54] 清空表
来源：http://wnm.xziqi.cn

TRUNCATE TABLE logs;
来源：http://qfq.ctjpmb.com

[Q55] 排名（并列占位）
来源：http://qlr.havefunace.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://zvl.jianghu66.top

[Q56] 密集排名（并列不占位）
来源：http://add.zycfv.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ffy.mhx1999.top

[Q57] 行号
来源：http://fvd.0kj1m.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ixu.meibo888.top

[Q58] 累计求和
来源：http://qgj.jinqigfzy.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://oen.smart0.xyz

[Q59] 分组内累计
来源：http://nlw.0kj1m.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://tql.zdqjudy.top

[Q60] 取上一行 / 下一行
来源：http://bjg.yj20258.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://kqi.chenzaomai.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://tjn.fzhhl.top

[Q61] 移动平均
来源：http://ixe.tianlin.xyz

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://thm.zhoulong.xyz

[Q62] 分组占比
来源：http://ued.dianchejie.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://uhf.mhx1999.top

[Q63] 开启事务
来源：http://naf.ehwqpu.com

START TRANSACTION;                -- 或 BEGIN
来源：http://qcu.jianghu66.top

[Q64] 提交事务
来源：http://mef.hfpthk.cn

COMMIT;
来源：http://ovg.xingfuxueyuan.xyz

[Q65] 回滚事务
来源：http://lyw.zhiwuduotai.top

ROLLBACK;
来源：http://msd.aibaodan.cn

[Q66] 行锁查询
来源：http://fdp.sweek.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://csf.nwbrower.top

[Q67] 设置隔离级别
来源：http://rgd.hfpthk.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://vui.tanke756.top

[Q68] 保存点
来源：http://qcy.c1oappe.top

SAVEPOINT sp1;
来源：http://eeq.cashguo.top

ROLLBACK TO sp1;
来源：http://yje.ppjwa.cn

[Q69] 查看执行计划
来源：http://vlo.havefunace.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://fjo.zhixingplan.top

[Q70] 更新统计信息
来源：http://nig.shanyushiyangkeji.top

ANALYZE TABLE users;
来源：http://qgp.zhaomingkeji.xyz

[Q71] 查看建表语句
来源：http://mmj.52xcode.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://rmj.quarkkingdee.top

[Q72] 查看索引
来源：http://lzl.vehdjk.com

SHOW INDEX FROM users;
来源：http://htt.316326.xyz

[Q73] 查看表状态
来源：http://yue.yj20258888.top

SHOW TABLE STATUS LIKE 'users';
来源：http://xar.xuetiantiany.cn

[Q74] 强制使用索引
来源：http://odh.ivvv.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://oaj.pengpengdd.cyou

[Q75] 日期格式化
来源：http://dgh.pengpengdd.cyou

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mky.fktsv.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mxk.shzxlz.cn

[Q76] 按天统计
来源：http://tfp.tarul.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://dek.ywan-chungtsiang.top

[Q77] 时间加减
来源：http://kit.svipenyu.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://xhg.fengsongda.top

[Q78] 当前时间
来源：http://nrw.c1oappe.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://fcv.nwbrower.top

[Q79] 字符串拼接
来源：http://xrg.yj20258.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://jyo.nwbrower.top

[Q80] 字符串截取
来源：http://dfg.yj20258.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://elu.sysykeji.top

[Q81] 字符串替换
来源：http://ubn.zhengqikj.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://qio.zhijiandao.cn

[Q82] 字符长度与字节长度
来源：http://gwo.haohaochexian.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://raa.jyoumei.cn

[Q83] 大小写转换
来源：http://tob.jinqigufen.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://vtc.feifeiyinyue.top

[Q84] 去除首尾空格
来源：http://guo.tian-w.cn

SELECT TRIM(name) FROM users;
来源：http://jto.haohaochexian.top

[Q85] 数值取整
来源：http://pxg.xinyue.icu

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wob.xingfuxueyuan.xyz

[Q86] 读取 JSON 字段
来源：http://avd.vehdjk.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://yhr.chenjidiqi.icu

[Q87] JSON 字段做条件
来源：http://mcs.fktsv.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://exj.bbcook.cn

[Q88] 行转列（条件聚合）
来源：http://kul.snrcjt.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://stx.birdmap.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://nyc.ehwqpu.com

[Q89] 判断表是否存在
来源：http://mpx.quarkkingdee.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ges.snrcjt.cn

[Q90] 生成序号列
来源：http://arc.sxryk.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://nhs.xingfuxueyuan.xyz

================================================================================
来源：http://ger.meibo888.top

R. Bash 专题
来源：http://fcg.xziqi.cn

================================================================================
来源：http://kpb.yfazqb.com

[R01] shebang 与严格模式
来源：http://wle.dianchejie.cn

#!/usr/bin/env bash
来源：http://aiw.andypj.xyz

set -euo pipefail
来源：http://yml.havefunace.top

[R02] 变量赋值与使用
来源：http://zjl.xingfuxueyuan.xyz

name="Tom"; echo "$name"
来源：http://qgk.ydzc1.top

[R03] 只读变量
来源：http://mqr.jianghu66.top

readonly PI=3.14
来源：http://uul.uphjek.com

[R04] 位置参数
来源：http://typ.yvedp.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://rmq.zhoulong.xyz

[R05] 参数默认值
来源：http://wqb.meibo888.top

name="${1:-default}"
来源：http://pis.shuidangran.top

[R06] 判断命令是否存在
来源：http://wlg.iojbl.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ktr.jqgufenzy.top

[R07] if 判断文件
来源：http://zvh.wangshuangyany.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wum.316326.xyz

[R08] 数值比较
来源：http://vli.ppjwa.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://blv.yj20258.top

[R09] 字符串比较
来源：http://znc.shanyushiyangkeji.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://nze.birdmap.top

[R10] 正则匹配
来源：http://bgw.jianghu66.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://utv.jinghuilouyu.cn

[R11] case 多分支
来源：http://bjd.yueranfly.top

case "$1" in
来源：http://nol.cucudq.cn

start) echo "启动" ;;
来源：http://qhb.zhaomingkeji.xyz

stop)  echo "停止" ;;
来源：http://vru.shuidangran.top

*)     echo "未知命令" ;;
来源：http://foq.svipenyu.cn

esac
来源：http://soj.zhijiandao.cn

[R12] for 遍历文件
来源：http://kyo.hesvh.cn

for f in *.txt; do echo "$f"; done
来源：http://xcn.xziqi.cn

[R13] for 计数循环
来源：http://esu.jinghuilouyu.cn

for i in {1..10}; do echo "$i"; done
来源：http://vwa.tian-w.cn

[R14] C 风格 for
来源：http://rbk.c1oappe.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://nsb.bjfxy.top

[R15] while 逐行读文件
来源：http://ptq.yangfankeji.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://kvh.jinyuanbaomall.cn

[R16] until 等待条件
来源：http://csb.zdbjq.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://huk.zhijiandao.cn

[R17] 数组定义与取值
来源：http://rzg.zdqjudy.top

arr=(a b c); echo "${arr[0]}"
来源：http://non.zdbjq.cn

[R18] 遍历数组
来源：http://bda.ctjpmb.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://xyo.yueranfly.top

[R19] 数组长度
来源：http://gsu.vqdsnc.cn

echo "${#arr[@]}"
来源：http://ssb.ydzc1.top

[R20] 关联数组（字典）
来源：http://jaa.tanke756.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://tzj.yj20258888.top

[R21] 字符串长度
来源：http://rnv.snrcjt.cn

echo "${#s}"
来源：http://djk.tanke756.top

[R22] 截取子串
来源：http://xik.zhengqikj.top

echo "${s:0:5}"
来源：http://cyv.redwolf501.top

[R23] 字符串替换
来源：http://zqv.chenjidiqi.icu

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://nha.cheryme.top

[R24] 大小写转换
来源：http://bga.hnqzz.top

echo "${s^^}"; echo "${s,,}"
来源：http://lpw.zhongyouzk.top

[R25] 去后缀 / 去前缀
来源：http://pdk.bbcook.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://mar.ppjwa.cn

[R26] 命令替换
来源：http://ntf.daxiang520.top

now=$(date +%F); echo "$now"
来源：http://egk.sjlbkw.cn

[R27] 算术展开
来源：http://zba.guannengcc.top

echo $((1 + 2 * 3))
来源：http://tav.guowangkeji.top

[R28] 浮点运算
来源：http://cer.zhoulong.xyz

echo "scale=2; 10/3" | bc
来源：http://wlc.nwbrower.top

[R29] 定义函数
来源：http://art.cucudq.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://gnc.fzhhl.top

[R30] 函数返回状态码
来源：http://cih.tanke756.top

f() { return 0; }; f || echo "失败了"
来源：http://sxp.hcnkem.com

[R31] 局部变量
来源：http://fvt.zhoulong.xyz

f() { local x=1; echo "$x"; }
来源：http://ikg.sweek.top

[R32] 参数个数校验
来源：http://zok.zdbjq.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://zkc.xingfuxueyuan.xyz

[R33] 捕获错误并提示行号
来源：http://fuu.cdnleiting.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://gjy.aizwys.cn

[R34] 退出时清理
来源：http://uja.zhaomingkeji.xyz

trap 'rm -f "$tmp"' EXIT
来源：http://fjx.smart0.xyz

[R35] 后台执行并等待
来源：http://erm.yvedp.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://mlf.jqgufenzy.top

[R36] 并发执行多个任务
来源：http://krp.cashguo.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mir.yj20258.top

[R37] 把输出赋给变量
来源：http://njk.jqgfzy.top

files=$(ls -1)
来源：http://mdt.chenzaomai.com

[R38] 管道串联
来源：http://ddu.zhengqikj.top

cat a.txt | grep -i error | wc -l
来源：http://nwh.gogol.net.cn

[R39] 重定向标准输出与错误
来源：http://ejc.zdbjq.cn

cmd > out.log 2>&1
来源：http://cad.yj20258.top

[R40] 追加写日志
来源：http://efq.jqgfzy.top

echo "log" >> out.log
来源：http://tci.meibo888.top

[R41] 丢弃输出
来源：http://pwo.dianchejie.cn

cmd >/dev/null 2>&1
来源：http://dlm.xuetiantiany.cn

[R42] 输入重定向
来源：http://asj.smart0.xyz

wc -l < a.txt
来源：http://wao.ehwqpu.com

[R43] 按名字查找文件
来源：http://gjd.sxryk.cn

find . -name "*.log" -type f
来源：http://mxc.chenjidiqi.icu

[R44] 按修改时间查找
来源：http://zik.gotoacloud.top

find . -mtime -7 -type f
来源：http://gpd.hammf.cn

[R45] 批量删除
来源：http://jtv.jiagoushi.top


<!-- 参考信息 -->