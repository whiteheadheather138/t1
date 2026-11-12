代发 wailian999

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://tyw.ywan-chungtsiang.top

[Q18] 模糊匹配
来源：http://lez.bbcook.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://yct.chenzaomai.com

[Q19] 范围查询
来源：http://yno.dashuyun.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://oxb.kuanghao11.cn

[Q20] IN 列表
来源：http://idk.ywan-chungtsiang.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ili.yuanzhike.top

[Q21] 空值判断
来源：http://ejn.yanxiufei.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://mtb.redwolf501.top

[Q22] 排序
来源：http://aad.yj202588.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://jjk.yuanzhike.top

[Q23] 分页
来源：http://ynd.yj20258888.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://tzu.shanyushiyangkeji.top

[Q24] 去重
来源：http://dkr.ywan-chungtsiang.top

SELECT DISTINCT city FROM users;
来源：http://yhs.chenzaomai.com

[Q25] 只取前 N 条
来源：http://bsq.hammf.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://skv.shuidangran.top

[Q26] 计数
来源：http://jxm.daxiang520.top

SELECT COUNT(*) FROM users;
来源：http://ghb.yuxming.cn

[Q27] 条件计数
来源：http://uuu.pengpengdd.cyou

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ngy.sjlbkw.cn

[Q28] 求和与平均
来源：http://ggw.jinghuilouyu.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://rif.bjfxy.top

[Q29] 最大最小值
来源：http://xcy.meibo888.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://xfl.sjlbkw.cn

[Q30] 分组统计
来源：http://anz.mhx1999.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://tbv.chenzaomai.com

[Q31] 分组后过滤
来源：http://hqk.hcnkem.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://nmv.xylfe.cn

[Q32] 分组拼接字符串
来源：http://gid.meibo888.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://rie.feifeiyinyue.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://rdu.gogol.net.cn

[Q33] 多列分组
来源：http://fqu.aibaodan.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://xeq.shangyingyoupin.top

[Q34] 每组取第一条
来源：http://lgy.xziqi.cn

SELECT * FROM (
来源：http://bpq.zdqjudy.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ksv.nwbrower.top

) t WHERE rn = 1;
来源：http://tya.epnwcf.com

[Q35] 内连接
来源：http://uoz.chenlongwang.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://gtu.zdqjudy.top

[Q36] 左连接
来源：http://iqt.gotoacloud.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://tpa.nanxuanxn.top

[Q37] 右连接
来源：http://ktg.ehwqpu.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://eak.havefunace.top

[Q38] 全外连接（PostgreSQL）
来源：http://sox.zhixingplan.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://jvs.yongpay.top

[Q39] 自连接（查上下级）
来源：http://uaq.jqgufenzy.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://vvp.tarul.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mep.dianchejie.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://xbk.pengpengdd.cyou

SELECT * FROM colors CROSS JOIN sizes;
来源：http://xnq.uphjek.com

[Q41] 多表连接
来源：http://yrg.ywan-chungtsiang.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://fut.birdmap.top

JOIN users u ON u.id = o.user_id
来源：http://uve.shanyushiyangkeji.top

JOIN products p ON p.id = o.product_id;
来源：http://imz.sxryk.cn

[Q42] 连接条件附加过滤
来源：http://tck.xziqi.cn

SELECT u.name, o.amount FROM users u
来源：http://sqp.sufxvd.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://naq.yuanzhike.top

[Q43] 标量子查询
来源：http://zfd.hongshengwenyu.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://rgg.pycfn.com

[Q44] IN 子查询
来源：http://xwb.52xcode.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://buq.gzhubu.top

[Q45] EXISTS 判断存在
来源：http://yuh.zhixingplan.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fff.shanyushiyangkeji.top

[Q46] NOT EXISTS 判断不存在
来源：http://npr.hesvh.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://urd.gaohongyu789.top

[Q47] 与平均值比较
来源：http://zdr.guannengcc.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://nht.vqdsnc.cn

[Q48] CTE 公用表表达式
来源：http://ijk.xziqi.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://kbz.zdbjq.cn

SELECT * FROM t WHERE c > 5;
来源：http://onl.hesvh.cn

[Q49] 更新单行
来源：http://yvm.zycfv.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://qll.zhijiandao.cn

[Q50] 批量更新
来源：http://aah.smart0.xyz

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mkl.xziqi.cn

[Q51] 用子查询更新
来源：http://jcq.gaohongyu789.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wpx.zhiwuduotai.top

[Q52] 删除指定行
来源：http://cfw.0kj1m.cn

DELETE FROM users WHERE id = 10;
来源：http://str.haohaochexian.top

[Q53] 按条件删除
来源：http://lrx.9152youxi.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://jtu.fktsv.cn

[Q54] 清空表
来源：http://ito.shuidangran.top

TRUNCATE TABLE logs;
来源：http://bcp.pycfn.com

[Q55] 排名（并列占位）
来源：http://lmz.sxryk.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ndl.wangdashe.top

[Q56] 密集排名（并列不占位）
来源：http://yis.guannengcc.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mdm.jianghu66.top

[Q57] 行号
来源：http://eyu.gaohongyu789.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://pvr.snrcjt.cn

[Q58] 累计求和
来源：http://zae.andypj.xyz

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wvd.tarul.cn

[Q59] 分组内累计
来源：http://bfm.jyoumei.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://upc.yueranfly.top

[Q60] 取上一行 / 下一行
来源：http://khf.xziqi.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://qni.zhijiandao.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://fxh.jyoumei.cn

[Q61] 移动平均
来源：http://trn.zhiwuduotai.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://epd.9152youxi.cn

[Q62] 分组占比
来源：http://elc.pycfn.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://rme.xuetiantiany.cn

[Q63] 开启事务
来源：http://fgu.kuanghao11.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://cvd.daria6918.cn

[Q64] 提交事务
来源：http://ddq.xuanzx.com

COMMIT;
来源：http://xpn.gogol.net.cn

[Q65] 回滚事务
来源：http://law.ppjwa.cn

ROLLBACK;
来源：http://jgy.ywan-chungtsiang.top

[Q66] 行锁查询
来源：http://dkr.xuetiantiany.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://jph.pycfn.com

[Q67] 设置隔离级别
来源：http://cie.hfpthk.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://yng.cucudq.cn

[Q68] 保存点
来源：http://uxl.xinyue.icu

SAVEPOINT sp1;
来源：http://tcx.nanxuanxn.top

ROLLBACK TO sp1;
来源：http://scq.cucudq.cn

[Q69] 查看执行计划
来源：http://rrq.hesvh.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://icn.gzhubu.top

[Q70] 更新统计信息
来源：http://iaz.cheryme.top

ANALYZE TABLE users;
来源：http://ylp.jianghu66.top

[Q71] 查看建表语句
来源：http://nwm.kuanghao11.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://rae.cqqwz.cn

[Q72] 查看索引
来源：http://xse.mhx1999.top

SHOW INDEX FROM users;
来源：http://mjv.ydjk.org.cn

[Q73] 查看表状态
来源：http://wds.nwbrower.top

SHOW TABLE STATUS LIKE 'users';
来源：http://qvr.fanxiaobao.xyz

[Q74] 强制使用索引
来源：http://slj.jyoumei.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://auv.ybcxt.top

[Q75] 日期格式化
来源：http://ypa.jianghu66.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://eby.gotoacloud.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://xwf.jinghuilouyu.cn

[Q76] 按天统计
来源：http://ftp.daxiang520.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wsf.gaohongyu789.top

[Q77] 时间加减
来源：http://lis.316326.xyz

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://gaj.iojbl.cn

[Q78] 当前时间
来源：http://lqc.xuanzx.com

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://lne.zhijiandao.cn

[Q79] 字符串拼接
来源：http://zfh.zhengqikj.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://uww.zhoulong.xyz

[Q80] 字符串截取
来源：http://bpp.zhijiandao.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://gek.shzxlz.cn

[Q81] 字符串替换
来源：http://ovk.feifeiyinyue.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wfy.vehdjk.com

[Q82] 字符长度与字节长度
来源：http://xsc.shanyushiyangtech.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://bkr.jianghu66.top

[Q83] 大小写转换
来源：http://ext.svipenyu.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://lgi.yongpay.top

[Q84] 去除首尾空格
来源：http://nbn.shangyingyoupin.top

SELECT TRIM(name) FROM users;
来源：http://lws.zhongyouzk.top

[Q85] 数值取整
来源：http://eks.hesvh.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hmk.nanxuanxn.top

[Q86] 读取 JSON 字段
来源：http://aly.yonumen.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://xyh.vehdjk.com

[Q87] JSON 字段做条件
来源：http://gcv.fehbvm.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://cch.epnwcf.com

[Q88] 行转列（条件聚合）
来源：http://sbl.daria6918.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://lqo.dashuyun.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://cdo.fzhhl.top

[Q89] 判断表是否存在
来源：http://ikv.nwbrower.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://bdp.kuanghao11.cn

[Q90] 生成序号列
来源：http://dbo.nanxuanxn.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://boa.cheryme.top

================================================================================
来源：http://tyj.uphjek.com

R. Bash 专题
来源：http://rxd.shangyingyoupin.top

================================================================================
来源：http://vrp.sweek.top

[R01] shebang 与严格模式
来源：http://axk.yj20258.top

#!/usr/bin/env bash
来源：http://mbe.aizwys.cn

set -euo pipefail
来源：http://cqy.xuanzx.com

[R02] 变量赋值与使用
来源：http://ylw.hnxiangtu.top

name="Tom"; echo "$name"
来源：http://eic.yvedp.cn

[R03] 只读变量
来源：http://qrm.hnqzz.top

readonly PI=3.14
来源：http://vcq.fzhhl.top

[R04] 位置参数
来源：http://qyb.chenlongwang.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ach.wangshuangyany.cn

[R05] 参数默认值
来源：http://fiv.yfazqb.com

name="${1:-default}"
来源：http://wvy.hywenlv.cn

[R06] 判断命令是否存在
来源：http://bcc.yfazqb.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wvr.jqgufenzy.top

[R07] if 判断文件
来源：http://zxy.hywenlv.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://abj.jqgfzy.top

[R08] 数值比较
来源：http://sru.yj20258.top

if (( a > b )); then echo "a 更大"; fi
来源：http://prp.ehwqpu.com

[R09] 字符串比较
来源：http://zhr.xziqi.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mfq.9152youxi.cn

[R10] 正则匹配
来源：http://ise.feifeiyinyue.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://vwl.wangshuangyany.cn

[R11] case 多分支
来源：http://ibd.yanxiufei.cn

case "$1" in
来源：http://oei.uphjek.com

start) echo "启动" ;;
来源：http://wga.guowangkeji.top

stop)  echo "停止" ;;
来源：http://ith.jinqigfzy.top

*)     echo "未知命令" ;;
来源：http://pqa.hesvh.cn

esac
来源：http://gqi.cheryme.top

[R12] for 遍历文件
来源：http://owi.yonumen.top

for f in *.txt; do echo "$f"; done
来源：http://sww.zdbjq.cn

[R13] for 计数循环
来源：http://cuo.hcnkem.com

for i in {1..10}; do echo "$i"; done
来源：http://nyj.xuanzx.com

[R14] C 风格 for
来源：http://jzm.mhx1999.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://awg.wangdashe.top

[R15] while 逐行读文件
来源：http://lyl.cqqwz.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://xsc.tianlin.xyz

[R16] until 等待条件
来源：http://fxe.hesvh.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://cwa.vqdsnc.cn

[R17] 数组定义与取值
来源：http://yed.fengsongda.top

arr=(a b c); echo "${arr[0]}"
来源：http://ymc.hesvh.cn

[R18] 遍历数组
来源：http://zbl.yj20258888.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://eni.sufxvd.cn

[R19] 数组长度
来源：http://czs.jinqigufen.top

echo "${#arr[@]}"
来源：http://onv.uphjek.com

[R20] 关联数组（字典）
来源：http://yho.cheryme.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://pjs.jyoumei.cn

[R21] 字符串长度
来源：http://cwa.zhijiandao.cn

echo "${#s}"
来源：http://zwf.zhixingplan.top

[R22] 截取子串
来源：http://cjl.tanke756.top

echo "${s:0:5}"
来源：http://ogi.fanxiaobao.xyz

[R23] 字符串替换
来源：http://mfz.pycfn.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://pnw.guannengcc.top

[R24] 大小写转换
来源：http://fpn.hywenlv.cn

echo "${s^^}"; echo "${s,,}"
来源：http://iwg.chenlongwang.top

[R25] 去后缀 / 去前缀
来源：http://jze.sweek.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://ojg.zhongyouzk.top

[R26] 命令替换
来源：http://kht.hesvh.cn

now=$(date +%F); echo "$now"
来源：http://hgq.fzhhl.top

[R27] 算术展开
来源：http://vsr.zhoulong.xyz

echo $((1 + 2 * 3))
来源：http://xkc.nanxinkj.top

[R28] 浮点运算
来源：http://stu.guannengcc.top

echo "scale=2; 10/3" | bc
来源：http://cco.yuxming.cn

[R29] 定义函数
来源：http://ctf.mhx1999.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://lgn.svipenyu.cn

[R30] 函数返回状态码
来源：http://git.0kj1m.cn

f() { return 0; }; f || echo "失败了"
来源：http://eht.fehbvm.com

[R31] 局部变量
来源：http://fmq.daxiang520.top

f() { local x=1; echo "$x"; }
来源：http://zox.yuanzhike.top

[R32] 参数个数校验
来源：http://jvj.jqgufenzy.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://myn.yanxiufei.cn

[R33] 捕获错误并提示行号
来源：http://ywh.pengpengdd.cyou

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://rcq.sysykeji.top

[R34] 退出时清理
来源：http://kwv.cheryme.top

trap 'rm -f "$tmp"' EXIT
来源：http://zfj.ctjpmb.com

[R35] 后台执行并等待
来源：http://svb.zhaomingkeji.xyz

sleep 5 & pid=$!; wait "$pid"
来源：http://nnz.wangdashe.top

[R36] 并发执行多个任务
来源：http://nnx.guowangkeji.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://xyu.vehdjk.com

[R37] 把输出赋给变量
来源：http://hji.zhijiandao.cn

files=$(ls -1)
来源：http://lgy.ywan-chungtsiang.top

[R38] 管道串联
来源：http://qaj.fktsv.cn

cat a.txt | grep -i error | wc -l
来源：http://pdw.yfazqb.com

[R39] 重定向标准输出与错误
来源：http://hrl.gaohongyu789.top

cmd > out.log 2>&1
来源：http://ahj.svipenyu.cn

[R40] 追加写日志
来源：http://zwi.shangyingyoupin.top

echo "log" >> out.log
来源：http://ror.dianchejie.cn

[R41] 丢弃输出
来源：http://yrw.ehwqpu.com

cmd >/dev/null 2>&1
来源：http://fgh.yfazqb.com

[R42] 输入重定向
来源：http://cpb.xziqi.cn

wc -l < a.txt
来源：http://sxw.chenlongwang.top

[R43] 按名字查找文件
来源：http://aut.guannengcc.top

find . -name "*.log" -type f
来源：http://gwg.tian-w.cn

[R44] 按修改时间查找
来源：http://dig.wangshuangyany.cn

find . -mtime -7 -type f
来源：http://ffq.gogol.net.cn

[R45] 批量删除
来源：http://rkv.cheryme.top

find . -name "*.tmp" -delete
来源：http://reo.jinyuanbaomall.cn

[R46] 递归替换文件内容
来源：http://lkn.ctjpmb.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://fwu.hcnkem.com

[R47] sed 单行替换
来源：http://yvx.zycfv.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ltq.havefunace.top

[R48] awk 取指定列
来源：http://vvf.jinqigfzy.top

awk '{print $1, $3}' a.txt
来源：http://kbm.redwolf501.top

[R49] awk 带条件
来源：http://mkk.cheryme.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://eqy.smart0.xyz

[R50] awk 求和
来源：http://emm.pengpengdd.cyou

awk '{s += $2} END {print s}' a.txt
来源：http://pip.yj20258888.top

[R51] 排序去重取前几
来源：http://qiw.yueranfly.top

sort a.txt | uniq -c | sort -rn | head
来源：http://zle.hnqzz.top

[R52] 统计行数
来源：http://ipu.cdnleiting.top

wc -l a.txt
来源：http://prs.yj20258.top

[R53] 查看文件头与实时尾
来源：http://iyo.andypj.xyz

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://jis.ydjk.org.cn

[R54] 比较两个文件
来源：http://cag.yj20258.top

diff a.txt b.txt
来源：http://ppw.wangshuangyany.cn

[R55] 压缩与解压
来源：http://bwy.hcnkem.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://klu.xuetiantiany.cn

[R56] 远程拷贝
来源：http://oqj.kuanghao11.cn

scp file user@host:/path/
来源：http://kna.hysaishi.cn

[R57] 远程执行命令
来源：http://sqz.zhijiandao.cn

ssh user@host 'uptime'
来源：http://reb.pycfn.com

[R58] 下载文件
来源：http://mzt.fktsv.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://fyk.cqqwz.cn

[R59] 发 POST JSON
来源：http://sfk.zhaomingkeji.xyz

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://jkk.redwolf501.top

[R60] 只看 HTTP 状态码
来源：http://ygm.hcnkem.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ega.fengsongda.top

[R61] 磁盘占用
来源：http://ucg.dashuyun.cn

df -h;  du -sh *
来源：http://zku.andypj.xyz

[R62] 找最占空间的文件
来源：http://tus.fengsongda.top

du -ah . | sort -rh | head -10
来源：http://mld.bjfxy.top

[R63] 内存与进程
来源：http://ynu.yj20258888.top

free -h;  ps aux | grep nginx
来源：http://had.guowangkeji.top

[R64] 结束进程
来源：http://frj.tian-w.cn

kill -9 $(pgrep -f app.py)
来源：http://hvt.fanxiaobao.xyz

[R65] 查看端口占用
来源：http://xwj.uphjek.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://xgu.0kj1m.cn

[R66] 定时任务
来源：http://anp.bjfxy.top

crontab -e;  crontab -l
来源：http://kyj.zdbjq.cn

[R67] 生成随机十六进制串
来源：http://ilk.guowangkeji.top


<!-- 参考信息 -->