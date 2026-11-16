代发 wailian999

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://pnj.shzxlz.cn

[Q26] 计数
来源：http://hyu.xylfe.cn

SELECT COUNT(*) FROM users;
来源：http://iul.gogol.net.cn

[Q27] 条件计数
来源：http://jtr.xuetiantiany.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wct.vqdsnc.cn

[Q28] 求和与平均
来源：http://duy.daria6918.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://uyj.hfpthk.cn

[Q29] 最大最小值
来源：http://ide.hnxiangtu.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://liv.yuanzhike.top

[Q30] 分组统计
来源：http://rga.chenjidiqi.icu

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://qjf.cashguo.top

[Q31] 分组后过滤
来源：http://jsm.sweek.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://orq.yangfankeji.com

[Q32] 分组拼接字符串
来源：http://rcg.kuanghao11.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://war.ppjwa.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://gar.pycfn.com

[Q33] 多列分组
来源：http://uxq.yueranfly.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://fdt.zycfv.cn

[Q34] 每组取第一条
来源：http://sjn.sysykeji.top

SELECT * FROM (
来源：http://fqt.jqgufenzy.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://egv.zhongyouzk.top

) t WHERE rn = 1;
来源：http://kbt.cucudq.cn

[Q35] 内连接
来源：http://sxz.zhiwuduotai.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://evl.sufxvd.cn

[Q36] 左连接
来源：http://ajw.52xcode.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://bsp.nwbrower.top

[Q37] 右连接
来源：http://vxt.zhaomingkeji.xyz

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://iad.redwolf501.top

[Q38] 全外连接（PostgreSQL）
来源：http://uaf.kuanghao11.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ycd.yfazqb.com

[Q39] 自连接（查上下级）
来源：http://iab.zdbjq.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://unz.jinqigfzy.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://lfc.ywan-chungtsiang.top

[Q40] 交叉连接（笛卡尔积）
来源：http://qjk.hongshengwenyu.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://oqe.shanyushiyangkeji.top

[Q41] 多表连接
来源：http://xke.cheryme.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://leo.sxryk.cn

JOIN users u ON u.id = o.user_id
来源：http://pbl.jqgfzy.top

JOIN products p ON p.id = o.product_id;
来源：http://jst.chenlongwang.top

[Q42] 连接条件附加过滤
来源：http://flm.jinqigufen.top

SELECT u.name, o.amount FROM users u
来源：http://vwq.xziqi.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://aww.zdqjudy.top

[Q43] 标量子查询
来源：http://iwn.wangshuangyany.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://lya.ppjwa.cn

[Q44] IN 子查询
来源：http://nsr.vqdsnc.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ljc.bbcook.cn

[Q45] EXISTS 判断存在
来源：http://ftm.cheryme.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jiq.guowangkeji.top

[Q46] NOT EXISTS 判断不存在
来源：http://syv.zdbjq.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jse.hcnkem.com

[Q47] 与平均值比较
来源：http://ncm.pengpengdd.cyou

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://fsm.gaohongyu789.top

[Q48] CTE 公用表表达式
来源：http://tig.sufxvd.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://lpz.nanxinkj.top

SELECT * FROM t WHERE c > 5;
来源：http://uvd.aizwys.cn

[Q49] 更新单行
来源：http://tmh.sxryk.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://zyy.hongshengwenyu.top

[Q50] 批量更新
来源：http://noi.zhaomingkeji.xyz

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://jlk.vqdsnc.cn

[Q51] 用子查询更新
来源：http://tlq.cdnleiting.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mde.vehdjk.com

[Q52] 删除指定行
来源：http://ecb.jianghu66.top

DELETE FROM users WHERE id = 10;
来源：http://mpz.gogol.net.cn

[Q53] 按条件删除
来源：http://gen.vqdsnc.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://oas.zhoulong.xyz

[Q54] 清空表
来源：http://ann.ctjpmb.com

TRUNCATE TABLE logs;
来源：http://rep.jinghuilouyu.cn

[Q55] 排名（并列占位）
来源：http://axq.yueranfly.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://kca.zhongyouzk.top

[Q56] 密集排名（并列不占位）
来源：http://qnf.guannengcc.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://gqw.sxryk.cn

[Q57] 行号
来源：http://wll.sxryk.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://rkb.xingfuxueyuan.xyz

[Q58] 累计求和
来源：http://nqm.quarkkingdee.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wdo.jinyuanbaomall.cn

[Q59] 分组内累计
来源：http://dkl.0kj1m.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ktn.hesvh.cn

[Q60] 取上一行 / 下一行
来源：http://pgn.ppjwa.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://vul.daxiang520.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wnv.zdqjudy.top

[Q61] 移动平均
来源：http://hft.svipenyu.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://pnm.sxryk.cn

[Q62] 分组占比
来源：http://lmb.chenzaomai.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://dgf.gzhubu.top

[Q63] 开启事务
来源：http://lez.jqgufenzy.top

START TRANSACTION;                -- 或 BEGIN
来源：http://hzs.haohaochexian.top

[Q64] 提交事务
来源：http://ozh.kuanghao11.cn

COMMIT;
来源：http://mep.yonumen.top

[Q65] 回滚事务
来源：http://gtx.tian-w.cn

ROLLBACK;
来源：http://cmj.yonumen.top

[Q66] 行锁查询
来源：http://tcn.ybcxt.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://isr.wangdashe.top

[Q67] 设置隔离级别
来源：http://fyb.xingfuxueyuan.xyz

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://edh.vqdsnc.cn

[Q68] 保存点
来源：http://bab.hysaishi.cn

SAVEPOINT sp1;
来源：http://tgu.xziqi.cn

ROLLBACK TO sp1;
来源：http://mlu.xuanzx.com

[Q69] 查看执行计划
来源：http://zoe.snrcjt.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://vto.hesvh.cn

[Q70] 更新统计信息
来源：http://egg.yj202588.top

ANALYZE TABLE users;
来源：http://mko.zhoulong.xyz

[Q71] 查看建表语句
来源：http://fho.hywenlv.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://vlt.gaohongyu789.top

[Q72] 查看索引
来源：http://fzf.bbcook.cn

SHOW INDEX FROM users;
来源：http://gez.sjlbkw.cn

[Q73] 查看表状态
来源：http://rmp.wangshuangyany.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ntu.tanke756.top

[Q74] 强制使用索引
来源：http://jbx.yj202588.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://aec.shangyingyoupin.top

[Q75] 日期格式化
来源：http://xll.meibo888.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://pha.zhongyouzk.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://olj.hywenlv.cn

[Q76] 按天统计
来源：http://mbm.zhengqikj.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wwv.yonumen.top

[Q77] 时间加减
来源：http://yhk.hongshengwenyu.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://egv.zhixingplan.top

[Q78] 当前时间
来源：http://rmc.zdqjudy.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://dkp.jqgfzy.top

[Q79] 字符串拼接
来源：http://ows.ctjpmb.com

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://rys.bbcook.cn

[Q80] 字符串截取
来源：http://vdq.feifeiyinyue.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://vsb.c1oappe.top

[Q81] 字符串替换
来源：http://duq.guowangkeji.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://xrp.xuanzx.com

[Q82] 字符长度与字节长度
来源：http://qdj.nwbrower.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://sno.fehbvm.com

[Q83] 大小写转换
来源：http://fvx.tianlin.xyz

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://boj.quarkkingdee.top

[Q84] 去除首尾空格
来源：http://anm.pycfn.com

SELECT TRIM(name) FROM users;
来源：http://jmx.hywenlv.cn

[Q85] 数值取整
来源：http://tqq.jinghuilouyu.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://apt.aibaodan.cn

[Q86] 读取 JSON 字段
来源：http://ddg.zhaomingkeji.xyz

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ssg.haohaochexian.top

[Q87] JSON 字段做条件
来源：http://zas.xingfuxueyuan.xyz

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://atl.meibo888.top

[Q88] 行转列（条件聚合）
来源：http://vrk.redwolf501.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ojb.0kj1m.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ixw.yueranfly.top

[Q89] 判断表是否存在
来源：http://pem.andypj.xyz

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hyh.daxiang520.top

[Q90] 生成序号列
来源：http://iuk.gogol.net.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://xod.zhengqikj.top

================================================================================
来源：http://vxt.bjfxy.top

R. Bash 专题
来源：http://wmi.aibaodan.cn

================================================================================
来源：http://tzy.shangyingyoupin.top

[R01] shebang 与严格模式
来源：http://zit.shzxlz.cn

#!/usr/bin/env bash
来源：http://pnu.andypj.xyz

set -euo pipefail
来源：http://faq.pengpengdd.cyou

[R02] 变量赋值与使用
来源：http://dwp.bbcook.cn

name="Tom"; echo "$name"
来源：http://ujl.jinqigufen.top

[R03] 只读变量
来源：http://beh.aizwys.cn

readonly PI=3.14
来源：http://fmj.9152youxi.cn

[R04] 位置参数
来源：http://uqx.yanxiufei.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://qnv.zhongyouzk.top

[R05] 参数默认值
来源：http://wzm.ivvv.top

name="${1:-default}"
来源：http://ddd.jqgufenzy.top

[R06] 判断命令是否存在
来源：http://cxo.zhengqikj.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mvr.zycfv.cn

[R07] if 判断文件
来源：http://daw.hnxiangtu.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://xpi.yuanzhike.top

[R08] 数值比较
来源：http://fpr.hnxiangtu.top

if (( a > b )); then echo "a 更大"; fi
来源：http://myv.guannengcc.top

[R09] 字符串比较
来源：http://zlp.cashguo.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://zcj.chenzaomai.com

[R10] 正则匹配
来源：http://hst.zhiwuduotai.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://pze.smart0.xyz

[R11] case 多分支
来源：http://mwu.yj202588.top

case "$1" in
来源：http://ssf.jinqigufen.top

start) echo "启动" ;;
来源：http://lwl.guowangkeji.top

stop)  echo "停止" ;;
来源：http://hqk.daxiang520.top

*)     echo "未知命令" ;;
来源：http://dgt.redwolf501.top

esac
来源：http://bom.yangfankeji.com

[R12] for 遍历文件
来源：http://ehr.daria6918.cn

for f in *.txt; do echo "$f"; done
来源：http://myu.yangfankeji.com

[R13] for 计数循环
来源：http://qnl.sxryk.cn

for i in {1..10}; do echo "$i"; done
来源：http://rdd.bjfxy.top

[R14] C 风格 for
来源：http://oww.ywan-chungtsiang.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://jpb.yonumen.top

[R15] while 逐行读文件
来源：http://qof.haohaochexian.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://lyk.haohaochexian.top

[R16] until 等待条件
来源：http://uka.jianghu66.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://jna.zhiwuduotai.top

[R17] 数组定义与取值
来源：http://buh.xylfe.cn

arr=(a b c); echo "${arr[0]}"
来源：http://sfn.ctjpmb.com

[R18] 遍历数组
来源：http://zlh.zhongyouzk.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://sxe.gaohongyu789.top

[R19] 数组长度
来源：http://azr.shzxlz.cn

echo "${#arr[@]}"
来源：http://fxw.yuxming.cn

[R20] 关联数组（字典）
来源：http://qcn.feifeiyinyue.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mqj.jiagoushi.top

[R21] 字符串长度
来源：http://yjm.shanyushiyangtech.top

echo "${#s}"
来源：http://ywk.cqqwz.cn

[R22] 截取子串
来源：http://zyl.zhengqikj.top

echo "${s:0:5}"
来源：http://onx.cdnleiting.top

[R23] 字符串替换
来源：http://ogc.vehdjk.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://bbs.dianchejie.cn

[R24] 大小写转换
来源：http://hfk.sjlbkw.cn

echo "${s^^}"; echo "${s,,}"
来源：http://osa.zhiwuduotai.top

[R25] 去后缀 / 去前缀
来源：http://cyd.chenlongwang.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://ydl.nanxinkj.top

[R26] 命令替换
来源：http://qgd.zhiwuduotai.top

now=$(date +%F); echo "$now"
来源：http://dme.shanyushiyangkeji.top

[R27] 算术展开
来源：http://eng.hesvh.cn

echo $((1 + 2 * 3))
来源：http://nfh.shanyushiyangtech.top

[R28] 浮点运算
来源：http://sru.ivvv.top

echo "scale=2; 10/3" | bc
来源：http://ukr.yj202588.top

[R29] 定义函数
来源：http://scf.tian-w.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://upw.ehwqpu.com

[R30] 函数返回状态码
来源：http://pov.ppjwa.cn

f() { return 0; }; f || echo "失败了"
来源：http://pei.gotoacloud.top

[R31] 局部变量
来源：http://xyw.iojbl.cn

f() { local x=1; echo "$x"; }
来源：http://vhy.shzxlz.cn

[R32] 参数个数校验
来源：http://ycg.yonumen.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://txu.c1oappe.top

[R33] 捕获错误并提示行号
来源：http://ein.smart0.xyz

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://utg.wangdashe.top

[R34] 退出时清理
来源：http://whl.daxiang520.top

trap 'rm -f "$tmp"' EXIT
来源：http://bmx.gaohongyu789.top

[R35] 后台执行并等待
来源：http://siz.xingfuxueyuan.xyz

sleep 5 & pid=$!; wait "$pid"
来源：http://rvm.nwbrower.top

[R36] 并发执行多个任务
来源：http://uua.jqgfzy.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wfh.ivvv.top

[R37] 把输出赋给变量
来源：http://afb.tanke756.top

files=$(ls -1)
来源：http://btb.tarul.cn

[R38] 管道串联
来源：http://cna.zhiwuduotai.top

cat a.txt | grep -i error | wc -l
来源：http://jvw.bbcook.cn

[R39] 重定向标准输出与错误
来源：http://alx.guannengcc.top

cmd > out.log 2>&1
来源：http://gkm.c1oappe.top

[R40] 追加写日志
来源：http://mff.snrcjt.cn

echo "log" >> out.log
来源：http://hum.jyoumei.cn

[R41] 丢弃输出
来源：http://odm.jinghuilouyu.cn

cmd >/dev/null 2>&1
来源：http://clo.zhaomingkeji.xyz

[R42] 输入重定向
来源：http://tcz.ivvv.top

wc -l < a.txt
来源：http://awl.shangyingyoupin.top

[R43] 按名字查找文件
来源：http://vcp.xinyue.icu

find . -name "*.log" -type f
来源：http://cku.sweek.top

[R44] 按修改时间查找
来源：http://rhv.daria6918.cn

find . -mtime -7 -type f
来源：http://ebs.svipenyu.cn

[R45] 批量删除
来源：http://dat.jinqigufen.top

find . -name "*.tmp" -delete
来源：http://wqq.52xcode.cn

[R46] 递归替换文件内容
来源：http://ium.gogol.net.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://tpo.sjlbkw.cn

[R47] sed 单行替换
来源：http://mon.dianchejie.cn

sed -i 's/foo/bar/g' a.txt
来源：http://oot.nanxinkj.top

[R48] awk 取指定列
来源：http://gkh.sjlbkw.cn

awk '{print $1, $3}' a.txt
来源：http://hik.hongshengwenyu.top

[R49] awk 带条件
来源：http://njy.xuetiantiany.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://bvp.fktsv.cn

[R50] awk 求和
来源：http://sgr.yanxiufei.cn

awk '{s += $2} END {print s}' a.txt
来源：http://oyc.sweek.top

[R51] 排序去重取前几
来源：http://qom.jinqigufen.top

sort a.txt | uniq -c | sort -rn | head
来源：http://vwr.ehwqpu.com

[R52] 统计行数
来源：http://iwf.tarul.cn

wc -l a.txt
来源：http://war.ctjpmb.com

[R53] 查看文件头与实时尾
来源：http://wgh.yangfankeji.com

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://aep.cashguo.top

[R54] 比较两个文件
来源：http://foe.sweek.top

diff a.txt b.txt
来源：http://fnl.sysykeji.top

[R55] 压缩与解压
来源：http://rqu.tianlin.xyz

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://aof.ydzc1.top

[R56] 远程拷贝
来源：http://yio.316326.xyz

scp file user@host:/path/
来源：http://gcz.redwolf501.top

[R57] 远程执行命令
来源：http://prm.fehbvm.com

ssh user@host 'uptime'
来源：http://jro.ydjk.org.cn

[R58] 下载文件
来源：http://vrz.chenzaomai.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://xpy.cucudq.cn

[R59] 发 POST JSON
来源：http://smw.jqgfzy.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://awe.hfpthk.cn

[R60] 只看 HTTP 状态码
来源：http://wea.yueranfly.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ruf.sweek.top

[R61] 磁盘占用
来源：http://mon.chenzaomai.com

df -h;  du -sh *
来源：http://fky.guannengcc.top

[R62] 找最占空间的文件
来源：http://ekf.shanyushiyangtech.top

du -ah . | sort -rh | head -10
来源：http://jfu.jqgfzy.top

[R63] 内存与进程
来源：http://jgh.haohaochexian.top

free -h;  ps aux | grep nginx
来源：http://nap.chenjidiqi.icu

[R64] 结束进程
来源：http://jrz.sufxvd.cn

kill -9 $(pgrep -f app.py)
来源：http://enq.jlsjyb.cn

[R65] 查看端口占用
来源：http://rwe.dianchejie.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hij.ctjpmb.com

[R66] 定时任务
来源：http://hxc.chenlongwang.top

crontab -e;  crontab -l
来源：http://wpl.cucudq.cn

[R67] 生成随机十六进制串
来源：http://jjq.hammf.cn

openssl rand -hex 16
来源：http://lia.fanxiaobao.xyz

[R68] 计算文件校验值
来源：http://cmy.xuanzx.com

sha256sum a.txt;  md5sum a.txt
来源：http://lsa.xuanzx.com

[R69] 生成随机密码
来源：http://ong.birdmap.top

head -c 16 /dev/urandom | base64
来源：http://hoq.ybcxt.top

[R70] 时间戳与互转
来源：http://btn.jinyuanbaomall.cn

date +%s;  date -d @1700000000
来源：http://xva.zhijiandao.cn

[R71] 日期格式化
来源：http://hcf.chenjidiqi.icu

date +"%Y-%m-%d %H:%M:%S"
来源：http://xfi.yanxiufei.cn

[R72] 等待端口就绪
来源：http://qiz.ywan-chungtsiang.top

until nc -z localhost 3306; do sleep 1; done
来源：http://ukm.yj20258888.top

[R73] 分割大日志
来源：http://zrw.jinqigfzy.top

split -l 1000 big.log part_
来源：http://mth.nwbrower.top

[R74] 批量重命名
来源：http://pwv.epnwcf.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://lpg.tianlin.xyz

[R75] 导出环境变量
来源：http://knf.meibo888.top


<!-- 参考信息 -->