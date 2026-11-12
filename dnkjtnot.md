代发 wailian999

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://npo.zhijiandao.cn

[Q32] 分组拼接字符串
来源：http://opb.sweek.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://iwe.c1oappe.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://aws.bbcook.cn

[Q33] 多列分组
来源：http://nvb.fengsongda.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://pcd.fktsv.cn

[Q34] 每组取第一条
来源：http://mnv.fktsv.cn

SELECT * FROM (
来源：http://sbh.zhoulong.xyz

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://nqr.hywenlv.cn

) t WHERE rn = 1;
来源：http://tyb.epnwcf.com

[Q35] 内连接
来源：http://aph.shuidangran.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://aqh.xuetiantiany.cn

[Q36] 左连接
来源：http://kij.shzxlz.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://tpf.shangyingyoupin.top

[Q37] 右连接
来源：http://vtl.shanyushiyangtech.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://feu.chenjidiqi.icu

[Q38] 全外连接（PostgreSQL）
来源：http://sip.birdmap.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://cpx.zhiwuduotai.top

[Q39] 自连接（查上下级）
来源：http://xwx.wangdashe.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://gti.jianghu66.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://nec.tanke756.top

[Q40] 交叉连接（笛卡尔积）
来源：http://pnz.316326.xyz

SELECT * FROM colors CROSS JOIN sizes;
来源：http://tek.zhongyouzk.top

[Q41] 多表连接
来源：http://hku.chenlongwang.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://mis.yuxming.cn

JOIN users u ON u.id = o.user_id
来源：http://jsd.zycfv.cn

JOIN products p ON p.id = o.product_id;
来源：http://jgb.gotoacloud.top

[Q42] 连接条件附加过滤
来源：http://cmk.jlsjyb.cn

SELECT u.name, o.amount FROM users u
来源：http://syr.gogol.net.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://twy.yj202588.top

[Q43] 标量子查询
来源：http://tus.chenjidiqi.icu

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://beh.dianchejie.cn

[Q44] IN 子查询
来源：http://szm.xingfuxueyuan.xyz

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mzy.feifeiyinyue.top

[Q45] EXISTS 判断存在
来源：http://zrf.ydzc1.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ubn.chenzaomai.com

[Q46] NOT EXISTS 判断不存在
来源：http://anv.gaohongyu789.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xms.zhengqikj.top

[Q47] 与平均值比较
来源：http://tfu.ydjk.org.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://lay.zhixingplan.top

[Q48] CTE 公用表表达式
来源：http://aov.haohaochexian.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://lxb.aizwys.cn

SELECT * FROM t WHERE c > 5;
来源：http://dsd.hcnkem.com

[Q49] 更新单行
来源：http://ykx.aizwys.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ifm.gzhubu.top

[Q50] 批量更新
来源：http://cfw.snrcjt.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://glq.fehbvm.com

[Q51] 用子查询更新
来源：http://atr.fzhhl.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://bwz.sweek.top

[Q52] 删除指定行
来源：http://brf.feifeiyinyue.top

DELETE FROM users WHERE id = 10;
来源：http://grn.yanxiufei.cn

[Q53] 按条件删除
来源：http://vpi.jqgfzy.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wlf.ivvv.top

[Q54] 清空表
来源：http://tao.yangfankeji.com

TRUNCATE TABLE logs;
来源：http://bwr.chenjidiqi.icu

[Q55] 排名（并列占位）
来源：http://dvw.iojbl.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://zzq.yvedp.cn

[Q56] 密集排名（并列不占位）
来源：http://xxj.xuanzx.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hae.haohaochexian.top

[Q57] 行号
来源：http://ysn.hongshengwenyu.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://vlw.xylfe.cn

[Q58] 累计求和
来源：http://lhb.hnxiangtu.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://uhr.jqgufenzy.top

[Q59] 分组内累计
来源：http://yqh.fanxiaobao.xyz

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://nnw.epnwcf.com

[Q60] 取上一行 / 下一行
来源：http://hwe.ehwqpu.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://rsu.gotoacloud.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hnl.yfazqb.com

[Q61] 移动平均
来源：http://sbn.xingfuxueyuan.xyz

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://cab.smart0.xyz

[Q62] 分组占比
来源：http://mez.havefunace.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://vdn.guannengcc.top

[Q63] 开启事务
来源：http://vmc.fehbvm.com

START TRANSACTION;                -- 或 BEGIN
来源：http://bpr.haohaochexian.top

[Q64] 提交事务
来源：http://pxc.zhengqikj.top

COMMIT;
来源：http://ema.316326.xyz

[Q65] 回滚事务
来源：http://tax.shanyushiyangkeji.top

ROLLBACK;
来源：http://dlp.wangdashe.top

[Q66] 行锁查询
来源：http://ymf.jiagoushi.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://eex.xinyue.icu

[Q67] 设置隔离级别
来源：http://iqs.gzhubu.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wei.andypj.xyz

[Q68] 保存点
来源：http://csi.quarkkingdee.top

SAVEPOINT sp1;
来源：http://hfd.aibaodan.cn

ROLLBACK TO sp1;
来源：http://clx.xuetiantiany.cn

[Q69] 查看执行计划
来源：http://txt.redwolf501.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://zct.zdbjq.cn

[Q70] 更新统计信息
来源：http://hae.jinqigfzy.top

ANALYZE TABLE users;
来源：http://zkf.zhongyouzk.top

[Q71] 查看建表语句
来源：http://sie.zdqjudy.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://iwo.zhongyouzk.top

[Q72] 查看索引
来源：http://gpp.pengpengdd.cyou

SHOW INDEX FROM users;
来源：http://lwk.cqqwz.cn

[Q73] 查看表状态
来源：http://knl.snrcjt.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://vdm.ydjk.org.cn

[Q74] 强制使用索引
来源：http://zcu.shzxlz.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://okk.tianlin.xyz

[Q75] 日期格式化
来源：http://dky.redwolf501.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://kan.cucudq.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://kvq.yueranfly.top

[Q76] 按天统计
来源：http://fyd.zdbjq.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://gei.shangyingyoupin.top

[Q77] 时间加减
来源：http://ohw.tianlin.xyz

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://kvv.quarkkingdee.top

[Q78] 当前时间
来源：http://tye.smart0.xyz

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://cjh.shuidangran.top

[Q79] 字符串拼接
来源：http://laz.xziqi.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://xaj.pengpengdd.cyou

[Q80] 字符串截取
来源：http://ypq.haohaochexian.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://tys.fanxiaobao.xyz

[Q81] 字符串替换
来源：http://ktd.haohaochexian.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://alf.birdmap.top

[Q82] 字符长度与字节长度
来源：http://sol.guannengcc.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wee.kuanghao11.cn

[Q83] 大小写转换
来源：http://aur.mhx1999.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://pab.yj202588.top

[Q84] 去除首尾空格
来源：http://ljn.aizwys.cn

SELECT TRIM(name) FROM users;
来源：http://xcp.snrcjt.cn

[Q85] 数值取整
来源：http://btf.chenlongwang.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ypj.daria6918.cn

[Q86] 读取 JSON 字段
来源：http://aei.andypj.xyz

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://kub.epnwcf.com

[Q87] JSON 字段做条件
来源：http://xoc.tian-w.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mmp.52xcode.cn

[Q88] 行转列（条件聚合）
来源：http://uhl.cucudq.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://phe.aibaodan.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://afa.yonumen.top

[Q89] 判断表是否存在
来源：http://wxj.haohaochexian.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://vbx.iojbl.cn

[Q90] 生成序号列
来源：http://bma.jinqigufen.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ccu.yfazqb.com

================================================================================
来源：http://wrq.cdnleiting.top

R. Bash 专题
来源：http://cga.snrcjt.cn

================================================================================
来源：http://ksh.daria6918.cn

[R01] shebang 与严格模式
来源：http://sjm.ivvv.top

#!/usr/bin/env bash
来源：http://uhn.meibo888.top

set -euo pipefail
来源：http://ukm.shanyushiyangtech.top

[R02] 变量赋值与使用
来源：http://kce.zhixingplan.top

name="Tom"; echo "$name"
来源：http://pdv.ydzc1.top

[R03] 只读变量
来源：http://prr.hammf.cn

readonly PI=3.14
来源：http://jqo.sufxvd.cn

[R04] 位置参数
来源：http://zah.vehdjk.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://lsv.tianlin.xyz

[R05] 参数默认值
来源：http://eld.jianghu66.top

name="${1:-default}"
来源：http://seh.shuidangran.top

[R06] 判断命令是否存在
来源：http://nwv.zhiwuduotai.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://vzd.xuetiantiany.cn

[R07] if 判断文件
来源：http://vuq.gotoacloud.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://pvp.yonumen.top

[R08] 数值比较
来源：http://dmu.hongshengwenyu.top

if (( a > b )); then echo "a 更大"; fi
来源：http://jjw.jyoumei.cn

[R09] 字符串比较
来源：http://hwo.yonumen.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hyf.hnqzz.top

[R10] 正则匹配
来源：http://sdb.shuidangran.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://vtj.shanyushiyangkeji.top

[R11] case 多分支
来源：http://gxk.chenjidiqi.icu

case "$1" in
来源：http://prw.zhaomingkeji.xyz

start) echo "启动" ;;
来源：http://rfw.cashguo.top

stop)  echo "停止" ;;
来源：http://btr.quarkkingdee.top

*)     echo "未知命令" ;;
来源：http://hcx.kuanghao11.cn

esac
来源：http://exf.jianghu66.top

[R12] for 遍历文件
来源：http://btq.uphjek.com

for f in *.txt; do echo "$f"; done
来源：http://zuj.ivvv.top

[R13] for 计数循环
来源：http://arc.zhaomingkeji.xyz

for i in {1..10}; do echo "$i"; done
来源：http://chr.feifeiyinyue.top

[R14] C 风格 for
来源：http://egt.316326.xyz

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ijc.aizwys.cn

[R15] while 逐行读文件
来源：http://fax.ydjk.org.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://lko.ydjk.org.cn

[R16] until 等待条件
来源：http://kzy.meibo888.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ysg.tian-w.cn

[R17] 数组定义与取值
来源：http://een.ehwqpu.com

arr=(a b c); echo "${arr[0]}"
来源：http://tpt.c1oappe.top

[R18] 遍历数组
来源：http://slk.cqqwz.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://zty.zhongyouzk.top

[R19] 数组长度
来源：http://ive.52xcode.cn

echo "${#arr[@]}"
来源：http://xer.xuetiantiany.cn

[R20] 关联数组（字典）
来源：http://uej.jqgufenzy.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://lbv.fehbvm.com

[R21] 字符串长度
来源：http://yql.wangdashe.top

echo "${#s}"
来源：http://lrs.jyoumei.cn

[R22] 截取子串
来源：http://osv.meibo888.top

echo "${s:0:5}"
来源：http://bjl.hysaishi.cn

[R23] 字符串替换
来源：http://gtd.hcnkem.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://amk.jinqigufen.top

[R24] 大小写转换
来源：http://kfo.hywenlv.cn

echo "${s^^}"; echo "${s,,}"
来源：http://aft.tianlin.xyz

[R25] 去后缀 / 去前缀
来源：http://lsq.xinyue.icu

echo "${f%.txt}"; echo "${f#./}"
来源：http://ycq.tanke756.top

[R26] 命令替换
来源：http://lyx.xylfe.cn

now=$(date +%F); echo "$now"
来源：http://qou.yvedp.cn

[R27] 算术展开
来源：http://ijd.zhiwuduotai.top

echo $((1 + 2 * 3))
来源：http://njh.yuxming.cn

[R28] 浮点运算
来源：http://uau.svipenyu.cn

echo "scale=2; 10/3" | bc
来源：http://cyx.sufxvd.cn

[R29] 定义函数
来源：http://lwd.c1oappe.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ndu.cqqwz.cn

[R30] 函数返回状态码
来源：http://esb.tanke756.top

f() { return 0; }; f || echo "失败了"
来源：http://xjd.birdmap.top

[R31] 局部变量
来源：http://aue.guannengcc.top

f() { local x=1; echo "$x"; }
来源：http://kgm.fktsv.cn

[R32] 参数个数校验
来源：http://jli.jqgfzy.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://kpz.chenjidiqi.icu

[R33] 捕获错误并提示行号
来源：http://wco.sysykeji.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://xfp.daria6918.cn

[R34] 退出时清理
来源：http://tja.hnqzz.top

trap 'rm -f "$tmp"' EXIT
来源：http://dmk.shanyushiyangtech.top

[R35] 后台执行并等待
来源：http://kuj.ydzc1.top

sleep 5 & pid=$!; wait "$pid"
来源：http://wsl.wangshuangyany.cn

[R36] 并发执行多个任务
来源：http://gth.yj20258.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ypc.shuidangran.top

[R37] 把输出赋给变量
来源：http://pgp.shzxlz.cn

files=$(ls -1)
来源：http://fga.ppjwa.cn

[R38] 管道串联
来源：http://ivr.xinyue.icu

cat a.txt | grep -i error | wc -l
来源：http://glh.yvedp.cn

[R39] 重定向标准输出与错误
来源：http://chd.quarkkingdee.top

cmd > out.log 2>&1
来源：http://had.iojbl.cn

[R40] 追加写日志
来源：http://apf.wangshuangyany.cn

echo "log" >> out.log
来源：http://vge.fanxiaobao.xyz

[R41] 丢弃输出
来源：http://efa.tian-w.cn

cmd >/dev/null 2>&1
来源：http://obt.chenjidiqi.icu

[R42] 输入重定向
来源：http://qpi.sufxvd.cn

wc -l < a.txt
来源：http://tww.mhx1999.top

[R43] 按名字查找文件
来源：http://qaf.sweek.top

find . -name "*.log" -type f
来源：http://kve.jinyuanbaomall.cn

[R44] 按修改时间查找
来源：http://dss.yj20258.top

find . -mtime -7 -type f
来源：http://gln.fktsv.cn

[R45] 批量删除
来源：http://anw.iojbl.cn

find . -name "*.tmp" -delete
来源：http://dgv.guowangkeji.top

[R46] 递归替换文件内容
来源：http://onx.wangshuangyany.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://sxk.vqdsnc.cn

[R47] sed 单行替换
来源：http://ctp.ybcxt.top

sed -i 's/foo/bar/g' a.txt
来源：http://bag.xuetiantiany.cn

[R48] awk 取指定列
来源：http://qfn.shangyingyoupin.top

awk '{print $1, $3}' a.txt
来源：http://ofh.hysaishi.cn

[R49] awk 带条件
来源：http://nai.andypj.xyz

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://obe.cqqwz.cn

[R50] awk 求和
来源：http://gmq.yangfankeji.com

awk '{s += $2} END {print s}' a.txt
来源：http://elj.chenjidiqi.icu

[R51] 排序去重取前几
来源：http://kww.zhiwuduotai.top

sort a.txt | uniq -c | sort -rn | head
来源：http://kwc.jinqigfzy.top

[R52] 统计行数
来源：http://xem.nwbrower.top

wc -l a.txt
来源：http://wlv.ydzc1.top

[R53] 查看文件头与实时尾
来源：http://aan.dianchejie.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://gbv.cheryme.top

[R54] 比较两个文件
来源：http://uxd.svipenyu.cn

diff a.txt b.txt
来源：http://mvq.redwolf501.top

[R55] 压缩与解压
来源：http://dbi.pengpengdd.cyou

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ewr.cdnleiting.top

[R56] 远程拷贝
来源：http://ymh.pycfn.com

scp file user@host:/path/
来源：http://uso.gaohongyu789.top

[R57] 远程执行命令
来源：http://pkp.yanxiufei.cn

ssh user@host 'uptime'
来源：http://zdj.316326.xyz

[R58] 下载文件
来源：http://rci.bjfxy.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://efd.zhixingplan.top

[R59] 发 POST JSON
来源：http://vgl.jinqigufen.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://vsz.guannengcc.top

[R60] 只看 HTTP 状态码
来源：http://gta.0kj1m.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://sjj.quarkkingdee.top

[R61] 磁盘占用
来源：http://zdp.kuanghao11.cn

df -h;  du -sh *
来源：http://pzn.shangyingyoupin.top

[R62] 找最占空间的文件
来源：http://hrm.c1oappe.top

du -ah . | sort -rh | head -10
来源：http://osz.ydjk.org.cn

[R63] 内存与进程
来源：http://ipk.xuetiantiany.cn

free -h;  ps aux | grep nginx
来源：http://gta.bbcook.cn

[R64] 结束进程
来源：http://bny.shanyushiyangtech.top

kill -9 $(pgrep -f app.py)
来源：http://qcu.redwolf501.top

[R65] 查看端口占用
来源：http://mef.mhx1999.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://zuv.shuidangran.top

[R66] 定时任务
来源：http://lcu.ywan-chungtsiang.top

crontab -e;  crontab -l
来源：http://tvs.ctjpmb.com

[R67] 生成随机十六进制串
来源：http://bts.hcnkem.com

openssl rand -hex 16
来源：http://ycm.yueranfly.top

[R68] 计算文件校验值
来源：http://daf.daxiang520.top

sha256sum a.txt;  md5sum a.txt
来源：http://yvm.xuetiantiany.cn

[R69] 生成随机密码
来源：http://lpl.yuxming.cn

head -c 16 /dev/urandom | base64
来源：http://ksl.aizwys.cn

[R70] 时间戳与互转
来源：http://xji.zhaomingkeji.xyz

date +%s;  date -d @1700000000
来源：http://aqk.aizwys.cn

[R71] 日期格式化
来源：http://isy.birdmap.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://gmt.nanxuanxn.top

[R72] 等待端口就绪
来源：http://bej.aizwys.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://cey.meibo888.top

[R73] 分割大日志
来源：http://kyn.nwbrower.top

split -l 1000 big.log part_
来源：http://uaw.birdmap.top

[R74] 批量重命名
来源：http://wov.nanxinkj.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://xlb.ywan-chungtsiang.top

[R75] 导出环境变量
来源：http://wic.tian-w.cn

export PATH="$HOME/bin:$PATH"
来源：http://mmp.cashguo.top

[R76] 使用临时文件
来源：http://yvs.yj20258.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ovf.sxryk.cn

[R77] 读取用户输入
来源：http://bql.zhiwuduotai.top

read -rp "请输入: " ans
来源：http://whq.cdnleiting.top

[R78] 交互式菜单
来源：http://ksb.sweek.top

select opt in a b c; do echo "$opt"; break; done
来源：http://osn.shzxlz.cn

[R79] 解析命令行选项
来源：http://vym.xylfe.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://vhh.hongshengwenyu.top

[R80] 查看脚本执行耗时
来源：http://jnr.jlsjyb.cn

time ./run.sh
来源：http://jco.bbcook.cn

================================================================================
来源：http://jum.ppjwa.cn


<!-- 参考信息 -->