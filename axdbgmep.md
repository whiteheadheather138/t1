代发 wailian999

================================================================================
来源：http://uko.gaohongyu789.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hcw.uphjek.com

================================================================================
来源：http://bht.zhoulong.xyz

[Q01] 创建表
来源：http://lpz.jlsjyb.cn

CREATE TABLE users (
来源：http://ibn.hcnkem.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://aiy.fanxiaobao.xyz

name VARCHAR(50) NOT NULL,
来源：http://uld.nanxinkj.top

email VARCHAR(100) UNIQUE,
来源：http://bco.jinyuanbaomall.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://jhu.ppjwa.cn

);
来源：http://zji.nanxinkj.top

[Q02] 创建带外键的表
来源：http://zvz.sweek.top

CREATE TABLE orders (
来源：http://fhz.yuxming.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://xon.bbcook.cn

user_id INT NOT NULL,
来源：http://sas.andypj.xyz

amount DECIMAL(10, 2),
来源：http://jhh.zhijiandao.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ceo.shanyushiyangtech.top

);
来源：http://udo.mhx1999.top

[Q03] 增加列
来源：http://ypf.daria6918.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://fiz.jianghu66.top

[Q04] 修改列类型
来源：http://psd.zhijiandao.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://waz.ctjpmb.com

[Q05] 重命名列
来源：http://bcw.jqgfzy.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://jhj.chenlongwang.top

[Q06] 删除列
来源：http://vsg.gotoacloud.top

ALTER TABLE users DROP COLUMN age;
来源：http://qhx.hongshengwenyu.top

[Q07] 删除表
来源：http://ehr.fengsongda.top

DROP TABLE IF EXISTS orders;
来源：http://aek.nanxinkj.top

[Q08] 创建普通索引
来源：http://wds.iojbl.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://smg.fengsongda.top

[Q09] 创建唯一索引
来源：http://eil.sysykeji.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://moi.andypj.xyz

[Q10] 插入单行
来源：http://xqe.hnqzz.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ajv.dianchejie.cn

[Q11] 一次插入多行
来源：http://bnw.ydzc1.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://yjk.cqqwz.cn

[Q12] 插入后取自增 ID
来源：http://jjo.pycfn.com

INSERT INTO users (name) VALUES ('C');
来源：http://ate.chenzaomai.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://aeb.0kj1m.cn

[Q13] 忽略重复插入
来源：http://tdm.jinyuanbaomall.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://vyx.hesvh.cn

[Q14] 存在则更新（upsert）
来源：http://lfc.vehdjk.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://dzc.yj20258888.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://spl.vehdjk.com

[Q15] 查询全部
来源：http://flw.jqgfzy.top

SELECT * FROM users;
来源：http://phl.zycfv.cn

[Q16] 查询指定列
来源：http://ivf.tian-w.cn

SELECT id, name FROM users;
来源：http://zrd.yongpay.top

[Q17] 条件查询
来源：http://rei.fehbvm.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://fke.quarkkingdee.top

[Q18] 模糊匹配
来源：http://mkz.gzhubu.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://yxq.zhengqikj.top

[Q19] 范围查询
来源：http://tmq.tian-w.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://keu.mhx1999.top

[Q20] IN 列表
来源：http://ycr.c1oappe.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://akl.pengpengdd.cyou

[Q21] 空值判断
来源：http://dcl.gzhubu.top

SELECT * FROM users WHERE email IS NULL;
来源：http://wpt.xingfuxueyuan.xyz

[Q22] 排序
来源：http://adj.jqgfzy.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://shc.meibo888.top

[Q23] 分页
来源：http://ojj.hongshengwenyu.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://viz.xinyue.icu

[Q24] 去重
来源：http://gko.jinqigfzy.top

SELECT DISTINCT city FROM users;
来源：http://ieq.sweek.top

[Q25] 只取前 N 条
来源：http://sso.yfazqb.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://lqh.meibo888.top

[Q26] 计数
来源：http://juy.iojbl.cn

SELECT COUNT(*) FROM users;
来源：http://fbu.chenzaomai.com

[Q27] 条件计数
来源：http://gen.bjfxy.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ndv.gzhubu.top

[Q28] 求和与平均
来源：http://glw.zhongyouzk.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hjf.zhoulong.xyz

[Q29] 最大最小值
来源：http://zxt.quarkkingdee.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://got.pengpengdd.cyou

[Q30] 分组统计
来源：http://ixz.zhaomingkeji.xyz

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ugn.hongshengwenyu.top

[Q31] 分组后过滤
来源：http://nww.guannengcc.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://qsp.iojbl.cn

[Q32] 分组拼接字符串
来源：http://xvx.gaohongyu789.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://rlf.xingfuxueyuan.xyz

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://kvn.yuxming.cn

[Q33] 多列分组
来源：http://mmk.jqgfzy.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://dev.shanyushiyangkeji.top

[Q34] 每组取第一条
来源：http://rfn.bjfxy.top

SELECT * FROM (
来源：http://nbj.wangdashe.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ntc.ctjpmb.com

) t WHERE rn = 1;
来源：http://elj.hfpthk.cn

[Q35] 内连接
来源：http://twv.hysaishi.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://vwu.hfpthk.cn

[Q36] 左连接
来源：http://buu.sysykeji.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hlf.gaohongyu789.top

[Q37] 右连接
来源：http://kwd.chenzaomai.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://tfr.svipenyu.cn

[Q38] 全外连接（PostgreSQL）
来源：http://biz.ydzc1.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://elp.zdqjudy.top

[Q39] 自连接（查上下级）
来源：http://xnw.smart0.xyz

SELECT e.name, m.name AS manager FROM employees e
来源：http://tfk.zhongyouzk.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://cea.zhaomingkeji.xyz

[Q40] 交叉连接（笛卡尔积）
来源：http://qgk.gotoacloud.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://rls.cucudq.cn

[Q41] 多表连接
来源：http://lem.zhengqikj.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://rlt.pengpengdd.cyou

JOIN users u ON u.id = o.user_id
来源：http://rve.chenzaomai.com

JOIN products p ON p.id = o.product_id;
来源：http://hpb.jyoumei.cn

[Q42] 连接条件附加过滤
来源：http://ukd.quarkkingdee.top

SELECT u.name, o.amount FROM users u
来源：http://qjm.cdnleiting.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ezg.jianghu66.top

[Q43] 标量子查询
来源：http://fvz.pengpengdd.cyou

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ytu.ywan-chungtsiang.top

[Q44] IN 子查询
来源：http://gzg.tian-w.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://vta.cashguo.top

[Q45] EXISTS 判断存在
来源：http://lpk.havefunace.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hmh.yangfankeji.com

[Q46] NOT EXISTS 判断不存在
来源：http://isj.shanyushiyangkeji.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vgu.ivvv.top

[Q47] 与平均值比较
来源：http://tat.nanxuanxn.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://uma.zhiwuduotai.top

[Q48] CTE 公用表表达式
来源：http://ogj.andypj.xyz

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://uxx.aibaodan.cn

SELECT * FROM t WHERE c > 5;
来源：http://azc.yanxiufei.cn

[Q49] 更新单行
来源：http://aby.feifeiyinyue.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://qak.hnqzz.top

[Q50] 批量更新
来源：http://riz.hysaishi.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://aux.dianchejie.cn

[Q51] 用子查询更新
来源：http://byu.yj202588.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://vrw.fehbvm.com

[Q52] 删除指定行
来源：http://eut.sweek.top

DELETE FROM users WHERE id = 10;
来源：http://bac.mhx1999.top

[Q53] 按条件删除
来源：http://mwf.jinqigfzy.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hpm.shzxlz.cn

[Q54] 清空表
来源：http://zpy.chenjidiqi.icu

TRUNCATE TABLE logs;
来源：http://ajq.cheryme.top

[Q55] 排名（并列占位）
来源：http://oxl.sweek.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ata.yfazqb.com

[Q56] 密集排名（并列不占位）
来源：http://qxo.yj20258888.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://bpv.aizwys.cn

[Q57] 行号
来源：http://vwo.zhongyouzk.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://xaj.shangyingyoupin.top

[Q58] 累计求和
来源：http://rab.tarul.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://dvb.yongpay.top

[Q59] 分组内累计
来源：http://wap.fengsongda.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://btb.dashuyun.cn

[Q60] 取上一行 / 下一行
来源：http://lce.hnqzz.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://sjs.ydzc1.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://eqj.hcnkem.com

[Q61] 移动平均
来源：http://kqp.sjlbkw.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://pyu.pengpengdd.cyou

[Q62] 分组占比
来源：http://fra.shanyushiyangkeji.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://kkn.snrcjt.cn

[Q63] 开启事务
来源：http://bwg.gzhubu.top

START TRANSACTION;                -- 或 BEGIN
来源：http://ezs.cashguo.top

[Q64] 提交事务
来源：http://tpt.yj20258888.top

COMMIT;
来源：http://wmb.mhx1999.top

[Q65] 回滚事务
来源：http://gbb.sxryk.cn

ROLLBACK;
来源：http://fkl.redwolf501.top

[Q66] 行锁查询
来源：http://qzb.zdbjq.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://tnq.zhaomingkeji.xyz

[Q67] 设置隔离级别
来源：http://jwf.uphjek.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://xic.cashguo.top

[Q68] 保存点
来源：http://unv.hongshengwenyu.top

SAVEPOINT sp1;
来源：http://mlr.uphjek.com

ROLLBACK TO sp1;
来源：http://scl.uphjek.com

[Q69] 查看执行计划
来源：http://bbr.shzxlz.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://sis.hongshengwenyu.top

[Q70] 更新统计信息
来源：http://fbn.hywenlv.cn

ANALYZE TABLE users;
来源：http://tiv.gogol.net.cn

[Q71] 查看建表语句
来源：http://ipi.snrcjt.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://rpd.hfpthk.cn

[Q72] 查看索引
来源：http://fjy.sjlbkw.cn

SHOW INDEX FROM users;
来源：http://ido.chenjidiqi.icu

[Q73] 查看表状态
来源：http://ufv.fanxiaobao.xyz

SHOW TABLE STATUS LIKE 'users';
来源：http://rog.iojbl.cn

[Q74] 强制使用索引
来源：http://dls.yfazqb.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://dqj.tanke756.top

[Q75] 日期格式化
来源：http://bck.cashguo.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://eac.cdnleiting.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://lpn.shanyushiyangkeji.top

[Q76] 按天统计
来源：http://ghu.guowangkeji.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://pud.yanxiufei.cn

[Q77] 时间加减
来源：http://jrt.yongpay.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://eur.jinyuanbaomall.cn

[Q78] 当前时间
来源：http://zkv.sjlbkw.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://jqi.52xcode.cn

[Q79] 字符串拼接
来源：http://zhj.svipenyu.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://eut.bbcook.cn

[Q80] 字符串截取
来源：http://nur.guowangkeji.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://aqb.ehwqpu.com

[Q81] 字符串替换
来源：http://ioh.feifeiyinyue.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://xty.kuanghao11.cn

[Q82] 字符长度与字节长度
来源：http://mkd.fanxiaobao.xyz

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://fly.0kj1m.cn

[Q83] 大小写转换
来源：http://isv.shuidangran.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hfh.haohaochexian.top

[Q84] 去除首尾空格
来源：http://sxo.hammf.cn

SELECT TRIM(name) FROM users;
来源：http://tse.mhx1999.top

[Q85] 数值取整
来源：http://ssb.shanyushiyangtech.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://trx.xziqi.cn

[Q86] 读取 JSON 字段
来源：http://lht.aizwys.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://glr.cdnleiting.top

[Q87] JSON 字段做条件
来源：http://fyp.meibo888.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://eev.dianchejie.cn

[Q88] 行转列（条件聚合）
来源：http://ksa.zhaomingkeji.xyz

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://vft.yfazqb.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://djl.zycfv.cn

[Q89] 判断表是否存在
来源：http://plr.aibaodan.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://vsb.jiagoushi.top

[Q90] 生成序号列
来源：http://xal.aizwys.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://set.hcnkem.com

================================================================================
来源：http://isl.hnqzz.top

R. Bash 专题
来源：http://mrq.vehdjk.com

================================================================================
来源：http://lda.tarul.cn

[R01] shebang 与严格模式
来源：http://iet.havefunace.top

#!/usr/bin/env bash
来源：http://vur.tarul.cn

set -euo pipefail
来源：http://uel.snrcjt.cn

[R02] 变量赋值与使用
来源：http://ypj.pengpengdd.cyou

name="Tom"; echo "$name"
来源：http://lsk.yj202588.top

[R03] 只读变量
来源：http://rqh.svipenyu.cn

readonly PI=3.14
来源：http://xrk.gogol.net.cn

[R04] 位置参数
来源：http://bgh.meibo888.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://gnw.yangfankeji.com

[R05] 参数默认值
来源：http://wbp.xylfe.cn

name="${1:-default}"
来源：http://afl.gotoacloud.top

[R06] 判断命令是否存在
来源：http://ajy.cdnleiting.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://csm.xuanzx.com

[R07] if 判断文件
来源：http://ldz.tian-w.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://eab.daxiang520.top

[R08] 数值比较
来源：http://miq.tianlin.xyz

if (( a > b )); then echo "a 更大"; fi
来源：http://cbp.cashguo.top

[R09] 字符串比较
来源：http://jru.0kj1m.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://cuy.hongshengwenyu.top

[R10] 正则匹配
来源：http://qsv.snrcjt.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://kzj.shanyushiyangkeji.top

[R11] case 多分支
来源：http://yvt.tian-w.cn

case "$1" in
来源：http://hqw.shanyushiyangtech.top

start) echo "启动" ;;
来源：http://xom.aizwys.cn

stop)  echo "停止" ;;
来源：http://xdc.xingfuxueyuan.xyz

*)     echo "未知命令" ;;
来源：http://jca.sxryk.cn

esac
来源：http://iui.fktsv.cn

[R12] for 遍历文件
来源：http://hhu.pengpengdd.cyou

for f in *.txt; do echo "$f"; done
来源：http://ycn.tianlin.xyz

[R13] for 计数循环
来源：http://pnk.epnwcf.com

for i in {1..10}; do echo "$i"; done
来源：http://ias.uphjek.com

[R14] C 风格 for
来源：http://yvk.iojbl.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://avc.gaohongyu789.top

[R15] while 逐行读文件
来源：http://def.xingfuxueyuan.xyz

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://agi.hcnkem.com

[R16] until 等待条件
来源：http://pxx.hnxiangtu.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ttv.fzhhl.top

[R17] 数组定义与取值
来源：http://fdw.jqgfzy.top

arr=(a b c); echo "${arr[0]}"
来源：http://sgn.ctjpmb.com

[R18] 遍历数组
来源：http://ili.xziqi.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://zle.jiagoushi.top

[R19] 数组长度
来源：http://cgt.hnxiangtu.top

echo "${#arr[@]}"
来源：http://cbw.pengpengdd.cyou

[R20] 关联数组（字典）
来源：http://lps.ppjwa.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://lgf.jyoumei.cn

[R21] 字符串长度
来源：http://pie.havefunace.top

echo "${#s}"
来源：http://lyz.kuanghao11.cn

[R22] 截取子串
来源：http://adn.hammf.cn

echo "${s:0:5}"
来源：http://oos.fanxiaobao.xyz

[R23] 字符串替换
来源：http://jny.shzxlz.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://lqj.gotoacloud.top

[R24] 大小写转换
来源：http://agg.gzhubu.top

echo "${s^^}"; echo "${s,,}"
来源：http://caj.zhaomingkeji.xyz

[R25] 去后缀 / 去前缀
来源：http://smh.jinqigfzy.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://ijk.zhijiandao.cn

[R26] 命令替换
来源：http://gnm.xuanzx.com

now=$(date +%F); echo "$now"
来源：http://pfk.9152youxi.cn

[R27] 算术展开
来源：http://qgu.vehdjk.com

echo $((1 + 2 * 3))
来源：http://pqf.chenlongwang.top

[R28] 浮点运算
来源：http://ciw.pycfn.com

echo "scale=2; 10/3" | bc
来源：http://hjv.ywan-chungtsiang.top

[R29] 定义函数
来源：http://onv.cdnleiting.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://epl.tianlin.xyz

[R30] 函数返回状态码
来源：http://eqj.hesvh.cn

f() { return 0; }; f || echo "失败了"
来源：http://nax.yj202588.top

[R31] 局部变量
来源：http://cew.bjfxy.top

f() { local x=1; echo "$x"; }
来源：http://yrz.316326.xyz

[R32] 参数个数校验
来源：http://ifl.xziqi.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wqn.cdnleiting.top

[R33] 捕获错误并提示行号
来源：http://vih.yanxiufei.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://xcg.hongshengwenyu.top

[R34] 退出时清理
来源：http://uxn.fzhhl.top

trap 'rm -f "$tmp"' EXIT
来源：http://ljn.gogol.net.cn

[R35] 后台执行并等待
来源：http://txh.sjlbkw.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://phv.yj20258.top

[R36] 并发执行多个任务
来源：http://tga.shanyushiyangtech.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blh.yuxming.cn

[R37] 把输出赋给变量
来源：http://gwo.c1oappe.top

files=$(ls -1)
来源：http://bgv.hammf.cn

[R38] 管道串联
来源：http://hls.shzxlz.cn

cat a.txt | grep -i error | wc -l
来源：http://ssv.ppjwa.cn

[R39] 重定向标准输出与错误
来源：http://pbv.meibo888.top

cmd > out.log 2>&1
来源：http://fsr.sjlbkw.cn

[R40] 追加写日志
来源：http://kgd.fktsv.cn

echo "log" >> out.log
来源：http://rlb.yanxiufei.cn

[R41] 丢弃输出
来源：http://zfv.zhongyouzk.top

cmd >/dev/null 2>&1
来源：http://glj.0kj1m.cn

[R42] 输入重定向
来源：http://izz.havefunace.top

wc -l < a.txt
来源：http://jjn.hongshengwenyu.top

[R43] 按名字查找文件
来源：http://wns.shuidangran.top


<!-- 参考信息 -->