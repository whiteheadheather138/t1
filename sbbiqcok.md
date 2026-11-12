代发 wailian999

CREATE INDEX idx_users_email ON users(email);
来源：http://pvp.zhixingplan.top

[Q09] 创建唯一索引
来源：http://pnt.zhoulong.xyz

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wiz.tianlin.xyz

[Q10] 插入单行
来源：http://zek.hywenlv.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mpf.zhongyouzk.top

[Q11] 一次插入多行
来源：http://knu.jiagoushi.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://jgg.shanyushiyangkeji.top

[Q12] 插入后取自增 ID
来源：http://ano.jinqigufen.top

INSERT INTO users (name) VALUES ('C');
来源：http://ofz.guannengcc.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://vuk.cqqwz.cn

[Q13] 忽略重复插入
来源：http://jxu.tianlin.xyz

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://pgh.yfazqb.com

[Q14] 存在则更新（upsert）
来源：http://gxm.zhiwuduotai.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://dwv.fengsongda.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://bhn.zhiwuduotai.top

[Q15] 查询全部
来源：http://clr.jiagoushi.top

SELECT * FROM users;
来源：http://acw.meibo888.top

[Q16] 查询指定列
来源：http://hta.jinqigufen.top

SELECT id, name FROM users;
来源：http://jvl.cheryme.top

[Q17] 条件查询
来源：http://rso.redwolf501.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ftr.yvedp.cn

[Q18] 模糊匹配
来源：http://gsb.feifeiyinyue.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://pjd.yj20258.top

[Q19] 范围查询
来源：http://sqp.xinyue.icu

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://qve.jianghu66.top

[Q20] IN 列表
来源：http://mjy.hcnkem.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://fux.ybcxt.top

[Q21] 空值判断
来源：http://gzk.ppjwa.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ufj.mhx1999.top

[Q22] 排序
来源：http://wlg.jinqigufen.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://goe.andypj.xyz

[Q23] 分页
来源：http://cfr.pycfn.com

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://key.birdmap.top

[Q24] 去重
来源：http://bwu.havefunace.top

SELECT DISTINCT city FROM users;
来源：http://lry.guowangkeji.top

[Q25] 只取前 N 条
来源：http://brb.fktsv.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://vdh.shangyingyoupin.top

[Q26] 计数
来源：http://bjz.snrcjt.cn

SELECT COUNT(*) FROM users;
来源：http://ibg.shanyushiyangtech.top

[Q27] 条件计数
来源：http://ueb.quarkkingdee.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://goy.meibo888.top

[Q28] 求和与平均
来源：http://bij.chenlongwang.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://usg.dianchejie.cn

[Q29] 最大最小值
来源：http://nkg.guowangkeji.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://xxj.zhengqikj.top

[Q30] 分组统计
来源：http://sad.jinqigfzy.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://vvi.dianchejie.cn

[Q31] 分组后过滤
来源：http://yoh.ehwqpu.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://tuy.yuxming.cn

[Q32] 分组拼接字符串
来源：http://pkl.316326.xyz

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://tpw.hongshengwenyu.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://udd.zhaomingkeji.xyz

[Q33] 多列分组
来源：http://vpo.hongshengwenyu.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://cpn.52xcode.cn

[Q34] 每组取第一条
来源：http://rbr.shzxlz.cn

SELECT * FROM (
来源：http://fmk.yuxming.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://orr.0kj1m.cn

) t WHERE rn = 1;
来源：http://rpg.hammf.cn

[Q35] 内连接
来源：http://wod.c1oappe.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://pzo.xziqi.cn

[Q36] 左连接
来源：http://jwz.yanxiufei.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://tus.cashguo.top

[Q37] 右连接
来源：http://wse.hysaishi.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://fgj.jianghu66.top

[Q38] 全外连接（PostgreSQL）
来源：http://vyt.cucudq.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://kig.zhaomingkeji.xyz

[Q39] 自连接（查上下级）
来源：http://yxq.hcnkem.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://svi.shuidangran.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://pes.nanxinkj.top

[Q40] 交叉连接（笛卡尔积）
来源：http://aza.aibaodan.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://fkz.haohaochexian.top

[Q41] 多表连接
来源：http://jns.sweek.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://ptg.jyoumei.cn

JOIN users u ON u.id = o.user_id
来源：http://akq.shanyushiyangkeji.top

JOIN products p ON p.id = o.product_id;
来源：http://nro.dianchejie.cn

[Q42] 连接条件附加过滤
来源：http://mfm.fktsv.cn

SELECT u.name, o.amount FROM users u
来源：http://idk.svipenyu.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ecw.316326.xyz

[Q43] 标量子查询
来源：http://qbu.shuidangran.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hkl.quarkkingdee.top

[Q44] IN 子查询
来源：http://eqk.chenzaomai.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://yjs.mhx1999.top

[Q45] EXISTS 判断存在
来源：http://rhw.cdnleiting.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xzq.feifeiyinyue.top

[Q46] NOT EXISTS 判断不存在
来源：http://kug.jiagoushi.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://tru.shuidangran.top

[Q47] 与平均值比较
来源：http://myf.cdnleiting.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://kcw.shanyushiyangtech.top

[Q48] CTE 公用表表达式
来源：http://ttr.sjlbkw.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://lkx.jinqigufen.top

SELECT * FROM t WHERE c > 5;
来源：http://tcs.svipenyu.cn

[Q49] 更新单行
来源：http://uuh.hcnkem.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://aqe.smart0.xyz

[Q50] 批量更新
来源：http://aif.fzhhl.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mww.fanxiaobao.xyz

[Q51] 用子查询更新
来源：http://gpi.snrcjt.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://aqr.pengpengdd.cyou

[Q52] 删除指定行
来源：http://pdo.nanxuanxn.top

DELETE FROM users WHERE id = 10;
来源：http://pbg.xuetiantiany.cn

[Q53] 按条件删除
来源：http://vrq.zhaomingkeji.xyz

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://lmw.zhongyouzk.top

[Q54] 清空表
来源：http://osm.ydjk.org.cn

TRUNCATE TABLE logs;
来源：http://qzx.ydzc1.top

[Q55] 排名（并列占位）
来源：http://tiq.ivvv.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://krj.fanxiaobao.xyz

[Q56] 密集排名（并列不占位）
来源：http://lef.fzhhl.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://rvu.tarul.cn

[Q57] 行号
来源：http://gub.yuanzhike.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://tgn.yj20258.top

[Q58] 累计求和
来源：http://vrw.xinyue.icu

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://tly.xziqi.cn

[Q59] 分组内累计
来源：http://oly.fengsongda.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://sez.bbcook.cn

[Q60] 取上一行 / 下一行
来源：http://dsl.meibo888.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://vlv.fengsongda.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://tqa.chenzaomai.com

[Q61] 移动平均
来源：http://jxn.shuidangran.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://efl.ybcxt.top

[Q62] 分组占比
来源：http://oat.zhongyouzk.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ekt.uphjek.com

[Q63] 开启事务
来源：http://auq.zycfv.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://sla.ppjwa.cn

[Q64] 提交事务
来源：http://ghd.zdbjq.cn

COMMIT;
来源：http://rss.redwolf501.top

[Q65] 回滚事务
来源：http://jwh.jinqigufen.top

ROLLBACK;
来源：http://uij.ydjk.org.cn

[Q66] 行锁查询
来源：http://qcr.guannengcc.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://scg.zhongyouzk.top

[Q67] 设置隔离级别
来源：http://vwf.birdmap.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://oup.jqgufenzy.top

[Q68] 保存点
来源：http://jxl.hywenlv.cn

SAVEPOINT sp1;
来源：http://fpw.ywan-chungtsiang.top

ROLLBACK TO sp1;
来源：http://gri.tarul.cn

[Q69] 查看执行计划
来源：http://mig.fanxiaobao.xyz

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://bkv.sxryk.cn

[Q70] 更新统计信息
来源：http://lik.ydzc1.top

ANALYZE TABLE users;
来源：http://kxt.yanxiufei.cn

[Q71] 查看建表语句
来源：http://xfa.zdqjudy.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://syl.xinyue.icu

[Q72] 查看索引
来源：http://abo.dianchejie.cn

SHOW INDEX FROM users;
来源：http://hdv.sysykeji.top

[Q73] 查看表状态
来源：http://cjs.yangfankeji.com

SHOW TABLE STATUS LIKE 'users';
来源：http://jfv.hongshengwenyu.top

[Q74] 强制使用索引
来源：http://lid.yonumen.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://tck.ybcxt.top

[Q75] 日期格式化
来源：http://bag.sysykeji.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://cnk.zhoulong.xyz

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://pyi.guowangkeji.top

[Q76] 按天统计
来源：http://ooo.yuxming.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://txf.zhengqikj.top

[Q77] 时间加减
来源：http://zps.havefunace.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ifl.wangshuangyany.cn

[Q78] 当前时间
来源：http://bpa.hesvh.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://qct.zhengqikj.top

[Q79] 字符串拼接
来源：http://azr.xuetiantiany.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ukk.zdbjq.cn

[Q80] 字符串截取
来源：http://mxl.shangyingyoupin.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://jrh.jqgufenzy.top

[Q81] 字符串替换
来源：http://qhc.yuxming.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://xth.jqgfzy.top

[Q82] 字符长度与字节长度
来源：http://yri.shangyingyoupin.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://zqn.quarkkingdee.top

[Q83] 大小写转换
来源：http://dbu.xingfuxueyuan.xyz

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ish.ydzc1.top

[Q84] 去除首尾空格
来源：http://lee.xuetiantiany.cn

SELECT TRIM(name) FROM users;
来源：http://ejh.yangfankeji.com

[Q85] 数值取整
来源：http://lyb.yvedp.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://whe.andypj.xyz

[Q86] 读取 JSON 字段
来源：http://cnc.tanke756.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://vkf.zhengqikj.top

[Q87] JSON 字段做条件
来源：http://vty.dianchejie.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://drk.shanyushiyangkeji.top

[Q88] 行转列（条件聚合）
来源：http://jvz.sxryk.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://gzy.yuanzhike.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://dlt.xylfe.cn

[Q89] 判断表是否存在
来源：http://avm.jinghuilouyu.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://vwq.hongshengwenyu.top

[Q90] 生成序号列
来源：http://nho.zhixingplan.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://xmn.yonumen.top

================================================================================
来源：http://vaz.tianlin.xyz

R. Bash 专题
来源：http://rqt.hnqzz.top

================================================================================
来源：http://gdb.hysaishi.cn

[R01] shebang 与严格模式
来源：http://npd.cashguo.top

#!/usr/bin/env bash
来源：http://vwl.pengpengdd.cyou

set -euo pipefail
来源：http://urs.cheryme.top

[R02] 变量赋值与使用
来源：http://myw.jinyuanbaomall.cn

name="Tom"; echo "$name"
来源：http://bfb.cashguo.top

[R03] 只读变量
来源：http://grc.fanxiaobao.xyz

readonly PI=3.14
来源：http://dmq.haohaochexian.top

[R04] 位置参数
来源：http://lep.ybcxt.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ecq.jinqigufen.top

[R05] 参数默认值
来源：http://gcu.jlsjyb.cn

name="${1:-default}"
来源：http://hfe.jiagoushi.top

[R06] 判断命令是否存在
来源：http://ght.gaohongyu789.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://xlk.hfpthk.cn

[R07] if 判断文件
来源：http://lpp.zhiwuduotai.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://xjx.yangfankeji.com

[R08] 数值比较
来源：http://utp.snrcjt.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://xod.yangfankeji.com

[R09] 字符串比较
来源：http://nfw.jinqigufen.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ppb.ivvv.top

[R10] 正则匹配
来源：http://dfe.sxryk.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ooo.hfpthk.cn

[R11] case 多分支
来源：http://xpf.sufxvd.cn

case "$1" in
来源：http://awg.aibaodan.cn

start) echo "启动" ;;
来源：http://csg.yuanzhike.top

stop)  echo "停止" ;;
来源：http://ylp.mhx1999.top

*)     echo "未知命令" ;;
来源：http://cuu.9152youxi.cn

esac
来源：http://qtp.haohaochexian.top

[R12] for 遍历文件
来源：http://tqo.xingfuxueyuan.xyz

for f in *.txt; do echo "$f"; done
来源：http://iks.shzxlz.cn

[R13] for 计数循环
来源：http://yev.uphjek.com

for i in {1..10}; do echo "$i"; done
来源：http://cig.0kj1m.cn

[R14] C 风格 for
来源：http://uew.yuxming.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://uhd.jiagoushi.top

[R15] while 逐行读文件
来源：http://nrg.yuanzhike.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://imq.ivvv.top

[R16] until 等待条件
来源：http://aho.haohaochexian.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://kec.yongpay.top

[R17] 数组定义与取值
来源：http://mve.kuanghao11.cn

arr=(a b c); echo "${arr[0]}"
来源：http://zcn.yanxiufei.cn

[R18] 遍历数组
来源：http://hwt.cucudq.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://amq.jinqigfzy.top

[R19] 数组长度
来源：http://zhh.kuanghao11.cn

echo "${#arr[@]}"
来源：http://plg.nanxuanxn.top

[R20] 关联数组（字典）
来源：http://odo.uphjek.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://vox.jinqigfzy.top

[R21] 字符串长度
来源：http://rtb.xuanzx.com

echo "${#s}"
来源：http://nba.zhixingplan.top

[R22] 截取子串
来源：http://llv.andypj.xyz

echo "${s:0:5}"
来源：http://pla.nanxuanxn.top

[R23] 字符串替换
来源：http://hac.nanxinkj.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ktc.wangdashe.top

[R24] 大小写转换
来源：http://brm.jinyuanbaomall.cn

echo "${s^^}"; echo "${s,,}"
来源：http://bgh.zhongyouzk.top

[R25] 去后缀 / 去前缀
来源：http://spd.nanxinkj.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://oqf.cdnleiting.top

[R26] 命令替换
来源：http://iao.fengsongda.top

now=$(date +%F); echo "$now"
来源：http://gbe.xingfuxueyuan.xyz

[R27] 算术展开
来源：http://jcg.daria6918.cn

echo $((1 + 2 * 3))
来源：http://gde.sjlbkw.cn

[R28] 浮点运算
来源：http://cpv.zdbjq.cn

echo "scale=2; 10/3" | bc
来源：http://dix.xuetiantiany.cn

[R29] 定义函数
来源：http://lzq.gotoacloud.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://fkq.xinyue.icu

[R30] 函数返回状态码
来源：http://rjd.fengsongda.top

f() { return 0; }; f || echo "失败了"
来源：http://jlk.zhaomingkeji.xyz

[R31] 局部变量
来源：http://bry.ppjwa.cn

f() { local x=1; echo "$x"; }
来源：http://fwc.52xcode.cn

[R32] 参数个数校验
来源：http://ogv.shuidangran.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://fqn.chenzaomai.com

[R33] 捕获错误并提示行号
来源：http://yxo.snrcjt.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://eai.c1oappe.top

[R34] 退出时清理
来源：http://cob.ydzc1.top

trap 'rm -f "$tmp"' EXIT
来源：http://tjp.yongpay.top

[R35] 后台执行并等待
来源：http://vge.cashguo.top

sleep 5 & pid=$!; wait "$pid"
来源：http://lwq.shuidangran.top

[R36] 并发执行多个任务
来源：http://pig.yangfankeji.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://dhr.jiagoushi.top

[R37] 把输出赋给变量
来源：http://mnw.haohaochexian.top

files=$(ls -1)
来源：http://ene.xziqi.cn

[R38] 管道串联
来源：http://ysr.ppjwa.cn

cat a.txt | grep -i error | wc -l
来源：http://ley.zhengqikj.top

[R39] 重定向标准输出与错误
来源：http://bnc.wangdashe.top

cmd > out.log 2>&1
来源：http://ukx.cheryme.top

[R40] 追加写日志
来源：http://xyq.chenlongwang.top

echo "log" >> out.log
来源：http://wtt.9152youxi.cn

[R41] 丢弃输出
来源：http://xxi.ctjpmb.com

cmd >/dev/null 2>&1
来源：http://tcb.shangyingyoupin.top

[R42] 输入重定向
来源：http://hbe.ivvv.top

wc -l < a.txt
来源：http://sys.ehwqpu.com

[R43] 按名字查找文件
来源：http://gwn.ywan-chungtsiang.top

find . -name "*.log" -type f
来源：http://ipn.sjlbkw.cn

[R44] 按修改时间查找
来源：http://flk.smart0.xyz

find . -mtime -7 -type f
来源：http://tib.hysaishi.cn

[R45] 批量删除
来源：http://uef.shuidangran.top

find . -name "*.tmp" -delete
来源：http://yyh.daria6918.cn

[R46] 递归替换文件内容
来源：http://jxq.kuanghao11.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://xhz.chenjidiqi.icu

[R47] sed 单行替换
来源：http://uoo.vqdsnc.cn

sed -i 's/foo/bar/g' a.txt
来源：http://zpq.redwolf501.top

[R48] awk 取指定列
来源：http://adp.yj202588.top

awk '{print $1, $3}' a.txt
来源：http://xfm.kuanghao11.cn

[R49] awk 带条件
来源：http://zbm.cheryme.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://qrc.ydjk.org.cn

[R50] awk 求和
来源：http://gao.iojbl.cn

awk '{s += $2} END {print s}' a.txt
来源：http://tdu.xziqi.cn

[R51] 排序去重取前几
来源：http://vqz.xuanzx.com

sort a.txt | uniq -c | sort -rn | head
来源：http://hpf.smart0.xyz

[R52] 统计行数
来源：http://yim.zhoulong.xyz

wc -l a.txt
来源：http://zux.zhiwuduotai.top

[R53] 查看文件头与实时尾
来源：http://kix.zhongyouzk.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://qgc.svipenyu.cn

[R54] 比较两个文件
来源：http://eob.jyoumei.cn

diff a.txt b.txt
来源：http://ect.xuetiantiany.cn

[R55] 压缩与解压
来源：http://dnh.zhixingplan.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://jsd.bjfxy.top

[R56] 远程拷贝
来源：http://lvz.redwolf501.top

scp file user@host:/path/
来源：http://niq.gaohongyu789.top

[R57] 远程执行命令
来源：http://xaw.smart0.xyz


<!-- 参考信息 -->