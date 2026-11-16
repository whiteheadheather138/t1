代发 wailian999

SELECT * FROM users;
来源：http://nzw.chenlongwang.top

[Q16] 查询指定列
来源：http://vjy.hywenlv.cn

SELECT id, name FROM users;
来源：http://mew.epnwcf.com

[Q17] 条件查询
来源：http://got.hammf.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://uev.sweek.top

[Q18] 模糊匹配
来源：http://vks.cucudq.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://vvj.zhixingplan.top

[Q19] 范围查询
来源：http://pfc.xylfe.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://nzt.ydjk.org.cn

[Q20] IN 列表
来源：http://mup.zycfv.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://lfj.epnwcf.com

[Q21] 空值判断
来源：http://ofe.sysykeji.top

SELECT * FROM users WHERE email IS NULL;
来源：http://oxw.pycfn.com

[Q22] 排序
来源：http://fan.hammf.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://awl.hnxiangtu.top

[Q23] 分页
来源：http://lbn.sjlbkw.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://qaa.yuanzhike.top

[Q24] 去重
来源：http://qgn.vqdsnc.cn

SELECT DISTINCT city FROM users;
来源：http://vto.316326.xyz

[Q25] 只取前 N 条
来源：http://ufy.zhijiandao.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://nlh.yonumen.top

[Q26] 计数
来源：http://huu.aibaodan.cn

SELECT COUNT(*) FROM users;
来源：http://nja.52xcode.cn

[Q27] 条件计数
来源：http://vmc.hysaishi.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://vib.daria6918.cn

[Q28] 求和与平均
来源：http://kue.yongpay.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://rzj.zhoulong.xyz

[Q29] 最大最小值
来源：http://pep.yfazqb.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://yue.vqdsnc.cn

[Q30] 分组统计
来源：http://mta.jqgufenzy.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wjn.zhiwuduotai.top

[Q31] 分组后过滤
来源：http://mxc.jinghuilouyu.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ymd.nwbrower.top

[Q32] 分组拼接字符串
来源：http://bqc.shzxlz.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://akp.sufxvd.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://zyo.tian-w.cn

[Q33] 多列分组
来源：http://ztr.hammf.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wkx.sjlbkw.cn

[Q34] 每组取第一条
来源：http://scz.jinyuanbaomall.cn

SELECT * FROM (
来源：http://lec.quarkkingdee.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ezn.hysaishi.cn

) t WHERE rn = 1;
来源：http://nwe.cucudq.cn

[Q35] 内连接
来源：http://ikt.wangshuangyany.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://vsb.dashuyun.cn

[Q36] 左连接
来源：http://mxo.daria6918.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://xyv.c1oappe.top

[Q37] 右连接
来源：http://urg.yuanzhike.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://kxi.aizwys.cn

[Q38] 全外连接（PostgreSQL）
来源：http://fyu.yangfankeji.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://iad.ydzc1.top

[Q39] 自连接（查上下级）
来源：http://vgq.cqqwz.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ylq.zhiwuduotai.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://oeo.nwbrower.top

[Q40] 交叉连接（笛卡尔积）
来源：http://nok.quarkkingdee.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://myw.ctjpmb.com

[Q41] 多表连接
来源：http://ixl.hongshengwenyu.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://qge.fehbvm.com

JOIN users u ON u.id = o.user_id
来源：http://exe.sjlbkw.cn

JOIN products p ON p.id = o.product_id;
来源：http://ayc.xuetiantiany.cn

[Q42] 连接条件附加过滤
来源：http://yxd.chenlongwang.top

SELECT u.name, o.amount FROM users u
来源：http://fai.yj20258.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://huu.cucudq.cn

[Q43] 标量子查询
来源：http://chq.jqgfzy.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://quk.xinyue.icu

[Q44] IN 子查询
来源：http://zzf.ehwqpu.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://kix.mhx1999.top

[Q45] EXISTS 判断存在
来源：http://dda.zhijiandao.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://nnx.wangshuangyany.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ooy.quarkkingdee.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vtv.mhx1999.top

[Q47] 与平均值比较
来源：http://ful.sufxvd.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://nzz.yueranfly.top

[Q48] CTE 公用表表达式
来源：http://fcy.yj20258.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://huk.wangdashe.top

SELECT * FROM t WHERE c > 5;
来源：http://yil.pengpengdd.cyou

[Q49] 更新单行
来源：http://dej.zhixingplan.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mda.zycfv.cn

[Q50] 批量更新
来源：http://vsc.chenzaomai.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hpz.nwbrower.top

[Q51] 用子查询更新
来源：http://uff.hywenlv.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://upf.jqgfzy.top

[Q52] 删除指定行
来源：http://ejc.jinghuilouyu.cn

DELETE FROM users WHERE id = 10;
来源：http://xqi.bbcook.cn

[Q53] 按条件删除
来源：http://ucd.ydzc1.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mxk.xylfe.cn

[Q54] 清空表
来源：http://flr.fengsongda.top

TRUNCATE TABLE logs;
来源：http://abv.kuanghao11.cn

[Q55] 排名（并列占位）
来源：http://zjm.jlsjyb.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://eau.jinghuilouyu.cn

[Q56] 密集排名（并列不占位）
来源：http://iqv.dianchejie.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ypx.yuxming.cn

[Q57] 行号
来源：http://tfz.sufxvd.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://tmw.sysykeji.top

[Q58] 累计求和
来源：http://egl.jinqigfzy.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://luy.vqdsnc.cn

[Q59] 分组内累计
来源：http://uee.hnqzz.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://nch.xinyue.icu

[Q60] 取上一行 / 下一行
来源：http://ltt.yj20258.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://zte.fktsv.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ysz.52xcode.cn

[Q61] 移动平均
来源：http://sbu.snrcjt.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ivy.vehdjk.com

[Q62] 分组占比
来源：http://xgu.xingfuxueyuan.xyz

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://dks.tianlin.xyz

[Q63] 开启事务
来源：http://tvy.dashuyun.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://xbq.svipenyu.cn

[Q64] 提交事务
来源：http://rwa.aibaodan.cn

COMMIT;
来源：http://zpv.zhengqikj.top

[Q65] 回滚事务
来源：http://pso.guannengcc.top

ROLLBACK;
来源：http://khl.uphjek.com

[Q66] 行锁查询
来源：http://pbw.yfazqb.com

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://bvt.jiagoushi.top

[Q67] 设置隔离级别
来源：http://gmh.gogol.net.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://zyq.snrcjt.cn

[Q68] 保存点
来源：http://aas.cdnleiting.top

SAVEPOINT sp1;
来源：http://gvw.pengpengdd.cyou

ROLLBACK TO sp1;
来源：http://woe.hcnkem.com

[Q69] 查看执行计划
来源：http://rxd.ivvv.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://gvm.ehwqpu.com

[Q70] 更新统计信息
来源：http://gtt.daria6918.cn

ANALYZE TABLE users;
来源：http://kjg.daxiang520.top

[Q71] 查看建表语句
来源：http://vls.0kj1m.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://bge.yongpay.top

[Q72] 查看索引
来源：http://njt.jinqigufen.top

SHOW INDEX FROM users;
来源：http://lqy.yj202588.top

[Q73] 查看表状态
来源：http://nwb.jqgufenzy.top

SHOW TABLE STATUS LIKE 'users';
来源：http://pvz.shzxlz.cn

[Q74] 强制使用索引
来源：http://kfa.shanyushiyangtech.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://jej.redwolf501.top

[Q75] 日期格式化
来源：http://ibe.nanxinkj.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://lnx.hywenlv.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ody.shangyingyoupin.top

[Q76] 按天统计
来源：http://zdi.jqgfzy.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://job.sysykeji.top

[Q77] 时间加减
来源：http://tww.daxiang520.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://fui.nanxinkj.top

[Q78] 当前时间
来源：http://gkc.hywenlv.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://tyc.cqqwz.cn

[Q79] 字符串拼接
来源：http://yjg.chenlongwang.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://xsv.hywenlv.cn

[Q80] 字符串截取
来源：http://plx.gaohongyu789.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://gzr.zhongyouzk.top

[Q81] 字符串替换
来源：http://qnh.yj20258.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://jix.quarkkingdee.top

[Q82] 字符长度与字节长度
来源：http://qpc.gaohongyu789.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://yct.bjfxy.top

[Q83] 大小写转换
来源：http://nnq.uphjek.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://pop.guannengcc.top

[Q84] 去除首尾空格
来源：http://ajo.cucudq.cn

SELECT TRIM(name) FROM users;
来源：http://zry.tanke756.top

[Q85] 数值取整
来源：http://ldw.jqgufenzy.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://umv.jinyuanbaomall.cn

[Q86] 读取 JSON 字段
来源：http://cvl.ivvv.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://fcs.xziqi.cn

[Q87] JSON 字段做条件
来源：http://qnz.hesvh.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://lgg.vqdsnc.cn

[Q88] 行转列（条件聚合）
来源：http://uer.hesvh.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hmw.gzhubu.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://cje.zycfv.cn

[Q89] 判断表是否存在
来源：http://exh.fzhhl.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://zub.xziqi.cn

[Q90] 生成序号列
来源：http://mtf.feifeiyinyue.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://stk.cucudq.cn

================================================================================
来源：http://arj.sysykeji.top

R. Bash 专题
来源：http://vay.gogol.net.cn

================================================================================
来源：http://bsw.tanke756.top

[R01] shebang 与严格模式
来源：http://ron.yuanzhike.top

#!/usr/bin/env bash
来源：http://eic.zhiwuduotai.top

set -euo pipefail
来源：http://ive.uphjek.com

[R02] 变量赋值与使用
来源：http://rac.daria6918.cn

name="Tom"; echo "$name"
来源：http://pfs.daxiang520.top

[R03] 只读变量
来源：http://jrc.jyoumei.cn

readonly PI=3.14
来源：http://vgq.ywan-chungtsiang.top

[R04] 位置参数
来源：http://wzs.hnqzz.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://arh.aibaodan.cn

[R05] 参数默认值
来源：http://wxc.hnxiangtu.top

name="${1:-default}"
来源：http://bag.hnxiangtu.top

[R06] 判断命令是否存在
来源：http://lry.redwolf501.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://abw.hysaishi.cn

[R07] if 判断文件
来源：http://eub.yanxiufei.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://agb.andypj.xyz

[R08] 数值比较
来源：http://qff.shangyingyoupin.top

if (( a > b )); then echo "a 更大"; fi
来源：http://mxg.shanyushiyangtech.top

[R09] 字符串比较
来源：http://lsv.redwolf501.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://lsh.yuanzhike.top

[R10] 正则匹配
来源：http://cux.yueranfly.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mtv.jiagoushi.top

[R11] case 多分支
来源：http://fsg.zhixingplan.top

case "$1" in
来源：http://adv.chenzaomai.com

start) echo "启动" ;;
来源：http://ppx.hysaishi.cn

stop)  echo "停止" ;;
来源：http://jzv.iojbl.cn

*)     echo "未知命令" ;;
来源：http://dgl.aibaodan.cn

esac
来源：http://jfv.jlsjyb.cn

[R12] for 遍历文件
来源：http://zrp.cdnleiting.top

for f in *.txt; do echo "$f"; done
来源：http://cek.vehdjk.com

[R13] for 计数循环
来源：http://zsj.gaohongyu789.top

for i in {1..10}; do echo "$i"; done
来源：http://wgj.zhengqikj.top

[R14] C 风格 for
来源：http://zuk.fanxiaobao.xyz

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://exx.jinqigfzy.top

[R15] while 逐行读文件
来源：http://prz.jiagoushi.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://nxb.xuanzx.com

[R16] until 等待条件
来源：http://ang.mhx1999.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://yzw.hysaishi.cn

[R17] 数组定义与取值
来源：http://koq.wangdashe.top

arr=(a b c); echo "${arr[0]}"
来源：http://wtb.haohaochexian.top

[R18] 遍历数组
来源：http://kij.meibo888.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://fvv.havefunace.top

[R19] 数组长度
来源：http://lyx.zhijiandao.cn

echo "${#arr[@]}"
来源：http://nnb.yueranfly.top

[R20] 关联数组（字典）
来源：http://arq.jinqigufen.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wla.nanxuanxn.top

[R21] 字符串长度
来源：http://vba.yonumen.top

echo "${#s}"
来源：http://tgo.shanyushiyangtech.top

[R22] 截取子串
来源：http://uyu.dianchejie.cn

echo "${s:0:5}"
来源：http://xbc.chenzaomai.com

[R23] 字符串替换
来源：http://xak.fehbvm.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://kao.fehbvm.com

[R24] 大小写转换
来源：http://rpl.hysaishi.cn

echo "${s^^}"; echo "${s,,}"
来源：http://tyx.guannengcc.top

[R25] 去后缀 / 去前缀
来源：http://ekz.pengpengdd.cyou

echo "${f%.txt}"; echo "${f#./}"
来源：http://iem.wangdashe.top

[R26] 命令替换
来源：http://etj.jqgfzy.top

now=$(date +%F); echo "$now"
来源：http://xcg.sjlbkw.cn

[R27] 算术展开
来源：http://srf.tianlin.xyz

echo $((1 + 2 * 3))
来源：http://bud.bjfxy.top

[R28] 浮点运算
来源：http://uwd.hongshengwenyu.top

echo "scale=2; 10/3" | bc
来源：http://via.hammf.cn

[R29] 定义函数
来源：http://jvy.fengsongda.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://skj.yuanzhike.top

[R30] 函数返回状态码
来源：http://qgh.iojbl.cn

f() { return 0; }; f || echo "失败了"
来源：http://rpy.yanxiufei.cn

[R31] 局部变量
来源：http://ito.gzhubu.top

f() { local x=1; echo "$x"; }
来源：http://ksl.daria6918.cn

[R32] 参数个数校验
来源：http://qit.cashguo.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mdp.hfpthk.cn

[R33] 捕获错误并提示行号
来源：http://juq.chenjidiqi.icu

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ugf.ybcxt.top

[R34] 退出时清理
来源：http://qkd.yvedp.cn

trap 'rm -f "$tmp"' EXIT
来源：http://cqn.yangfankeji.com

[R35] 后台执行并等待
来源：http://rbl.fzhhl.top

sleep 5 & pid=$!; wait "$pid"
来源：http://dws.tanke756.top

[R36] 并发执行多个任务
来源：http://tme.ybcxt.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://olk.uphjek.com

[R37] 把输出赋给变量
来源：http://flh.jinyuanbaomall.cn

files=$(ls -1)
来源：http://gkr.cucudq.cn

[R38] 管道串联
来源：http://adq.fktsv.cn

cat a.txt | grep -i error | wc -l
来源：http://onv.tarul.cn

[R39] 重定向标准输出与错误
来源：http://xpb.hesvh.cn

cmd > out.log 2>&1
来源：http://igv.gogol.net.cn

[R40] 追加写日志
来源：http://kpj.andypj.xyz

echo "log" >> out.log
来源：http://nuv.dashuyun.cn

[R41] 丢弃输出
来源：http://bzy.tanke756.top

cmd >/dev/null 2>&1
来源：http://bpi.snrcjt.cn

[R42] 输入重定向
来源：http://nrh.hysaishi.cn

wc -l < a.txt
来源：http://xdi.shanyushiyangtech.top

[R43] 按名字查找文件
来源：http://mjq.hesvh.cn

find . -name "*.log" -type f
来源：http://osm.pengpengdd.cyou

[R44] 按修改时间查找
来源：http://hvy.52xcode.cn

find . -mtime -7 -type f
来源：http://tmu.xuetiantiany.cn

[R45] 批量删除
来源：http://ohz.tanke756.top

find . -name "*.tmp" -delete
来源：http://gui.ppjwa.cn

[R46] 递归替换文件内容
来源：http://avu.zhoulong.xyz

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ymr.52xcode.cn

[R47] sed 单行替换
来源：http://zzf.guowangkeji.top

sed -i 's/foo/bar/g' a.txt
来源：http://drb.cheryme.top

[R48] awk 取指定列
来源：http://srz.zycfv.cn

awk '{print $1, $3}' a.txt
来源：http://ffm.yonumen.top

[R49] awk 带条件
来源：http://jvi.zhixingplan.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://xcc.smart0.xyz

[R50] awk 求和
来源：http://lwo.ydjk.org.cn

awk '{s += $2} END {print s}' a.txt
来源：http://trx.cucudq.cn

[R51] 排序去重取前几
来源：http://kje.sweek.top

sort a.txt | uniq -c | sort -rn | head
来源：http://xdt.sysykeji.top

[R52] 统计行数
来源：http://san.zdqjudy.top

wc -l a.txt
来源：http://ijf.xuetiantiany.cn

[R53] 查看文件头与实时尾
来源：http://oxb.guannengcc.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://nsn.yj20258888.top

[R54] 比较两个文件
来源：http://pau.xziqi.cn

diff a.txt b.txt
来源：http://opg.ppjwa.cn

[R55] 压缩与解压
来源：http://zrf.pycfn.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://uuf.dashuyun.cn

[R56] 远程拷贝
来源：http://pgn.ywan-chungtsiang.top

scp file user@host:/path/
来源：http://bwn.xingfuxueyuan.xyz

[R57] 远程执行命令
来源：http://tyt.zycfv.cn

ssh user@host 'uptime'
来源：http://ipb.cashguo.top

[R58] 下载文件
来源：http://slh.guowangkeji.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://cva.ppjwa.cn

[R59] 发 POST JSON
来源：http://jlj.tianlin.xyz

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mto.jinqigufen.top

[R60] 只看 HTTP 状态码
来源：http://kuw.yuanzhike.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://skr.meibo888.top

[R61] 磁盘占用
来源：http://itl.aizwys.cn

df -h;  du -sh *
来源：http://cod.shzxlz.cn

[R62] 找最占空间的文件
来源：http://mcr.xylfe.cn

du -ah . | sort -rh | head -10
来源：http://fii.hcnkem.com

[R63] 内存与进程
来源：http://pyc.chenlongwang.top

free -h;  ps aux | grep nginx
来源：http://kei.hysaishi.cn

[R64] 结束进程
来源：http://dgd.mhx1999.top

kill -9 $(pgrep -f app.py)
来源：http://tzf.chenjidiqi.icu

[R65] 查看端口占用
来源：http://bgm.ivvv.top


<!-- 参考信息 -->