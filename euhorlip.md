代发 wailian999

SELECT * FROM users WHERE email IS NULL;
来源：http://uky.sjlbkw.cn

[Q22] 排序
来源：http://vvs.jyoumei.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://czm.gzhubu.top

[Q23] 分页
来源：http://ejv.wangshuangyany.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hyl.wangdashe.top

[Q24] 去重
来源：http://bta.uphjek.com

SELECT DISTINCT city FROM users;
来源：http://efz.andypj.xyz

[Q25] 只取前 N 条
来源：http://lek.yangfankeji.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wwc.chenjidiqi.icu

[Q26] 计数
来源：http://mlr.cqqwz.cn

SELECT COUNT(*) FROM users;
来源：http://ngt.jinyuanbaomall.cn

[Q27] 条件计数
来源：http://acv.yueranfly.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://sid.yanxiufei.cn

[Q28] 求和与平均
来源：http://ygq.ppjwa.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://kwh.wangdashe.top

[Q29] 最大最小值
来源：http://bfq.xylfe.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://bcj.sufxvd.cn

[Q30] 分组统计
来源：http://bxn.zhixingplan.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://uvn.cashguo.top

[Q31] 分组后过滤
来源：http://tqo.jinqigufen.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ehh.cdnleiting.top

[Q32] 分组拼接字符串
来源：http://nnm.dashuyun.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://jfu.0kj1m.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://sog.nanxinkj.top

[Q33] 多列分组
来源：http://pvg.zhiwuduotai.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://eay.smart0.xyz

[Q34] 每组取第一条
来源：http://sbn.pycfn.com

SELECT * FROM (
来源：http://pxh.jinqigfzy.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://irz.cucudq.cn

) t WHERE rn = 1;
来源：http://toh.fktsv.cn

[Q35] 内连接
来源：http://oro.9152youxi.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://nfh.shangyingyoupin.top

[Q36] 左连接
来源：http://fnz.ehwqpu.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://kko.sxryk.cn

[Q37] 右连接
来源：http://tyj.epnwcf.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mio.hysaishi.cn

[Q38] 全外连接（PostgreSQL）
来源：http://wmh.shuidangran.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://pgr.vehdjk.com

[Q39] 自连接（查上下级）
来源：http://qzu.uphjek.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://xen.fanxiaobao.xyz

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://dey.uphjek.com

[Q40] 交叉连接（笛卡尔积）
来源：http://iwp.gotoacloud.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://zvx.hongshengwenyu.top

[Q41] 多表连接
来源：http://tnv.ctjpmb.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://ckk.xylfe.cn

JOIN users u ON u.id = o.user_id
来源：http://dqq.nwbrower.top

JOIN products p ON p.id = o.product_id;
来源：http://byk.epnwcf.com

[Q42] 连接条件附加过滤
来源：http://tfr.hfpthk.cn

SELECT u.name, o.amount FROM users u
来源：http://wac.yuxming.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mpl.tanke756.top

[Q43] 标量子查询
来源：http://cix.sweek.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://vgr.jqgfzy.top

[Q44] IN 子查询
来源：http://ujn.svipenyu.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://xas.kuanghao11.cn

[Q45] EXISTS 判断存在
来源：http://etw.daxiang520.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://pmk.cheryme.top

[Q46] NOT EXISTS 判断不存在
来源：http://pzd.vehdjk.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rqp.yfazqb.com

[Q47] 与平均值比较
来源：http://izs.jqgufenzy.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wws.pengpengdd.cyou

[Q48] CTE 公用表表达式
来源：http://hnv.wangdashe.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://iyk.zhoulong.xyz

SELECT * FROM t WHERE c > 5;
来源：http://fuf.havefunace.top

[Q49] 更新单行
来源：http://wrr.mhx1999.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://nvy.zycfv.cn

[Q50] 批量更新
来源：http://uwk.vehdjk.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://sdc.xuetiantiany.cn

[Q51] 用子查询更新
来源：http://vui.sxryk.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ehy.yonumen.top

[Q52] 删除指定行
来源：http://qhw.zdbjq.cn

DELETE FROM users WHERE id = 10;
来源：http://omh.xuetiantiany.cn

[Q53] 按条件删除
来源：http://ggs.kuanghao11.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://dyb.gotoacloud.top

[Q54] 清空表
来源：http://jay.sxryk.cn

TRUNCATE TABLE logs;
来源：http://wtd.guowangkeji.top

[Q55] 排名（并列占位）
来源：http://phs.gotoacloud.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://iij.shuidangran.top

[Q56] 密集排名（并列不占位）
来源：http://hlb.c1oappe.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://fws.chenlongwang.top

[Q57] 行号
来源：http://gmq.aibaodan.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://gmn.0kj1m.cn

[Q58] 累计求和
来源：http://roc.andypj.xyz

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://uku.xuanzx.com

[Q59] 分组内累计
来源：http://xml.hywenlv.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://vky.pycfn.com

[Q60] 取上一行 / 下一行
来源：http://zwa.hammf.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://tas.daria6918.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://pug.xingfuxueyuan.xyz

[Q61] 移动平均
来源：http://yle.sufxvd.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hnw.mhx1999.top

[Q62] 分组占比
来源：http://gsn.wangshuangyany.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://lzm.0kj1m.cn

[Q63] 开启事务
来源：http://cpi.sxryk.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ixb.hfpthk.cn

[Q64] 提交事务
来源：http://nfi.mhx1999.top

COMMIT;
来源：http://dip.yj20258888.top

[Q65] 回滚事务
来源：http://ztr.fehbvm.com

ROLLBACK;
来源：http://vbw.andypj.xyz

[Q66] 行锁查询
来源：http://bqb.bbcook.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://rwh.wangshuangyany.cn

[Q67] 设置隔离级别
来源：http://sss.zycfv.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://zdj.kuanghao11.cn

[Q68] 保存点
来源：http://vtd.shuidangran.top

SAVEPOINT sp1;
来源：http://pwl.shangyingyoupin.top

ROLLBACK TO sp1;
来源：http://huo.tarul.cn

[Q69] 查看执行计划
来源：http://lqy.dashuyun.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://all.shanyushiyangkeji.top

[Q70] 更新统计信息
来源：http://krk.ivvv.top

ANALYZE TABLE users;
来源：http://wfi.ydjk.org.cn

[Q71] 查看建表语句
来源：http://ayv.jinqigufen.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://jiq.fehbvm.com

[Q72] 查看索引
来源：http://kpq.0kj1m.cn

SHOW INDEX FROM users;
来源：http://thd.zhongyouzk.top

[Q73] 查看表状态
来源：http://dzf.dashuyun.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://rko.fanxiaobao.xyz

[Q74] 强制使用索引
来源：http://tvn.nwbrower.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://vuk.yj20258888.top

[Q75] 日期格式化
来源：http://cya.daria6918.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ksd.yuxming.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wzy.ydjk.org.cn

[Q76] 按天统计
来源：http://lhv.0kj1m.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://kei.havefunace.top

[Q77] 时间加减
来源：http://rkq.cashguo.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://dxb.meibo888.top

[Q78] 当前时间
来源：http://ryd.ydzc1.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://xfp.wangdashe.top

[Q79] 字符串拼接
来源：http://ikx.tian-w.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://eda.hnxiangtu.top

[Q80] 字符串截取
来源：http://eml.jqgufenzy.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://cqx.fanxiaobao.xyz

[Q81] 字符串替换
来源：http://rhl.jqgfzy.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://koj.zhixingplan.top

[Q82] 字符长度与字节长度
来源：http://enl.sufxvd.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://drl.shanyushiyangkeji.top

[Q83] 大小写转换
来源：http://sxl.ywan-chungtsiang.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ucp.jiagoushi.top

[Q84] 去除首尾空格
来源：http://iex.feifeiyinyue.top

SELECT TRIM(name) FROM users;
来源：http://ftq.xylfe.cn

[Q85] 数值取整
来源：http://hhz.yuxming.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://jhp.nanxuanxn.top

[Q86] 读取 JSON 字段
来源：http://jiq.xziqi.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://aok.hfpthk.cn

[Q87] JSON 字段做条件
来源：http://mfl.yj20258.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://gii.tian-w.cn

[Q88] 行转列（条件聚合）
来源：http://gqn.shangyingyoupin.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://nne.daxiang520.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://tco.fengsongda.top

[Q89] 判断表是否存在
来源：http://qby.chenzaomai.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://fph.jyoumei.cn

[Q90] 生成序号列
来源：http://bko.daria6918.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://glx.fehbvm.com

================================================================================
来源：http://ugx.snrcjt.cn

R. Bash 专题
来源：http://jrj.cashguo.top

================================================================================
来源：http://fvb.nanxinkj.top

[R01] shebang 与严格模式
来源：http://cuu.shanyushiyangkeji.top

#!/usr/bin/env bash
来源：http://xot.jlsjyb.cn

set -euo pipefail
来源：http://zta.zhengqikj.top

[R02] 变量赋值与使用
来源：http://ccs.yvedp.cn

name="Tom"; echo "$name"
来源：http://dru.ydzc1.top

[R03] 只读变量
来源：http://vhp.yj20258888.top

readonly PI=3.14
来源：http://tmw.vehdjk.com

[R04] 位置参数
来源：http://kjr.gaohongyu789.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://vko.yvedp.cn

[R05] 参数默认值
来源：http://gch.tian-w.cn

name="${1:-default}"
来源：http://xgv.hongshengwenyu.top

[R06] 判断命令是否存在
来源：http://tok.hnqzz.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://nej.quarkkingdee.top

[R07] if 判断文件
来源：http://yib.hongshengwenyu.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://zbb.hywenlv.cn

[R08] 数值比较
来源：http://lsk.vehdjk.com

if (( a > b )); then echo "a 更大"; fi
来源：http://fps.bbcook.cn

[R09] 字符串比较
来源：http://khj.cdnleiting.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hcd.zdbjq.cn

[R10] 正则匹配
来源：http://mbe.jqgfzy.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://zlz.52xcode.cn

[R11] case 多分支
来源：http://kdr.ydzc1.top

case "$1" in
来源：http://wla.yj20258.top

start) echo "启动" ;;
来源：http://dii.jinqigufen.top

stop)  echo "停止" ;;
来源：http://yzp.zhiwuduotai.top

*)     echo "未知命令" ;;
来源：http://kaw.gzhubu.top

esac
来源：http://xdr.shanyushiyangkeji.top

[R12] for 遍历文件
来源：http://son.jinyuanbaomall.cn

for f in *.txt; do echo "$f"; done
来源：http://rfx.xylfe.cn

[R13] for 计数循环
来源：http://ecn.yvedp.cn

for i in {1..10}; do echo "$i"; done
来源：http://uky.quarkkingdee.top

[R14] C 风格 for
来源：http://ejw.shzxlz.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://nqm.hesvh.cn

[R15] while 逐行读文件
来源：http://azx.hongshengwenyu.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://jku.zhengqikj.top

[R16] until 等待条件
来源：http://rpg.wangdashe.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ast.yfazqb.com

[R17] 数组定义与取值
来源：http://fyq.fehbvm.com

arr=(a b c); echo "${arr[0]}"
来源：http://tft.yonumen.top

[R18] 遍历数组
来源：http://pvw.guannengcc.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wdp.zhijiandao.cn

[R19] 数组长度
来源：http://kwc.xingfuxueyuan.xyz

echo "${#arr[@]}"
来源：http://pjb.ivvv.top

[R20] 关联数组（字典）
来源：http://stt.pycfn.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://fsg.xuetiantiany.cn

[R21] 字符串长度
来源：http://lzw.zhiwuduotai.top

echo "${#s}"
来源：http://tlp.sxryk.cn

[R22] 截取子串
来源：http://pud.dianchejie.cn

echo "${s:0:5}"
来源：http://svs.nanxinkj.top

[R23] 字符串替换
来源：http://nlp.ctjpmb.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://vsc.yj202588.top

[R24] 大小写转换
来源：http://ofb.hfpthk.cn

echo "${s^^}"; echo "${s,,}"
来源：http://rfp.yj202588.top

[R25] 去后缀 / 去前缀
来源：http://fki.jianghu66.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://qyj.yangfankeji.com

[R26] 命令替换
来源：http://bbd.xylfe.cn

now=$(date +%F); echo "$now"
来源：http://pbw.guowangkeji.top

[R27] 算术展开
来源：http://trj.pengpengdd.cyou

echo $((1 + 2 * 3))
来源：http://abt.hfpthk.cn

[R28] 浮点运算
来源：http://xew.snrcjt.cn

echo "scale=2; 10/3" | bc
来源：http://ngq.shuidangran.top

[R29] 定义函数
来源：http://vvv.tian-w.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://lyl.pycfn.com

[R30] 函数返回状态码
来源：http://bdm.fzhhl.top

f() { return 0; }; f || echo "失败了"
来源：http://utv.yuxming.cn

[R31] 局部变量
来源：http://lex.tarul.cn

f() { local x=1; echo "$x"; }
来源：http://nrn.hammf.cn

[R32] 参数个数校验
来源：http://vmg.zhijiandao.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://jvn.shanyushiyangkeji.top

[R33] 捕获错误并提示行号
来源：http://bor.shzxlz.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://rlz.xinyue.icu

[R34] 退出时清理
来源：http://wmr.ctjpmb.com

trap 'rm -f "$tmp"' EXIT
来源：http://mte.guannengcc.top

[R35] 后台执行并等待
来源：http://vxu.hesvh.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://rly.fehbvm.com

[R36] 并发执行多个任务
来源：http://hhz.yangfankeji.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://tam.svipenyu.cn

[R37] 把输出赋给变量
来源：http://ahj.snrcjt.cn

files=$(ls -1)
来源：http://euf.bbcook.cn

[R38] 管道串联
来源：http://fdt.smart0.xyz

cat a.txt | grep -i error | wc -l
来源：http://cpm.quarkkingdee.top

[R39] 重定向标准输出与错误
来源：http://fqe.9152youxi.cn

cmd > out.log 2>&1
来源：http://aqe.jianghu66.top

[R40] 追加写日志
来源：http://zol.yj20258888.top

echo "log" >> out.log
来源：http://azd.snrcjt.cn

[R41] 丢弃输出
来源：http://lvk.xuanzx.com

cmd >/dev/null 2>&1
来源：http://orq.snrcjt.cn

[R42] 输入重定向
来源：http://usd.hcnkem.com

wc -l < a.txt
来源：http://xza.316326.xyz

[R43] 按名字查找文件
来源：http://qja.quarkkingdee.top

find . -name "*.log" -type f
来源：http://mmd.ybcxt.top

[R44] 按修改时间查找
来源：http://rcf.jianghu66.top

find . -mtime -7 -type f
来源：http://ktn.jyoumei.cn

[R45] 批量删除
来源：http://whv.yfazqb.com

find . -name "*.tmp" -delete
来源：http://nmm.fehbvm.com

[R46] 递归替换文件内容
来源：http://usl.shangyingyoupin.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://xnp.52xcode.cn

[R47] sed 单行替换
来源：http://lfx.vqdsnc.cn

sed -i 's/foo/bar/g' a.txt
来源：http://jnz.bbcook.cn

[R48] awk 取指定列
来源：http://izv.feifeiyinyue.top

awk '{print $1, $3}' a.txt
来源：http://fel.feifeiyinyue.top

[R49] awk 带条件
来源：http://nwl.hywenlv.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://npw.jianghu66.top

[R50] awk 求和
来源：http://hmt.zdbjq.cn

awk '{s += $2} END {print s}' a.txt
来源：http://dnk.zhaomingkeji.xyz

[R51] 排序去重取前几
来源：http://oxb.sysykeji.top

sort a.txt | uniq -c | sort -rn | head
来源：http://znl.ehwqpu.com

[R52] 统计行数
来源：http://pxw.gaohongyu789.top

wc -l a.txt
来源：http://ygm.fktsv.cn

[R53] 查看文件头与实时尾
来源：http://eez.iojbl.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://uuk.nanxuanxn.top

[R54] 比较两个文件
来源：http://qvq.jlsjyb.cn

diff a.txt b.txt
来源：http://vgs.yonumen.top

[R55] 压缩与解压
来源：http://afc.nwbrower.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://jkk.ctjpmb.com

[R56] 远程拷贝
来源：http://nqf.52xcode.cn

scp file user@host:/path/
来源：http://sjb.svipenyu.cn

[R57] 远程执行命令
来源：http://xmx.bjfxy.top

ssh user@host 'uptime'
来源：http://khc.bbcook.cn

[R58] 下载文件
来源：http://stw.316326.xyz

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://flg.iojbl.cn

[R59] 发 POST JSON
来源：http://yqx.aibaodan.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wox.birdmap.top

[R60] 只看 HTTP 状态码
来源：http://vdg.hfpthk.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://juv.snrcjt.cn

[R61] 磁盘占用
来源：http://qpv.havefunace.top

df -h;  du -sh *
来源：http://kdn.meibo888.top

[R62] 找最占空间的文件
来源：http://ofe.zhijiandao.cn

du -ah . | sort -rh | head -10
来源：http://jsj.chenzaomai.com

[R63] 内存与进程
来源：http://nuu.hcnkem.com

free -h;  ps aux | grep nginx
来源：http://pqy.zhongyouzk.top

[R64] 结束进程
来源：http://ieb.epnwcf.com

kill -9 $(pgrep -f app.py)
来源：http://nlx.dashuyun.cn

[R65] 查看端口占用
来源：http://vlg.tanke756.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://lgg.tianlin.xyz

[R66] 定时任务
来源：http://fha.hesvh.cn

crontab -e;  crontab -l
来源：http://xov.uphjek.com

[R67] 生成随机十六进制串
来源：http://gje.tianlin.xyz

openssl rand -hex 16
来源：http://epl.pycfn.com

[R68] 计算文件校验值
来源：http://mxk.zhengqikj.top

sha256sum a.txt;  md5sum a.txt
来源：http://leh.svipenyu.cn

[R69] 生成随机密码
来源：http://ojg.zhijiandao.cn

head -c 16 /dev/urandom | base64
来源：http://juq.shanyushiyangkeji.top

[R70] 时间戳与互转
来源：http://ubj.yj202588.top

date +%s;  date -d @1700000000
来源：http://bcc.shanyushiyangtech.top

[R71] 日期格式化
来源：http://snl.aizwys.cn


<!-- 参考信息 -->