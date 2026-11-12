代发 wailian999

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ohp.vqdsnc.cn

[Q05] 重命名列
来源：http://oef.gotoacloud.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hlm.andypj.xyz

[Q06] 删除列
来源：http://pas.jianghu66.top

ALTER TABLE users DROP COLUMN age;
来源：http://uef.jianghu66.top

[Q07] 删除表
来源：http://pdd.shanyushiyangtech.top

DROP TABLE IF EXISTS orders;
来源：http://pse.sjlbkw.cn

[Q08] 创建普通索引
来源：http://cxu.feifeiyinyue.top

CREATE INDEX idx_users_email ON users(email);
来源：http://bvt.ybcxt.top

[Q09] 创建唯一索引
来源：http://azo.gzhubu.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://cgn.c1oappe.top

[Q10] 插入单行
来源：http://quy.shuidangran.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://kuf.redwolf501.top

[Q11] 一次插入多行
来源：http://arh.hesvh.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://kso.shanyushiyangkeji.top

[Q12] 插入后取自增 ID
来源：http://gfc.gzhubu.top

INSERT INTO users (name) VALUES ('C');
来源：http://rxd.ppjwa.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://zmv.pengpengdd.cyou

[Q13] 忽略重复插入
来源：http://all.ydzc1.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://bhm.pengpengdd.cyou

[Q14] 存在则更新（upsert）
来源：http://uey.c1oappe.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://iwz.guowangkeji.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://jyw.yonumen.top

[Q15] 查询全部
来源：http://qxw.shangyingyoupin.top

SELECT * FROM users;
来源：http://njn.sufxvd.cn

[Q16] 查询指定列
来源：http://ijm.ybcxt.top

SELECT id, name FROM users;
来源：http://smz.jlsjyb.cn

[Q17] 条件查询
来源：http://wie.0kj1m.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://yhc.jinyuanbaomall.cn

[Q18] 模糊匹配
来源：http://mkt.gzhubu.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wun.aizwys.cn

[Q19] 范围查询
来源：http://dqm.dashuyun.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://pbw.gotoacloud.top

[Q20] IN 列表
来源：http://qxe.cashguo.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://gtg.yonumen.top

[Q21] 空值判断
来源：http://cdp.yj20258888.top

SELECT * FROM users WHERE email IS NULL;
来源：http://ebc.wangdashe.top

[Q22] 排序
来源：http://lji.guannengcc.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://obu.shzxlz.cn

[Q23] 分页
来源：http://poy.fengsongda.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://nxv.xuanzx.com

[Q24] 去重
来源：http://syg.wangdashe.top

SELECT DISTINCT city FROM users;
来源：http://zzg.haohaochexian.top

[Q25] 只取前 N 条
来源：http://zbe.xuetiantiany.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://xft.yueranfly.top

[Q26] 计数
来源：http://edx.shangyingyoupin.top

SELECT COUNT(*) FROM users;
来源：http://azr.vehdjk.com

[Q27] 条件计数
来源：http://zjo.yj20258.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://rgo.haohaochexian.top

[Q28] 求和与平均
来源：http://nyz.zhiwuduotai.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://zez.fehbvm.com

[Q29] 最大最小值
来源：http://avb.vehdjk.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://utq.yj202588.top

[Q30] 分组统计
来源：http://kws.sxryk.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://yxs.yfazqb.com

[Q31] 分组后过滤
来源：http://vmh.yj20258888.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://qxk.smart0.xyz

[Q32] 分组拼接字符串
来源：http://tfw.hysaishi.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://gip.xinyue.icu

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://yew.fanxiaobao.xyz

[Q33] 多列分组
来源：http://ogt.yj20258888.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://kvh.feifeiyinyue.top

[Q34] 每组取第一条
来源：http://epv.birdmap.top

SELECT * FROM (
来源：http://dyv.pengpengdd.cyou

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://neq.yonumen.top

) t WHERE rn = 1;
来源：http://mkt.hesvh.cn

[Q35] 内连接
来源：http://lag.gotoacloud.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://zdf.yj202588.top

[Q36] 左连接
来源：http://exb.hcnkem.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://gga.nanxinkj.top

[Q37] 右连接
来源：http://aha.shanyushiyangtech.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hbn.fehbvm.com

[Q38] 全外连接（PostgreSQL）
来源：http://nuv.fktsv.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://rbj.sweek.top

[Q39] 自连接（查上下级）
来源：http://zij.andypj.xyz

SELECT e.name, m.name AS manager FROM employees e
来源：http://rwz.sysykeji.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://pdx.yangfankeji.com

[Q40] 交叉连接（笛卡尔积）
来源：http://vew.ppjwa.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://zuy.uphjek.com

[Q41] 多表连接
来源：http://ocu.sxryk.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://rsz.jinyuanbaomall.cn

JOIN users u ON u.id = o.user_id
来源：http://ggl.hesvh.cn

JOIN products p ON p.id = o.product_id;
来源：http://twj.andypj.xyz

[Q42] 连接条件附加过滤
来源：http://mmx.havefunace.top

SELECT u.name, o.amount FROM users u
来源：http://odb.dashuyun.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://dhf.haohaochexian.top

[Q43] 标量子查询
来源：http://mxc.hysaishi.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://csc.zhijiandao.cn

[Q44] IN 子查询
来源：http://nwp.gaohongyu789.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://lao.tianlin.xyz

[Q45] EXISTS 判断存在
来源：http://wor.9152youxi.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kvr.ywan-chungtsiang.top

[Q46] NOT EXISTS 判断不存在
来源：http://jbv.jlsjyb.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://owc.cucudq.cn

[Q47] 与平均值比较
来源：http://tco.bbcook.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mqt.0kj1m.cn

[Q48] CTE 公用表表达式
来源：http://ymh.sxryk.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hks.jqgfzy.top

SELECT * FROM t WHERE c > 5;
来源：http://gzh.hammf.cn

[Q49] 更新单行
来源：http://kxq.zhengqikj.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wxd.zhijiandao.cn

[Q50] 批量更新
来源：http://zed.xuanzx.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ook.andypj.xyz

[Q51] 用子查询更新
来源：http://pzb.cashguo.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://xxz.hnxiangtu.top

[Q52] 删除指定行
来源：http://wqd.yfazqb.com

DELETE FROM users WHERE id = 10;
来源：http://lbv.zhaomingkeji.xyz

[Q53] 按条件删除
来源：http://cdk.vqdsnc.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://nvv.bjfxy.top

[Q54] 清空表
来源：http://fyj.pengpengdd.cyou

TRUNCATE TABLE logs;
来源：http://yop.jqgfzy.top

[Q55] 排名（并列占位）
来源：http://ist.feifeiyinyue.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://qwi.hcnkem.com

[Q56] 密集排名（并列不占位）
来源：http://zwl.xziqi.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://gsx.fehbvm.com

[Q57] 行号
来源：http://psh.xziqi.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mcg.tianlin.xyz

[Q58] 累计求和
来源：http://nar.xziqi.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://yiz.zhiwuduotai.top

[Q59] 分组内累计
来源：http://zwr.0kj1m.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://kko.tarul.cn

[Q60] 取上一行 / 下一行
来源：http://uqz.jqgfzy.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://oec.shanyushiyangtech.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://btt.yongpay.top

[Q61] 移动平均
来源：http://ssx.hammf.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://umy.meibo888.top

[Q62] 分组占比
来源：http://wob.jinqigufen.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://kua.birdmap.top

[Q63] 开启事务
来源：http://pud.cdnleiting.top

START TRANSACTION;                -- 或 BEGIN
来源：http://tfo.iojbl.cn

[Q64] 提交事务
来源：http://oxc.ydjk.org.cn

COMMIT;
来源：http://tkv.jlsjyb.cn

[Q65] 回滚事务
来源：http://ifv.hysaishi.cn

ROLLBACK;
来源：http://ies.sweek.top

[Q66] 行锁查询
来源：http://vvt.tanke756.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://iyg.9152youxi.cn

[Q67] 设置隔离级别
来源：http://vvr.jyoumei.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://gcw.wangdashe.top

[Q68] 保存点
来源：http://tsl.jlsjyb.cn

SAVEPOINT sp1;
来源：http://hko.zdbjq.cn

ROLLBACK TO sp1;
来源：http://nnn.meibo888.top

[Q69] 查看执行计划
来源：http://ayx.zhengqikj.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://iwj.nwbrower.top

[Q70] 更新统计信息
来源：http://vpi.zhijiandao.cn

ANALYZE TABLE users;
来源：http://ofg.dianchejie.cn

[Q71] 查看建表语句
来源：http://aij.shangyingyoupin.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ais.ppjwa.cn

[Q72] 查看索引
来源：http://psv.fengsongda.top

SHOW INDEX FROM users;
来源：http://avr.hammf.cn

[Q73] 查看表状态
来源：http://edu.daria6918.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://awu.yanxiufei.cn

[Q74] 强制使用索引
来源：http://rjb.vehdjk.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ekj.yvedp.cn

[Q75] 日期格式化
来源：http://rxx.vehdjk.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ruw.ydzc1.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://pig.cashguo.top

[Q76] 按天统计
来源：http://hzy.gaohongyu789.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://oht.jyoumei.cn

[Q77] 时间加减
来源：http://huj.hammf.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wsa.nwbrower.top

[Q78] 当前时间
来源：http://cbf.guannengcc.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://nym.tarul.cn

[Q79] 字符串拼接
来源：http://ktx.zdbjq.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://qbd.hfpthk.cn

[Q80] 字符串截取
来源：http://mrv.gogol.net.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ugy.mhx1999.top

[Q81] 字符串替换
来源：http://wsf.haohaochexian.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://bqw.xylfe.cn

[Q82] 字符长度与字节长度
来源：http://xsx.hnxiangtu.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://def.aizwys.cn

[Q83] 大小写转换
来源：http://ddz.pycfn.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hfq.yuanzhike.top

[Q84] 去除首尾空格
来源：http://cnv.nanxinkj.top

SELECT TRIM(name) FROM users;
来源：http://zkr.vqdsnc.cn

[Q85] 数值取整
来源：http://sco.jlsjyb.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://pyo.ivvv.top

[Q86] 读取 JSON 字段
来源：http://dhk.jinyuanbaomall.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wcp.yj20258888.top

[Q87] JSON 字段做条件
来源：http://trd.jianghu66.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mit.c1oappe.top

[Q88] 行转列（条件聚合）
来源：http://ixn.jqgfzy.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://nlw.sysykeji.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://uew.ywan-chungtsiang.top

[Q89] 判断表是否存在
来源：http://gkf.shuidangran.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://eqc.sysykeji.top

[Q90] 生成序号列
来源：http://bmh.xziqi.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://jqx.tarul.cn

================================================================================
来源：http://gfj.zdqjudy.top

R. Bash 专题
来源：http://iuw.xziqi.cn

================================================================================
来源：http://wwp.sjlbkw.cn

[R01] shebang 与严格模式
来源：http://ddh.fengsongda.top

#!/usr/bin/env bash
来源：http://lqr.cucudq.cn

set -euo pipefail
来源：http://roa.shanyushiyangkeji.top

[R02] 变量赋值与使用
来源：http://sdl.ehwqpu.com

name="Tom"; echo "$name"
来源：http://bsi.epnwcf.com

[R03] 只读变量
来源：http://rka.0kj1m.cn

readonly PI=3.14
来源：http://clw.zhixingplan.top

[R04] 位置参数
来源：http://sbv.0kj1m.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://efu.tanke756.top

[R05] 参数默认值
来源：http://drq.redwolf501.top

name="${1:-default}"
来源：http://wnk.jlsjyb.cn

[R06] 判断命令是否存在
来源：http://izk.52xcode.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://xyo.yfazqb.com

[R07] if 判断文件
来源：http://hje.hammf.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hcx.zhengqikj.top

[R08] 数值比较
来源：http://ibn.xuetiantiany.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://tsy.hammf.cn

[R09] 字符串比较
来源：http://kel.tianlin.xyz

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://zgr.fktsv.cn

[R10] 正则匹配
来源：http://sir.fehbvm.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://tmm.shzxlz.cn

[R11] case 多分支
来源：http://hjt.guannengcc.top

case "$1" in
来源：http://crx.0kj1m.cn

start) echo "启动" ;;
来源：http://yif.yvedp.cn

stop)  echo "停止" ;;
来源：http://fiq.cdnleiting.top

*)     echo "未知命令" ;;
来源：http://uyr.zycfv.cn

esac
来源：http://lvy.daria6918.cn

[R12] for 遍历文件
来源：http://kbp.aibaodan.cn

for f in *.txt; do echo "$f"; done
来源：http://oqz.ctjpmb.com

[R13] for 计数循环
来源：http://zfi.chenzaomai.com

for i in {1..10}; do echo "$i"; done
来源：http://cub.xziqi.cn

[R14] C 风格 for
来源：http://wye.pycfn.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://haw.hongshengwenyu.top

[R15] while 逐行读文件
来源：http://zdw.ivvv.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://xpb.jianghu66.top

[R16] until 等待条件
来源：http://fpo.316326.xyz

until [[ -f done.flag ]]; do sleep 1; done
来源：http://xqv.wangshuangyany.cn

[R17] 数组定义与取值
来源：http://ytl.sjlbkw.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ohk.yuanzhike.top

[R18] 遍历数组
来源：http://hpl.jinqigfzy.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://fub.vqdsnc.cn

[R19] 数组长度
来源：http://zld.ppjwa.cn

echo "${#arr[@]}"
来源：http://kzr.xuanzx.com

[R20] 关联数组（字典）
来源：http://ovg.fzhhl.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://kny.chenjidiqi.icu

[R21] 字符串长度
来源：http://wgl.hcnkem.com

echo "${#s}"
来源：http://syb.chenjidiqi.icu

[R22] 截取子串
来源：http://yrg.yonumen.top

echo "${s:0:5}"
来源：http://cjs.jqgufenzy.top

[R23] 字符串替换
来源：http://zzc.yj20258.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://vew.daria6918.cn

[R24] 大小写转换
来源：http://cnm.nanxinkj.top

echo "${s^^}"; echo "${s,,}"
来源：http://fpz.ybcxt.top

[R25] 去后缀 / 去前缀
来源：http://sfq.vqdsnc.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://bsp.yongpay.top

[R26] 命令替换
来源：http://oej.gzhubu.top

now=$(date +%F); echo "$now"
来源：http://nvn.bjfxy.top

[R27] 算术展开
来源：http://nfo.shanyushiyangkeji.top

echo $((1 + 2 * 3))
来源：http://lcc.cucudq.cn

[R28] 浮点运算
来源：http://xgd.yueranfly.top

echo "scale=2; 10/3" | bc
来源：http://bre.nanxinkj.top

[R29] 定义函数
来源：http://cbd.nanxinkj.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://nvq.yvedp.cn

[R30] 函数返回状态码
来源：http://phk.hfpthk.cn

f() { return 0; }; f || echo "失败了"
来源：http://cpr.meibo888.top

[R31] 局部变量
来源：http://ckj.shzxlz.cn

f() { local x=1; echo "$x"; }
来源：http://gbr.fanxiaobao.xyz

[R32] 参数个数校验
来源：http://fpk.cashguo.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://jmx.cqqwz.cn

[R33] 捕获错误并提示行号
来源：http://pis.zhiwuduotai.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://glm.aibaodan.cn

[R34] 退出时清理
来源：http://yiq.sysykeji.top

trap 'rm -f "$tmp"' EXIT
来源：http://otx.yangfankeji.com

[R35] 后台执行并等待
来源：http://kro.shangyingyoupin.top

sleep 5 & pid=$!; wait "$pid"
来源：http://rnp.ywan-chungtsiang.top

[R36] 并发执行多个任务
来源：http://xkc.zhixingplan.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://zli.yuxming.cn

[R37] 把输出赋给变量
来源：http://vrw.ehwqpu.com

files=$(ls -1)
来源：http://rzq.feifeiyinyue.top

[R38] 管道串联
来源：http://pda.redwolf501.top

cat a.txt | grep -i error | wc -l
来源：http://lbj.hesvh.cn

[R39] 重定向标准输出与错误
来源：http://dgc.cdnleiting.top

cmd > out.log 2>&1
来源：http://tni.birdmap.top

[R40] 追加写日志
来源：http://sph.nanxinkj.top

echo "log" >> out.log
来源：http://twl.fengsongda.top

[R41] 丢弃输出
来源：http://eqw.bbcook.cn

cmd >/dev/null 2>&1
来源：http://pcd.mhx1999.top

[R42] 输入重定向
来源：http://ith.tanke756.top

wc -l < a.txt
来源：http://xgt.52xcode.cn

[R43] 按名字查找文件
来源：http://fjn.quarkkingdee.top

find . -name "*.log" -type f
来源：http://uci.ctjpmb.com

[R44] 按修改时间查找
来源：http://wmt.dashuyun.cn

find . -mtime -7 -type f
来源：http://gjf.jinqigufen.top

[R45] 批量删除
来源：http://kui.gogol.net.cn

find . -name "*.tmp" -delete
来源：http://qtk.tanke756.top

[R46] 递归替换文件内容
来源：http://svg.gaohongyu789.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://pjl.xinyue.icu

[R47] sed 单行替换
来源：http://yos.sweek.top

sed -i 's/foo/bar/g' a.txt
来源：http://qdc.jianghu66.top

[R48] awk 取指定列
来源：http://gon.xuetiantiany.cn

awk '{print $1, $3}' a.txt
来源：http://mif.tanke756.top

[R49] awk 带条件
来源：http://jzu.fengsongda.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ftz.gogol.net.cn

[R50] awk 求和
来源：http://cda.daria6918.cn

awk '{s += $2} END {print s}' a.txt
来源：http://gnk.jqgfzy.top

[R51] 排序去重取前几
来源：http://oou.sufxvd.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ral.aizwys.cn

[R52] 统计行数
来源：http://nru.andypj.xyz

wc -l a.txt
来源：http://dnc.fzhhl.top

[R53] 查看文件头与实时尾
来源：http://ljf.jinyuanbaomall.cn


<!-- 参考信息 -->