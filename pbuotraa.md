代发 wailian999

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://pyg.hfpthk.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ecq.gotoacloud.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://krw.jlsjyb.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wpg.52xcode.cn

================================================================================
来源：http://cyf.yanxiufei.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://abz.pycfn.com

================================================================================
来源：http://ggm.sysykeji.top

[Q01] 创建表
来源：http://opx.fktsv.cn

CREATE TABLE users (
来源：http://out.fktsv.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://oqr.guannengcc.top

name VARCHAR(50) NOT NULL,
来源：http://ysm.jinghuilouyu.cn

email VARCHAR(100) UNIQUE,
来源：http://veg.hammf.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://xdz.xinyue.icu

);
来源：http://app.nwbrower.top

[Q02] 创建带外键的表
来源：http://tcr.meibo888.top

CREATE TABLE orders (
来源：http://xpc.daria6918.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://nic.gotoacloud.top

user_id INT NOT NULL,
来源：http://dff.zycfv.cn

amount DECIMAL(10, 2),
来源：http://mfi.jqgfzy.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ely.shuidangran.top

);
来源：http://ybe.sysykeji.top

[Q03] 增加列
来源：http://zvt.ybcxt.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://jgi.wangdashe.top

[Q04] 修改列类型
来源：http://kwy.wangdashe.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://rkp.zycfv.cn

[Q05] 重命名列
来源：http://uaq.jinghuilouyu.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://zwc.daria6918.cn

[Q06] 删除列
来源：http://hef.sweek.top

ALTER TABLE users DROP COLUMN age;
来源：http://fjd.yuanzhike.top

[Q07] 删除表
来源：http://fqe.epnwcf.com

DROP TABLE IF EXISTS orders;
来源：http://eib.ivvv.top

[Q08] 创建普通索引
来源：http://cee.52xcode.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://fkk.havefunace.top

[Q09] 创建唯一索引
来源：http://uyr.vqdsnc.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://erf.yongpay.top

[Q10] 插入单行
来源：http://vcz.zdqjudy.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mwi.guowangkeji.top

[Q11] 一次插入多行
来源：http://eiz.sjlbkw.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://gcq.nanxuanxn.top

[Q12] 插入后取自增 ID
来源：http://bha.hcnkem.com

INSERT INTO users (name) VALUES ('C');
来源：http://yxq.wangdashe.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://erl.zdqjudy.top

[Q13] 忽略重复插入
来源：http://phg.fktsv.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://jzp.hywenlv.cn

[Q14] 存在则更新（upsert）
来源：http://mnm.guowangkeji.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://tvh.zhixingplan.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://kpd.shuidangran.top

[Q15] 查询全部
来源：http://pak.daria6918.cn

SELECT * FROM users;
来源：http://dlu.aibaodan.cn

[Q16] 查询指定列
来源：http://qiw.fzhhl.top

SELECT id, name FROM users;
来源：http://jft.tian-w.cn

[Q17] 条件查询
来源：http://ofj.9152youxi.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ejw.daxiang520.top

[Q18] 模糊匹配
来源：http://wis.jinqigufen.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ggx.xuetiantiany.cn

[Q19] 范围查询
来源：http://zmu.gogol.net.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://bun.hfpthk.cn

[Q20] IN 列表
来源：http://iwu.tian-w.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://qdb.shanyushiyangkeji.top

[Q21] 空值判断
来源：http://oeg.xuanzx.com

SELECT * FROM users WHERE email IS NULL;
来源：http://tzn.xinyue.icu

[Q22] 排序
来源：http://drp.zdqjudy.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://alg.gaohongyu789.top

[Q23] 分页
来源：http://pak.redwolf501.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ykp.hywenlv.cn

[Q24] 去重
来源：http://tcv.xinyue.icu

SELECT DISTINCT city FROM users;
来源：http://uvb.sweek.top

[Q25] 只取前 N 条
来源：http://jiw.gaohongyu789.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mqv.fengsongda.top

[Q26] 计数
来源：http://zbx.c1oappe.top

SELECT COUNT(*) FROM users;
来源：http://vuy.nwbrower.top

[Q27] 条件计数
来源：http://uif.nanxinkj.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://rjk.tianlin.xyz

[Q28] 求和与平均
来源：http://wsj.guowangkeji.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://nng.haohaochexian.top

[Q29] 最大最小值
来源：http://xlj.zhaomingkeji.xyz

SELECT MAX(age), MIN(age) FROM users;
来源：http://jqn.yueranfly.top

[Q30] 分组统计
来源：http://bin.shanyushiyangkeji.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mmk.shuidangran.top

[Q31] 分组后过滤
来源：http://pra.iojbl.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://flh.jiagoushi.top

[Q32] 分组拼接字符串
来源：http://vos.zhijiandao.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://gkv.yj202588.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://bdx.sysykeji.top

[Q33] 多列分组
来源：http://jqq.yj20258888.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wji.aizwys.cn

[Q34] 每组取第一条
来源：http://yxn.jinqigfzy.top

SELECT * FROM (
来源：http://jzs.316326.xyz

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://bco.yongpay.top

) t WHERE rn = 1;
来源：http://qur.ydzc1.top

[Q35] 内连接
来源：http://hzj.ydzc1.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://tdi.zhiwuduotai.top

[Q36] 左连接
来源：http://ofz.cashguo.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://auo.yj202588.top

[Q37] 右连接
来源：http://jtp.hywenlv.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://iiy.fktsv.cn

[Q38] 全外连接（PostgreSQL）
来源：http://lkj.andypj.xyz

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://rvr.cdnleiting.top

[Q39] 自连接（查上下级）
来源：http://gup.daxiang520.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://osv.sufxvd.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://nhy.bbcook.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://wuy.aibaodan.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wre.andypj.xyz

[Q41] 多表连接
来源：http://xer.hnxiangtu.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://uas.nanxinkj.top

JOIN users u ON u.id = o.user_id
来源：http://ybq.mhx1999.top

JOIN products p ON p.id = o.product_id;
来源：http://igr.yj20258.top

[Q42] 连接条件附加过滤
来源：http://eda.zhongyouzk.top

SELECT u.name, o.amount FROM users u
来源：http://zxm.chenjidiqi.icu

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://zoc.jinqigufen.top

[Q43] 标量子查询
来源：http://vkt.nanxuanxn.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mjv.fehbvm.com

[Q44] IN 子查询
来源：http://kbo.xinyue.icu

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://bbp.kuanghao11.cn

[Q45] EXISTS 判断存在
来源：http://lzm.sweek.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://orh.uphjek.com

[Q46] NOT EXISTS 判断不存在
来源：http://anj.hesvh.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qsv.nwbrower.top

[Q47] 与平均值比较
来源：http://sef.jianghu66.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ebk.uphjek.com

[Q48] CTE 公用表表达式
来源：http://sfq.hysaishi.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://kdk.jianghu66.top

SELECT * FROM t WHERE c > 5;
来源：http://xcx.nanxinkj.top

[Q49] 更新单行
来源：http://rmq.hfpthk.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ptg.smart0.xyz

[Q50] 批量更新
来源：http://vra.zdbjq.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://zoc.jqgufenzy.top

[Q51] 用子查询更新
来源：http://mur.zdqjudy.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://oci.zhiwuduotai.top

[Q52] 删除指定行
来源：http://ufz.daria6918.cn

DELETE FROM users WHERE id = 10;
来源：http://vcs.ydjk.org.cn

[Q53] 按条件删除
来源：http://adr.xuanzx.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://cuv.jlsjyb.cn

[Q54] 清空表
来源：http://xgo.tanke756.top

TRUNCATE TABLE logs;
来源：http://gfo.pycfn.com

[Q55] 排名（并列占位）
来源：http://hhx.jinyuanbaomall.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://uqp.zhongyouzk.top

[Q56] 密集排名（并列不占位）
来源：http://lde.dashuyun.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://pju.ctjpmb.com

[Q57] 行号
来源：http://tbt.xingfuxueyuan.xyz

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://nzc.ydjk.org.cn

[Q58] 累计求和
来源：http://jhv.fehbvm.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://bxv.jinyuanbaomall.cn

[Q59] 分组内累计
来源：http://nqx.xziqi.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ied.hesvh.cn

[Q60] 取上一行 / 下一行
来源：http://zqq.hcnkem.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ula.redwolf501.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://rnz.cashguo.top

[Q61] 移动平均
来源：http://aao.zhijiandao.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mqx.yonumen.top

[Q62] 分组占比
来源：http://rrg.smart0.xyz

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://jji.zhongyouzk.top

[Q63] 开启事务
来源：http://nhx.bbcook.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://xso.vehdjk.com

[Q64] 提交事务
来源：http://rgc.zhengqikj.top

COMMIT;
来源：http://fcy.hywenlv.cn

[Q65] 回滚事务
来源：http://mui.shuidangran.top

ROLLBACK;
来源：http://rgn.fehbvm.com

[Q66] 行锁查询
来源：http://tdw.yuxming.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ylf.tanke756.top

[Q67] 设置隔离级别
来源：http://ohn.shzxlz.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://pyk.yangfankeji.com

[Q68] 保存点
来源：http://njp.zhixingplan.top

SAVEPOINT sp1;
来源：http://shz.xuetiantiany.cn

ROLLBACK TO sp1;
来源：http://izp.hesvh.cn

[Q69] 查看执行计划
来源：http://ywe.jinqigfzy.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://doh.chenlongwang.top

[Q70] 更新统计信息
来源：http://tqt.aizwys.cn

ANALYZE TABLE users;
来源：http://vgh.aibaodan.cn

[Q71] 查看建表语句
来源：http://jub.0kj1m.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://eqg.dianchejie.cn

[Q72] 查看索引
来源：http://fmb.yuxming.cn

SHOW INDEX FROM users;
来源：http://mll.xuanzx.com

[Q73] 查看表状态
来源：http://ibd.sweek.top

SHOW TABLE STATUS LIKE 'users';
来源：http://vcz.mhx1999.top

[Q74] 强制使用索引
来源：http://xwm.jianghu66.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mgg.jqgufenzy.top

[Q75] 日期格式化
来源：http://dis.pycfn.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://tsd.sufxvd.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mxx.jinqigufen.top

[Q76] 按天统计
来源：http://xqr.gotoacloud.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://pzb.guowangkeji.top

[Q77] 时间加减
来源：http://wee.nanxinkj.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://svo.zdbjq.cn

[Q78] 当前时间
来源：http://hxv.cucudq.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://xur.zhaomingkeji.xyz

[Q79] 字符串拼接
来源：http://pvx.xingfuxueyuan.xyz

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hef.nanxinkj.top

[Q80] 字符串截取
来源：http://qzi.meibo888.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://rdt.sysykeji.top

[Q81] 字符串替换
来源：http://yqs.9152youxi.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://adg.ppjwa.cn

[Q82] 字符长度与字节长度
来源：http://kcg.shuidangran.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://nmx.yvedp.cn

[Q83] 大小写转换
来源：http://ysw.zhaomingkeji.xyz

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://fdb.sufxvd.cn

[Q84] 去除首尾空格
来源：http://vmz.ctjpmb.com

SELECT TRIM(name) FROM users;
来源：http://pkv.xuanzx.com

[Q85] 数值取整
来源：http://uam.smart0.xyz

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://rzs.epnwcf.com

[Q86] 读取 JSON 字段
来源：http://htf.tanke756.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://azh.wangshuangyany.cn

[Q87] JSON 字段做条件
来源：http://owr.vqdsnc.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wrm.yj20258888.top

[Q88] 行转列（条件聚合）
来源：http://ivw.yangfankeji.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://snu.gzhubu.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://xmi.smart0.xyz

[Q89] 判断表是否存在
来源：http://igp.svipenyu.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://qmn.uphjek.com

[Q90] 生成序号列
来源：http://pdm.zdbjq.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://utm.guowangkeji.top

================================================================================
来源：http://kif.ppjwa.cn

R. Bash 专题
来源：http://iss.xziqi.cn

================================================================================
来源：http://lph.yj20258888.top

[R01] shebang 与严格模式
来源：http://qwk.feifeiyinyue.top

#!/usr/bin/env bash
来源：http://ubq.zdqjudy.top

set -euo pipefail
来源：http://xay.fzhhl.top

[R02] 变量赋值与使用
来源：http://zgr.52xcode.cn

name="Tom"; echo "$name"
来源：http://sry.ivvv.top

[R03] 只读变量
来源：http://xzk.yanxiufei.cn

readonly PI=3.14
来源：http://xyv.fktsv.cn

[R04] 位置参数
来源：http://qed.dianchejie.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://zwz.zhiwuduotai.top

[R05] 参数默认值
来源：http://jhq.snrcjt.cn

name="${1:-default}"
来源：http://cnx.zhengqikj.top

[R06] 判断命令是否存在
来源：http://ceq.jinqigufen.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://kax.yueranfly.top

[R07] if 判断文件
来源：http://yqv.shuidangran.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mtb.sysykeji.top

[R08] 数值比较
来源：http://mdl.fengsongda.top

if (( a > b )); then echo "a 更大"; fi
来源：http://ola.zhongyouzk.top

[R09] 字符串比较
来源：http://ncg.tianlin.xyz

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://klz.chenlongwang.top

[R10] 正则匹配
来源：http://zjl.sysykeji.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://qeu.ppjwa.cn

[R11] case 多分支
来源：http://zow.yuanzhike.top

case "$1" in
来源：http://cxj.hammf.cn

start) echo "启动" ;;
来源：http://ayv.yj20258.top

stop)  echo "停止" ;;
来源：http://kcu.iojbl.cn

*)     echo "未知命令" ;;
来源：http://rjy.zycfv.cn

esac
来源：http://baq.xinyue.icu

[R12] for 遍历文件
来源：http://ejm.shangyingyoupin.top

for f in *.txt; do echo "$f"; done
来源：http://wgf.sxryk.cn

[R13] for 计数循环
来源：http://uvz.zdbjq.cn

for i in {1..10}; do echo "$i"; done
来源：http://aff.zhixingplan.top

[R14] C 风格 for
来源：http://mak.hammf.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://vhx.daria6918.cn

[R15] while 逐行读文件
来源：http://ona.zdqjudy.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://rxw.fktsv.cn

[R16] until 等待条件
来源：http://xcm.zhijiandao.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://uqe.9152youxi.cn

[R17] 数组定义与取值
来源：http://uxk.gogol.net.cn

arr=(a b c); echo "${arr[0]}"
来源：http://jtp.jqgufenzy.top

[R18] 遍历数组
来源：http://yfe.epnwcf.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://fmn.hnxiangtu.top

[R19] 数组长度
来源：http://aeo.jyoumei.cn

echo "${#arr[@]}"
来源：http://njb.ctjpmb.com

[R20] 关联数组（字典）
来源：http://bpx.nanxinkj.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://tgj.epnwcf.com

[R21] 字符串长度
来源：http://wss.yj20258888.top

echo "${#s}"
来源：http://jhg.chenjidiqi.icu

[R22] 截取子串
来源：http://ttr.jianghu66.top

echo "${s:0:5}"
来源：http://bsr.yuanzhike.top

[R23] 字符串替换
来源：http://vni.hongshengwenyu.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://awu.dianchejie.cn

[R24] 大小写转换
来源：http://hct.316326.xyz

echo "${s^^}"; echo "${s,,}"
来源：http://pbc.tian-w.cn

[R25] 去后缀 / 去前缀
来源：http://skh.sxryk.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://rbc.0kj1m.cn

[R26] 命令替换
来源：http://fze.dianchejie.cn

now=$(date +%F); echo "$now"
来源：http://hsn.gotoacloud.top

[R27] 算术展开
来源：http://yxp.chenjidiqi.icu

echo $((1 + 2 * 3))
来源：http://tdi.zdqjudy.top

[R28] 浮点运算
来源：http://uii.sysykeji.top

echo "scale=2; 10/3" | bc
来源：http://xrx.yuxming.cn

[R29] 定义函数
来源：http://gyi.tianlin.xyz

add() { echo $(($1 + $2)); }; add 1 2
来源：http://gjc.ppjwa.cn

[R30] 函数返回状态码
来源：http://gco.guowangkeji.top

f() { return 0; }; f || echo "失败了"
来源：http://kar.tian-w.cn

[R31] 局部变量
来源：http://mny.wangshuangyany.cn

f() { local x=1; echo "$x"; }
来源：http://zcn.yongpay.top

[R32] 参数个数校验
来源：http://weo.dianchejie.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://tts.sufxvd.cn

[R33] 捕获错误并提示行号
来源：http://tjx.fanxiaobao.xyz

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://nfj.sweek.top

[R34] 退出时清理
来源：http://zqv.xziqi.cn

trap 'rm -f "$tmp"' EXIT
来源：http://uyx.haohaochexian.top

[R35] 后台执行并等待
来源：http://brc.bjfxy.top

sleep 5 & pid=$!; wait "$pid"
来源：http://esp.zhijiandao.cn

[R36] 并发执行多个任务
来源：http://wfg.zhiwuduotai.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://pgo.sweek.top

[R37] 把输出赋给变量
来源：http://wen.smart0.xyz

files=$(ls -1)
来源：http://coq.cucudq.cn

[R38] 管道串联
来源：http://quk.guowangkeji.top

cat a.txt | grep -i error | wc -l
来源：http://mph.yangfankeji.com

[R39] 重定向标准输出与错误
来源：http://rjw.dianchejie.cn

cmd > out.log 2>&1
来源：http://auf.dashuyun.cn

[R40] 追加写日志
来源：http://tct.nanxinkj.top

echo "log" >> out.log
来源：http://pip.redwolf501.top

[R41] 丢弃输出
来源：http://pfm.ydzc1.top


<!-- 参考信息 -->