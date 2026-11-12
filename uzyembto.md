代发 wailian999

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://zhz.vehdjk.com

[Q05] 重命名列
来源：http://bkk.ppjwa.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://tnh.c1oappe.top

[Q06] 删除列
来源：http://wuj.fzhhl.top

ALTER TABLE users DROP COLUMN age;
来源：http://jkj.gogol.net.cn

[Q07] 删除表
来源：http://xxt.nwbrower.top

DROP TABLE IF EXISTS orders;
来源：http://suv.xinyue.icu

[Q08] 创建普通索引
来源：http://tob.jyoumei.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://grj.pengpengdd.cyou

[Q09] 创建唯一索引
来源：http://wve.fzhhl.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wmt.sweek.top

[Q10] 插入单行
来源：http://coy.cucudq.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://zfr.jinyuanbaomall.cn

[Q11] 一次插入多行
来源：http://slv.c1oappe.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://tve.jinqigufen.top

[Q12] 插入后取自增 ID
来源：http://pjn.cucudq.cn

INSERT INTO users (name) VALUES ('C');
来源：http://mjk.meibo888.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://glp.jinyuanbaomall.cn

[Q13] 忽略重复插入
来源：http://lja.dianchejie.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://zpd.ydzc1.top

[Q14] 存在则更新（upsert）
来源：http://xrh.fehbvm.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://qjt.bbcook.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://sqw.jlsjyb.cn

[Q15] 查询全部
来源：http://gxn.ctjpmb.com

SELECT * FROM users;
来源：http://vbz.jianghu66.top

[Q16] 查询指定列
来源：http://ygf.hcnkem.com

SELECT id, name FROM users;
来源：http://ffc.cqqwz.cn

[Q17] 条件查询
来源：http://fjj.jiagoushi.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ucg.daxiang520.top

[Q18] 模糊匹配
来源：http://fsu.fanxiaobao.xyz

SELECT * FROM users WHERE name LIKE '张%';
来源：http://erl.haohaochexian.top

[Q19] 范围查询
来源：http://gkn.sysykeji.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ifj.fehbvm.com

[Q20] IN 列表
来源：http://lic.tarul.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://lem.yueranfly.top

[Q21] 空值判断
来源：http://crm.kuanghao11.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://idn.jinqigufen.top

[Q22] 排序
来源：http://qgw.birdmap.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://xrj.mhx1999.top

[Q23] 分页
来源：http://bpu.wangshuangyany.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ccz.aibaodan.cn

[Q24] 去重
来源：http://hex.xinyue.icu

SELECT DISTINCT city FROM users;
来源：http://qjx.zhixingplan.top

[Q25] 只取前 N 条
来源：http://hyx.jlsjyb.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ojq.hammf.cn

[Q26] 计数
来源：http://ynz.ehwqpu.com

SELECT COUNT(*) FROM users;
来源：http://iqv.yj202588.top

[Q27] 条件计数
来源：http://igi.tarul.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ibx.guannengcc.top

[Q28] 求和与平均
来源：http://gdy.hywenlv.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://fgw.ydzc1.top

[Q29] 最大最小值
来源：http://krg.shuidangran.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://mpv.shzxlz.cn

[Q30] 分组统计
来源：http://vis.bbcook.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://fvj.yangfankeji.com

[Q31] 分组后过滤
来源：http://diq.hnxiangtu.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://apb.chenlongwang.top

[Q32] 分组拼接字符串
来源：http://uxd.yuanzhike.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ldp.ydzc1.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ngj.fzhhl.top

[Q33] 多列分组
来源：http://thq.iojbl.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://iow.meibo888.top

[Q34] 每组取第一条
来源：http://dsd.cashguo.top

SELECT * FROM (
来源：http://yiw.hammf.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://vrx.zhiwuduotai.top

) t WHERE rn = 1;
来源：http://sug.haohaochexian.top

[Q35] 内连接
来源：http://qwc.jlsjyb.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://bxh.hongshengwenyu.top

[Q36] 左连接
来源：http://yfg.guowangkeji.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://odq.ybcxt.top

[Q37] 右连接
来源：http://kfr.fehbvm.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://rdb.ybcxt.top

[Q38] 全外连接（PostgreSQL）
来源：http://luy.shanyushiyangkeji.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://gir.vqdsnc.cn

[Q39] 自连接（查上下级）
来源：http://ujb.zycfv.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://cjc.smart0.xyz

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://zqc.kuanghao11.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://qhn.hnxiangtu.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://phe.hammf.cn

[Q41] 多表连接
来源：http://hnr.chenjidiqi.icu

SELECT o.id, u.name, p.title FROM orders o
来源：http://kbv.52xcode.cn

JOIN users u ON u.id = o.user_id
来源：http://xxs.nanxuanxn.top

JOIN products p ON p.id = o.product_id;
来源：http://skn.dianchejie.cn

[Q42] 连接条件附加过滤
来源：http://cul.jiagoushi.top

SELECT u.name, o.amount FROM users u
来源：http://qbi.yfazqb.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://qkb.jinqigufen.top

[Q43] 标量子查询
来源：http://eid.fehbvm.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://zbg.ydjk.org.cn

[Q44] IN 子查询
来源：http://eft.redwolf501.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://qkg.meibo888.top

[Q45] EXISTS 判断存在
来源：http://nrb.redwolf501.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://reo.shzxlz.cn

[Q46] NOT EXISTS 判断不存在
来源：http://lke.daria6918.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://uzo.chenjidiqi.icu

[Q47] 与平均值比较
来源：http://txr.hongshengwenyu.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://eqj.yanxiufei.cn

[Q48] CTE 公用表表达式
来源：http://klj.cucudq.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hcj.cdnleiting.top

SELECT * FROM t WHERE c > 5;
来源：http://cow.xuanzx.com

[Q49] 更新单行
来源：http://xsa.nanxuanxn.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://emy.yuanzhike.top

[Q50] 批量更新
来源：http://kgw.fzhhl.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://rlh.jqgufenzy.top

[Q51] 用子查询更新
来源：http://vur.hfpthk.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://jim.316326.xyz

[Q52] 删除指定行
来源：http://oxc.smart0.xyz

DELETE FROM users WHERE id = 10;
来源：http://hsy.yuxming.cn

[Q53] 按条件删除
来源：http://eec.aizwys.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://lpz.jyoumei.cn

[Q54] 清空表
来源：http://mgz.zdbjq.cn

TRUNCATE TABLE logs;
来源：http://tau.yvedp.cn

[Q55] 排名（并列占位）
来源：http://irk.fanxiaobao.xyz

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://qxv.zhongyouzk.top

[Q56] 密集排名（并列不占位）
来源：http://roo.tianlin.xyz

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://cna.tian-w.cn

[Q57] 行号
来源：http://bao.hywenlv.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://qtr.jqgufenzy.top

[Q58] 累计求和
来源：http://iwd.daxiang520.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://twa.zycfv.cn

[Q59] 分组内累计
来源：http://wra.jinqigufen.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://swj.hfpthk.cn

[Q60] 取上一行 / 下一行
来源：http://gpy.yuanzhike.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://fhh.ehwqpu.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ykd.tanke756.top

[Q61] 移动平均
来源：http://kkh.feifeiyinyue.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://lyv.dashuyun.cn

[Q62] 分组占比
来源：http://igg.aibaodan.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://oib.hammf.cn

[Q63] 开启事务
来源：http://cho.cucudq.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://whw.yonumen.top

[Q64] 提交事务
来源：http://pzn.52xcode.cn

COMMIT;
来源：http://eph.9152youxi.cn

[Q65] 回滚事务
来源：http://jpy.zhaomingkeji.xyz

ROLLBACK;
来源：http://vjh.hysaishi.cn

[Q66] 行锁查询
来源：http://bmb.52xcode.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wjs.tanke756.top

[Q67] 设置隔离级别
来源：http://wfg.cdnleiting.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://rfb.andypj.xyz

[Q68] 保存点
来源：http://qmh.zdbjq.cn

SAVEPOINT sp1;
来源：http://fyp.yongpay.top

ROLLBACK TO sp1;
来源：http://dnq.ivvv.top

[Q69] 查看执行计划
来源：http://ifl.sjlbkw.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://bok.bbcook.cn

[Q70] 更新统计信息
来源：http://jgd.sweek.top

ANALYZE TABLE users;
来源：http://pok.shanyushiyangtech.top

[Q71] 查看建表语句
来源：http://xov.sjlbkw.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://gdz.nwbrower.top

[Q72] 查看索引
来源：http://csk.chenlongwang.top

SHOW INDEX FROM users;
来源：http://opy.jqgufenzy.top

[Q73] 查看表状态
来源：http://tyr.xinyue.icu

SHOW TABLE STATUS LIKE 'users';
来源：http://tam.fengsongda.top

[Q74] 强制使用索引
来源：http://mkv.yangfankeji.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ciu.zhiwuduotai.top

[Q75] 日期格式化
来源：http://ksu.ivvv.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ytm.uphjek.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://lox.sweek.top

[Q76] 按天统计
来源：http://xcv.zycfv.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://nua.gotoacloud.top

[Q77] 时间加减
来源：http://aoe.mhx1999.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hnq.nanxuanxn.top

[Q78] 当前时间
来源：http://zhq.0kj1m.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hfw.aibaodan.cn

[Q79] 字符串拼接
来源：http://gpf.cucudq.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mod.jyoumei.cn

[Q80] 字符串截取
来源：http://ubw.hywenlv.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ymg.pycfn.com

[Q81] 字符串替换
来源：http://peg.jqgfzy.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ehh.gogol.net.cn

[Q82] 字符长度与字节长度
来源：http://ttt.sweek.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://dza.havefunace.top

[Q83] 大小写转换
来源：http://jir.nwbrower.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://amq.ehwqpu.com

[Q84] 去除首尾空格
来源：http://pxl.0kj1m.cn

SELECT TRIM(name) FROM users;
来源：http://osf.fktsv.cn

[Q85] 数值取整
来源：http://iwx.hnxiangtu.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://thn.yangfankeji.com

[Q86] 读取 JSON 字段
来源：http://aiq.zdbjq.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wuy.nanxuanxn.top

[Q87] JSON 字段做条件
来源：http://pwi.zdqjudy.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://yvg.xuetiantiany.cn

[Q88] 行转列（条件聚合）
来源：http://ukf.ehwqpu.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://sgi.316326.xyz

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://cem.ybcxt.top

[Q89] 判断表是否存在
来源：http://nvl.havefunace.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://swf.xylfe.cn

[Q90] 生成序号列
来源：http://bxx.shanyushiyangtech.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wjv.ydzc1.top

================================================================================
来源：http://wyb.xinyue.icu

R. Bash 专题
来源：http://jnq.jinqigufen.top

================================================================================
来源：http://cuj.chenjidiqi.icu

[R01] shebang 与严格模式
来源：http://xqz.zhaomingkeji.xyz

#!/usr/bin/env bash
来源：http://wec.jinyuanbaomall.cn

set -euo pipefail
来源：http://oee.zhongyouzk.top

[R02] 变量赋值与使用
来源：http://sgd.zhoulong.xyz

name="Tom"; echo "$name"
来源：http://czt.yj20258.top

[R03] 只读变量
来源：http://zcc.birdmap.top

readonly PI=3.14
来源：http://pvy.tian-w.cn

[R04] 位置参数
来源：http://udg.hammf.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://bai.hcnkem.com

[R05] 参数默认值
来源：http://ypa.ybcxt.top

name="${1:-default}"
来源：http://gpa.jqgufenzy.top

[R06] 判断命令是否存在
来源：http://zef.ydzc1.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://emm.sjlbkw.cn

[R07] if 判断文件
来源：http://qzd.yuanzhike.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://aab.ivvv.top

[R08] 数值比较
来源：http://imy.epnwcf.com

if (( a > b )); then echo "a 更大"; fi
来源：http://qui.jinqigufen.top

[R09] 字符串比较
来源：http://vyh.sweek.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://cxq.gzhubu.top

[R10] 正则匹配
来源：http://nwc.52xcode.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://sik.jiagoushi.top

[R11] case 多分支
来源：http://gfw.ydjk.org.cn

case "$1" in
来源：http://uxw.gaohongyu789.top

start) echo "启动" ;;
来源：http://fix.hcnkem.com

stop)  echo "停止" ;;
来源：http://epp.chenzaomai.com

*)     echo "未知命令" ;;
来源：http://aok.meibo888.top

esac
来源：http://pcm.chenzaomai.com

[R12] for 遍历文件
来源：http://tij.xinyue.icu

for f in *.txt; do echo "$f"; done
来源：http://aws.ybcxt.top

[R13] for 计数循环
来源：http://anh.hongshengwenyu.top

for i in {1..10}; do echo "$i"; done
来源：http://njk.9152youxi.cn

[R14] C 风格 for
来源：http://ixz.ctjpmb.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://xuk.ybcxt.top

[R15] while 逐行读文件
来源：http://frc.jinqigfzy.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://smo.jiagoushi.top

[R16] until 等待条件
来源：http://kem.ydzc1.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://llr.chenlongwang.top

[R17] 数组定义与取值
来源：http://tth.sufxvd.cn

arr=(a b c); echo "${arr[0]}"
来源：http://fgi.yonumen.top

[R18] 遍历数组
来源：http://vpj.guowangkeji.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ker.xinyue.icu

[R19] 数组长度
来源：http://qcc.xingfuxueyuan.xyz

echo "${#arr[@]}"
来源：http://vxb.ywan-chungtsiang.top

[R20] 关联数组（字典）
来源：http://cnd.yuxming.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://fnm.yonumen.top

[R21] 字符串长度
来源：http://ohg.tianlin.xyz

echo "${#s}"
来源：http://png.ywan-chungtsiang.top

[R22] 截取子串
来源：http://vqq.vehdjk.com

echo "${s:0:5}"
来源：http://jqq.uphjek.com

[R23] 字符串替换
来源：http://mdx.chenlongwang.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://gai.xziqi.cn

[R24] 大小写转换
来源：http://kiu.zhiwuduotai.top

echo "${s^^}"; echo "${s,,}"
来源：http://ekz.daria6918.cn

[R25] 去后缀 / 去前缀
来源：http://qlx.jinyuanbaomall.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://mfs.tianlin.xyz

[R26] 命令替换
来源：http://ila.daxiang520.top

now=$(date +%F); echo "$now"
来源：http://kld.bbcook.cn

[R27] 算术展开
来源：http://edv.uphjek.com

echo $((1 + 2 * 3))
来源：http://ecm.yj20258888.top

[R28] 浮点运算
来源：http://dsh.0kj1m.cn

echo "scale=2; 10/3" | bc
来源：http://mgj.cdnleiting.top

[R29] 定义函数
来源：http://tjp.hysaishi.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ltl.nanxuanxn.top

[R30] 函数返回状态码
来源：http://lid.jinqigufen.top

f() { return 0; }; f || echo "失败了"
来源：http://fjw.vqdsnc.cn

[R31] 局部变量
来源：http://jsa.zhijiandao.cn

f() { local x=1; echo "$x"; }
来源：http://dlg.vqdsnc.cn

[R32] 参数个数校验
来源：http://uuf.uphjek.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hpm.nanxuanxn.top

[R33] 捕获错误并提示行号
来源：http://ihb.wangshuangyany.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://oqh.jinghuilouyu.cn

[R34] 退出时清理
来源：http://ois.vqdsnc.cn

trap 'rm -f "$tmp"' EXIT
来源：http://wsp.sxryk.cn

[R35] 后台执行并等待
来源：http://ysv.zdbjq.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://xmb.sufxvd.cn

[R36] 并发执行多个任务
来源：http://hji.shanyushiyangkeji.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://lmy.gogol.net.cn

[R37] 把输出赋给变量
来源：http://ivw.9152youxi.cn

files=$(ls -1)
来源：http://pru.zhaomingkeji.xyz

[R38] 管道串联
来源：http://yhf.sufxvd.cn

cat a.txt | grep -i error | wc -l
来源：http://iof.cheryme.top

[R39] 重定向标准输出与错误
来源：http://cth.chenlongwang.top

cmd > out.log 2>&1
来源：http://thi.zdqjudy.top

[R40] 追加写日志
来源：http://brk.hysaishi.cn

echo "log" >> out.log
来源：http://xgf.jyoumei.cn

[R41] 丢弃输出
来源：http://cax.daria6918.cn

cmd >/dev/null 2>&1
来源：http://rkd.ppjwa.cn

[R42] 输入重定向
来源：http://jnk.hongshengwenyu.top

wc -l < a.txt
来源：http://noa.shanyushiyangkeji.top

[R43] 按名字查找文件
来源：http://fkf.hnxiangtu.top

find . -name "*.log" -type f
来源：http://sqf.sweek.top

[R44] 按修改时间查找
来源：http://mlz.fehbvm.com

find . -mtime -7 -type f
来源：http://mjh.hammf.cn

[R45] 批量删除
来源：http://dav.yueranfly.top

find . -name "*.tmp" -delete
来源：http://cxd.sjlbkw.cn

[R46] 递归替换文件内容
来源：http://xjm.quarkkingdee.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://fdp.fktsv.cn

[R47] sed 单行替换
来源：http://usb.bbcook.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ybf.hfpthk.cn

[R48] awk 取指定列
来源：http://ukb.ivvv.top

awk '{print $1, $3}' a.txt
来源：http://tbr.316326.xyz

[R49] awk 带条件
来源：http://okz.sysykeji.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://kcd.mhx1999.top

[R50] awk 求和
来源：http://ywd.shanyushiyangtech.top

awk '{s += $2} END {print s}' a.txt
来源：http://whs.hammf.cn

[R51] 排序去重取前几
来源：http://bwk.daria6918.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ewl.nanxinkj.top

[R52] 统计行数
来源：http://kyw.fanxiaobao.xyz

wc -l a.txt
来源：http://ocn.jiagoushi.top

[R53] 查看文件头与实时尾
来源：http://tno.cashguo.top


<!-- 参考信息 -->