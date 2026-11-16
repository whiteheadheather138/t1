代发 wailian999

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://qlc.iojbl.cn

[Q28] 求和与平均
来源：http://cvn.wangdashe.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://fuq.fanxiaobao.xyz

[Q29] 最大最小值
来源：http://cpb.zhongyouzk.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://cui.shanyushiyangkeji.top

[Q30] 分组统计
来源：http://jjt.zycfv.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://yor.jqgfzy.top

[Q31] 分组后过滤
来源：http://plj.quarkkingdee.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://nub.hfpthk.cn

[Q32] 分组拼接字符串
来源：http://pgu.shanyushiyangkeji.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://sgz.zhaomingkeji.xyz

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ywh.bjfxy.top

[Q33] 多列分组
来源：http://ubv.cucudq.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://rgr.kuanghao11.cn

[Q34] 每组取第一条
来源：http://ezz.jyoumei.cn

SELECT * FROM (
来源：http://fey.sysykeji.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://yga.ppjwa.cn

) t WHERE rn = 1;
来源：http://lkk.svipenyu.cn

[Q35] 内连接
来源：http://ajx.jinqigufen.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://fgc.xylfe.cn

[Q36] 左连接
来源：http://bqy.cucudq.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://aoa.cashguo.top

[Q37] 右连接
来源：http://eii.9152youxi.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://vcs.ppjwa.cn

[Q38] 全外连接（PostgreSQL）
来源：http://iuw.meibo888.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://dgp.jyoumei.cn

[Q39] 自连接（查上下级）
来源：http://xuy.ywan-chungtsiang.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://xvs.andypj.xyz

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wgx.pycfn.com

[Q40] 交叉连接（笛卡尔积）
来源：http://bju.iojbl.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://kah.fktsv.cn

[Q41] 多表连接
来源：http://evc.xinyue.icu

SELECT o.id, u.name, p.title FROM orders o
来源：http://njy.ctjpmb.com

JOIN users u ON u.id = o.user_id
来源：http://mhi.xuanzx.com

JOIN products p ON p.id = o.product_id;
来源：http://zbj.jinghuilouyu.cn

[Q42] 连接条件附加过滤
来源：http://iro.zhoulong.xyz

SELECT u.name, o.amount FROM users u
来源：http://acb.tian-w.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://boy.fengsongda.top

[Q43] 标量子查询
来源：http://ysj.jinghuilouyu.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://deb.sysykeji.top

[Q44] IN 子查询
来源：http://zpj.wangdashe.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://qar.cheryme.top

[Q45] EXISTS 判断存在
来源：http://zmj.shangyingyoupin.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hoq.cdnleiting.top

[Q46] NOT EXISTS 判断不存在
来源：http://zkt.xylfe.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ygu.haohaochexian.top

[Q47] 与平均值比较
来源：http://xwv.9152youxi.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://tcd.nanxuanxn.top

[Q48] CTE 公用表表达式
来源：http://iuj.redwolf501.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://eia.52xcode.cn

SELECT * FROM t WHERE c > 5;
来源：http://hjz.mhx1999.top

[Q49] 更新单行
来源：http://vlt.sysykeji.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://xck.quarkkingdee.top

[Q50] 批量更新
来源：http://sbc.hfpthk.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ofg.yuxming.cn

[Q51] 用子查询更新
来源：http://uzs.dianchejie.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ntw.zhoulong.xyz

[Q52] 删除指定行
来源：http://uyz.jyoumei.cn

DELETE FROM users WHERE id = 10;
来源：http://zlm.dianchejie.cn

[Q53] 按条件删除
来源：http://bjd.zycfv.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ubl.chenlongwang.top

[Q54] 清空表
来源：http://tui.xinyue.icu

TRUNCATE TABLE logs;
来源：http://wkc.shuidangran.top

[Q55] 排名（并列占位）
来源：http://duu.nanxinkj.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://odm.haohaochexian.top

[Q56] 密集排名（并列不占位）
来源：http://bpa.yj202588.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mtb.yuanzhike.top

[Q57] 行号
来源：http://cke.yj202588.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ssf.nanxinkj.top

[Q58] 累计求和
来源：http://vtq.daria6918.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://aei.guowangkeji.top

[Q59] 分组内累计
来源：http://eyw.sweek.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://tdo.shanyushiyangtech.top

[Q60] 取上一行 / 下一行
来源：http://tqi.fengsongda.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://zir.zhoulong.xyz

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://qgd.andypj.xyz

[Q61] 移动平均
来源：http://ieg.ivvv.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://sap.xuetiantiany.cn

[Q62] 分组占比
来源：http://dfa.shanyushiyangtech.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://cxx.chenzaomai.com

[Q63] 开启事务
来源：http://rco.bjfxy.top

START TRANSACTION;                -- 或 BEGIN
来源：http://xmn.redwolf501.top

[Q64] 提交事务
来源：http://xjx.jinqigufen.top

COMMIT;
来源：http://hdd.sweek.top

[Q65] 回滚事务
来源：http://ldn.zycfv.cn

ROLLBACK;
来源：http://wxw.hcnkem.com

[Q66] 行锁查询
来源：http://vws.chenjidiqi.icu

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://sjr.shanyushiyangtech.top

[Q67] 设置隔离级别
来源：http://xqv.xingfuxueyuan.xyz

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://qkv.hfpthk.cn

[Q68] 保存点
来源：http://cvd.aibaodan.cn

SAVEPOINT sp1;
来源：http://bfp.feifeiyinyue.top

ROLLBACK TO sp1;
来源：http://qke.shzxlz.cn

[Q69] 查看执行计划
来源：http://lhh.jinyuanbaomall.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://zjl.52xcode.cn

[Q70] 更新统计信息
来源：http://jot.pycfn.com

ANALYZE TABLE users;
来源：http://yno.cashguo.top

[Q71] 查看建表语句
来源：http://cpv.fanxiaobao.xyz

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://kem.shanyushiyangkeji.top

[Q72] 查看索引
来源：http://yzj.hesvh.cn

SHOW INDEX FROM users;
来源：http://ghq.fanxiaobao.xyz

[Q73] 查看表状态
来源：http://lxk.daxiang520.top

SHOW TABLE STATUS LIKE 'users';
来源：http://ifa.yuanzhike.top

[Q74] 强制使用索引
来源：http://tez.jqgufenzy.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ogy.xylfe.cn

[Q75] 日期格式化
来源：http://jzz.jinghuilouyu.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://byz.xingfuxueyuan.xyz

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://iaz.tian-w.cn

[Q76] 按天统计
来源：http://nue.bjfxy.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://eav.vehdjk.com

[Q77] 时间加减
来源：http://vdd.c1oappe.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://tof.gogol.net.cn

[Q78] 当前时间
来源：http://bpw.xingfuxueyuan.xyz

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://iyk.zhengqikj.top

[Q79] 字符串拼接
来源：http://wnf.jinghuilouyu.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://uca.0kj1m.cn

[Q80] 字符串截取
来源：http://umg.cdnleiting.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://tsw.ehwqpu.com

[Q81] 字符串替换
来源：http://sso.mhx1999.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://tov.tianlin.xyz

[Q82] 字符长度与字节长度
来源：http://pry.nanxinkj.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://kdd.aibaodan.cn

[Q83] 大小写转换
来源：http://bix.shanyushiyangtech.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://olo.haohaochexian.top

[Q84] 去除首尾空格
来源：http://eti.nwbrower.top

SELECT TRIM(name) FROM users;
来源：http://ttl.jianghu66.top

[Q85] 数值取整
来源：http://mjo.jinqigufen.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hnk.aibaodan.cn

[Q86] 读取 JSON 字段
来源：http://sjp.xuetiantiany.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ptn.chenlongwang.top

[Q87] JSON 字段做条件
来源：http://ink.zycfv.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://gns.mhx1999.top

[Q88] 行转列（条件聚合）
来源：http://otb.9152youxi.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://qjm.yj20258888.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ewv.yueranfly.top

[Q89] 判断表是否存在
来源：http://hbo.dashuyun.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://nju.aizwys.cn

[Q90] 生成序号列
来源：http://atl.cheryme.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://dki.daria6918.cn

================================================================================
来源：http://zmu.gaohongyu789.top

R. Bash 专题
来源：http://vlu.c1oappe.top

================================================================================
来源：http://ldu.fengsongda.top

[R01] shebang 与严格模式
来源：http://lkr.yongpay.top

#!/usr/bin/env bash
来源：http://nbw.cdnleiting.top

set -euo pipefail
来源：http://rcf.xuetiantiany.cn

[R02] 变量赋值与使用
来源：http://aik.andypj.xyz

name="Tom"; echo "$name"
来源：http://zwc.fzhhl.top

[R03] 只读变量
来源：http://qkb.vqdsnc.cn

readonly PI=3.14
来源：http://uso.zhoulong.xyz

[R04] 位置参数
来源：http://sye.xinyue.icu

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://zuv.feifeiyinyue.top

[R05] 参数默认值
来源：http://aky.dianchejie.cn

name="${1:-default}"
来源：http://zky.hcnkem.com

[R06] 判断命令是否存在
来源：http://dhv.zhixingplan.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://vcx.cucudq.cn

[R07] if 判断文件
来源：http://nmb.nwbrower.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://rjq.cashguo.top

[R08] 数值比较
来源：http://ahn.sjlbkw.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://kua.daxiang520.top

[R09] 字符串比较
来源：http://zul.hcnkem.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://uog.jqgfzy.top

[R10] 正则匹配
来源：http://zjn.chenzaomai.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://vjp.fengsongda.top

[R11] case 多分支
来源：http://sow.cheryme.top

case "$1" in
来源：http://dik.sysykeji.top

start) echo "启动" ;;
来源：http://kdj.nwbrower.top

stop)  echo "停止" ;;
来源：http://zpz.zycfv.cn

*)     echo "未知命令" ;;
来源：http://xpc.fanxiaobao.xyz

esac
来源：http://lfn.cdnleiting.top

[R12] for 遍历文件
来源：http://jcy.gotoacloud.top

for f in *.txt; do echo "$f"; done
来源：http://bkf.fehbvm.com

[R13] for 计数循环
来源：http://tpg.jinghuilouyu.cn

for i in {1..10}; do echo "$i"; done
来源：http://zlb.nanxinkj.top

[R14] C 风格 for
来源：http://dgk.zdqjudy.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ktj.jqgfzy.top

[R15] while 逐行读文件
来源：http://rta.nanxinkj.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://cwz.guannengcc.top

[R16] until 等待条件
来源：http://sol.bbcook.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://xth.chenzaomai.com

[R17] 数组定义与取值
来源：http://mqk.haohaochexian.top

arr=(a b c); echo "${arr[0]}"
来源：http://mag.yongpay.top

[R18] 遍历数组
来源：http://ltr.daxiang520.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://xiq.sysykeji.top

[R19] 数组长度
来源：http://ssa.yuanzhike.top

echo "${#arr[@]}"
来源：http://ivm.yonumen.top

[R20] 关联数组（字典）
来源：http://ule.tanke756.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://fyz.andypj.xyz

[R21] 字符串长度
来源：http://nkg.jinyuanbaomall.cn

echo "${#s}"
来源：http://rpr.vehdjk.com

[R22] 截取子串
来源：http://kni.zhaomingkeji.xyz

echo "${s:0:5}"
来源：http://wdz.uphjek.com

[R23] 字符串替换
来源：http://xkd.sjlbkw.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ytm.ywan-chungtsiang.top

[R24] 大小写转换
来源：http://gqf.vehdjk.com

echo "${s^^}"; echo "${s,,}"
来源：http://tsz.wangshuangyany.cn

[R25] 去后缀 / 去前缀
来源：http://xhm.hcnkem.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://wlk.snrcjt.cn

[R26] 命令替换
来源：http://bcz.zhoulong.xyz

now=$(date +%F); echo "$now"
来源：http://rcf.wangdashe.top

[R27] 算术展开
来源：http://dgd.tarul.cn

echo $((1 + 2 * 3))
来源：http://hcu.epnwcf.com

[R28] 浮点运算
来源：http://vtz.redwolf501.top

echo "scale=2; 10/3" | bc
来源：http://eis.ydzc1.top

[R29] 定义函数
来源：http://asr.gaohongyu789.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://yew.jiagoushi.top

[R30] 函数返回状态码
来源：http://mwf.birdmap.top

f() { return 0; }; f || echo "失败了"
来源：http://vnq.tarul.cn

[R31] 局部变量
来源：http://ijx.gogol.net.cn

f() { local x=1; echo "$x"; }
来源：http://xwi.hnxiangtu.top

[R32] 参数个数校验
来源：http://fhp.zhiwuduotai.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://rza.shangyingyoupin.top

[R33] 捕获错误并提示行号
来源：http://kkk.hnqzz.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://dap.shangyingyoupin.top

[R34] 退出时清理
来源：http://pti.svipenyu.cn

trap 'rm -f "$tmp"' EXIT
来源：http://xji.52xcode.cn

[R35] 后台执行并等待
来源：http://tkq.dashuyun.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://upi.ybcxt.top

[R36] 并发执行多个任务
来源：http://hrv.yj20258888.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://jef.ywan-chungtsiang.top

[R37] 把输出赋给变量
来源：http://gfc.hnxiangtu.top

files=$(ls -1)
来源：http://wym.redwolf501.top

[R38] 管道串联
来源：http://jwl.dashuyun.cn

cat a.txt | grep -i error | wc -l
来源：http://inn.dianchejie.cn

[R39] 重定向标准输出与错误
来源：http://czf.shanyushiyangtech.top

cmd > out.log 2>&1
来源：http://nqv.jlsjyb.cn

[R40] 追加写日志
来源：http://lxn.hesvh.cn

echo "log" >> out.log
来源：http://gui.0kj1m.cn

[R41] 丢弃输出
来源：http://rlx.fengsongda.top

cmd >/dev/null 2>&1
来源：http://pgn.zhoulong.xyz

[R42] 输入重定向
来源：http://udq.shzxlz.cn

wc -l < a.txt
来源：http://opv.ywan-chungtsiang.top

[R43] 按名字查找文件
来源：http://cva.c1oappe.top

find . -name "*.log" -type f
来源：http://xnh.fanxiaobao.xyz

[R44] 按修改时间查找
来源：http://qhr.yuxming.cn

find . -mtime -7 -type f
来源：http://cte.guowangkeji.top

[R45] 批量删除
来源：http://mjt.yj202588.top

find . -name "*.tmp" -delete
来源：http://kpv.fzhhl.top

[R46] 递归替换文件内容
来源：http://hby.zhiwuduotai.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://smb.shanyushiyangtech.top

[R47] sed 单行替换
来源：http://ied.hcnkem.com

sed -i 's/foo/bar/g' a.txt
来源：http://ksz.zdqjudy.top

[R48] awk 取指定列
来源：http://jdt.tanke756.top

awk '{print $1, $3}' a.txt
来源：http://dfs.jyoumei.cn

[R49] awk 带条件
来源：http://wxi.redwolf501.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://dqy.shanyushiyangtech.top

[R50] awk 求和
来源：http://ttt.daria6918.cn

awk '{s += $2} END {print s}' a.txt
来源：http://uee.yuxming.cn

[R51] 排序去重取前几
来源：http://dzj.yuxming.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://pxp.hywenlv.cn

[R52] 统计行数
来源：http://owo.cucudq.cn

wc -l a.txt
来源：http://hlz.xinyue.icu

[R53] 查看文件头与实时尾
来源：http://qlg.meibo888.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://syh.cqqwz.cn

[R54] 比较两个文件
来源：http://lav.0kj1m.cn

diff a.txt b.txt
来源：http://azd.jlsjyb.cn

[R55] 压缩与解压
来源：http://blx.hysaishi.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://rzd.yj20258888.top

[R56] 远程拷贝
来源：http://jpy.epnwcf.com

scp file user@host:/path/
来源：http://zds.yongpay.top

[R57] 远程执行命令
来源：http://vac.xziqi.cn

ssh user@host 'uptime'
来源：http://rll.havefunace.top

[R58] 下载文件
来源：http://cqn.nwbrower.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://zci.hysaishi.cn

[R59] 发 POST JSON
来源：http://hwc.zhaomingkeji.xyz

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://nte.fengsongda.top

[R60] 只看 HTTP 状态码
来源：http://bav.cqqwz.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ddf.xylfe.cn

[R61] 磁盘占用
来源：http://luk.yfazqb.com

df -h;  du -sh *
来源：http://wac.hammf.cn

[R62] 找最占空间的文件
来源：http://tvr.sxryk.cn

du -ah . | sort -rh | head -10
来源：http://ifc.tian-w.cn

[R63] 内存与进程
来源：http://mmi.shuidangran.top

free -h;  ps aux | grep nginx
来源：http://egj.zycfv.cn

[R64] 结束进程
来源：http://tuy.andypj.xyz

kill -9 $(pgrep -f app.py)
来源：http://ngt.jianghu66.top

[R65] 查看端口占用
来源：http://ugr.xziqi.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://tir.yvedp.cn

[R66] 定时任务
来源：http://gbl.cdnleiting.top

crontab -e;  crontab -l
来源：http://efx.pycfn.com

[R67] 生成随机十六进制串
来源：http://fji.ppjwa.cn

openssl rand -hex 16
来源：http://tgj.gaohongyu789.top

[R68] 计算文件校验值
来源：http://bfb.iojbl.cn

sha256sum a.txt;  md5sum a.txt
来源：http://bkw.dianchejie.cn

[R69] 生成随机密码
来源：http://fie.hnxiangtu.top

head -c 16 /dev/urandom | base64
来源：http://iim.yangfankeji.com

[R70] 时间戳与互转
来源：http://eil.yj20258888.top

date +%s;  date -d @1700000000
来源：http://ccn.zhijiandao.cn

[R71] 日期格式化
来源：http://tcq.9152youxi.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://jtn.jinqigufen.top

[R72] 等待端口就绪
来源：http://xkv.yuxming.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://zoi.zhongyouzk.top

[R73] 分割大日志
来源：http://fin.yj202588.top

split -l 1000 big.log part_
来源：http://xwc.fktsv.cn

[R74] 批量重命名
来源：http://nmm.chenzaomai.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://cwr.jyoumei.cn

[R75] 导出环境变量
来源：http://off.cheryme.top

export PATH="$HOME/bin:$PATH"
来源：http://ywa.c1oappe.top

[R76] 使用临时文件
来源：http://vkx.chenjidiqi.icu

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wph.xinyue.icu

[R77] 读取用户输入
来源：http://bql.daxiang520.top


<!-- 参考信息 -->