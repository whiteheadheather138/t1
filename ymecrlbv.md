代发 wailian999

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://pzz.chenlongwang.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://exc.xingfuxueyuan.xyz

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://gni.xingfuxueyuan.xyz

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://uwm.smart0.xyz

================================================================================
来源：http://qab.guannengcc.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://nbo.52xcode.cn

================================================================================
来源：http://mkc.tian-w.cn

[Q01] 创建表
来源：http://nzd.cashguo.top

CREATE TABLE users (
来源：http://lgc.shuidangran.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mcb.yuanzhike.top

name VARCHAR(50) NOT NULL,
来源：http://fgx.nanxuanxn.top

email VARCHAR(100) UNIQUE,
来源：http://nzi.tian-w.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://bwx.quarkkingdee.top

);
来源：http://imv.316326.xyz

[Q02] 创建带外键的表
来源：http://uwc.zhixingplan.top

CREATE TABLE orders (
来源：http://xoy.sxryk.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://bis.redwolf501.top

user_id INT NOT NULL,
来源：http://ecx.xylfe.cn

amount DECIMAL(10, 2),
来源：http://idv.zdbjq.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://yqm.redwolf501.top

);
来源：http://ufy.jqgufenzy.top

[Q03] 增加列
来源：http://ltz.tarul.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://cjj.zhixingplan.top

[Q04] 修改列类型
来源：http://ogg.gogol.net.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wwh.zhaomingkeji.xyz

[Q05] 重命名列
来源：http://rtt.cqqwz.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://gki.iojbl.cn

[Q06] 删除列
来源：http://vtx.ydzc1.top

ALTER TABLE users DROP COLUMN age;
来源：http://zwc.tarul.cn

[Q07] 删除表
来源：http://dwn.svipenyu.cn

DROP TABLE IF EXISTS orders;
来源：http://ytf.tianlin.xyz

[Q08] 创建普通索引
来源：http://nbe.daxiang520.top

CREATE INDEX idx_users_email ON users(email);
来源：http://kvp.yanxiufei.cn

[Q09] 创建唯一索引
来源：http://sub.c1oappe.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://cih.hnxiangtu.top

[Q10] 插入单行
来源：http://qms.yvedp.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mlg.pengpengdd.cyou

[Q11] 一次插入多行
来源：http://llz.aibaodan.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://rjw.fanxiaobao.xyz

[Q12] 插入后取自增 ID
来源：http://riv.smart0.xyz

INSERT INTO users (name) VALUES ('C');
来源：http://peg.gotoacloud.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://efv.yfazqb.com

[Q13] 忽略重复插入
来源：http://wrb.tian-w.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://zva.daxiang520.top

[Q14] 存在则更新（upsert）
来源：http://zyq.dianchejie.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://use.ydzc1.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://xus.xylfe.cn

[Q15] 查询全部
来源：http://jam.yj20258.top

SELECT * FROM users;
来源：http://ngv.yanxiufei.cn

[Q16] 查询指定列
来源：http://god.jinghuilouyu.cn

SELECT id, name FROM users;
来源：http://azh.wangdashe.top

[Q17] 条件查询
来源：http://ciw.tianlin.xyz

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hfo.daria6918.cn

[Q18] 模糊匹配
来源：http://xxr.zhaomingkeji.xyz

SELECT * FROM users WHERE name LIKE '张%';
来源：http://cgn.xylfe.cn

[Q19] 范围查询
来源：http://baw.uphjek.com

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hkl.sweek.top

[Q20] IN 列表
来源：http://bre.bbcook.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://skv.feifeiyinyue.top

[Q21] 空值判断
来源：http://ool.hnqzz.top

SELECT * FROM users WHERE email IS NULL;
来源：http://ztm.tianlin.xyz

[Q22] 排序
来源：http://fku.yangfankeji.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://vye.ydjk.org.cn

[Q23] 分页
来源：http://qyp.jyoumei.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ezq.jlsjyb.cn

[Q24] 去重
来源：http://gkk.sxryk.cn

SELECT DISTINCT city FROM users;
来源：http://qld.jiagoushi.top

[Q25] 只取前 N 条
来源：http://hdb.chenjidiqi.icu

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hkg.xuetiantiany.cn

[Q26] 计数
来源：http://mtl.shangyingyoupin.top

SELECT COUNT(*) FROM users;
来源：http://kof.kuanghao11.cn

[Q27] 条件计数
来源：http://mdi.vqdsnc.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://koz.c1oappe.top

[Q28] 求和与平均
来源：http://zwe.9152youxi.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://dui.sxryk.cn

[Q29] 最大最小值
来源：http://ngy.aibaodan.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://zpb.hfpthk.cn

[Q30] 分组统计
来源：http://kvj.tanke756.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://jcl.chenlongwang.top

[Q31] 分组后过滤
来源：http://pks.jianghu66.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://gdc.aizwys.cn

[Q32] 分组拼接字符串
来源：http://yqq.yj202588.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://dvz.hnxiangtu.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://jws.yueranfly.top

[Q33] 多列分组
来源：http://zqw.shanyushiyangtech.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://xxk.316326.xyz

[Q34] 每组取第一条
来源：http://xbi.xuetiantiany.cn

SELECT * FROM (
来源：http://ahj.cheryme.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://jde.ehwqpu.com

) t WHERE rn = 1;
来源：http://ubr.hammf.cn

[Q35] 内连接
来源：http://lch.ydjk.org.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://rve.nanxinkj.top

[Q36] 左连接
来源：http://xnu.cheryme.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://fig.ydjk.org.cn

[Q37] 右连接
来源：http://fgo.shanyushiyangtech.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://jpv.wangshuangyany.cn

[Q38] 全外连接（PostgreSQL）
来源：http://zrw.fehbvm.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://yir.gzhubu.top

[Q39] 自连接（查上下级）
来源：http://duw.jinghuilouyu.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://jtu.jqgfzy.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://llr.shangyingyoupin.top

[Q40] 交叉连接（笛卡尔积）
来源：http://zag.sufxvd.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://skb.gzhubu.top

[Q41] 多表连接
来源：http://tqx.sysykeji.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://qol.pycfn.com

JOIN users u ON u.id = o.user_id
来源：http://dcn.fehbvm.com

JOIN products p ON p.id = o.product_id;
来源：http://uae.fengsongda.top

[Q42] 连接条件附加过滤
来源：http://qsm.cqqwz.cn

SELECT u.name, o.amount FROM users u
来源：http://czu.yueranfly.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://qgf.dianchejie.cn

[Q43] 标量子查询
来源：http://sbg.vehdjk.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://svb.0kj1m.cn

[Q44] IN 子查询
来源：http://gua.guannengcc.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mje.zycfv.cn

[Q45] EXISTS 判断存在
来源：http://mov.cucudq.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ekh.gzhubu.top

[Q46] NOT EXISTS 判断不存在
来源：http://vrz.jinghuilouyu.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://swx.xingfuxueyuan.xyz

[Q47] 与平均值比较
来源：http://cuv.andypj.xyz

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://tgi.hongshengwenyu.top

[Q48] CTE 公用表表达式
来源：http://zkz.cdnleiting.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://yns.shuidangran.top

SELECT * FROM t WHERE c > 5;
来源：http://dir.uphjek.com

[Q49] 更新单行
来源：http://fck.guannengcc.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://sov.meibo888.top

[Q50] 批量更新
来源：http://hgc.jinghuilouyu.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://vqe.zhengqikj.top

[Q51] 用子查询更新
来源：http://wuk.jianghu66.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mcx.zhoulong.xyz

[Q52] 删除指定行
来源：http://ryq.aibaodan.cn

DELETE FROM users WHERE id = 10;
来源：http://olw.zhoulong.xyz

[Q53] 按条件删除
来源：http://lpn.hcnkem.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://tdr.smart0.xyz

[Q54] 清空表
来源：http://ues.chenlongwang.top

TRUNCATE TABLE logs;
来源：http://kum.jqgfzy.top

[Q55] 排名（并列占位）
来源：http://uyp.quarkkingdee.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://xsp.yfazqb.com

[Q56] 密集排名（并列不占位）
来源：http://iym.316326.xyz

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://azq.wangdashe.top

[Q57] 行号
来源：http://rbv.xziqi.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hxi.fehbvm.com

[Q58] 累计求和
来源：http://ite.pycfn.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://rjo.wangshuangyany.cn

[Q59] 分组内累计
来源：http://zid.shangyingyoupin.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ddt.ybcxt.top

[Q60] 取上一行 / 下一行
来源：http://uyx.yueranfly.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wmh.redwolf501.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://tit.cucudq.cn

[Q61] 移动平均
来源：http://cuy.shanyushiyangtech.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ivg.316326.xyz

[Q62] 分组占比
来源：http://rdg.jyoumei.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ecg.zdqjudy.top

[Q63] 开启事务
来源：http://jwx.birdmap.top

START TRANSACTION;                -- 或 BEGIN
来源：http://sxb.0kj1m.cn

[Q64] 提交事务
来源：http://fjc.yanxiufei.cn

COMMIT;
来源：http://kdf.sjlbkw.cn

[Q65] 回滚事务
来源：http://mva.haohaochexian.top

ROLLBACK;
来源：http://mig.guowangkeji.top

[Q66] 行锁查询
来源：http://dmo.ctjpmb.com

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hnv.tarul.cn

[Q67] 设置隔离级别
来源：http://uvk.shangyingyoupin.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://lfk.tarul.cn

[Q68] 保存点
来源：http://uja.gotoacloud.top

SAVEPOINT sp1;
来源：http://pqs.zdbjq.cn

ROLLBACK TO sp1;
来源：http://ikb.ctjpmb.com

[Q69] 查看执行计划
来源：http://tla.guowangkeji.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://rwi.zdqjudy.top

[Q70] 更新统计信息
来源：http://xbo.yvedp.cn

ANALYZE TABLE users;
来源：http://lwu.yj202588.top

[Q71] 查看建表语句
来源：http://dew.sjlbkw.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mwv.pycfn.com

[Q72] 查看索引
来源：http://ugt.chenzaomai.com

SHOW INDEX FROM users;
来源：http://saa.meibo888.top

[Q73] 查看表状态
来源：http://uhx.zdbjq.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://huu.9152youxi.cn

[Q74] 强制使用索引
来源：http://tno.nwbrower.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://akq.jqgfzy.top

[Q75] 日期格式化
来源：http://jso.jinqigufen.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://jij.jinqigfzy.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://bqz.hnxiangtu.top

[Q76] 按天统计
来源：http://xej.mhx1999.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://jxq.quarkkingdee.top

[Q77] 时间加减
来源：http://jht.hcnkem.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://eis.gogol.net.cn

[Q78] 当前时间
来源：http://pyw.nanxuanxn.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://cbb.yj20258.top

[Q79] 字符串拼接
来源：http://dqs.fanxiaobao.xyz

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://kyr.ywan-chungtsiang.top

[Q80] 字符串截取
来源：http://mjj.jinyuanbaomall.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://beg.dashuyun.cn

[Q81] 字符串替换
来源：http://vfd.kuanghao11.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://rvp.cheryme.top

[Q82] 字符长度与字节长度
来源：http://jkf.cheryme.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://llq.sxryk.cn

[Q83] 大小写转换
来源：http://rby.shanyushiyangkeji.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://dlb.yongpay.top

[Q84] 去除首尾空格
来源：http://mci.bbcook.cn

SELECT TRIM(name) FROM users;
来源：http://yrm.guowangkeji.top

[Q85] 数值取整
来源：http://jcc.zhongyouzk.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://cml.yanxiufei.cn

[Q86] 读取 JSON 字段
来源：http://vyn.birdmap.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://bzf.jinyuanbaomall.cn

[Q87] JSON 字段做条件
来源：http://qqo.zdbjq.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wpn.hysaishi.cn

[Q88] 行转列（条件聚合）
来源：http://htq.tarul.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://fra.yvedp.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blq.fzhhl.top

[Q89] 判断表是否存在
来源：http://bfs.fanxiaobao.xyz

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://fgp.hysaishi.cn

[Q90] 生成序号列
来源：http://mik.mhx1999.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://evb.sysykeji.top

================================================================================
来源：http://kua.hysaishi.cn

R. Bash 专题
来源：http://bcw.zhaomingkeji.xyz

================================================================================
来源：http://qfe.ctjpmb.com

[R01] shebang 与严格模式
来源：http://ykz.wangshuangyany.cn

#!/usr/bin/env bash
来源：http://qxu.wangshuangyany.cn

set -euo pipefail
来源：http://hfd.dianchejie.cn

[R02] 变量赋值与使用
来源：http://gjf.zhongyouzk.top

name="Tom"; echo "$name"
来源：http://uhp.fktsv.cn

[R03] 只读变量
来源：http://uqh.wangshuangyany.cn

readonly PI=3.14
来源：http://pub.feifeiyinyue.top

[R04] 位置参数
来源：http://iho.ivvv.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://zks.sweek.top

[R05] 参数默认值
来源：http://uey.ivvv.top

name="${1:-default}"
来源：http://xit.jlsjyb.cn

[R06] 判断命令是否存在
来源：http://jju.zhongyouzk.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://zal.sxryk.cn

[R07] if 判断文件
来源：http://ubd.tianlin.xyz

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://dnv.fengsongda.top

[R08] 数值比较
来源：http://jte.epnwcf.com

if (( a > b )); then echo "a 更大"; fi
来源：http://nfc.nanxuanxn.top

[R09] 字符串比较
来源：http://wiu.guowangkeji.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://qwz.mhx1999.top

[R10] 正则匹配
来源：http://ngw.fktsv.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://tvu.jqgfzy.top

[R11] case 多分支
来源：http://szv.redwolf501.top

case "$1" in
来源：http://maj.yonumen.top

start) echo "启动" ;;
来源：http://xeh.ydjk.org.cn

stop)  echo "停止" ;;
来源：http://icl.jlsjyb.cn

*)     echo "未知命令" ;;
来源：http://hks.jlsjyb.cn

esac
来源：http://wkx.pycfn.com

[R12] for 遍历文件
来源：http://vaw.yvedp.cn

for f in *.txt; do echo "$f"; done
来源：http://mid.hesvh.cn

[R13] for 计数循环
来源：http://ohy.shuidangran.top

for i in {1..10}; do echo "$i"; done
来源：http://aog.yuanzhike.top

[R14] C 风格 for
来源：http://tlz.epnwcf.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://cye.yangfankeji.com

[R15] while 逐行读文件
来源：http://hrq.ppjwa.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://yel.xuetiantiany.cn

[R16] until 等待条件
来源：http://ymj.chenjidiqi.icu

until [[ -f done.flag ]]; do sleep 1; done
来源：http://jqj.hysaishi.cn

[R17] 数组定义与取值
来源：http://ice.xingfuxueyuan.xyz

arr=(a b c); echo "${arr[0]}"
来源：http://iki.yuanzhike.top

[R18] 遍历数组
来源：http://fzc.pycfn.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://vrr.fktsv.cn

[R19] 数组长度
来源：http://qhi.nanxuanxn.top

echo "${#arr[@]}"
来源：http://wep.zhijiandao.cn

[R20] 关联数组（字典）
来源：http://ydm.hcnkem.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://jsj.tanke756.top

[R21] 字符串长度
来源：http://wbi.52xcode.cn

echo "${#s}"
来源：http://vmd.jqgfzy.top

[R22] 截取子串
来源：http://itw.pycfn.com

echo "${s:0:5}"
来源：http://bpm.zdbjq.cn

[R23] 字符串替换
来源：http://hbe.ctjpmb.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wrd.gotoacloud.top

[R24] 大小写转换
来源：http://ywp.zhiwuduotai.top

echo "${s^^}"; echo "${s,,}"
来源：http://uwi.zhaomingkeji.xyz

[R25] 去后缀 / 去前缀
来源：http://bvo.zhoulong.xyz

echo "${f%.txt}"; echo "${f#./}"
来源：http://zmo.zhongyouzk.top

[R26] 命令替换
来源：http://gnr.vehdjk.com

now=$(date +%F); echo "$now"
来源：http://aqw.ydjk.org.cn

[R27] 算术展开
来源：http://sda.redwolf501.top

echo $((1 + 2 * 3))
来源：http://qpp.hcnkem.com

[R28] 浮点运算
来源：http://wbn.ivvv.top

echo "scale=2; 10/3" | bc
来源：http://sju.ywan-chungtsiang.top

[R29] 定义函数
来源：http://uny.gotoacloud.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ycw.zhoulong.xyz

[R30] 函数返回状态码
来源：http://tkf.yangfankeji.com

f() { return 0; }; f || echo "失败了"
来源：http://wca.zhixingplan.top

[R31] 局部变量
来源：http://itz.kuanghao11.cn

f() { local x=1; echo "$x"; }
来源：http://tip.chenzaomai.com

[R32] 参数个数校验
来源：http://vog.9152youxi.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://bhr.gaohongyu789.top

[R33] 捕获错误并提示行号
来源：http://hcy.shuidangran.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://nmq.dianchejie.cn

[R34] 退出时清理
来源：http://kca.yanxiufei.cn

trap 'rm -f "$tmp"' EXIT
来源：http://vcg.aibaodan.cn

[R35] 后台执行并等待
来源：http://ruw.yangfankeji.com

sleep 5 & pid=$!; wait "$pid"
来源：http://wkp.fehbvm.com

[R36] 并发执行多个任务
来源：http://kig.0kj1m.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://qso.svipenyu.cn

[R37] 把输出赋给变量
来源：http://dxn.vqdsnc.cn

files=$(ls -1)
来源：http://dtw.jqgufenzy.top

[R38] 管道串联
来源：http://you.havefunace.top

cat a.txt | grep -i error | wc -l
来源：http://bog.zhoulong.xyz

[R39] 重定向标准输出与错误
来源：http://oki.kuanghao11.cn

cmd > out.log 2>&1
来源：http://lic.xziqi.cn

[R40] 追加写日志
来源：http://rpn.ivvv.top

echo "log" >> out.log
来源：http://ten.sxryk.cn

[R41] 丢弃输出
来源：http://ulm.jinqigufen.top


<!-- 参考信息 -->