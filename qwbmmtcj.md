代发 wailian999

CREATE INDEX idx_users_email ON users(email);
来源：http://ofm.jinqigfzy.top

[Q09] 创建唯一索引
来源：http://woc.havefunace.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://gag.hesvh.cn

[Q10] 插入单行
来源：http://abq.hywenlv.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://vfh.yuxming.cn

[Q11] 一次插入多行
来源：http://rzf.vehdjk.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://gvq.xziqi.cn

[Q12] 插入后取自增 ID
来源：http://tiw.dianchejie.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ziu.shanyushiyangtech.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://aca.sweek.top

[Q13] 忽略重复插入
来源：http://sby.jlsjyb.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://agz.zdbjq.cn

[Q14] 存在则更新（upsert）
来源：http://rwr.yueranfly.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://kkd.zhaomingkeji.xyz

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://uhf.52xcode.cn

[Q15] 查询全部
来源：http://uev.zycfv.cn

SELECT * FROM users;
来源：http://gme.epnwcf.com

[Q16] 查询指定列
来源：http://fwy.zhoulong.xyz

SELECT id, name FROM users;
来源：http://ppq.9152youxi.cn

[Q17] 条件查询
来源：http://tpv.yvedp.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://iww.jyoumei.cn

[Q18] 模糊匹配
来源：http://ykd.svipenyu.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://uqh.aibaodan.cn

[Q19] 范围查询
来源：http://idq.jianghu66.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://pkl.aibaodan.cn

[Q20] IN 列表
来源：http://lpe.hywenlv.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ciz.jyoumei.cn

[Q21] 空值判断
来源：http://znv.xinyue.icu

SELECT * FROM users WHERE email IS NULL;
来源：http://wma.shanyushiyangtech.top

[Q22] 排序
来源：http://wgi.guannengcc.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://fau.ydjk.org.cn

[Q23] 分页
来源：http://fzi.uphjek.com

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://gsd.hysaishi.cn

[Q24] 去重
来源：http://rci.cheryme.top

SELECT DISTINCT city FROM users;
来源：http://yde.gogol.net.cn

[Q25] 只取前 N 条
来源：http://oxw.gzhubu.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://urk.yvedp.cn

[Q26] 计数
来源：http://eki.wangshuangyany.cn

SELECT COUNT(*) FROM users;
来源：http://ohe.birdmap.top

[Q27] 条件计数
来源：http://gjx.yueranfly.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://udr.hfpthk.cn

[Q28] 求和与平均
来源：http://wdr.tanke756.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://qgo.mhx1999.top

[Q29] 最大最小值
来源：http://nwf.ydzc1.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://wwa.tian-w.cn

[Q30] 分组统计
来源：http://vge.cheryme.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://lgx.fzhhl.top

[Q31] 分组后过滤
来源：http://wxa.chenjidiqi.icu

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ihl.jqgufenzy.top

[Q32] 分组拼接字符串
来源：http://ojf.nwbrower.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://qxy.fanxiaobao.xyz

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://phx.xuanzx.com

[Q33] 多列分组
来源：http://qke.dianchejie.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://vlg.shanyushiyangtech.top

[Q34] 每组取第一条
来源：http://ole.shangyingyoupin.top

SELECT * FROM (
来源：http://fob.ppjwa.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://nla.ywan-chungtsiang.top

) t WHERE rn = 1;
来源：http://uwe.yj20258888.top

[Q35] 内连接
来源：http://yfh.sweek.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://pzo.fengsongda.top

[Q36] 左连接
来源：http://rwz.yanxiufei.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://osx.gzhubu.top

[Q37] 右连接
来源：http://bdy.cqqwz.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://rfm.ydzc1.top

[Q38] 全外连接（PostgreSQL）
来源：http://ljx.zhoulong.xyz

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ynv.zhijiandao.cn

[Q39] 自连接（查上下级）
来源：http://qfd.dianchejie.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://haa.dianchejie.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://bwg.ydjk.org.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://cog.jlsjyb.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://rab.yuanzhike.top

[Q41] 多表连接
来源：http://iho.pengpengdd.cyou

SELECT o.id, u.name, p.title FROM orders o
来源：http://flq.yanxiufei.cn

JOIN users u ON u.id = o.user_id
来源：http://jwm.epnwcf.com

JOIN products p ON p.id = o.product_id;
来源：http://ucl.fktsv.cn

[Q42] 连接条件附加过滤
来源：http://iij.zhoulong.xyz

SELECT u.name, o.amount FROM users u
来源：http://int.zhixingplan.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mgu.hongshengwenyu.top

[Q43] 标量子查询
来源：http://bbf.316326.xyz

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mja.ybcxt.top

[Q44] IN 子查询
来源：http://wzt.mhx1999.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ozd.dashuyun.cn

[Q45] EXISTS 判断存在
来源：http://nsx.birdmap.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vgz.ppjwa.cn

[Q46] NOT EXISTS 判断不存在
来源：http://xqd.xuanzx.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qoa.jinqigufen.top

[Q47] 与平均值比较
来源：http://bez.xinyue.icu

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://xaz.cheryme.top

[Q48] CTE 公用表表达式
来源：http://mgf.hfpthk.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://qrk.yfazqb.com

SELECT * FROM t WHERE c > 5;
来源：http://dpi.jinqigfzy.top

[Q49] 更新单行
来源：http://ujv.nwbrower.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://xev.sweek.top

[Q50] 批量更新
来源：http://wgm.hnqzz.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ekn.zhiwuduotai.top

[Q51] 用子查询更新
来源：http://qsg.vehdjk.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hjn.chenlongwang.top

[Q52] 删除指定行
来源：http://rch.hcnkem.com

DELETE FROM users WHERE id = 10;
来源：http://tzs.fktsv.cn

[Q53] 按条件删除
来源：http://vss.shanyushiyangkeji.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://nyq.fehbvm.com

[Q54] 清空表
来源：http://gbg.haohaochexian.top

TRUNCATE TABLE logs;
来源：http://azi.jlsjyb.cn

[Q55] 排名（并列占位）
来源：http://vpv.jiagoushi.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://pkf.xylfe.cn

[Q56] 密集排名（并列不占位）
来源：http://rrq.meibo888.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ddo.gzhubu.top

[Q57] 行号
来源：http://rhp.fzhhl.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://anz.redwolf501.top

[Q58] 累计求和
来源：http://nvz.smart0.xyz

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hnf.feifeiyinyue.top

[Q59] 分组内累计
来源：http://iqu.yuanzhike.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ocg.ivvv.top

[Q60] 取上一行 / 下一行
来源：http://uhn.gotoacloud.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://qto.jyoumei.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://rek.xziqi.cn

[Q61] 移动平均
来源：http://zlo.shangyingyoupin.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://cza.fengsongda.top

[Q62] 分组占比
来源：http://ueg.haohaochexian.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://nva.ydjk.org.cn

[Q63] 开启事务
来源：http://jdt.shuidangran.top

START TRANSACTION;                -- 或 BEGIN
来源：http://qad.xinyue.icu

[Q64] 提交事务
来源：http://qsw.smart0.xyz

COMMIT;
来源：http://cop.ydjk.org.cn

[Q65] 回滚事务
来源：http://xxd.nwbrower.top

ROLLBACK;
来源：http://emu.tarul.cn

[Q66] 行锁查询
来源：http://kuo.svipenyu.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://oqd.316326.xyz

[Q67] 设置隔离级别
来源：http://tpa.aibaodan.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://vyh.shangyingyoupin.top

[Q68] 保存点
来源：http://knu.mhx1999.top

SAVEPOINT sp1;
来源：http://acl.gogol.net.cn

ROLLBACK TO sp1;
来源：http://ccl.feifeiyinyue.top

[Q69] 查看执行计划
来源：http://sxk.jinqigufen.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://fgs.aibaodan.cn

[Q70] 更新统计信息
来源：http://cex.smart0.xyz

ANALYZE TABLE users;
来源：http://vfn.dianchejie.cn

[Q71] 查看建表语句
来源：http://ssr.yj20258.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://kyc.smart0.xyz

[Q72] 查看索引
来源：http://ddo.zhoulong.xyz

SHOW INDEX FROM users;
来源：http://ucy.gaohongyu789.top

[Q73] 查看表状态
来源：http://rfi.jqgufenzy.top

SHOW TABLE STATUS LIKE 'users';
来源：http://xhb.cucudq.cn

[Q74] 强制使用索引
来源：http://wwj.aibaodan.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://zkw.nanxinkj.top

[Q75] 日期格式化
来源：http://hlb.yangfankeji.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://xuv.hammf.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://opa.hongshengwenyu.top

[Q76] 按天统计
来源：http://zxm.snrcjt.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://kif.vehdjk.com

[Q77] 时间加减
来源：http://jwb.zhongyouzk.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ult.shuidangran.top

[Q78] 当前时间
来源：http://gyb.gotoacloud.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://own.haohaochexian.top

[Q79] 字符串拼接
来源：http://axl.ydzc1.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://iar.zhixingplan.top

[Q80] 字符串截取
来源：http://nyl.svipenyu.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://eld.nwbrower.top

[Q81] 字符串替换
来源：http://vry.xuetiantiany.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://uiw.vehdjk.com

[Q82] 字符长度与字节长度
来源：http://ioe.mhx1999.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://bhp.sufxvd.cn

[Q83] 大小写转换
来源：http://fqm.chenlongwang.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://bbk.zdbjq.cn

[Q84] 去除首尾空格
来源：http://ihz.shangyingyoupin.top

SELECT TRIM(name) FROM users;
来源：http://bxf.xylfe.cn

[Q85] 数值取整
来源：http://hcx.snrcjt.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://gbu.tarul.cn

[Q86] 读取 JSON 字段
来源：http://uml.andypj.xyz

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://fpt.yangfankeji.com

[Q87] JSON 字段做条件
来源：http://hbf.zhengqikj.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://rui.wangshuangyany.cn

[Q88] 行转列（条件聚合）
来源：http://dxr.birdmap.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://voa.fktsv.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://xjh.smart0.xyz

[Q89] 判断表是否存在
来源：http://ega.dianchejie.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://upd.birdmap.top

[Q90] 生成序号列
来源：http://yqm.guowangkeji.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://tmv.sxryk.cn

================================================================================
来源：http://pbf.xziqi.cn

R. Bash 专题
来源：http://fbw.ivvv.top

================================================================================
来源：http://brr.fzhhl.top

[R01] shebang 与严格模式
来源：http://tyg.yvedp.cn

#!/usr/bin/env bash
来源：http://zud.zhixingplan.top

set -euo pipefail
来源：http://qoo.zhaomingkeji.xyz

[R02] 变量赋值与使用
来源：http://dpu.uphjek.com

name="Tom"; echo "$name"
来源：http://zzy.smart0.xyz

[R03] 只读变量
来源：http://ipl.tarul.cn

readonly PI=3.14
来源：http://bsk.hongshengwenyu.top

[R04] 位置参数
来源：http://cru.zhixingplan.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ipu.jqgfzy.top

[R05] 参数默认值
来源：http://jpp.jyoumei.cn

name="${1:-default}"
来源：http://rqx.hcnkem.com

[R06] 判断命令是否存在
来源：http://xon.jinqigufen.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ibg.ivvv.top

[R07] if 判断文件
来源：http://pcq.birdmap.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wcx.aibaodan.cn

[R08] 数值比较
来源：http://qzv.hnqzz.top

if (( a > b )); then echo "a 更大"; fi
来源：http://tmt.zdqjudy.top

[R09] 字符串比较
来源：http://zpg.xuetiantiany.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://maw.hywenlv.cn

[R10] 正则匹配
来源：http://jgx.c1oappe.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://kvb.zdqjudy.top

[R11] case 多分支
来源：http://lvo.cashguo.top

case "$1" in
来源：http://jkf.yfazqb.com

start) echo "启动" ;;
来源：http://zut.zhongyouzk.top

stop)  echo "停止" ;;
来源：http://rlq.zhiwuduotai.top

*)     echo "未知命令" ;;
来源：http://mab.xziqi.cn

esac
来源：http://bky.jlsjyb.cn

[R12] for 遍历文件
来源：http://wbu.daria6918.cn

for f in *.txt; do echo "$f"; done
来源：http://fbq.chenjidiqi.icu

[R13] for 计数循环
来源：http://xzg.zhiwuduotai.top

for i in {1..10}; do echo "$i"; done
来源：http://net.c1oappe.top

[R14] C 风格 for
来源：http://doz.shanyushiyangkeji.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://pym.guowangkeji.top

[R15] while 逐行读文件
来源：http://vok.tarul.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://gyq.shanyushiyangkeji.top

[R16] until 等待条件
来源：http://uon.nanxinkj.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://fnb.hnxiangtu.top

[R17] 数组定义与取值
来源：http://vqo.jqgfzy.top

arr=(a b c); echo "${arr[0]}"
来源：http://bym.epnwcf.com

[R18] 遍历数组
来源：http://nxs.xylfe.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://nkg.yvedp.cn

[R19] 数组长度
来源：http://ubc.shzxlz.cn

echo "${#arr[@]}"
来源：http://jmn.guowangkeji.top

[R20] 关联数组（字典）
来源：http://ifx.bbcook.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://sgv.sxryk.cn

[R21] 字符串长度
来源：http://mvq.52xcode.cn

echo "${#s}"
来源：http://zcg.yvedp.cn

[R22] 截取子串
来源：http://ulc.nanxuanxn.top

echo "${s:0:5}"
来源：http://nda.dashuyun.cn

[R23] 字符串替换
来源：http://lmh.jinqigfzy.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://qbh.zhaomingkeji.xyz

[R24] 大小写转换
来源：http://rcc.ydjk.org.cn

echo "${s^^}"; echo "${s,,}"
来源：http://tho.gaohongyu789.top

[R25] 去后缀 / 去前缀
来源：http://xwz.hesvh.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://hrq.shangyingyoupin.top

[R26] 命令替换
来源：http://wod.zhiwuduotai.top

now=$(date +%F); echo "$now"
来源：http://gpn.sweek.top

[R27] 算术展开
来源：http://ros.feifeiyinyue.top

echo $((1 + 2 * 3))
来源：http://sqi.bjfxy.top

[R28] 浮点运算
来源：http://ctm.svipenyu.cn

echo "scale=2; 10/3" | bc
来源：http://eqz.havefunace.top

[R29] 定义函数
来源：http://owf.zhongyouzk.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mxg.smart0.xyz

[R30] 函数返回状态码
来源：http://qhw.jlsjyb.cn

f() { return 0; }; f || echo "失败了"
来源：http://yhb.yvedp.cn

[R31] 局部变量
来源：http://szg.xinyue.icu

f() { local x=1; echo "$x"; }
来源：http://slz.havefunace.top

[R32] 参数个数校验
来源：http://fpn.zhijiandao.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://kxr.jinqigufen.top

[R33] 捕获错误并提示行号
来源：http://abu.birdmap.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://qfa.ppjwa.cn

[R34] 退出时清理
来源：http://oyl.tian-w.cn

trap 'rm -f "$tmp"' EXIT
来源：http://int.haohaochexian.top

[R35] 后台执行并等待
来源：http://ahq.c1oappe.top

sleep 5 & pid=$!; wait "$pid"
来源：http://vmz.gzhubu.top

[R36] 并发执行多个任务
来源：http://owk.andypj.xyz

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://xck.guowangkeji.top

[R37] 把输出赋给变量
来源：http://whe.nanxinkj.top

files=$(ls -1)
来源：http://tlo.cashguo.top

[R38] 管道串联
来源：http://dyl.zhijiandao.cn

cat a.txt | grep -i error | wc -l
来源：http://ucj.tarul.cn

[R39] 重定向标准输出与错误
来源：http://zmv.xuetiantiany.cn

cmd > out.log 2>&1
来源：http://uzx.c1oappe.top

[R40] 追加写日志
来源：http://mkz.sufxvd.cn

echo "log" >> out.log
来源：http://hut.zycfv.cn

[R41] 丢弃输出
来源：http://pdq.shuidangran.top

cmd >/dev/null 2>&1
来源：http://zxc.cheryme.top

[R42] 输入重定向
来源：http://hjr.shanyushiyangkeji.top

wc -l < a.txt
来源：http://mdc.tian-w.cn

[R43] 按名字查找文件
来源：http://aiw.redwolf501.top

find . -name "*.log" -type f
来源：http://xko.hfpthk.cn

[R44] 按修改时间查找
来源：http://nsq.guannengcc.top

find . -mtime -7 -type f
来源：http://pmj.fktsv.cn

[R45] 批量删除
来源：http://lfq.nanxuanxn.top

find . -name "*.tmp" -delete
来源：http://pal.smart0.xyz

[R46] 递归替换文件内容
来源：http://yhr.zhiwuduotai.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://okx.hywenlv.cn

[R47] sed 单行替换
来源：http://uvv.yuanzhike.top

sed -i 's/foo/bar/g' a.txt
来源：http://zxc.gzhubu.top

[R48] awk 取指定列
来源：http://lvr.xylfe.cn

awk '{print $1, $3}' a.txt
来源：http://unl.shanyushiyangkeji.top

[R49] awk 带条件
来源：http://app.nanxuanxn.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://gfe.tianlin.xyz

[R50] awk 求和
来源：http://txl.quarkkingdee.top

awk '{s += $2} END {print s}' a.txt
来源：http://wvk.pengpengdd.cyou

[R51] 排序去重取前几
来源：http://nld.havefunace.top

sort a.txt | uniq -c | sort -rn | head
来源：http://rdn.jlsjyb.cn

[R52] 统计行数
来源：http://kox.yj202588.top

wc -l a.txt
来源：http://lsi.vehdjk.com

[R53] 查看文件头与实时尾
来源：http://wpv.wangshuangyany.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://vdz.yonumen.top

[R54] 比较两个文件
来源：http://pjv.pengpengdd.cyou

diff a.txt b.txt
来源：http://kpp.sufxvd.cn

[R55] 压缩与解压
来源：http://nbq.shanyushiyangkeji.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://lhy.smart0.xyz

[R56] 远程拷贝
来源：http://fgm.xuanzx.com

scp file user@host:/path/
来源：http://iiw.yueranfly.top

[R57] 远程执行命令
来源：http://urn.nwbrower.top


<!-- 参考信息 -->