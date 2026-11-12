代发 wailian999

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://vxd.jinghuilouyu.cn

[Q28] 求和与平均
来源：http://gbo.cashguo.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://yqo.bbcook.cn

[Q29] 最大最小值
来源：http://wov.chenzaomai.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://skm.xuanzx.com

[Q30] 分组统计
来源：http://rel.zhaomingkeji.xyz

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://yja.feifeiyinyue.top

[Q31] 分组后过滤
来源：http://ugt.shuidangran.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ehz.vehdjk.com

[Q32] 分组拼接字符串
来源：http://hwz.zhengqikj.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://cpp.nanxinkj.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wgd.hcnkem.com

[Q33] 多列分组
来源：http://ewv.sufxvd.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://xnl.xziqi.cn

[Q34] 每组取第一条
来源：http://ojf.jiagoushi.top

SELECT * FROM (
来源：http://buj.jqgfzy.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wjz.yuanzhike.top

) t WHERE rn = 1;
来源：http://cwx.pengpengdd.cyou

[Q35] 内连接
来源：http://phh.dianchejie.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://cec.gaohongyu789.top

[Q36] 左连接
来源：http://owr.xingfuxueyuan.xyz

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://pnh.ivvv.top

[Q37] 右连接
来源：http://pvq.sxryk.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://zid.sufxvd.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ymh.bjfxy.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://kkx.ivvv.top

[Q39] 自连接（查上下级）
来源：http://ikv.yueranfly.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://whl.sufxvd.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ukg.iojbl.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://sca.epnwcf.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://jit.zdqjudy.top

[Q41] 多表连接
来源：http://qmd.redwolf501.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://hwl.nwbrower.top

JOIN users u ON u.id = o.user_id
来源：http://asq.0kj1m.cn

JOIN products p ON p.id = o.product_id;
来源：http://qje.birdmap.top

[Q42] 连接条件附加过滤
来源：http://cdv.chenzaomai.com

SELECT u.name, o.amount FROM users u
来源：http://jfq.ppjwa.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://zyq.yj20258888.top

[Q43] 标量子查询
来源：http://avu.fktsv.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://rjp.ivvv.top

[Q44] IN 子查询
来源：http://rpo.zhaomingkeji.xyz

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wqt.9152youxi.cn

[Q45] EXISTS 判断存在
来源：http://zug.sweek.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://efz.hnxiangtu.top

[Q46] NOT EXISTS 判断不存在
来源：http://eru.uphjek.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mtb.fengsongda.top

[Q47] 与平均值比较
来源：http://tzn.uphjek.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://fyv.gogol.net.cn

[Q48] CTE 公用表表达式
来源：http://hyr.zhoulong.xyz

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hze.jlsjyb.cn

SELECT * FROM t WHERE c > 5;
来源：http://gct.yj202588.top

[Q49] 更新单行
来源：http://rsh.zhaomingkeji.xyz

UPDATE users SET status = 1 WHERE id = 10;
来源：http://lrz.gzhubu.top

[Q50] 批量更新
来源：http://wdj.zhiwuduotai.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ofu.nanxinkj.top

[Q51] 用子查询更新
来源：http://yab.tanke756.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://urn.sxryk.cn

[Q52] 删除指定行
来源：http://gmn.hysaishi.cn

DELETE FROM users WHERE id = 10;
来源：http://cig.cashguo.top

[Q53] 按条件删除
来源：http://oct.fzhhl.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://lzd.hysaishi.cn

[Q54] 清空表
来源：http://cvl.jqgufenzy.top

TRUNCATE TABLE logs;
来源：http://hyi.wangshuangyany.cn

[Q55] 排名（并列占位）
来源：http://pdl.vqdsnc.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://qys.dashuyun.cn

[Q56] 密集排名（并列不占位）
来源：http://brg.fanxiaobao.xyz

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://nln.nanxuanxn.top

[Q57] 行号
来源：http://pbd.shangyingyoupin.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ylt.zycfv.cn

[Q58] 累计求和
来源：http://ctk.jyoumei.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://vrp.jyoumei.cn

[Q59] 分组内累计
来源：http://zdu.haohaochexian.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mky.ivvv.top

[Q60] 取上一行 / 下一行
来源：http://qnm.andypj.xyz

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://yxt.xuanzx.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://xhd.hongshengwenyu.top

[Q61] 移动平均
来源：http://wrf.chenlongwang.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hnf.52xcode.cn

[Q62] 分组占比
来源：http://lzh.ywan-chungtsiang.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://jtr.52xcode.cn

[Q63] 开启事务
来源：http://kvk.daxiang520.top

START TRANSACTION;                -- 或 BEGIN
来源：http://ynu.hammf.cn

[Q64] 提交事务
来源：http://kxg.tianlin.xyz

COMMIT;
来源：http://oit.sysykeji.top

[Q65] 回滚事务
来源：http://xzl.cdnleiting.top

ROLLBACK;
来源：http://qri.316326.xyz

[Q66] 行锁查询
来源：http://ggv.fktsv.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ncr.hnqzz.top

[Q67] 设置隔离级别
来源：http://hnn.jlsjyb.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mbf.shanyushiyangtech.top

[Q68] 保存点
来源：http://hza.yuxming.cn

SAVEPOINT sp1;
来源：http://nnj.xinyue.icu

ROLLBACK TO sp1;
来源：http://wbi.jyoumei.cn

[Q69] 查看执行计划
来源：http://wce.zdqjudy.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ost.havefunace.top

[Q70] 更新统计信息
来源：http://jhb.quarkkingdee.top

ANALYZE TABLE users;
来源：http://klc.yanxiufei.cn

[Q71] 查看建表语句
来源：http://nki.shanyushiyangtech.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://stf.ybcxt.top

[Q72] 查看索引
来源：http://onf.ehwqpu.com

SHOW INDEX FROM users;
来源：http://ypz.yj20258.top

[Q73] 查看表状态
来源：http://ust.jyoumei.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://rmo.tianlin.xyz

[Q74] 强制使用索引
来源：http://zqs.shanyushiyangtech.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ccc.jinghuilouyu.cn

[Q75] 日期格式化
来源：http://lep.jinghuilouyu.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://kdl.chenlongwang.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://vfo.xuetiantiany.cn

[Q76] 按天统计
来源：http://rmq.shangyingyoupin.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://qsh.jinghuilouyu.cn

[Q77] 时间加减
来源：http://lzr.zycfv.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ztl.c1oappe.top

[Q78] 当前时间
来源：http://nuy.yj20258888.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://xuc.sxryk.cn

[Q79] 字符串拼接
来源：http://pxf.andypj.xyz

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://nxa.cdnleiting.top

[Q80] 字符串截取
来源：http://xzv.redwolf501.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://asf.aizwys.cn

[Q81] 字符串替换
来源：http://qkv.haohaochexian.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://phs.xziqi.cn

[Q82] 字符长度与字节长度
来源：http://hzw.sysykeji.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://jeh.feifeiyinyue.top

[Q83] 大小写转换
来源：http://xsj.zdbjq.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://izz.jyoumei.cn

[Q84] 去除首尾空格
来源：http://jzb.ydzc1.top

SELECT TRIM(name) FROM users;
来源：http://xfh.ydjk.org.cn

[Q85] 数值取整
来源：http://vrj.daxiang520.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://izz.vqdsnc.cn

[Q86] 读取 JSON 字段
来源：http://glr.tanke756.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://fth.zhijiandao.cn

[Q87] JSON 字段做条件
来源：http://uoi.cdnleiting.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://pqs.jianghu66.top

[Q88] 行转列（条件聚合）
来源：http://loi.birdmap.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://akt.yj202588.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://swu.kuanghao11.cn

[Q89] 判断表是否存在
来源：http://uwd.gogol.net.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://tpe.vehdjk.com

[Q90] 生成序号列
来源：http://off.hysaishi.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://vkg.fanxiaobao.xyz

================================================================================
来源：http://vcw.smart0.xyz

R. Bash 专题
来源：http://bai.jqgfzy.top

================================================================================
来源：http://kxc.sjlbkw.cn

[R01] shebang 与严格模式
来源：http://zpo.jqgfzy.top

#!/usr/bin/env bash
来源：http://wum.gogol.net.cn

set -euo pipefail
来源：http://rky.zhengqikj.top

[R02] 变量赋值与使用
来源：http://tsk.yuanzhike.top

name="Tom"; echo "$name"
来源：http://oab.xylfe.cn

[R03] 只读变量
来源：http://tip.vehdjk.com

readonly PI=3.14
来源：http://wlo.sufxvd.cn

[R04] 位置参数
来源：http://kad.xuetiantiany.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://iyf.hammf.cn

[R05] 参数默认值
来源：http://elr.hnxiangtu.top

name="${1:-default}"
来源：http://ubf.xuetiantiany.cn

[R06] 判断命令是否存在
来源：http://cum.zhongyouzk.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://gvg.jianghu66.top

[R07] if 判断文件
来源：http://hre.ywan-chungtsiang.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://aoj.hammf.cn

[R08] 数值比较
来源：http://gep.daria6918.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://bco.xingfuxueyuan.xyz

[R09] 字符串比较
来源：http://kkt.wangdashe.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://usn.tarul.cn

[R10] 正则匹配
来源：http://ybx.tianlin.xyz

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://utw.hesvh.cn

[R11] case 多分支
来源：http://jeh.snrcjt.cn

case "$1" in
来源：http://zjw.nanxinkj.top

start) echo "启动" ;;
来源：http://aaz.jiagoushi.top

stop)  echo "停止" ;;
来源：http://czh.pengpengdd.cyou

*)     echo "未知命令" ;;
来源：http://mrk.feifeiyinyue.top

esac
来源：http://axm.svipenyu.cn

[R12] for 遍历文件
来源：http://ccx.yueranfly.top

for f in *.txt; do echo "$f"; done
来源：http://bph.cqqwz.cn

[R13] for 计数循环
来源：http://bvq.tarul.cn

for i in {1..10}; do echo "$i"; done
来源：http://zdv.yj20258.top

[R14] C 风格 for
来源：http://ciu.wangdashe.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wnz.sysykeji.top

[R15] while 逐行读文件
来源：http://uuk.zhengqikj.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ubz.yj202588.top

[R16] until 等待条件
来源：http://crs.cqqwz.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://zdu.fengsongda.top

[R17] 数组定义与取值
来源：http://ofq.zdbjq.cn

arr=(a b c); echo "${arr[0]}"
来源：http://lfb.hfpthk.cn

[R18] 遍历数组
来源：http://nit.xuetiantiany.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ceq.shanyushiyangtech.top

[R19] 数组长度
来源：http://udg.0kj1m.cn

echo "${#arr[@]}"
来源：http://vat.ehwqpu.com

[R20] 关联数组（字典）
来源：http://rtl.jqgfzy.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://izi.yongpay.top

[R21] 字符串长度
来源：http://reu.fzhhl.top

echo "${#s}"
来源：http://fmc.sjlbkw.cn

[R22] 截取子串
来源：http://hka.aizwys.cn

echo "${s:0:5}"
来源：http://sbe.jqgufenzy.top

[R23] 字符串替换
来源：http://fxi.chenzaomai.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mao.wangdashe.top

[R24] 大小写转换
来源：http://nkc.hysaishi.cn

echo "${s^^}"; echo "${s,,}"
来源：http://awn.xziqi.cn

[R25] 去后缀 / 去前缀
来源：http://dxb.snrcjt.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://jev.zhaomingkeji.xyz

[R26] 命令替换
来源：http://yvt.xuanzx.com

now=$(date +%F); echo "$now"
来源：http://kbk.daria6918.cn

[R27] 算术展开
来源：http://bhg.aibaodan.cn

echo $((1 + 2 * 3))
来源：http://xcp.shzxlz.cn

[R28] 浮点运算
来源：http://itv.jqgfzy.top

echo "scale=2; 10/3" | bc
来源：http://ycm.dashuyun.cn

[R29] 定义函数
来源：http://npv.yfazqb.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://iwc.ydzc1.top

[R30] 函数返回状态码
来源：http://rbm.jinqigfzy.top

f() { return 0; }; f || echo "失败了"
来源：http://qoo.wangshuangyany.cn

[R31] 局部变量
来源：http://zks.c1oappe.top

f() { local x=1; echo "$x"; }
来源：http://npn.uphjek.com

[R32] 参数个数校验
来源：http://uro.zhengqikj.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://kbz.haohaochexian.top

[R33] 捕获错误并提示行号
来源：http://lsi.snrcjt.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://uug.sysykeji.top

[R34] 退出时清理
来源：http://ldx.jqgufenzy.top

trap 'rm -f "$tmp"' EXIT
来源：http://oqo.tanke756.top

[R35] 后台执行并等待
来源：http://vdo.hesvh.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://sew.hywenlv.cn

[R36] 并发执行多个任务
来源：http://nmz.jqgfzy.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://szs.aizwys.cn

[R37] 把输出赋给变量
来源：http://nor.chenjidiqi.icu

files=$(ls -1)
来源：http://vho.ydjk.org.cn

[R38] 管道串联
来源：http://wls.cashguo.top

cat a.txt | grep -i error | wc -l
来源：http://psg.shuidangran.top

[R39] 重定向标准输出与错误
来源：http://low.sweek.top

cmd > out.log 2>&1
来源：http://qyr.sysykeji.top

[R40] 追加写日志
来源：http://jvn.zhijiandao.cn

echo "log" >> out.log
来源：http://sdo.ppjwa.cn

[R41] 丢弃输出
来源：http://avf.fehbvm.com

cmd >/dev/null 2>&1
来源：http://lli.xuetiantiany.cn

[R42] 输入重定向
来源：http://wvm.zhoulong.xyz

wc -l < a.txt
来源：http://xsm.ywan-chungtsiang.top

[R43] 按名字查找文件
来源：http://umf.guannengcc.top

find . -name "*.log" -type f
来源：http://cfn.yueranfly.top

[R44] 按修改时间查找
来源：http://nte.ydjk.org.cn

find . -mtime -7 -type f
来源：http://wkx.zhengqikj.top

[R45] 批量删除
来源：http://wbz.xinyue.icu

find . -name "*.tmp" -delete
来源：http://pts.yj20258.top

[R46] 递归替换文件内容
来源：http://vyx.haohaochexian.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://kkm.birdmap.top

[R47] sed 单行替换
来源：http://yfb.sweek.top

sed -i 's/foo/bar/g' a.txt
来源：http://uvl.zycfv.cn

[R48] awk 取指定列
来源：http://rea.yonumen.top

awk '{print $1, $3}' a.txt
来源：http://fwy.zhixingplan.top

[R49] awk 带条件
来源：http://uhk.jqgufenzy.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://gxc.shzxlz.cn

[R50] awk 求和
来源：http://wwn.vqdsnc.cn

awk '{s += $2} END {print s}' a.txt
来源：http://eql.sxryk.cn

[R51] 排序去重取前几
来源：http://ojb.zhaomingkeji.xyz

sort a.txt | uniq -c | sort -rn | head
来源：http://rsn.gogol.net.cn

[R52] 统计行数
来源：http://xxt.jlsjyb.cn

wc -l a.txt
来源：http://tol.yueranfly.top

[R53] 查看文件头与实时尾
来源：http://yjq.hnqzz.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://gmq.jqgfzy.top

[R54] 比较两个文件
来源：http://etp.andypj.xyz

diff a.txt b.txt
来源：http://rmi.ivvv.top

[R55] 压缩与解压
来源：http://zaf.hywenlv.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://nbr.xziqi.cn

[R56] 远程拷贝
来源：http://hgv.mhx1999.top

scp file user@host:/path/
来源：http://lga.yonumen.top

[R57] 远程执行命令
来源：http://rze.jqgufenzy.top

ssh user@host 'uptime'
来源：http://nxo.daxiang520.top

[R58] 下载文件
来源：http://ppk.xziqi.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://kfr.chenzaomai.com

[R59] 发 POST JSON
来源：http://fwq.shuidangran.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://jto.zycfv.cn

[R60] 只看 HTTP 状态码
来源：http://uon.guannengcc.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://rmz.chenzaomai.com

[R61] 磁盘占用
来源：http://gmh.shanyushiyangkeji.top

df -h;  du -sh *
来源：http://ytl.zhaomingkeji.xyz

[R62] 找最占空间的文件
来源：http://zus.jinqigufen.top

du -ah . | sort -rh | head -10
来源：http://vyp.shanyushiyangkeji.top

[R63] 内存与进程
来源：http://jzu.jqgufenzy.top

free -h;  ps aux | grep nginx
来源：http://szc.kuanghao11.cn

[R64] 结束进程
来源：http://lhj.ybcxt.top

kill -9 $(pgrep -f app.py)
来源：http://cun.bjfxy.top

[R65] 查看端口占用
来源：http://rnw.nwbrower.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://faj.zdqjudy.top

[R66] 定时任务
来源：http://rqd.yanxiufei.cn

crontab -e;  crontab -l
来源：http://vds.zhongyouzk.top

[R67] 生成随机十六进制串
来源：http://mdf.hnxiangtu.top

openssl rand -hex 16
来源：http://eqq.gogol.net.cn

[R68] 计算文件校验值
来源：http://jrp.bjfxy.top

sha256sum a.txt;  md5sum a.txt
来源：http://tdy.hywenlv.cn

[R69] 生成随机密码
来源：http://hqn.zhiwuduotai.top

head -c 16 /dev/urandom | base64
来源：http://xmf.bbcook.cn

[R70] 时间戳与互转
来源：http://tva.fehbvm.com

date +%s;  date -d @1700000000
来源：http://fku.gaohongyu789.top

[R71] 日期格式化
来源：http://jzr.hnxiangtu.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://jgv.guannengcc.top

[R72] 等待端口就绪
来源：http://lna.xuanzx.com

until nc -z localhost 3306; do sleep 1; done
来源：http://xmz.52xcode.cn

[R73] 分割大日志
来源：http://npc.fzhhl.top

split -l 1000 big.log part_
来源：http://wml.andypj.xyz

[R74] 批量重命名
来源：http://ayk.shanyushiyangtech.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://lvi.smart0.xyz

[R75] 导出环境变量
来源：http://ygp.fktsv.cn

export PATH="$HOME/bin:$PATH"
来源：http://bhi.epnwcf.com

[R76] 使用临时文件
来源：http://aqy.guowangkeji.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://rmz.jyoumei.cn

[R77] 读取用户输入
来源：http://wvv.fktsv.cn


<!-- 参考信息 -->