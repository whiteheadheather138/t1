代发 wailian999

SELECT * FROM users;
来源：http://ysh.hnxiangtu.top

[Q16] 查询指定列
来源：http://vpk.hammf.cn

SELECT id, name FROM users;
来源：http://xop.fengsongda.top

[Q17] 条件查询
来源：http://axq.nanxuanxn.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://omz.xylfe.cn

[Q18] 模糊匹配
来源：http://lyo.cqqwz.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://tss.yonumen.top

[Q19] 范围查询
来源：http://vvp.cdnleiting.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://rob.tianlin.xyz

[Q20] IN 列表
来源：http://zoz.daxiang520.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://vta.yj20258.top

[Q21] 空值判断
来源：http://xdx.cqqwz.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://qyw.quarkkingdee.top

[Q22] 排序
来源：http://xxg.gzhubu.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://npd.c1oappe.top

[Q23] 分页
来源：http://vyj.xylfe.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://qhe.fehbvm.com

[Q24] 去重
来源：http://yyf.ehwqpu.com

SELECT DISTINCT city FROM users;
来源：http://wue.hfpthk.cn

[Q25] 只取前 N 条
来源：http://dql.shanyushiyangkeji.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://qbo.zhixingplan.top

[Q26] 计数
来源：http://hkp.jinqigfzy.top

SELECT COUNT(*) FROM users;
来源：http://ksh.yonumen.top

[Q27] 条件计数
来源：http://vcl.ivvv.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://asx.snrcjt.cn

[Q28] 求和与平均
来源：http://ffn.ybcxt.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://egv.guannengcc.top

[Q29] 最大最小值
来源：http://crz.feifeiyinyue.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://lda.jqgufenzy.top

[Q30] 分组统计
来源：http://qjv.ybcxt.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://fzr.shanyushiyangtech.top

[Q31] 分组后过滤
来源：http://hma.smart0.xyz

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ies.hongshengwenyu.top

[Q32] 分组拼接字符串
来源：http://qsr.daria6918.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ksy.yfazqb.com

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://grx.hammf.cn

[Q33] 多列分组
来源：http://ezq.tianlin.xyz

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://vbr.xingfuxueyuan.xyz

[Q34] 每组取第一条
来源：http://bua.mhx1999.top

SELECT * FROM (
来源：http://seo.zdqjudy.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://rzd.fanxiaobao.xyz

) t WHERE rn = 1;
来源：http://epf.ppjwa.cn

[Q35] 内连接
来源：http://aqt.shanyushiyangkeji.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://vsd.pycfn.com

[Q36] 左连接
来源：http://nzs.jqgufenzy.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hpv.c1oappe.top

[Q37] 右连接
来源：http://kli.ydzc1.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://qmu.hongshengwenyu.top

[Q38] 全外连接（PostgreSQL）
来源：http://qbj.gzhubu.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ayy.tian-w.cn

[Q39] 自连接（查上下级）
来源：http://opc.daria6918.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://kex.aibaodan.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://gpq.zhongyouzk.top

[Q40] 交叉连接（笛卡尔积）
来源：http://etn.cucudq.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://djf.sjlbkw.cn

[Q41] 多表连接
来源：http://yom.jqgufenzy.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://hwr.jianghu66.top

JOIN users u ON u.id = o.user_id
来源：http://yrx.vehdjk.com

JOIN products p ON p.id = o.product_id;
来源：http://edu.mhx1999.top

[Q42] 连接条件附加过滤
来源：http://yho.yj20258888.top

SELECT u.name, o.amount FROM users u
来源：http://nky.nanxinkj.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://qdf.guannengcc.top

[Q43] 标量子查询
来源：http://hgd.0kj1m.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://nkf.wangshuangyany.cn

[Q44] IN 子查询
来源：http://lmi.gogol.net.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://jaa.xziqi.cn

[Q45] EXISTS 判断存在
来源：http://cyo.jiagoushi.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://lom.chenlongwang.top

[Q46] NOT EXISTS 判断不存在
来源：http://cge.dashuyun.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ybt.jqgufenzy.top

[Q47] 与平均值比较
来源：http://djy.dianchejie.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://otm.jinqigufen.top

[Q48] CTE 公用表表达式
来源：http://dfm.bbcook.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://bev.ybcxt.top

SELECT * FROM t WHERE c > 5;
来源：http://cnp.snrcjt.cn

[Q49] 更新单行
来源：http://pto.sxryk.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hrq.jinghuilouyu.cn

[Q50] 批量更新
来源：http://wwr.cqqwz.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://emi.yueranfly.top

[Q51] 用子查询更新
来源：http://ijl.aibaodan.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://fck.smart0.xyz

[Q52] 删除指定行
来源：http://yss.zycfv.cn

DELETE FROM users WHERE id = 10;
来源：http://msj.yj20258888.top

[Q53] 按条件删除
来源：http://cqo.andypj.xyz

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://kiq.wangshuangyany.cn

[Q54] 清空表
来源：http://lem.bbcook.cn

TRUNCATE TABLE logs;
来源：http://sbl.jiagoushi.top

[Q55] 排名（并列占位）
来源：http://hrq.cheryme.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://jqk.guannengcc.top

[Q56] 密集排名（并列不占位）
来源：http://zgu.shuidangran.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://cwl.shuidangran.top

[Q57] 行号
来源：http://lxx.yj20258888.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mjm.jiagoushi.top

[Q58] 累计求和
来源：http://suh.guannengcc.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hed.yonumen.top

[Q59] 分组内累计
来源：http://yhi.chenlongwang.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mjh.havefunace.top

[Q60] 取上一行 / 下一行
来源：http://hju.xuetiantiany.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mbg.hammf.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ndp.redwolf501.top

[Q61] 移动平均
来源：http://jde.xylfe.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://jns.xingfuxueyuan.xyz

[Q62] 分组占比
来源：http://rnz.uphjek.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://jwt.cheryme.top

[Q63] 开启事务
来源：http://uth.aizwys.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://qsk.nanxuanxn.top

[Q64] 提交事务
来源：http://vfk.hnqzz.top

COMMIT;
来源：http://oly.nwbrower.top

[Q65] 回滚事务
来源：http://qun.dianchejie.cn

ROLLBACK;
来源：http://zdv.nanxuanxn.top

[Q66] 行锁查询
来源：http://phl.shanyushiyangtech.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://zab.jinghuilouyu.cn

[Q67] 设置隔离级别
来源：http://tnp.tarul.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://snr.hammf.cn

[Q68] 保存点
来源：http://krs.jyoumei.cn

SAVEPOINT sp1;
来源：http://zce.meibo888.top

ROLLBACK TO sp1;
来源：http://iif.hnqzz.top

[Q69] 查看执行计划
来源：http://bax.zhengqikj.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://xqg.9152youxi.cn

[Q70] 更新统计信息
来源：http://xka.ppjwa.cn

ANALYZE TABLE users;
来源：http://gde.snrcjt.cn

[Q71] 查看建表语句
来源：http://btf.cqqwz.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://xgf.jianghu66.top

[Q72] 查看索引
来源：http://poe.xuetiantiany.cn

SHOW INDEX FROM users;
来源：http://bao.smart0.xyz

[Q73] 查看表状态
来源：http://tay.hywenlv.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://kyl.fehbvm.com

[Q74] 强制使用索引
来源：http://wwl.fzhhl.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hhr.epnwcf.com

[Q75] 日期格式化
来源：http://utm.tarul.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://amk.c1oappe.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://yay.daxiang520.top

[Q76] 按天统计
来源：http://dfb.yj20258.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://jqp.yueranfly.top

[Q77] 时间加减
来源：http://tts.ppjwa.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wza.ctjpmb.com

[Q78] 当前时间
来源：http://vtv.daxiang520.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://rim.xingfuxueyuan.xyz

[Q79] 字符串拼接
来源：http://trb.iojbl.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://yev.tarul.cn

[Q80] 字符串截取
来源：http://fai.snrcjt.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://bml.tanke756.top

[Q81] 字符串替换
来源：http://xwu.andypj.xyz

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://jrc.daria6918.cn

[Q82] 字符长度与字节长度
来源：http://cjw.quarkkingdee.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://vzy.yuanzhike.top

[Q83] 大小写转换
来源：http://olx.xylfe.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ivm.ppjwa.cn

[Q84] 去除首尾空格
来源：http://zyp.uphjek.com

SELECT TRIM(name) FROM users;
来源：http://xzp.zhiwuduotai.top

[Q85] 数值取整
来源：http://heh.chenlongwang.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://xkw.yj20258888.top

[Q86] 读取 JSON 字段
来源：http://fzn.jyoumei.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://qjp.xuanzx.com

[Q87] JSON 字段做条件
来源：http://zjw.xuanzx.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://pbx.yueranfly.top

[Q88] 行转列（条件聚合）
来源：http://oop.xuanzx.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://nhz.shanyushiyangtech.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://xtj.epnwcf.com

[Q89] 判断表是否存在
来源：http://uqb.jyoumei.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://pkj.xylfe.cn

[Q90] 生成序号列
来源：http://wvv.yj20258.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://pha.shuidangran.top

================================================================================
来源：http://xmj.pengpengdd.cyou

R. Bash 专题
来源：http://szb.gzhubu.top

================================================================================
来源：http://ulf.svipenyu.cn

[R01] shebang 与严格模式
来源：http://iiw.zhiwuduotai.top

#!/usr/bin/env bash
来源：http://sin.vehdjk.com

set -euo pipefail
来源：http://vhk.pycfn.com

[R02] 变量赋值与使用
来源：http://mua.shuidangran.top

name="Tom"; echo "$name"
来源：http://aoa.xziqi.cn

[R03] 只读变量
来源：http://viy.sysykeji.top

readonly PI=3.14
来源：http://kpy.sysykeji.top

[R04] 位置参数
来源：http://xgi.yueranfly.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wwx.zhixingplan.top

[R05] 参数默认值
来源：http://nvn.ctjpmb.com

name="${1:-default}"
来源：http://vha.jqgfzy.top

[R06] 判断命令是否存在
来源：http://kgd.zdbjq.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://imk.shanyushiyangtech.top

[R07] if 判断文件
来源：http://igr.tarul.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://tzx.cdnleiting.top

[R08] 数值比较
来源：http://xam.jinyuanbaomall.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://dyd.chenzaomai.com

[R09] 字符串比较
来源：http://beq.xingfuxueyuan.xyz

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ssa.bjfxy.top

[R10] 正则匹配
来源：http://qnl.ybcxt.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://jng.yj202588.top

[R11] case 多分支
来源：http://pdi.fanxiaobao.xyz

case "$1" in
来源：http://gvo.zhoulong.xyz

start) echo "启动" ;;
来源：http://ktf.yuanzhike.top

stop)  echo "停止" ;;
来源：http://pdp.bjfxy.top

*)     echo "未知命令" ;;
来源：http://cpq.chenlongwang.top

esac
来源：http://xkz.gaohongyu789.top

[R12] for 遍历文件
来源：http://hjn.chenlongwang.top

for f in *.txt; do echo "$f"; done
来源：http://lsx.sjlbkw.cn

[R13] for 计数循环
来源：http://rfk.nanxuanxn.top

for i in {1..10}; do echo "$i"; done
来源：http://ubu.zhaomingkeji.xyz

[R14] C 风格 for
来源：http://upr.daxiang520.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://fak.shangyingyoupin.top

[R15] while 逐行读文件
来源：http://iwv.c1oappe.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://pad.svipenyu.cn

[R16] until 等待条件
来源：http://php.sysykeji.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wut.xuetiantiany.cn

[R17] 数组定义与取值
来源：http://tzb.zhiwuduotai.top

arr=(a b c); echo "${arr[0]}"
来源：http://htw.hywenlv.cn

[R18] 遍历数组
来源：http://tsw.shanyushiyangkeji.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://vdh.tian-w.cn

[R19] 数组长度
来源：http://yfm.hcnkem.com

echo "${#arr[@]}"
来源：http://pqu.nwbrower.top

[R20] 关联数组（字典）
来源：http://gqi.zhaomingkeji.xyz

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://uaj.tanke756.top

[R21] 字符串长度
来源：http://xom.gotoacloud.top

echo "${#s}"
来源：http://rao.chenjidiqi.icu

[R22] 截取子串
来源：http://jww.yongpay.top

echo "${s:0:5}"
来源：http://kax.redwolf501.top

[R23] 字符串替换
来源：http://mnb.jqgfzy.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://tmf.wangdashe.top

[R24] 大小写转换
来源：http://wnw.fengsongda.top

echo "${s^^}"; echo "${s,,}"
来源：http://itq.havefunace.top

[R25] 去后缀 / 去前缀
来源：http://cvr.dianchejie.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://edw.vqdsnc.cn

[R26] 命令替换
来源：http://vil.daria6918.cn

now=$(date +%F); echo "$now"
来源：http://jgs.dashuyun.cn

[R27] 算术展开
来源：http://cyh.ivvv.top

echo $((1 + 2 * 3))
来源：http://fhn.shuidangran.top

[R28] 浮点运算
来源：http://jdl.yangfankeji.com

echo "scale=2; 10/3" | bc
来源：http://mim.yuxming.cn

[R29] 定义函数
来源：http://dcg.jinqigufen.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://vnt.bjfxy.top

[R30] 函数返回状态码
来源：http://jaw.zhongyouzk.top

f() { return 0; }; f || echo "失败了"
来源：http://wan.jinyuanbaomall.cn

[R31] 局部变量
来源：http://rpz.meibo888.top

f() { local x=1; echo "$x"; }
来源：http://fvf.yfazqb.com

[R32] 参数个数校验
来源：http://smq.vehdjk.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://vdt.chenlongwang.top

[R33] 捕获错误并提示行号
来源：http://ibv.ppjwa.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ouv.cucudq.cn

[R34] 退出时清理
来源：http://miy.guowangkeji.top

trap 'rm -f "$tmp"' EXIT
来源：http://itr.yj20258.top

[R35] 后台执行并等待
来源：http://yjr.epnwcf.com

sleep 5 & pid=$!; wait "$pid"
来源：http://psm.sjlbkw.cn

[R36] 并发执行多个任务
来源：http://yof.tianlin.xyz

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://gkh.dianchejie.cn

[R37] 把输出赋给变量
来源：http://bcc.tian-w.cn

files=$(ls -1)
来源：http://kfg.bbcook.cn

[R38] 管道串联
来源：http://hev.bbcook.cn

cat a.txt | grep -i error | wc -l
来源：http://geu.xinyue.icu

[R39] 重定向标准输出与错误
来源：http://oht.zhixingplan.top

cmd > out.log 2>&1
来源：http://qvl.fanxiaobao.xyz

[R40] 追加写日志
来源：http://myh.gogol.net.cn

echo "log" >> out.log
来源：http://qcw.gaohongyu789.top

[R41] 丢弃输出
来源：http://pef.daxiang520.top

cmd >/dev/null 2>&1
来源：http://njy.shzxlz.cn

[R42] 输入重定向
来源：http://xsz.yuxming.cn

wc -l < a.txt
来源：http://zuj.hysaishi.cn

[R43] 按名字查找文件
来源：http://opo.iojbl.cn

find . -name "*.log" -type f
来源：http://uoi.yvedp.cn

[R44] 按修改时间查找
来源：http://jie.jyoumei.cn

find . -mtime -7 -type f
来源：http://jck.hongshengwenyu.top

[R45] 批量删除
来源：http://gat.hysaishi.cn

find . -name "*.tmp" -delete
来源：http://wql.chenzaomai.com

[R46] 递归替换文件内容
来源：http://tcs.aibaodan.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://pne.vehdjk.com

[R47] sed 单行替换
来源：http://kyj.dashuyun.cn

sed -i 's/foo/bar/g' a.txt
来源：http://cel.gaohongyu789.top

[R48] awk 取指定列
来源：http://pov.jlsjyb.cn

awk '{print $1, $3}' a.txt
来源：http://sui.redwolf501.top

[R49] awk 带条件
来源：http://pmo.kuanghao11.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://tti.yueranfly.top

[R50] awk 求和
来源：http://ojs.chenjidiqi.icu

awk '{s += $2} END {print s}' a.txt
来源：http://eiz.cashguo.top

[R51] 排序去重取前几
来源：http://sku.birdmap.top

sort a.txt | uniq -c | sort -rn | head
来源：http://dpq.pengpengdd.cyou

[R52] 统计行数
来源：http://aoc.bbcook.cn

wc -l a.txt
来源：http://cam.sweek.top

[R53] 查看文件头与实时尾
来源：http://ein.mhx1999.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://bbh.jyoumei.cn

[R54] 比较两个文件
来源：http://auj.chenzaomai.com

diff a.txt b.txt
来源：http://kwb.wangdashe.top

[R55] 压缩与解压
来源：http://tdc.jlsjyb.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://rxe.yuanzhike.top

[R56] 远程拷贝
来源：http://mqy.ivvv.top

scp file user@host:/path/
来源：http://umx.zdbjq.cn

[R57] 远程执行命令
来源：http://kpd.yueranfly.top

ssh user@host 'uptime'
来源：http://jnt.guowangkeji.top

[R58] 下载文件
来源：http://rqk.gaohongyu789.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://bee.ivvv.top

[R59] 发 POST JSON
来源：http://day.zhaomingkeji.xyz

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://qkx.yj20258.top

[R60] 只看 HTTP 状态码
来源：http://hmk.zdqjudy.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mgh.shanyushiyangkeji.top

[R61] 磁盘占用
来源：http://sgo.feifeiyinyue.top

df -h;  du -sh *
来源：http://joz.ydzc1.top

[R62] 找最占空间的文件
来源：http://wey.0kj1m.cn

du -ah . | sort -rh | head -10
来源：http://jdd.wangdashe.top

[R63] 内存与进程
来源：http://uhj.ydzc1.top

free -h;  ps aux | grep nginx
来源：http://oce.zhengqikj.top

[R64] 结束进程
来源：http://rar.yj20258888.top

kill -9 $(pgrep -f app.py)
来源：http://yeh.aizwys.cn

[R65] 查看端口占用
来源：http://ldh.9152youxi.cn


<!-- 参考信息 -->