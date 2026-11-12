代发 wailian999

);
来源：http://izj.bjfxy.top

[Q03] 增加列
来源：http://qzl.snrcjt.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://yse.xuetiantiany.cn

[Q04] 修改列类型
来源：http://fnb.jiagoushi.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://niq.birdmap.top

[Q05] 重命名列
来源：http://xyj.shuidangran.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://dey.zhengqikj.top

[Q06] 删除列
来源：http://nbk.ivvv.top

ALTER TABLE users DROP COLUMN age;
来源：http://uap.hammf.cn

[Q07] 删除表
来源：http://oje.jyoumei.cn

DROP TABLE IF EXISTS orders;
来源：http://gdt.zhaomingkeji.xyz

[Q08] 创建普通索引
来源：http://cap.pengpengdd.cyou

CREATE INDEX idx_users_email ON users(email);
来源：http://lsf.gzhubu.top

[Q09] 创建唯一索引
来源：http://hkf.fktsv.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://gms.redwolf501.top

[Q10] 插入单行
来源：http://gdd.zhaomingkeji.xyz

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://nee.yj20258.top

[Q11] 一次插入多行
来源：http://mpl.cqqwz.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hau.hywenlv.cn

[Q12] 插入后取自增 ID
来源：http://cwk.xingfuxueyuan.xyz

INSERT INTO users (name) VALUES ('C');
来源：http://uat.meibo888.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://qjp.52xcode.cn

[Q13] 忽略重复插入
来源：http://fll.xylfe.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ubb.sufxvd.cn

[Q14] 存在则更新（upsert）
来源：http://pao.pengpengdd.cyou

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://vjn.epnwcf.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wfj.zhiwuduotai.top

[Q15] 查询全部
来源：http://tzl.mhx1999.top

SELECT * FROM users;
来源：http://lio.jqgufenzy.top

[Q16] 查询指定列
来源：http://fix.wangdashe.top

SELECT id, name FROM users;
来源：http://wba.jyoumei.cn

[Q17] 条件查询
来源：http://muq.gotoacloud.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ccd.sysykeji.top

[Q18] 模糊匹配
来源：http://bzu.yonumen.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://pul.sjlbkw.cn

[Q19] 范围查询
来源：http://fyy.epnwcf.com

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://psj.bbcook.cn

[Q20] IN 列表
来源：http://xpz.fzhhl.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://erd.epnwcf.com

[Q21] 空值判断
来源：http://rqv.xingfuxueyuan.xyz

SELECT * FROM users WHERE email IS NULL;
来源：http://qop.chenlongwang.top

[Q22] 排序
来源：http://vpg.andypj.xyz

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://sxr.yangfankeji.com

[Q23] 分页
来源：http://ols.svipenyu.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://bzw.jinghuilouyu.cn

[Q24] 去重
来源：http://usd.pycfn.com

SELECT DISTINCT city FROM users;
来源：http://ohx.yueranfly.top

[Q25] 只取前 N 条
来源：http://ufp.jianghu66.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://zwa.zhixingplan.top

[Q26] 计数
来源：http://ora.jqgufenzy.top

SELECT COUNT(*) FROM users;
来源：http://inm.guowangkeji.top

[Q27] 条件计数
来源：http://los.nanxuanxn.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://uxi.havefunace.top

[Q28] 求和与平均
来源：http://axt.bbcook.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://rwk.jqgufenzy.top

[Q29] 最大最小值
来源：http://onc.smart0.xyz

SELECT MAX(age), MIN(age) FROM users;
来源：http://xke.tianlin.xyz

[Q30] 分组统计
来源：http://fug.9152youxi.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://xjf.gaohongyu789.top

[Q31] 分组后过滤
来源：http://wna.yfazqb.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://chd.zdbjq.cn

[Q32] 分组拼接字符串
来源：http://tya.0kj1m.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://irt.yj20258.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://cwi.fehbvm.com

[Q33] 多列分组
来源：http://dmi.yvedp.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hmw.ydjk.org.cn

[Q34] 每组取第一条
来源：http://ktp.ybcxt.top

SELECT * FROM (
来源：http://wvk.zhijiandao.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://afv.xziqi.cn

) t WHERE rn = 1;
来源：http://gxn.ywan-chungtsiang.top

[Q35] 内连接
来源：http://ysy.fengsongda.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://aay.yj20258888.top

[Q36] 左连接
来源：http://cvk.c1oappe.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://exm.gzhubu.top

[Q37] 右连接
来源：http://agq.yj20258888.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ibz.jinyuanbaomall.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ivw.guannengcc.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://pmp.cdnleiting.top

[Q39] 自连接（查上下级）
来源：http://ueb.feifeiyinyue.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://mzh.yvedp.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://vyo.yuxming.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://nnx.tarul.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://dey.dianchejie.cn

[Q41] 多表连接
来源：http://tva.iojbl.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://bgj.sweek.top

JOIN users u ON u.id = o.user_id
来源：http://hbk.pycfn.com

JOIN products p ON p.id = o.product_id;
来源：http://hlh.meibo888.top

[Q42] 连接条件附加过滤
来源：http://rfh.zycfv.cn

SELECT u.name, o.amount FROM users u
来源：http://hse.cashguo.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ayn.kuanghao11.cn

[Q43] 标量子查询
来源：http://kly.meibo888.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://dqe.xinyue.icu

[Q44] IN 子查询
来源：http://chd.tian-w.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://sut.cheryme.top

[Q45] EXISTS 判断存在
来源：http://ltq.tarul.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ada.xuetiantiany.cn

[Q46] NOT EXISTS 判断不存在
来源：http://fni.uphjek.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ktr.kuanghao11.cn

[Q47] 与平均值比较
来源：http://dwj.feifeiyinyue.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://iqr.chenjidiqi.icu

[Q48] CTE 公用表表达式
来源：http://tzg.daxiang520.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://dgs.ehwqpu.com

SELECT * FROM t WHERE c > 5;
来源：http://kfq.chenlongwang.top

[Q49] 更新单行
来源：http://wzj.iojbl.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://zgy.birdmap.top

[Q50] 批量更新
来源：http://cgd.hysaishi.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://cop.tarul.cn

[Q51] 用子查询更新
来源：http://axt.jqgufenzy.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://kqb.shanyushiyangtech.top

[Q52] 删除指定行
来源：http://yqp.jyoumei.cn

DELETE FROM users WHERE id = 10;
来源：http://ygb.sweek.top

[Q53] 按条件删除
来源：http://iwr.svipenyu.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mba.yvedp.cn

[Q54] 清空表
来源：http://nnj.zhongyouzk.top

TRUNCATE TABLE logs;
来源：http://kum.guowangkeji.top

[Q55] 排名（并列占位）
来源：http://xvh.gogol.net.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wct.fzhhl.top

[Q56] 密集排名（并列不占位）
来源：http://tba.jinqigufen.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://fca.yj20258.top

[Q57] 行号
来源：http://abm.mhx1999.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://jsm.cqqwz.cn

[Q58] 累计求和
来源：http://kal.gaohongyu789.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://paq.aizwys.cn

[Q59] 分组内累计
来源：http://tjw.cqqwz.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mym.yuxming.cn

[Q60] 取上一行 / 下一行
来源：http://den.haohaochexian.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wcr.ppjwa.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://lrk.jqgufenzy.top

[Q61] 移动平均
来源：http://lkh.nanxinkj.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hur.cucudq.cn

[Q62] 分组占比
来源：http://irx.wangshuangyany.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://luq.nwbrower.top

[Q63] 开启事务
来源：http://gfe.svipenyu.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ynj.shangyingyoupin.top

[Q64] 提交事务
来源：http://usd.hfpthk.cn

COMMIT;
来源：http://zyi.yfazqb.com

[Q65] 回滚事务
来源：http://mbb.zhengqikj.top

ROLLBACK;
来源：http://fnb.wangshuangyany.cn

[Q66] 行锁查询
来源：http://ift.feifeiyinyue.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://akg.vqdsnc.cn

[Q67] 设置隔离级别
来源：http://rsa.gzhubu.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://xaf.jiagoushi.top

[Q68] 保存点
来源：http://slq.yanxiufei.cn

SAVEPOINT sp1;
来源：http://dbz.gotoacloud.top

ROLLBACK TO sp1;
来源：http://dbh.jiagoushi.top

[Q69] 查看执行计划
来源：http://dai.zhiwuduotai.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ofx.wangdashe.top

[Q70] 更新统计信息
来源：http://yyf.zhongyouzk.top

ANALYZE TABLE users;
来源：http://zsg.xziqi.cn

[Q71] 查看建表语句
来源：http://usr.hcnkem.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://lvj.sufxvd.cn

[Q72] 查看索引
来源：http://qjw.yfazqb.com

SHOW INDEX FROM users;
来源：http://umi.yangfankeji.com

[Q73] 查看表状态
来源：http://rbe.0kj1m.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ulh.guowangkeji.top

[Q74] 强制使用索引
来源：http://mpw.smart0.xyz

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://lci.andypj.xyz

[Q75] 日期格式化
来源：http://jxv.yfazqb.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://tmp.shzxlz.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mfl.hfpthk.cn

[Q76] 按天统计
来源：http://fds.dianchejie.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://bwq.yfazqb.com

[Q77] 时间加减
来源：http://xej.xinyue.icu

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://iyg.shuidangran.top

[Q78] 当前时间
来源：http://hoa.yj20258888.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://nql.jiagoushi.top

[Q79] 字符串拼接
来源：http://byp.chenjidiqi.icu

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://leu.wangshuangyany.cn

[Q80] 字符串截取
来源：http://day.yonumen.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://nbw.fehbvm.com

[Q81] 字符串替换
来源：http://dfa.chenjidiqi.icu

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://iut.fzhhl.top

[Q82] 字符长度与字节长度
来源：http://xvx.zdqjudy.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wmq.epnwcf.com

[Q83] 大小写转换
来源：http://wtm.zdqjudy.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://feh.zhengqikj.top

[Q84] 去除首尾空格
来源：http://cap.yuxming.cn

SELECT TRIM(name) FROM users;
来源：http://odr.zhijiandao.cn

[Q85] 数值取整
来源：http://rob.hnqzz.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ltk.52xcode.cn

[Q86] 读取 JSON 字段
来源：http://rsa.snrcjt.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://zab.ehwqpu.com

[Q87] JSON 字段做条件
来源：http://yfj.uphjek.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://enh.quarkkingdee.top

[Q88] 行转列（条件聚合）
来源：http://gfg.smart0.xyz

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://drn.0kj1m.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://pfa.guannengcc.top

[Q89] 判断表是否存在
来源：http://wtt.cheryme.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://gyo.hfpthk.cn

[Q90] 生成序号列
来源：http://wfa.yuxming.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://gmp.shzxlz.cn

================================================================================
来源：http://yef.yongpay.top

R. Bash 专题
来源：http://ban.pycfn.com

================================================================================
来源：http://vci.pycfn.com

[R01] shebang 与严格模式
来源：http://gzm.sufxvd.cn

#!/usr/bin/env bash
来源：http://pls.cqqwz.cn

set -euo pipefail
来源：http://cpm.jyoumei.cn

[R02] 变量赋值与使用
来源：http://fzo.yvedp.cn

name="Tom"; echo "$name"
来源：http://asy.jiagoushi.top

[R03] 只读变量
来源：http://kxo.cheryme.top

readonly PI=3.14
来源：http://lip.zdbjq.cn

[R04] 位置参数
来源：http://vwq.dashuyun.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://npf.nwbrower.top

[R05] 参数默认值
来源：http://ntg.hfpthk.cn

name="${1:-default}"
来源：http://vpl.shanyushiyangkeji.top

[R06] 判断命令是否存在
来源：http://uki.guannengcc.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://rev.9152youxi.cn

[R07] if 判断文件
来源：http://qyo.vqdsnc.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://svf.jinghuilouyu.cn

[R08] 数值比较
来源：http://nxo.nanxuanxn.top

if (( a > b )); then echo "a 更大"; fi
来源：http://rpt.tian-w.cn

[R09] 字符串比较
来源：http://ked.gaohongyu789.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://qwb.hesvh.cn

[R10] 正则匹配
来源：http://jub.xuetiantiany.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://bbj.birdmap.top

[R11] case 多分支
来源：http://aoj.hesvh.cn

case "$1" in
来源：http://ved.cashguo.top

start) echo "启动" ;;
来源：http://pjz.jinqigfzy.top

stop)  echo "停止" ;;
来源：http://dfd.zdbjq.cn

*)     echo "未知命令" ;;
来源：http://yun.quarkkingdee.top

esac
来源：http://gwy.feifeiyinyue.top

[R12] for 遍历文件
来源：http://zso.sufxvd.cn

for f in *.txt; do echo "$f"; done
来源：http://voa.nwbrower.top

[R13] for 计数循环
来源：http://lar.zhiwuduotai.top

for i in {1..10}; do echo "$i"; done
来源：http://poa.cheryme.top

[R14] C 风格 for
来源：http://xpu.kuanghao11.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://qpp.uphjek.com

[R15] while 逐行读文件
来源：http://soo.jinqigfzy.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://lhm.tarul.cn

[R16] until 等待条件
来源：http://lod.vehdjk.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://vpt.sweek.top

[R17] 数组定义与取值
来源：http://khl.hnxiangtu.top

arr=(a b c); echo "${arr[0]}"
来源：http://jlr.pycfn.com

[R18] 遍历数组
来源：http://ibc.zhijiandao.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://jtl.0kj1m.cn

[R19] 数组长度
来源：http://gbo.epnwcf.com

echo "${#arr[@]}"
来源：http://irq.bbcook.cn

[R20] 关联数组（字典）
来源：http://evt.fengsongda.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://vjw.aizwys.cn

[R21] 字符串长度
来源：http://wru.zhaomingkeji.xyz

echo "${#s}"
来源：http://nze.wangshuangyany.cn

[R22] 截取子串
来源：http://gym.xylfe.cn

echo "${s:0:5}"
来源：http://bxx.c1oappe.top

[R23] 字符串替换
来源：http://nte.nwbrower.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://vik.zhengqikj.top

[R24] 大小写转换
来源：http://rck.vehdjk.com

echo "${s^^}"; echo "${s,,}"
来源：http://zhh.xylfe.cn

[R25] 去后缀 / 去前缀
来源：http://cxv.fehbvm.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://hpr.andypj.xyz

[R26] 命令替换
来源：http://xes.ctjpmb.com

now=$(date +%F); echo "$now"
来源：http://zck.52xcode.cn

[R27] 算术展开
来源：http://mxr.xziqi.cn

echo $((1 + 2 * 3))
来源：http://oxk.haohaochexian.top

[R28] 浮点运算
来源：http://ace.c1oappe.top

echo "scale=2; 10/3" | bc
来源：http://jvc.hfpthk.cn

[R29] 定义函数
来源：http://ygw.fehbvm.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://klh.yueranfly.top

[R30] 函数返回状态码
来源：http://zqx.feifeiyinyue.top

f() { return 0; }; f || echo "失败了"
来源：http://jvd.chenlongwang.top

[R31] 局部变量
来源：http://dkb.zhijiandao.cn

f() { local x=1; echo "$x"; }
来源：http://mit.meibo888.top

[R32] 参数个数校验
来源：http://uku.jqgfzy.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://lju.sjlbkw.cn

[R33] 捕获错误并提示行号
来源：http://rka.aibaodan.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://xnx.bjfxy.top

[R34] 退出时清理
来源：http://inv.jiagoushi.top

trap 'rm -f "$tmp"' EXIT
来源：http://dqq.cdnleiting.top

[R35] 后台执行并等待
来源：http://drl.jqgfzy.top

sleep 5 & pid=$!; wait "$pid"
来源：http://jyu.jyoumei.cn

[R36] 并发执行多个任务
来源：http://kvf.guannengcc.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://jpn.hcnkem.com

[R37] 把输出赋给变量
来源：http://cok.hywenlv.cn

files=$(ls -1)
来源：http://ssp.sysykeji.top

[R38] 管道串联
来源：http://qte.cqqwz.cn

cat a.txt | grep -i error | wc -l
来源：http://buu.ehwqpu.com

[R39] 重定向标准输出与错误
来源：http://ekv.jqgfzy.top

cmd > out.log 2>&1
来源：http://zwi.fktsv.cn

[R40] 追加写日志
来源：http://sfj.jqgufenzy.top

echo "log" >> out.log
来源：http://auy.tarul.cn

[R41] 丢弃输出
来源：http://zin.yvedp.cn

cmd >/dev/null 2>&1
来源：http://nyu.nanxuanxn.top

[R42] 输入重定向
来源：http://alv.zhiwuduotai.top

wc -l < a.txt
来源：http://axa.yj20258.top

[R43] 按名字查找文件
来源：http://huu.cucudq.cn

find . -name "*.log" -type f
来源：http://sgv.xuetiantiany.cn

[R44] 按修改时间查找
来源：http://mfh.iojbl.cn

find . -mtime -7 -type f
来源：http://gts.chenzaomai.com

[R45] 批量删除
来源：http://xzx.jinghuilouyu.cn

find . -name "*.tmp" -delete
来源：http://ebn.svipenyu.cn

[R46] 递归替换文件内容
来源：http://kix.kuanghao11.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://msi.9152youxi.cn

[R47] sed 单行替换
来源：http://mtj.sysykeji.top

sed -i 's/foo/bar/g' a.txt
来源：http://tmu.chenzaomai.com

[R48] awk 取指定列
来源：http://lpl.yj202588.top

awk '{print $1, $3}' a.txt
来源：http://cfg.yj202588.top

[R49] awk 带条件
来源：http://bhh.fktsv.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://aha.tarul.cn

[R50] awk 求和
来源：http://ybl.guowangkeji.top

awk '{s += $2} END {print s}' a.txt
来源：http://efq.xinyue.icu

[R51] 排序去重取前几
来源：http://qov.nanxuanxn.top


<!-- 参考信息 -->