代发 wailian999

SELECT * FROM users;
来源：http://thk.zhixingplan.top

[Q16] 查询指定列
来源：http://cyo.chenzaomai.com

SELECT id, name FROM users;
来源：http://bsm.haohaochexian.top

[Q17] 条件查询
来源：http://xnv.cucudq.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://eiq.hammf.cn

[Q18] 模糊匹配
来源：http://rik.xuetiantiany.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://dks.zhixingplan.top

[Q19] 范围查询
来源：http://ihd.zhoulong.xyz

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://jzv.zdqjudy.top

[Q20] IN 列表
来源：http://bnb.snrcjt.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://nhd.gaohongyu789.top

[Q21] 空值判断
来源：http://lpj.pycfn.com

SELECT * FROM users WHERE email IS NULL;
来源：http://fzh.yj20258888.top

[Q22] 排序
来源：http://cnn.guowangkeji.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://cbn.svipenyu.cn

[Q23] 分页
来源：http://tjq.cashguo.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://uxh.shanyushiyangtech.top

[Q24] 去重
来源：http://whr.cucudq.cn

SELECT DISTINCT city FROM users;
来源：http://rqw.smart0.xyz

[Q25] 只取前 N 条
来源：http://ezh.ybcxt.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://puz.chenzaomai.com

[Q26] 计数
来源：http://ctb.9152youxi.cn

SELECT COUNT(*) FROM users;
来源：http://ydh.yuanzhike.top

[Q27] 条件计数
来源：http://bdj.zdqjudy.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wlu.bjfxy.top

[Q28] 求和与平均
来源：http://eil.yj202588.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://sds.yj202588.top

[Q29] 最大最小值
来源：http://xhm.hesvh.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ebm.shuidangran.top

[Q30] 分组统计
来源：http://rjg.ybcxt.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://zzb.bbcook.cn

[Q31] 分组后过滤
来源：http://oik.cashguo.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://tnn.epnwcf.com

[Q32] 分组拼接字符串
来源：http://ygn.chenjidiqi.icu

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://jun.xuanzx.com

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wze.vqdsnc.cn

[Q33] 多列分组
来源：http://pta.zdqjudy.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://fys.aizwys.cn

[Q34] 每组取第一条
来源：http://bup.jinqigfzy.top

SELECT * FROM (
来源：http://kae.hfpthk.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hxj.xylfe.cn

) t WHERE rn = 1;
来源：http://qmh.zhijiandao.cn

[Q35] 内连接
来源：http://ykk.gaohongyu789.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://rwe.yuxming.cn

[Q36] 左连接
来源：http://rvt.hongshengwenyu.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://qqj.guowangkeji.top

[Q37] 右连接
来源：http://lgd.redwolf501.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://oqv.xylfe.cn

[Q38] 全外连接（PostgreSQL）
来源：http://txk.gogol.net.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://egz.fzhhl.top

[Q39] 自连接（查上下级）
来源：http://yjw.zhongyouzk.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://khb.bjfxy.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wmd.xinyue.icu

[Q40] 交叉连接（笛卡尔积）
来源：http://ely.ivvv.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://uqd.hysaishi.cn

[Q41] 多表连接
来源：http://zfr.9152youxi.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://coo.feifeiyinyue.top

JOIN users u ON u.id = o.user_id
来源：http://vux.sufxvd.cn

JOIN products p ON p.id = o.product_id;
来源：http://nsq.feifeiyinyue.top

[Q42] 连接条件附加过滤
来源：http://tlw.dashuyun.cn

SELECT u.name, o.amount FROM users u
来源：http://kml.yfazqb.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ktv.zdqjudy.top

[Q43] 标量子查询
来源：http://gku.zhongyouzk.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://xoo.jinqigfzy.top

[Q44] IN 子查询
来源：http://eup.tanke756.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://puo.jyoumei.cn

[Q45] EXISTS 判断存在
来源：http://ocd.cdnleiting.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://sja.wangdashe.top

[Q46] NOT EXISTS 判断不存在
来源：http://obs.jqgufenzy.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://pac.bjfxy.top

[Q47] 与平均值比较
来源：http://pbo.dashuyun.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://kme.shanyushiyangtech.top

[Q48] CTE 公用表表达式
来源：http://lje.birdmap.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ijg.jinqigfzy.top

SELECT * FROM t WHERE c > 5;
来源：http://eey.yonumen.top

[Q49] 更新单行
来源：http://bht.dianchejie.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://kwe.hnxiangtu.top

[Q50] 批量更新
来源：http://oum.andypj.xyz

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://lru.guowangkeji.top

[Q51] 用子查询更新
来源：http://xvw.xingfuxueyuan.xyz

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ket.sufxvd.cn

[Q52] 删除指定行
来源：http://hrf.jqgfzy.top

DELETE FROM users WHERE id = 10;
来源：http://ave.gzhubu.top

[Q53] 按条件删除
来源：http://kth.52xcode.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://soc.hnxiangtu.top

[Q54] 清空表
来源：http://isu.dashuyun.cn

TRUNCATE TABLE logs;
来源：http://wrm.jinyuanbaomall.cn

[Q55] 排名（并列占位）
来源：http://fza.yangfankeji.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://yzi.gzhubu.top

[Q56] 密集排名（并列不占位）
来源：http://pfz.daxiang520.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://xjd.cucudq.cn

[Q57] 行号
来源：http://ndp.pycfn.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ksj.feifeiyinyue.top

[Q58] 累计求和
来源：http://sms.guowangkeji.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://lzz.pycfn.com

[Q59] 分组内累计
来源：http://zmw.nwbrower.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://itm.nanxuanxn.top

[Q60] 取上一行 / 下一行
来源：http://axi.tarul.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://flr.guowangkeji.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://fvb.pengpengdd.cyou

[Q61] 移动平均
来源：http://wtu.hammf.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://asz.yonumen.top

[Q62] 分组占比
来源：http://yan.aibaodan.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://goi.shzxlz.cn

[Q63] 开启事务
来源：http://mlc.xingfuxueyuan.xyz

START TRANSACTION;                -- 或 BEGIN
来源：http://jmx.yuanzhike.top

[Q64] 提交事务
来源：http://ens.yuxming.cn

COMMIT;
来源：http://dyr.zycfv.cn

[Q65] 回滚事务
来源：http://gzf.pengpengdd.cyou

ROLLBACK;
来源：http://bsh.vqdsnc.cn

[Q66] 行锁查询
来源：http://ygl.vqdsnc.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://dnm.andypj.xyz

[Q67] 设置隔离级别
来源：http://jkt.sufxvd.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ujk.ywan-chungtsiang.top

[Q68] 保存点
来源：http://aot.cucudq.cn

SAVEPOINT sp1;
来源：http://eih.guannengcc.top

ROLLBACK TO sp1;
来源：http://ksp.redwolf501.top

[Q69] 查看执行计划
来源：http://uxy.yanxiufei.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://zyj.aizwys.cn

[Q70] 更新统计信息
来源：http://wxc.wangdashe.top

ANALYZE TABLE users;
来源：http://urc.chenlongwang.top

[Q71] 查看建表语句
来源：http://rzn.jianghu66.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://nhj.zhiwuduotai.top

[Q72] 查看索引
来源：http://tqq.fzhhl.top

SHOW INDEX FROM users;
来源：http://xwy.ctjpmb.com

[Q73] 查看表状态
来源：http://kon.ydzc1.top

SHOW TABLE STATUS LIKE 'users';
来源：http://zui.meibo888.top

[Q74] 强制使用索引
来源：http://stg.shangyingyoupin.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ipd.52xcode.cn

[Q75] 日期格式化
来源：http://cyu.shanyushiyangtech.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hai.jianghu66.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://bdl.andypj.xyz

[Q76] 按天统计
来源：http://ses.yvedp.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://tun.guannengcc.top

[Q77] 时间加减
来源：http://pzc.redwolf501.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://uml.bjfxy.top

[Q78] 当前时间
来源：http://rer.hesvh.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://pqv.pengpengdd.cyou

[Q79] 字符串拼接
来源：http://nue.cucudq.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ejh.cucudq.cn

[Q80] 字符串截取
来源：http://avz.shzxlz.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://xvq.gogol.net.cn

[Q81] 字符串替换
来源：http://ywi.gzhubu.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ayg.xinyue.icu

[Q82] 字符长度与字节长度
来源：http://xqi.sufxvd.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://pef.sjlbkw.cn

[Q83] 大小写转换
来源：http://kir.sxryk.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://eim.hammf.cn

[Q84] 去除首尾空格
来源：http://odj.316326.xyz

SELECT TRIM(name) FROM users;
来源：http://owt.jianghu66.top

[Q85] 数值取整
来源：http://nri.feifeiyinyue.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://kvk.haohaochexian.top

[Q86] 读取 JSON 字段
来源：http://zuv.hcnkem.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://jha.sweek.top

[Q87] JSON 字段做条件
来源：http://lek.jiagoushi.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://vcn.shanyushiyangtech.top

[Q88] 行转列（条件聚合）
来源：http://imh.fzhhl.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://isl.kuanghao11.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://fsv.ydjk.org.cn

[Q89] 判断表是否存在
来源：http://kth.shuidangran.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://xnt.redwolf501.top

[Q90] 生成序号列
来源：http://nuo.hongshengwenyu.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://jyy.dianchejie.cn

================================================================================
来源：http://rys.sxryk.cn

R. Bash 专题
来源：http://trx.nwbrower.top

================================================================================
来源：http://fei.chenlongwang.top

[R01] shebang 与严格模式
来源：http://sca.yvedp.cn

#!/usr/bin/env bash
来源：http://cbq.zhengqikj.top

set -euo pipefail
来源：http://jeb.hnxiangtu.top

[R02] 变量赋值与使用
来源：http://uwk.jinqigufen.top

name="Tom"; echo "$name"
来源：http://jdo.jinqigufen.top

[R03] 只读变量
来源：http://ghe.smart0.xyz

readonly PI=3.14
来源：http://eqd.ehwqpu.com

[R04] 位置参数
来源：http://ggg.kuanghao11.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://eoh.hammf.cn

[R05] 参数默认值
来源：http://yah.snrcjt.cn

name="${1:-default}"
来源：http://uqe.xuetiantiany.cn

[R06] 判断命令是否存在
来源：http://qur.jqgufenzy.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://dmm.nwbrower.top

[R07] if 判断文件
来源：http://ita.gotoacloud.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://rof.0kj1m.cn

[R08] 数值比较
来源：http://nuo.quarkkingdee.top

if (( a > b )); then echo "a 更大"; fi
来源：http://wql.jqgufenzy.top

[R09] 字符串比较
来源：http://ier.yj20258888.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://yyd.tianlin.xyz

[R10] 正则匹配
来源：http://udu.meibo888.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://bwd.chenzaomai.com

[R11] case 多分支
来源：http://iru.gotoacloud.top

case "$1" in
来源：http://vfn.uphjek.com

start) echo "启动" ;;
来源：http://bnb.xziqi.cn

stop)  echo "停止" ;;
来源：http://sot.cdnleiting.top

*)     echo "未知命令" ;;
来源：http://hog.bbcook.cn

esac
来源：http://ssr.ybcxt.top

[R12] for 遍历文件
来源：http://kms.chenzaomai.com

for f in *.txt; do echo "$f"; done
来源：http://ips.tanke756.top

[R13] for 计数循环
来源：http://cgf.fzhhl.top

for i in {1..10}; do echo "$i"; done
来源：http://iiv.nwbrower.top

[R14] C 风格 for
来源：http://jva.xylfe.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://jgt.xziqi.cn

[R15] while 逐行读文件
来源：http://sdd.ydjk.org.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://swv.316326.xyz

[R16] until 等待条件
来源：http://hsa.andypj.xyz

until [[ -f done.flag ]]; do sleep 1; done
来源：http://otr.chenlongwang.top

[R17] 数组定义与取值
来源：http://zwr.tanke756.top

arr=(a b c); echo "${arr[0]}"
来源：http://dxt.fktsv.cn

[R18] 遍历数组
来源：http://lpp.c1oappe.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://xak.smart0.xyz

[R19] 数组长度
来源：http://yww.fktsv.cn

echo "${#arr[@]}"
来源：http://unn.9152youxi.cn

[R20] 关联数组（字典）
来源：http://awi.aizwys.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://xhh.xziqi.cn

[R21] 字符串长度
来源：http://jjx.gaohongyu789.top

echo "${#s}"
来源：http://hql.wangdashe.top

[R22] 截取子串
来源：http://lah.smart0.xyz

echo "${s:0:5}"
来源：http://vuk.jianghu66.top

[R23] 字符串替换
来源：http://mra.shanyushiyangtech.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://zlj.tarul.cn

[R24] 大小写转换
来源：http://yem.epnwcf.com

echo "${s^^}"; echo "${s,,}"
来源：http://exw.nwbrower.top

[R25] 去后缀 / 去前缀
来源：http://hzg.yj202588.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://esz.ybcxt.top

[R26] 命令替换
来源：http://efu.cheryme.top

now=$(date +%F); echo "$now"
来源：http://oar.316326.xyz

[R27] 算术展开
来源：http://yfq.zhongyouzk.top

echo $((1 + 2 * 3))
来源：http://mww.mhx1999.top

[R28] 浮点运算
来源：http://tea.fanxiaobao.xyz

echo "scale=2; 10/3" | bc
来源：http://xty.hnxiangtu.top

[R29] 定义函数
来源：http://xcm.ppjwa.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mcm.daxiang520.top

[R30] 函数返回状态码
来源：http://jbd.sufxvd.cn

f() { return 0; }; f || echo "失败了"
来源：http://lhd.316326.xyz

[R31] 局部变量
来源：http://kbb.chenzaomai.com

f() { local x=1; echo "$x"; }
来源：http://cje.nanxuanxn.top

[R32] 参数个数校验
来源：http://rys.yvedp.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hma.zhengqikj.top

[R33] 捕获错误并提示行号
来源：http://pgq.yfazqb.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://tkd.zdbjq.cn

[R34] 退出时清理
来源：http://obr.yuxming.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ici.jinghuilouyu.cn

[R35] 后台执行并等待
来源：http://nxl.nanxuanxn.top

sleep 5 & pid=$!; wait "$pid"
来源：http://ler.daria6918.cn

[R36] 并发执行多个任务
来源：http://wim.shuidangran.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ebp.jiagoushi.top

[R37] 把输出赋给变量
来源：http://uyw.snrcjt.cn

files=$(ls -1)
来源：http://uih.fktsv.cn

[R38] 管道串联
来源：http://vzm.zhengqikj.top

cat a.txt | grep -i error | wc -l
来源：http://wbk.tianlin.xyz

[R39] 重定向标准输出与错误
来源：http://usq.aizwys.cn

cmd > out.log 2>&1
来源：http://efd.jlsjyb.cn

[R40] 追加写日志
来源：http://tab.quarkkingdee.top

echo "log" >> out.log
来源：http://eus.andypj.xyz

[R41] 丢弃输出
来源：http://qnx.vehdjk.com

cmd >/dev/null 2>&1
来源：http://nae.epnwcf.com

[R42] 输入重定向
来源：http://opb.yuanzhike.top

wc -l < a.txt
来源：http://hvq.yueranfly.top

[R43] 按名字查找文件
来源：http://ezg.svipenyu.cn

find . -name "*.log" -type f
来源：http://ett.316326.xyz

[R44] 按修改时间查找
来源：http://qks.jianghu66.top

find . -mtime -7 -type f
来源：http://dfg.iojbl.cn

[R45] 批量删除
来源：http://pep.jyoumei.cn

find . -name "*.tmp" -delete
来源：http://skk.daxiang520.top

[R46] 递归替换文件内容
来源：http://cqm.52xcode.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hup.sxryk.cn

[R47] sed 单行替换
来源：http://rey.shuidangran.top

sed -i 's/foo/bar/g' a.txt
来源：http://ehn.xylfe.cn

[R48] awk 取指定列
来源：http://psc.cqqwz.cn

awk '{print $1, $3}' a.txt
来源：http://ugz.ywan-chungtsiang.top

[R49] awk 带条件
来源：http://hoa.hysaishi.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://esr.zhongyouzk.top

[R50] awk 求和
来源：http://xcp.wangdashe.top

awk '{s += $2} END {print s}' a.txt
来源：http://zib.guannengcc.top

[R51] 排序去重取前几
来源：http://azf.yangfankeji.com

sort a.txt | uniq -c | sort -rn | head
来源：http://hah.jqgfzy.top

[R52] 统计行数
来源：http://acr.ywan-chungtsiang.top

wc -l a.txt
来源：http://isv.feifeiyinyue.top

[R53] 查看文件头与实时尾
来源：http://mun.iojbl.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ywh.bbcook.cn

[R54] 比较两个文件
来源：http://khu.bjfxy.top

diff a.txt b.txt
来源：http://fha.zdqjudy.top

[R55] 压缩与解压
来源：http://hkw.ybcxt.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mxu.feifeiyinyue.top

[R56] 远程拷贝
来源：http://npv.epnwcf.com

scp file user@host:/path/
来源：http://ncy.ctjpmb.com

[R57] 远程执行命令
来源：http://rsd.ybcxt.top

ssh user@host 'uptime'
来源：http://asm.bjfxy.top

[R58] 下载文件
来源：http://cff.fanxiaobao.xyz

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://qfd.aibaodan.cn

[R59] 发 POST JSON
来源：http://kff.jqgufenzy.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ekc.chenzaomai.com

[R60] 只看 HTTP 状态码
来源：http://fld.jqgufenzy.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mcj.hysaishi.cn

[R61] 磁盘占用
来源：http://vfv.ybcxt.top

df -h;  du -sh *
来源：http://jaa.aibaodan.cn

[R62] 找最占空间的文件
来源：http://okp.zhaomingkeji.xyz

du -ah . | sort -rh | head -10
来源：http://yjv.daxiang520.top

[R63] 内存与进程
来源：http://tnh.shanyushiyangkeji.top

free -h;  ps aux | grep nginx
来源：http://vsi.jianghu66.top

[R64] 结束进程
来源：http://kfy.zhijiandao.cn

kill -9 $(pgrep -f app.py)
来源：http://hlq.fanxiaobao.xyz

[R65] 查看端口占用
来源：http://jdp.quarkkingdee.top


<!-- 参考信息 -->