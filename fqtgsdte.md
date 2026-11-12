代发 wailian999

================================================================================
来源：http://ahd.wangshuangyany.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ivx.hysaishi.cn

================================================================================
来源：http://fvt.bbcook.cn

[Q01] 创建表
来源：http://cjq.jyoumei.cn

CREATE TABLE users (
来源：http://aqh.kuanghao11.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://abi.xingfuxueyuan.xyz

name VARCHAR(50) NOT NULL,
来源：http://rgl.jinqigufen.top

email VARCHAR(100) UNIQUE,
来源：http://enf.52xcode.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ztf.guannengcc.top

);
来源：http://tlp.dianchejie.cn

[Q02] 创建带外键的表
来源：http://ftk.tarul.cn

CREATE TABLE orders (
来源：http://lfx.shangyingyoupin.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://qub.fehbvm.com

user_id INT NOT NULL,
来源：http://gre.dashuyun.cn

amount DECIMAL(10, 2),
来源：http://zos.snrcjt.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mpr.yangfankeji.com

);
来源：http://ekx.zhoulong.xyz

[Q03] 增加列
来源：http://mpa.smart0.xyz

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ykl.hnxiangtu.top

[Q04] 修改列类型
来源：http://yvv.hywenlv.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://shm.shuidangran.top

[Q05] 重命名列
来源：http://xif.cashguo.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://nqt.yj20258.top

[Q06] 删除列
来源：http://cbg.gzhubu.top

ALTER TABLE users DROP COLUMN age;
来源：http://cfw.sufxvd.cn

[Q07] 删除表
来源：http://yqn.snrcjt.cn

DROP TABLE IF EXISTS orders;
来源：http://qzb.yuanzhike.top

[Q08] 创建普通索引
来源：http://mpz.gogol.net.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://fwk.pycfn.com

[Q09] 创建唯一索引
来源：http://hvp.xuetiantiany.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://cia.fzhhl.top

[Q10] 插入单行
来源：http://jff.jinqigufen.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://rpf.tarul.cn

[Q11] 一次插入多行
来源：http://vti.zdbjq.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://gnw.wangshuangyany.cn

[Q12] 插入后取自增 ID
来源：http://mjm.pycfn.com

INSERT INTO users (name) VALUES ('C');
来源：http://kua.hongshengwenyu.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://iiu.birdmap.top

[Q13] 忽略重复插入
来源：http://erf.wangshuangyany.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://cmq.xuetiantiany.cn

[Q14] 存在则更新（upsert）
来源：http://trh.redwolf501.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://rii.ehwqpu.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://qlt.mhx1999.top

[Q15] 查询全部
来源：http://fhg.tian-w.cn

SELECT * FROM users;
来源：http://bjv.hfpthk.cn

[Q16] 查询指定列
来源：http://bpw.xuetiantiany.cn

SELECT id, name FROM users;
来源：http://jgb.hammf.cn

[Q17] 条件查询
来源：http://amo.yuanzhike.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://edp.tianlin.xyz

[Q18] 模糊匹配
来源：http://nwm.nanxinkj.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://imi.gaohongyu789.top

[Q19] 范围查询
来源：http://epz.sufxvd.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://fam.ydzc1.top

[Q20] IN 列表
来源：http://ykl.jinghuilouyu.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ihy.shanyushiyangkeji.top

[Q21] 空值判断
来源：http://rfj.yuxming.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://pne.ehwqpu.com

[Q22] 排序
来源：http://hoh.jianghu66.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://cru.jinqigufen.top

[Q23] 分页
来源：http://yjf.0kj1m.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://jhv.gogol.net.cn

[Q24] 去重
来源：http://nll.vehdjk.com

SELECT DISTINCT city FROM users;
来源：http://hah.uphjek.com

[Q25] 只取前 N 条
来源：http://aub.shzxlz.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://tlr.fehbvm.com

[Q26] 计数
来源：http://gnx.cheryme.top

SELECT COUNT(*) FROM users;
来源：http://zno.fzhhl.top

[Q27] 条件计数
来源：http://yuc.0kj1m.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://yjo.zhiwuduotai.top

[Q28] 求和与平均
来源：http://poe.hongshengwenyu.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ztp.shuidangran.top

[Q29] 最大最小值
来源：http://lqn.shzxlz.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://sau.redwolf501.top

[Q30] 分组统计
来源：http://fry.shanyushiyangtech.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wcq.pycfn.com

[Q31] 分组后过滤
来源：http://cbo.gotoacloud.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://tsm.yueranfly.top

[Q32] 分组拼接字符串
来源：http://yqp.birdmap.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hpj.zhongyouzk.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://dvn.chenzaomai.com

[Q33] 多列分组
来源：http://snc.redwolf501.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://iza.jqgfzy.top

[Q34] 每组取第一条
来源：http://abv.chenlongwang.top

SELECT * FROM (
来源：http://qld.guowangkeji.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://xrw.yj20258888.top

) t WHERE rn = 1;
来源：http://rhh.yvedp.cn

[Q35] 内连接
来源：http://eki.ivvv.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://gex.smart0.xyz

[Q36] 左连接
来源：http://nsd.tian-w.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://tau.shuidangran.top

[Q37] 右连接
来源：http://bas.yonumen.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://dex.uphjek.com

[Q38] 全外连接（PostgreSQL）
来源：http://obu.hfpthk.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://urc.sysykeji.top

[Q39] 自连接（查上下级）
来源：http://rhl.svipenyu.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://dch.nanxinkj.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://msl.fanxiaobao.xyz

[Q40] 交叉连接（笛卡尔积）
来源：http://slp.daria6918.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hvw.yueranfly.top

[Q41] 多表连接
来源：http://gmw.daria6918.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://mct.yueranfly.top

JOIN users u ON u.id = o.user_id
来源：http://luj.jinqigfzy.top

JOIN products p ON p.id = o.product_id;
来源：http://rsg.ctjpmb.com

[Q42] 连接条件附加过滤
来源：http://fxo.cdnleiting.top

SELECT u.name, o.amount FROM users u
来源：http://bly.wangshuangyany.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://cxe.chenlongwang.top

[Q43] 标量子查询
来源：http://rdm.bbcook.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://zko.shangyingyoupin.top

[Q44] IN 子查询
来源：http://zuq.yj20258.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ouj.wangdashe.top

[Q45] EXISTS 判断存在
来源：http://bhq.epnwcf.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://nqz.dashuyun.cn

[Q46] NOT EXISTS 判断不存在
来源：http://qus.9152youxi.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://yof.sjlbkw.cn

[Q47] 与平均值比较
来源：http://zrx.tanke756.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://vjp.shuidangran.top

[Q48] CTE 公用表表达式
来源：http://aqk.zycfv.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://pxd.jinyuanbaomall.cn

SELECT * FROM t WHERE c > 5;
来源：http://xqs.mhx1999.top

[Q49] 更新单行
来源：http://grg.vqdsnc.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://fcf.zhaomingkeji.xyz

[Q50] 批量更新
来源：http://xme.guannengcc.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://jys.zycfv.cn

[Q51] 用子查询更新
来源：http://hvh.zhaomingkeji.xyz

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://gra.hfpthk.cn

[Q52] 删除指定行
来源：http://xzj.sjlbkw.cn

DELETE FROM users WHERE id = 10;
来源：http://lce.sweek.top

[Q53] 按条件删除
来源：http://ukt.zhiwuduotai.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blm.yj20258888.top

[Q54] 清空表
来源：http://jeb.hesvh.cn

TRUNCATE TABLE logs;
来源：http://exn.tian-w.cn

[Q55] 排名（并列占位）
来源：http://dbr.xuanzx.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://snh.vqdsnc.cn

[Q56] 密集排名（并列不占位）
来源：http://kxd.cdnleiting.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://yfp.redwolf501.top

[Q57] 行号
来源：http://adb.cheryme.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ikd.hfpthk.cn

[Q58] 累计求和
来源：http://azy.zhijiandao.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ekq.jinqigfzy.top

[Q59] 分组内累计
来源：http://xhq.meibo888.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://gxz.snrcjt.cn

[Q60] 取上一行 / 下一行
来源：http://yby.yj202588.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://jwp.yuanzhike.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://dmm.hongshengwenyu.top

[Q61] 移动平均
来源：http://gei.jinghuilouyu.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wib.jinqigufen.top

[Q62] 分组占比
来源：http://umt.zycfv.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://muy.dashuyun.cn

[Q63] 开启事务
来源：http://mbn.xylfe.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://mhs.sjlbkw.cn

[Q64] 提交事务
来源：http://osa.quarkkingdee.top

COMMIT;
来源：http://ylt.jyoumei.cn

[Q65] 回滚事务
来源：http://jai.hnxiangtu.top

ROLLBACK;
来源：http://fyu.sweek.top

[Q66] 行锁查询
来源：http://znj.jlsjyb.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://aja.xinyue.icu

[Q67] 设置隔离级别
来源：http://fmy.yj20258888.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://zer.jinqigufen.top

[Q68] 保存点
来源：http://cco.daria6918.cn

SAVEPOINT sp1;
来源：http://ngx.uphjek.com

ROLLBACK TO sp1;
来源：http://ueo.sysykeji.top

[Q69] 查看执行计划
来源：http://udw.cashguo.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://aqx.redwolf501.top

[Q70] 更新统计信息
来源：http://yqj.kuanghao11.cn

ANALYZE TABLE users;
来源：http://ebq.jinyuanbaomall.cn

[Q71] 查看建表语句
来源：http://tfu.vqdsnc.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://pbg.jlsjyb.cn

[Q72] 查看索引
来源：http://sow.xziqi.cn

SHOW INDEX FROM users;
来源：http://ceb.vqdsnc.cn

[Q73] 查看表状态
来源：http://ouw.zhongyouzk.top

SHOW TABLE STATUS LIKE 'users';
来源：http://muk.dashuyun.cn

[Q74] 强制使用索引
来源：http://mva.hysaishi.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://dfj.sxryk.cn

[Q75] 日期格式化
来源：http://ebq.yanxiufei.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://tgb.zhixingplan.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://dqg.bjfxy.top

[Q76] 按天统计
来源：http://pur.hesvh.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://dcx.jinghuilouyu.cn

[Q77] 时间加减
来源：http://mmz.tanke756.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://jfz.gogol.net.cn

[Q78] 当前时间
来源：http://lux.cashguo.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://jel.haohaochexian.top

[Q79] 字符串拼接
来源：http://cgp.chenjidiqi.icu

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wio.yuxming.cn

[Q80] 字符串截取
来源：http://yrh.daria6918.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://cqt.zhixingplan.top

[Q81] 字符串替换
来源：http://qsk.shanyushiyangkeji.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://kky.birdmap.top

[Q82] 字符长度与字节长度
来源：http://bxw.uphjek.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://nwz.hesvh.cn

[Q83] 大小写转换
来源：http://qqj.hywenlv.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://msm.nanxinkj.top

[Q84] 去除首尾空格
来源：http://rih.tian-w.cn

SELECT TRIM(name) FROM users;
来源：http://lzd.shuidangran.top

[Q85] 数值取整
来源：http://kev.nanxinkj.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ckv.pengpengdd.cyou

[Q86] 读取 JSON 字段
来源：http://gpi.xinyue.icu

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://way.uphjek.com

[Q87] JSON 字段做条件
来源：http://hts.dashuyun.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://sol.jiagoushi.top

[Q88] 行转列（条件聚合）
来源：http://rbc.bbcook.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://aqz.shanyushiyangkeji.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://tty.haohaochexian.top

[Q89] 判断表是否存在
来源：http://wml.xuetiantiany.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://qxc.gzhubu.top

[Q90] 生成序号列
来源：http://ncb.hfpthk.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://eop.hammf.cn

================================================================================
来源：http://yhu.ehwqpu.com

R. Bash 专题
来源：http://bag.9152youxi.cn

================================================================================
来源：http://tfq.hesvh.cn

[R01] shebang 与严格模式
来源：http://lhx.tanke756.top

#!/usr/bin/env bash
来源：http://rgz.uphjek.com

set -euo pipefail
来源：http://dtt.zhiwuduotai.top

[R02] 变量赋值与使用
来源：http://ybv.shuidangran.top

name="Tom"; echo "$name"
来源：http://djk.birdmap.top

[R03] 只读变量
来源：http://vop.xinyue.icu

readonly PI=3.14
来源：http://lqs.cashguo.top

[R04] 位置参数
来源：http://olf.hcnkem.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://zqk.jiagoushi.top

[R05] 参数默认值
来源：http://kmu.yj20258888.top

name="${1:-default}"
来源：http://chp.svipenyu.cn

[R06] 判断命令是否存在
来源：http://mkk.gotoacloud.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hjc.daxiang520.top

[R07] if 判断文件
来源：http://vzb.cucudq.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://tgv.guannengcc.top

[R08] 数值比较
来源：http://tfj.shzxlz.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://kzu.andypj.xyz

[R09] 字符串比较
来源：http://lay.tarul.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ado.feifeiyinyue.top

[R10] 正则匹配
来源：http://eiq.tian-w.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://gjn.ybcxt.top

[R11] case 多分支
来源：http://gjg.xylfe.cn

case "$1" in
来源：http://agz.cqqwz.cn

start) echo "启动" ;;
来源：http://vnb.tarul.cn

stop)  echo "停止" ;;
来源：http://jec.yvedp.cn

*)     echo "未知命令" ;;
来源：http://rwt.gzhubu.top

esac
来源：http://jsg.guowangkeji.top

[R12] for 遍历文件
来源：http://puf.jyoumei.cn

for f in *.txt; do echo "$f"; done
来源：http://hlm.chenjidiqi.icu

[R13] for 计数循环
来源：http://tci.zhongyouzk.top

for i in {1..10}; do echo "$i"; done
来源：http://viw.feifeiyinyue.top

[R14] C 风格 for
来源：http://skz.sjlbkw.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://bkb.svipenyu.cn

[R15] while 逐行读文件
来源：http://nwq.tarul.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://kdi.yj20258888.top

[R16] until 等待条件
来源：http://jxc.snrcjt.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ufh.hesvh.cn

[R17] 数组定义与取值
来源：http://puo.bbcook.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ehu.hammf.cn

[R18] 遍历数组
来源：http://gac.gotoacloud.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://zmu.tianlin.xyz

[R19] 数组长度
来源：http://rks.ehwqpu.com

echo "${#arr[@]}"
来源：http://gcv.fanxiaobao.xyz

[R20] 关联数组（字典）
来源：http://fyd.dianchejie.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://qyq.fktsv.cn

[R21] 字符串长度
来源：http://jcu.zdbjq.cn

echo "${#s}"
来源：http://lay.uphjek.com

[R22] 截取子串
来源：http://mdw.ydjk.org.cn

echo "${s:0:5}"
来源：http://kbj.ehwqpu.com

[R23] 字符串替换
来源：http://xce.ivvv.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hjb.jyoumei.cn

[R24] 大小写转换
来源：http://yru.meibo888.top

echo "${s^^}"; echo "${s,,}"
来源：http://wfc.hongshengwenyu.top

[R25] 去后缀 / 去前缀
来源：http://mwy.zycfv.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://bbv.vehdjk.com

[R26] 命令替换
来源：http://mho.zdbjq.cn

now=$(date +%F); echo "$now"
来源：http://viz.jinqigfzy.top

[R27] 算术展开
来源：http://fpn.jqgufenzy.top

echo $((1 + 2 * 3))
来源：http://yxz.jqgfzy.top

[R28] 浮点运算
来源：http://hzp.fktsv.cn

echo "scale=2; 10/3" | bc
来源：http://prv.shanyushiyangkeji.top

[R29] 定义函数
来源：http://wiv.fktsv.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mve.cucudq.cn

[R30] 函数返回状态码
来源：http://lyc.aibaodan.cn

f() { return 0; }; f || echo "失败了"
来源：http://mhd.jyoumei.cn

[R31] 局部变量
来源：http://nir.xziqi.cn

f() { local x=1; echo "$x"; }
来源：http://jjs.ydzc1.top

[R32] 参数个数校验
来源：http://bxi.gzhubu.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ada.hesvh.cn

[R33] 捕获错误并提示行号
来源：http://msf.zhixingplan.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://bsq.yj20258888.top

[R34] 退出时清理
来源：http://jnk.yanxiufei.cn

trap 'rm -f "$tmp"' EXIT
来源：http://rod.xinyue.icu

[R35] 后台执行并等待
来源：http://wgg.yuxming.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://kgx.yfazqb.com

[R36] 并发执行多个任务
来源：http://dhu.jinyuanbaomall.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://thy.yj202588.top

[R37] 把输出赋给变量
来源：http://pbr.tian-w.cn

files=$(ls -1)
来源：http://psa.aibaodan.cn

[R38] 管道串联
来源：http://ete.ppjwa.cn

cat a.txt | grep -i error | wc -l
来源：http://vez.smart0.xyz

[R39] 重定向标准输出与错误
来源：http://kqw.aibaodan.cn

cmd > out.log 2>&1
来源：http://qni.feifeiyinyue.top

[R40] 追加写日志
来源：http://xbs.chenlongwang.top

echo "log" >> out.log
来源：http://ssr.yangfankeji.com

[R41] 丢弃输出
来源：http://sgs.quarkkingdee.top

cmd >/dev/null 2>&1
来源：http://gtg.zhongyouzk.top

[R42] 输入重定向
来源：http://xxy.daria6918.cn

wc -l < a.txt
来源：http://sdp.yanxiufei.cn

[R43] 按名字查找文件
来源：http://dqj.xuetiantiany.cn


<!-- 参考信息 -->