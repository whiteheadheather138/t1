代发 wailian999

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://gkj.shanyushiyangkeji.top

[Q20] IN 列表
来源：http://crx.jinyuanbaomall.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://clc.yueranfly.top

[Q21] 空值判断
来源：http://nyr.iojbl.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ede.aizwys.cn

[Q22] 排序
来源：http://dpi.guannengcc.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://lef.yj20258888.top

[Q23] 分页
来源：http://vpg.xinyue.icu

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://urp.ehwqpu.com

[Q24] 去重
来源：http://dlw.wangshuangyany.cn

SELECT DISTINCT city FROM users;
来源：http://kcc.yuxming.cn

[Q25] 只取前 N 条
来源：http://pre.jinyuanbaomall.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hyu.nanxuanxn.top

[Q26] 计数
来源：http://vyo.ydjk.org.cn

SELECT COUNT(*) FROM users;
来源：http://qoq.hfpthk.cn

[Q27] 条件计数
来源：http://jxs.xinyue.icu

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://nsh.fanxiaobao.xyz

[Q28] 求和与平均
来源：http://mbo.quarkkingdee.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://jnd.fzhhl.top

[Q29] 最大最小值
来源：http://nsv.hesvh.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://kdr.quarkkingdee.top

[Q30] 分组统计
来源：http://eyy.hesvh.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://nyu.fehbvm.com

[Q31] 分组后过滤
来源：http://fvi.fzhhl.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://coc.mhx1999.top

[Q32] 分组拼接字符串
来源：http://ayr.fktsv.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://lyj.hammf.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ywh.yanxiufei.cn

[Q33] 多列分组
来源：http://tyj.gogol.net.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://jvn.ppjwa.cn

[Q34] 每组取第一条
来源：http://kdu.chenjidiqi.icu

SELECT * FROM (
来源：http://jje.tanke756.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://cjv.ivvv.top

) t WHERE rn = 1;
来源：http://dtv.52xcode.cn

[Q35] 内连接
来源：http://gdr.jinyuanbaomall.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://frq.ydjk.org.cn

[Q36] 左连接
来源：http://ggw.epnwcf.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://atv.sxryk.cn

[Q37] 右连接
来源：http://fss.bjfxy.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://efh.jiagoushi.top

[Q38] 全外连接（PostgreSQL）
来源：http://vzm.hfpthk.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://tsd.jyoumei.cn

[Q39] 自连接（查上下级）
来源：http://uqb.xuanzx.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://auh.pengpengdd.cyou

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://uvm.dianchejie.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://csg.jqgfzy.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://sfq.zhongyouzk.top

[Q41] 多表连接
来源：http://eue.0kj1m.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://hwf.chenzaomai.com

JOIN users u ON u.id = o.user_id
来源：http://kza.tarul.cn

JOIN products p ON p.id = o.product_id;
来源：http://don.sufxvd.cn

[Q42] 连接条件附加过滤
来源：http://kjr.chenzaomai.com

SELECT u.name, o.amount FROM users u
来源：http://eav.zycfv.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://lbw.zhoulong.xyz

[Q43] 标量子查询
来源：http://rkf.yj20258888.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://efb.yangfankeji.com

[Q44] IN 子查询
来源：http://ove.shzxlz.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ruu.yj20258.top

[Q45] EXISTS 判断存在
来源：http://uwf.ydjk.org.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vnm.jlsjyb.cn

[Q46] NOT EXISTS 判断不存在
来源：http://dgp.zycfv.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kun.fzhhl.top

[Q47] 与平均值比较
来源：http://tzg.chenlongwang.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ptt.redwolf501.top

[Q48] CTE 公用表表达式
来源：http://jnv.fktsv.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://gdm.bbcook.cn

SELECT * FROM t WHERE c > 5;
来源：http://odu.jqgfzy.top

[Q49] 更新单行
来源：http://ufd.zhijiandao.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ejc.ppjwa.cn

[Q50] 批量更新
来源：http://ses.hammf.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://oxe.cucudq.cn

[Q51] 用子查询更新
来源：http://fgv.wangshuangyany.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://fgk.chenlongwang.top

[Q52] 删除指定行
来源：http://oxb.yuanzhike.top

DELETE FROM users WHERE id = 10;
来源：http://vjl.cdnleiting.top

[Q53] 按条件删除
来源：http://mbo.xinyue.icu

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ndt.snrcjt.cn

[Q54] 清空表
来源：http://qsu.quarkkingdee.top

TRUNCATE TABLE logs;
来源：http://bzo.ehwqpu.com

[Q55] 排名（并列占位）
来源：http://pfp.hywenlv.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://zje.hesvh.cn

[Q56] 密集排名（并列不占位）
来源：http://iar.tianlin.xyz

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://bqb.yfazqb.com

[Q57] 行号
来源：http://zik.pycfn.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://dky.0kj1m.cn

[Q58] 累计求和
来源：http://gnb.sxryk.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://czc.fktsv.cn

[Q59] 分组内累计
来源：http://qxu.yuxming.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://fnk.daria6918.cn

[Q60] 取上一行 / 下一行
来源：http://hqd.zhoulong.xyz

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hmd.xingfuxueyuan.xyz

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://iir.ppjwa.cn

[Q61] 移动平均
来源：http://ief.cashguo.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://bfr.bbcook.cn

[Q62] 分组占比
来源：http://xhx.52xcode.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://eth.zdqjudy.top

[Q63] 开启事务
来源：http://yve.hesvh.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://oyg.cdnleiting.top

[Q64] 提交事务
来源：http://vls.meibo888.top

COMMIT;
来源：http://jnl.uphjek.com

[Q65] 回滚事务
来源：http://sks.wangdashe.top

ROLLBACK;
来源：http://teu.yvedp.cn

[Q66] 行锁查询
来源：http://bhl.sweek.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://vho.aibaodan.cn

[Q67] 设置隔离级别
来源：http://zxp.zycfv.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ttk.chenjidiqi.icu

[Q68] 保存点
来源：http://xwl.hongshengwenyu.top

SAVEPOINT sp1;
来源：http://jan.gaohongyu789.top

ROLLBACK TO sp1;
来源：http://xfk.xinyue.icu

[Q69] 查看执行计划
来源：http://jtg.yongpay.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://jbq.jinghuilouyu.cn

[Q70] 更新统计信息
来源：http://tmg.smart0.xyz

ANALYZE TABLE users;
来源：http://gos.c1oappe.top

[Q71] 查看建表语句
来源：http://tkr.zycfv.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://gnz.cheryme.top

[Q72] 查看索引
来源：http://hco.chenlongwang.top

SHOW INDEX FROM users;
来源：http://dpp.shzxlz.cn

[Q73] 查看表状态
来源：http://rcj.316326.xyz

SHOW TABLE STATUS LIKE 'users';
来源：http://lao.cqqwz.cn

[Q74] 强制使用索引
来源：http://jrr.shangyingyoupin.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://iov.yj20258888.top

[Q75] 日期格式化
来源：http://ohj.9152youxi.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://dea.meibo888.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://oxx.daxiang520.top

[Q76] 按天统计
来源：http://dap.dashuyun.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://qxk.nanxinkj.top

[Q77] 时间加减
来源：http://nkz.wangshuangyany.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ztj.snrcjt.cn

[Q78] 当前时间
来源：http://ham.bjfxy.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://lzt.gaohongyu789.top

[Q79] 字符串拼接
来源：http://uqb.hywenlv.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://aec.xinyue.icu

[Q80] 字符串截取
来源：http://eee.epnwcf.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://njp.cashguo.top

[Q81] 字符串替换
来源：http://qsb.yj20258.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://pof.hywenlv.cn

[Q82] 字符长度与字节长度
来源：http://zpy.316326.xyz

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://vep.chenjidiqi.icu

[Q83] 大小写转换
来源：http://rpw.tanke756.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://jyv.shangyingyoupin.top

[Q84] 去除首尾空格
来源：http://xgg.zhixingplan.top

SELECT TRIM(name) FROM users;
来源：http://kei.cqqwz.cn

[Q85] 数值取整
来源：http://cqf.feifeiyinyue.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://nvz.cucudq.cn

[Q86] 读取 JSON 字段
来源：http://arq.0kj1m.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://rul.cqqwz.cn

[Q87] JSON 字段做条件
来源：http://fkf.316326.xyz

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://rnv.ivvv.top

[Q88] 行转列（条件聚合）
来源：http://daa.0kj1m.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://exo.iojbl.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ogw.yuxming.cn

[Q89] 判断表是否存在
来源：http://bcr.guannengcc.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ity.yonumen.top

[Q90] 生成序号列
来源：http://eik.yfazqb.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ltz.sweek.top

================================================================================
来源：http://oep.tarul.cn

R. Bash 专题
来源：http://lxy.wangshuangyany.cn

================================================================================
来源：http://hwr.xuetiantiany.cn

[R01] shebang 与严格模式
来源：http://hzl.ppjwa.cn

#!/usr/bin/env bash
来源：http://yoq.zhixingplan.top

set -euo pipefail
来源：http://mbe.yj20258888.top

[R02] 变量赋值与使用
来源：http://jfa.sufxvd.cn

name="Tom"; echo "$name"
来源：http://pzf.xingfuxueyuan.xyz

[R03] 只读变量
来源：http://tbf.aizwys.cn

readonly PI=3.14
来源：http://wjq.jinqigufen.top

[R04] 位置参数
来源：http://oag.tian-w.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://xvo.havefunace.top

[R05] 参数默认值
来源：http://wkd.zhoulong.xyz

name="${1:-default}"
来源：http://iik.havefunace.top

[R06] 判断命令是否存在
来源：http://fmd.smart0.xyz

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://pic.gaohongyu789.top

[R07] if 判断文件
来源：http://nmg.zhongyouzk.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ysm.gaohongyu789.top

[R08] 数值比较
来源：http://hoh.shanyushiyangkeji.top

if (( a > b )); then echo "a 更大"; fi
来源：http://lph.tian-w.cn

[R09] 字符串比较
来源：http://bly.jqgfzy.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://dqu.hongshengwenyu.top

[R10] 正则匹配
来源：http://qrk.gogol.net.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://fun.sweek.top

[R11] case 多分支
来源：http://vwf.gaohongyu789.top

case "$1" in
来源：http://yzn.shanyushiyangtech.top

start) echo "启动" ;;
来源：http://syc.chenjidiqi.icu

stop)  echo "停止" ;;
来源：http://kjj.pengpengdd.cyou

*)     echo "未知命令" ;;
来源：http://zft.ctjpmb.com

esac
来源：http://tlj.epnwcf.com

[R12] for 遍历文件
来源：http://rwe.daxiang520.top

for f in *.txt; do echo "$f"; done
来源：http://kuh.fktsv.cn

[R13] for 计数循环
来源：http://kqt.pengpengdd.cyou

for i in {1..10}; do echo "$i"; done
来源：http://xdk.yuanzhike.top

[R14] C 风格 for
来源：http://hjo.daria6918.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://tcl.kuanghao11.cn

[R15] while 逐行读文件
来源：http://lhe.jinghuilouyu.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://jzb.sjlbkw.cn

[R16] until 等待条件
来源：http://czx.haohaochexian.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://huz.daria6918.cn

[R17] 数组定义与取值
来源：http://oww.hywenlv.cn

arr=(a b c); echo "${arr[0]}"
来源：http://bjn.ppjwa.cn

[R18] 遍历数组
来源：http://zdt.uphjek.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://lxq.52xcode.cn

[R19] 数组长度
来源：http://mad.hysaishi.cn

echo "${#arr[@]}"
来源：http://qiu.gotoacloud.top

[R20] 关联数组（字典）
来源：http://nid.zdqjudy.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://vth.wangshuangyany.cn

[R21] 字符串长度
来源：http://kzg.zycfv.cn

echo "${#s}"
来源：http://nci.gogol.net.cn

[R22] 截取子串
来源：http://klu.hammf.cn

echo "${s:0:5}"
来源：http://lci.andypj.xyz

[R23] 字符串替换
来源：http://lra.yfazqb.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://kvq.hnxiangtu.top

[R24] 大小写转换
来源：http://mcm.c1oappe.top

echo "${s^^}"; echo "${s,,}"
来源：http://xse.smart0.xyz

[R25] 去后缀 / 去前缀
来源：http://grb.svipenyu.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://jnb.hnxiangtu.top

[R26] 命令替换
来源：http://ryc.aibaodan.cn

now=$(date +%F); echo "$now"
来源：http://rpv.dashuyun.cn

[R27] 算术展开
来源：http://xue.jqgufenzy.top

echo $((1 + 2 * 3))
来源：http://uqr.tianlin.xyz

[R28] 浮点运算
来源：http://hpl.zhixingplan.top

echo "scale=2; 10/3" | bc
来源：http://yst.hywenlv.cn

[R29] 定义函数
来源：http://nkg.shangyingyoupin.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://dxq.xinyue.icu

[R30] 函数返回状态码
来源：http://huk.daria6918.cn

f() { return 0; }; f || echo "失败了"
来源：http://jyv.meibo888.top

[R31] 局部变量
来源：http://qzv.redwolf501.top

f() { local x=1; echo "$x"; }
来源：http://dav.ydzc1.top

[R32] 参数个数校验
来源：http://dpq.kuanghao11.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ckt.gzhubu.top

[R33] 捕获错误并提示行号
来源：http://ldg.tarul.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mkb.hysaishi.cn

[R34] 退出时清理
来源：http://phu.hammf.cn

trap 'rm -f "$tmp"' EXIT
来源：http://dtp.ppjwa.cn

[R35] 后台执行并等待
来源：http://kyf.xylfe.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ykb.gogol.net.cn

[R36] 并发执行多个任务
来源：http://pfu.jyoumei.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ubf.dashuyun.cn

[R37] 把输出赋给变量
来源：http://zna.daxiang520.top

files=$(ls -1)
来源：http://qpf.jlsjyb.cn

[R38] 管道串联
来源：http://nac.iojbl.cn

cat a.txt | grep -i error | wc -l
来源：http://vtq.zhijiandao.cn

[R39] 重定向标准输出与错误
来源：http://trt.yuxming.cn

cmd > out.log 2>&1
来源：http://zds.ppjwa.cn

[R40] 追加写日志
来源：http://lhc.chenzaomai.com

echo "log" >> out.log
来源：http://stq.hammf.cn

[R41] 丢弃输出
来源：http://hyt.nwbrower.top

cmd >/dev/null 2>&1
来源：http://mkf.cqqwz.cn

[R42] 输入重定向
来源：http://tff.smart0.xyz

wc -l < a.txt
来源：http://xnu.gogol.net.cn

[R43] 按名字查找文件
来源：http://zwk.xuanzx.com

find . -name "*.log" -type f
来源：http://qvc.iojbl.cn

[R44] 按修改时间查找
来源：http://eco.gogol.net.cn

find . -mtime -7 -type f
来源：http://xtg.yanxiufei.cn

[R45] 批量删除
来源：http://dtm.yj202588.top

find . -name "*.tmp" -delete
来源：http://mbz.yj202588.top

[R46] 递归替换文件内容
来源：http://yss.aizwys.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ril.hesvh.cn

[R47] sed 单行替换
来源：http://ivh.gotoacloud.top

sed -i 's/foo/bar/g' a.txt
来源：http://rud.quarkkingdee.top

[R48] awk 取指定列
来源：http://mlg.hnxiangtu.top

awk '{print $1, $3}' a.txt
来源：http://fxd.yanxiufei.cn

[R49] awk 带条件
来源：http://hgc.tarul.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://siy.daxiang520.top

[R50] awk 求和
来源：http://wjz.zhiwuduotai.top

awk '{s += $2} END {print s}' a.txt
来源：http://vfm.andypj.xyz

[R51] 排序去重取前几
来源：http://tjb.uphjek.com

sort a.txt | uniq -c | sort -rn | head
来源：http://mef.gaohongyu789.top

[R52] 统计行数
来源：http://ghr.wangshuangyany.cn

wc -l a.txt
来源：http://xpr.daxiang520.top

[R53] 查看文件头与实时尾
来源：http://edx.shzxlz.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://rxc.cheryme.top

[R54] 比较两个文件
来源：http://bom.vqdsnc.cn

diff a.txt b.txt
来源：http://tkb.cheryme.top

[R55] 压缩与解压
来源：http://yuh.xinyue.icu

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://gna.bbcook.cn

[R56] 远程拷贝
来源：http://anv.tarul.cn

scp file user@host:/path/
来源：http://qli.ivvv.top

[R57] 远程执行命令
来源：http://aau.andypj.xyz

ssh user@host 'uptime'
来源：http://zeb.vqdsnc.cn

[R58] 下载文件
来源：http://msr.dianchejie.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://nam.hongshengwenyu.top

[R59] 发 POST JSON
来源：http://oml.andypj.xyz

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://vvw.sxryk.cn

[R60] 只看 HTTP 状态码
来源：http://loa.redwolf501.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://bls.bjfxy.top

[R61] 磁盘占用
来源：http://xtg.epnwcf.com

df -h;  du -sh *
来源：http://btg.jinghuilouyu.cn

[R62] 找最占空间的文件
来源：http://gum.yfazqb.com

du -ah . | sort -rh | head -10
来源：http://tew.feifeiyinyue.top

[R63] 内存与进程
来源：http://mzn.chenjidiqi.icu

free -h;  ps aux | grep nginx
来源：http://czy.ywan-chungtsiang.top

[R64] 结束进程
来源：http://akv.sjlbkw.cn

kill -9 $(pgrep -f app.py)
来源：http://khz.yj202588.top

[R65] 查看端口占用
来源：http://sma.yfazqb.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://dva.yj202588.top

[R66] 定时任务
来源：http://nwy.shangyingyoupin.top

crontab -e;  crontab -l
来源：http://tmv.vqdsnc.cn

[R67] 生成随机十六进制串
来源：http://nls.fzhhl.top

openssl rand -hex 16
来源：http://qxn.zhijiandao.cn

[R68] 计算文件校验值
来源：http://ati.nanxinkj.top

sha256sum a.txt;  md5sum a.txt
来源：http://dhj.cucudq.cn

[R69] 生成随机密码
来源：http://nny.daria6918.cn


<!-- 参考信息 -->