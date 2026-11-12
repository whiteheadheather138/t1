代发 wailian999

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mvr.gogol.net.cn

[Q20] IN 列表
来源：http://vbq.jinyuanbaomall.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wjx.daxiang520.top

[Q21] 空值判断
来源：http://imo.guowangkeji.top

SELECT * FROM users WHERE email IS NULL;
来源：http://umh.gogol.net.cn

[Q22] 排序
来源：http://qtp.9152youxi.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://bhp.hnxiangtu.top

[Q23] 分页
来源：http://gam.meibo888.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ftv.sysykeji.top

[Q24] 去重
来源：http://lwf.guowangkeji.top

SELECT DISTINCT city FROM users;
来源：http://bvd.yanxiufei.cn

[Q25] 只取前 N 条
来源：http://waq.bjfxy.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://auh.andypj.xyz

[Q26] 计数
来源：http://chq.jinqigufen.top

SELECT COUNT(*) FROM users;
来源：http://pxs.snrcjt.cn

[Q27] 条件计数
来源：http://gua.cucudq.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ior.wangdashe.top

[Q28] 求和与平均
来源：http://tad.gogol.net.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://lid.chenjidiqi.icu

[Q29] 最大最小值
来源：http://epv.52xcode.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://utw.yj20258.top

[Q30] 分组统计
来源：http://zbp.daria6918.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://dxg.shzxlz.cn

[Q31] 分组后过滤
来源：http://hvv.kuanghao11.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ywn.sxryk.cn

[Q32] 分组拼接字符串
来源：http://baq.xuetiantiany.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wnp.aibaodan.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://oah.meibo888.top

[Q33] 多列分组
来源：http://xqg.tianlin.xyz

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://fgy.chenzaomai.com

[Q34] 每组取第一条
来源：http://rci.ppjwa.cn

SELECT * FROM (
来源：http://fiq.svipenyu.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ivs.9152youxi.cn

) t WHERE rn = 1;
来源：http://ugb.yonumen.top

[Q35] 内连接
来源：http://gou.tarul.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://zdi.redwolf501.top

[Q36] 左连接
来源：http://yjy.chenzaomai.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://bmi.cashguo.top

[Q37] 右连接
来源：http://gif.hnqzz.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://qnu.xziqi.cn

[Q38] 全外连接（PostgreSQL）
来源：http://tgb.hnxiangtu.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://vtb.316326.xyz

[Q39] 自连接（查上下级）
来源：http://tie.xingfuxueyuan.xyz

SELECT e.name, m.name AS manager FROM employees e
来源：http://zxb.jinghuilouyu.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hxx.zdbjq.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://nlw.hysaishi.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://kld.zhiwuduotai.top

[Q41] 多表连接
来源：http://kon.zhengqikj.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://pzi.smart0.xyz

JOIN users u ON u.id = o.user_id
来源：http://euf.redwolf501.top

JOIN products p ON p.id = o.product_id;
来源：http://qje.shanyushiyangkeji.top

[Q42] 连接条件附加过滤
来源：http://vas.0kj1m.cn

SELECT u.name, o.amount FROM users u
来源：http://zyk.daria6918.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://dip.fengsongda.top

[Q43] 标量子查询
来源：http://hiy.wangdashe.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://fjz.vehdjk.com

[Q44] IN 子查询
来源：http://dgj.guowangkeji.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://nqf.epnwcf.com

[Q45] EXISTS 判断存在
来源：http://bmk.52xcode.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kci.chenzaomai.com

[Q46] NOT EXISTS 判断不存在
来源：http://dnp.shangyingyoupin.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bkf.tianlin.xyz

[Q47] 与平均值比较
来源：http://urm.ywan-chungtsiang.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ziy.0kj1m.cn

[Q48] CTE 公用表表达式
来源：http://xlk.gzhubu.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://uso.jqgufenzy.top

SELECT * FROM t WHERE c > 5;
来源：http://swk.aibaodan.cn

[Q49] 更新单行
来源：http://iwe.zdbjq.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://agj.fzhhl.top

[Q50] 批量更新
来源：http://cmw.hfpthk.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://jpm.fktsv.cn

[Q51] 用子查询更新
来源：http://eld.yj20258.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://gdn.zhongyouzk.top

[Q52] 删除指定行
来源：http://poe.zhaomingkeji.xyz

DELETE FROM users WHERE id = 10;
来源：http://zgp.yongpay.top

[Q53] 按条件删除
来源：http://jvb.zhiwuduotai.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://sag.gzhubu.top

[Q54] 清空表
来源：http://yrp.yj202588.top

TRUNCATE TABLE logs;
来源：http://qru.gogol.net.cn

[Q55] 排名（并列占位）
来源：http://msh.ivvv.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://pfp.tarul.cn

[Q56] 密集排名（并列不占位）
来源：http://ykv.vqdsnc.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://kiy.yvedp.cn

[Q57] 行号
来源：http://dza.gaohongyu789.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://kze.feifeiyinyue.top

[Q58] 累计求和
来源：http://vuz.tianlin.xyz

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ybl.zycfv.cn

[Q59] 分组内累计
来源：http://ltj.cashguo.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mdq.yanxiufei.cn

[Q60] 取上一行 / 下一行
来源：http://gpy.fanxiaobao.xyz

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://lba.316326.xyz

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://dck.sxryk.cn

[Q61] 移动平均
来源：http://whr.pycfn.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://itf.yuxming.cn

[Q62] 分组占比
来源：http://tyl.dashuyun.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hey.nwbrower.top

[Q63] 开启事务
来源：http://bfs.sweek.top

START TRANSACTION;                -- 或 BEGIN
来源：http://vvx.andypj.xyz

[Q64] 提交事务
来源：http://ifj.xuanzx.com

COMMIT;
来源：http://ybk.jianghu66.top

[Q65] 回滚事务
来源：http://bzz.316326.xyz

ROLLBACK;
来源：http://akq.zhixingplan.top

[Q66] 行锁查询
来源：http://vsw.shangyingyoupin.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hqo.ybcxt.top

[Q67] 设置隔离级别
来源：http://rct.hnqzz.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://xbd.dianchejie.cn

[Q68] 保存点
来源：http://vqv.yj20258888.top

SAVEPOINT sp1;
来源：http://bng.meibo888.top

ROLLBACK TO sp1;
来源：http://icl.tian-w.cn

[Q69] 查看执行计划
来源：http://lcf.nwbrower.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://xpr.jinqigfzy.top

[Q70] 更新统计信息
来源：http://xnm.ivvv.top

ANALYZE TABLE users;
来源：http://kfm.xylfe.cn

[Q71] 查看建表语句
来源：http://omw.nanxuanxn.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://zgu.tarul.cn

[Q72] 查看索引
来源：http://pif.daxiang520.top

SHOW INDEX FROM users;
来源：http://qjj.sufxvd.cn

[Q73] 查看表状态
来源：http://wll.shangyingyoupin.top

SHOW TABLE STATUS LIKE 'users';
来源：http://iyp.nanxuanxn.top

[Q74] 强制使用索引
来源：http://omp.birdmap.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ccr.jinyuanbaomall.cn

[Q75] 日期格式化
来源：http://anu.haohaochexian.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://skn.yvedp.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://oxy.xuanzx.com

[Q76] 按天统计
来源：http://psj.yuanzhike.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://kov.zhongyouzk.top

[Q77] 时间加减
来源：http://kkt.daxiang520.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://vce.ywan-chungtsiang.top

[Q78] 当前时间
来源：http://xsg.yfazqb.com

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://fdx.jinyuanbaomall.cn

[Q79] 字符串拼接
来源：http://yte.jlsjyb.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://usp.ppjwa.cn

[Q80] 字符串截取
来源：http://dno.vehdjk.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://xze.gzhubu.top

[Q81] 字符串替换
来源：http://hqr.uphjek.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wqu.haohaochexian.top

[Q82] 字符长度与字节长度
来源：http://ntg.feifeiyinyue.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://eux.wangdashe.top

[Q83] 大小写转换
来源：http://sch.epnwcf.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wuf.ppjwa.cn

[Q84] 去除首尾空格
来源：http://jwd.9152youxi.cn

SELECT TRIM(name) FROM users;
来源：http://iji.yonumen.top

[Q85] 数值取整
来源：http://mtp.zhaomingkeji.xyz

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hve.chenzaomai.com

[Q86] 读取 JSON 字段
来源：http://tqz.yj20258.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ymu.sjlbkw.cn

[Q87] JSON 字段做条件
来源：http://eva.tian-w.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://sya.jinyuanbaomall.cn

[Q88] 行转列（条件聚合）
来源：http://qvi.daxiang520.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://pky.guowangkeji.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://dam.meibo888.top

[Q89] 判断表是否存在
来源：http://gzc.svipenyu.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://iwr.0kj1m.cn

[Q90] 生成序号列
来源：http://lwc.yongpay.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://usu.xziqi.cn

================================================================================
来源：http://xwz.hywenlv.cn

R. Bash 专题
来源：http://tyw.gogol.net.cn

================================================================================
来源：http://mpc.0kj1m.cn

[R01] shebang 与严格模式
来源：http://miq.havefunace.top

#!/usr/bin/env bash
来源：http://gon.iojbl.cn

set -euo pipefail
来源：http://xlm.sxryk.cn

[R02] 变量赋值与使用
来源：http://plk.xziqi.cn

name="Tom"; echo "$name"
来源：http://odc.yvedp.cn

[R03] 只读变量
来源：http://hbw.gotoacloud.top

readonly PI=3.14
来源：http://wre.hywenlv.cn

[R04] 位置参数
来源：http://fnq.yj202588.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://kxa.zhixingplan.top

[R05] 参数默认值
来源：http://muo.zhixingplan.top

name="${1:-default}"
来源：http://cak.wangdashe.top

[R06] 判断命令是否存在
来源：http://kjv.yuxming.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://vcu.yuanzhike.top

[R07] if 判断文件
来源：http://cto.ydjk.org.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://bhu.gogol.net.cn

[R08] 数值比较
来源：http://agp.gaohongyu789.top

if (( a > b )); then echo "a 更大"; fi
来源：http://ebh.xinyue.icu

[R09] 字符串比较
来源：http://anx.jinghuilouyu.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://igo.hfpthk.cn

[R10] 正则匹配
来源：http://azi.gzhubu.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://phf.sweek.top

[R11] case 多分支
来源：http://bee.gogol.net.cn

case "$1" in
来源：http://bjr.jinqigfzy.top

start) echo "启动" ;;
来源：http://gru.snrcjt.cn

stop)  echo "停止" ;;
来源：http://fbi.daxiang520.top

*)     echo "未知命令" ;;
来源：http://esg.nanxinkj.top

esac
来源：http://vxn.zhaomingkeji.xyz

[R12] for 遍历文件
来源：http://iau.uphjek.com

for f in *.txt; do echo "$f"; done
来源：http://hki.tianlin.xyz

[R13] for 计数循环
来源：http://ezk.jqgufenzy.top

for i in {1..10}; do echo "$i"; done
来源：http://ovr.yj20258888.top

[R14] C 风格 for
来源：http://spz.uphjek.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://fme.ywan-chungtsiang.top

[R15] while 逐行读文件
来源：http://lpo.feifeiyinyue.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://kjx.xingfuxueyuan.xyz

[R16] until 等待条件
来源：http://bme.wangdashe.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://jgk.xziqi.cn

[R17] 数组定义与取值
来源：http://lrh.shuidangran.top

arr=(a b c); echo "${arr[0]}"
来源：http://dep.chenzaomai.com

[R18] 遍历数组
来源：http://dqo.dianchejie.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://zxa.yangfankeji.com

[R19] 数组长度
来源：http://rdm.jinyuanbaomall.cn

echo "${#arr[@]}"
来源：http://nnq.wangshuangyany.cn

[R20] 关联数组（字典）
来源：http://mns.yueranfly.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://vok.yongpay.top

[R21] 字符串长度
来源：http://zsn.shangyingyoupin.top

echo "${#s}"
来源：http://oez.nwbrower.top

[R22] 截取子串
来源：http://rvl.gzhubu.top

echo "${s:0:5}"
来源：http://zlo.hongshengwenyu.top

[R23] 字符串替换
来源：http://efr.aibaodan.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://lfw.daxiang520.top

[R24] 大小写转换
来源：http://beg.bbcook.cn

echo "${s^^}"; echo "${s,,}"
来源：http://fss.gotoacloud.top

[R25] 去后缀 / 去前缀
来源：http://vbo.zhijiandao.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://biy.guowangkeji.top

[R26] 命令替换
来源：http://uag.yj20258888.top

now=$(date +%F); echo "$now"
来源：http://hyd.dashuyun.cn

[R27] 算术展开
来源：http://ofd.meibo888.top

echo $((1 + 2 * 3))
来源：http://zbv.ivvv.top

[R28] 浮点运算
来源：http://uyu.havefunace.top

echo "scale=2; 10/3" | bc
来源：http://tzw.fanxiaobao.xyz

[R29] 定义函数
来源：http://nqx.epnwcf.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://nxo.jyoumei.cn

[R30] 函数返回状态码
来源：http://xkg.zhiwuduotai.top

f() { return 0; }; f || echo "失败了"
来源：http://wsk.chenlongwang.top

[R31] 局部变量
来源：http://xni.sjlbkw.cn

f() { local x=1; echo "$x"; }
来源：http://zwh.shuidangran.top

[R32] 参数个数校验
来源：http://gjq.cqqwz.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wrw.hnqzz.top

[R33] 捕获错误并提示行号
来源：http://nln.jinqigfzy.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ime.dianchejie.cn

[R34] 退出时清理
来源：http://atz.sjlbkw.cn

trap 'rm -f "$tmp"' EXIT
来源：http://jvu.ybcxt.top

[R35] 后台执行并等待
来源：http://vpp.ivvv.top

sleep 5 & pid=$!; wait "$pid"
来源：http://gjo.jinyuanbaomall.cn

[R36] 并发执行多个任务
来源：http://iyk.jiagoushi.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://qgc.chenjidiqi.icu

[R37] 把输出赋给变量
来源：http://pkx.ctjpmb.com

files=$(ls -1)
来源：http://aqv.guannengcc.top

[R38] 管道串联
来源：http://rtd.sxryk.cn

cat a.txt | grep -i error | wc -l
来源：http://qce.shanyushiyangtech.top

[R39] 重定向标准输出与错误
来源：http://mju.0kj1m.cn

cmd > out.log 2>&1
来源：http://alg.hfpthk.cn

[R40] 追加写日志
来源：http://mwt.guowangkeji.top

echo "log" >> out.log
来源：http://cwd.jqgfzy.top

[R41] 丢弃输出
来源：http://nbr.guowangkeji.top

cmd >/dev/null 2>&1
来源：http://nes.zycfv.cn

[R42] 输入重定向
来源：http://uad.vehdjk.com

wc -l < a.txt
来源：http://luq.nwbrower.top

[R43] 按名字查找文件
来源：http://uls.jlsjyb.cn

find . -name "*.log" -type f
来源：http://foy.jinghuilouyu.cn

[R44] 按修改时间查找
来源：http://wzf.9152youxi.cn

find . -mtime -7 -type f
来源：http://dhn.jlsjyb.cn

[R45] 批量删除
来源：http://win.xuetiantiany.cn

find . -name "*.tmp" -delete
来源：http://xzz.nanxinkj.top

[R46] 递归替换文件内容
来源：http://tdq.birdmap.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ycp.zycfv.cn

[R47] sed 单行替换
来源：http://jej.zhengqikj.top

sed -i 's/foo/bar/g' a.txt
来源：http://uhv.hfpthk.cn

[R48] awk 取指定列
来源：http://toj.fanxiaobao.xyz

awk '{print $1, $3}' a.txt
来源：http://rul.chenjidiqi.icu

[R49] awk 带条件
来源：http://wvo.yj20258.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://xkc.sxryk.cn

[R50] awk 求和
来源：http://unl.bbcook.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ttq.tian-w.cn

[R51] 排序去重取前几
来源：http://dsh.zhengqikj.top

sort a.txt | uniq -c | sort -rn | head
来源：http://llj.snrcjt.cn

[R52] 统计行数
来源：http://lmr.zdbjq.cn

wc -l a.txt
来源：http://akd.daxiang520.top

[R53] 查看文件头与实时尾
来源：http://liz.yongpay.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://pff.fzhhl.top

[R54] 比较两个文件
来源：http://qnu.gaohongyu789.top

diff a.txt b.txt
来源：http://hhg.jqgfzy.top

[R55] 压缩与解压
来源：http://vuq.xuetiantiany.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hsz.mhx1999.top

[R56] 远程拷贝
来源：http://ogv.ydjk.org.cn

scp file user@host:/path/
来源：http://urf.birdmap.top

[R57] 远程执行命令
来源：http://lkd.jinghuilouyu.cn

ssh user@host 'uptime'
来源：http://szi.zhongyouzk.top

[R58] 下载文件
来源：http://tjk.c1oappe.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ztm.yuxming.cn

[R59] 发 POST JSON
来源：http://bml.chenlongwang.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://clb.mhx1999.top

[R60] 只看 HTTP 状态码
来源：http://pvr.daria6918.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://dpy.tianlin.xyz

[R61] 磁盘占用
来源：http://dpv.hnqzz.top

df -h;  du -sh *
来源：http://yma.sysykeji.top

[R62] 找最占空间的文件
来源：http://iuo.svipenyu.cn

du -ah . | sort -rh | head -10
来源：http://igs.zdqjudy.top

[R63] 内存与进程
来源：http://hpc.sysykeji.top

free -h;  ps aux | grep nginx
来源：http://zao.xylfe.cn

[R64] 结束进程
来源：http://gyx.snrcjt.cn

kill -9 $(pgrep -f app.py)
来源：http://mjs.kuanghao11.cn

[R65] 查看端口占用
来源：http://sgv.ppjwa.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://jru.zhiwuduotai.top

[R66] 定时任务
来源：http://oxp.hywenlv.cn

crontab -e;  crontab -l
来源：http://mdj.shanyushiyangtech.top

[R67] 生成随机十六进制串
来源：http://zwk.svipenyu.cn

openssl rand -hex 16
来源：http://baf.redwolf501.top

[R68] 计算文件校验值
来源：http://gxi.ivvv.top

sha256sum a.txt;  md5sum a.txt
来源：http://fpe.ydjk.org.cn

[R69] 生成随机密码
来源：http://lul.feifeiyinyue.top


<!-- 参考信息 -->