代发 wailian999

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://zdd.sufxvd.cn

[Q32] 分组拼接字符串
来源：http://zlz.daxiang520.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://xdw.shanyushiyangtech.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://vbs.yanxiufei.cn

[Q33] 多列分组
来源：http://quo.hnqzz.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://emj.jinqigfzy.top

[Q34] 每组取第一条
来源：http://ezr.vehdjk.com

SELECT * FROM (
来源：http://igm.hnxiangtu.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://sbl.aizwys.cn

) t WHERE rn = 1;
来源：http://zpt.ydjk.org.cn

[Q35] 内连接
来源：http://uig.shzxlz.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://nmi.yj202588.top

[Q36] 左连接
来源：http://orq.hysaishi.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ool.snrcjt.cn

[Q37] 右连接
来源：http://vsp.xingfuxueyuan.xyz

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://pyg.nanxuanxn.top

[Q38] 全外连接（PostgreSQL）
来源：http://sjy.kuanghao11.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wsb.xuanzx.com

[Q39] 自连接（查上下级）
来源：http://esg.hammf.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ann.zdqjudy.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://bfq.xingfuxueyuan.xyz

[Q40] 交叉连接（笛卡尔积）
来源：http://npw.cqqwz.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://raa.hongshengwenyu.top

[Q41] 多表连接
来源：http://vov.yj202588.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://bxq.hysaishi.cn

JOIN users u ON u.id = o.user_id
来源：http://sko.jinyuanbaomall.cn

JOIN products p ON p.id = o.product_id;
来源：http://qug.chenjidiqi.icu

[Q42] 连接条件附加过滤
来源：http://rud.bjfxy.top

SELECT u.name, o.amount FROM users u
来源：http://tui.guowangkeji.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://rml.haohaochexian.top

[Q43] 标量子查询
来源：http://vyx.zdqjudy.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://fzz.shanyushiyangkeji.top

[Q44] IN 子查询
来源：http://mka.jinqigfzy.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://cii.mhx1999.top

[Q45] EXISTS 判断存在
来源：http://xwv.daxiang520.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vsv.zycfv.cn

[Q46] NOT EXISTS 判断不存在
来源：http://dmh.xuanzx.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://dlv.snrcjt.cn

[Q47] 与平均值比较
来源：http://hnt.zhiwuduotai.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://tsl.c1oappe.top

[Q48] CTE 公用表表达式
来源：http://hdw.smart0.xyz

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://uoi.jqgufenzy.top

SELECT * FROM t WHERE c > 5;
来源：http://xtj.jqgfzy.top

[Q49] 更新单行
来源：http://jkt.hammf.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://egj.yangfankeji.com

[Q50] 批量更新
来源：http://plf.ppjwa.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://urz.aibaodan.cn

[Q51] 用子查询更新
来源：http://dnm.aibaodan.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://fvu.yonumen.top

[Q52] 删除指定行
来源：http://yso.yuxming.cn

DELETE FROM users WHERE id = 10;
来源：http://gwq.jlsjyb.cn

[Q53] 按条件删除
来源：http://yjn.yueranfly.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ecz.jianghu66.top

[Q54] 清空表
来源：http://baj.316326.xyz

TRUNCATE TABLE logs;
来源：http://thp.ydzc1.top

[Q55] 排名（并列占位）
来源：http://ewd.tian-w.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://zfj.wangdashe.top

[Q56] 密集排名（并列不占位）
来源：http://mny.jinyuanbaomall.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://sqf.ivvv.top

[Q57] 行号
来源：http://tys.zhijiandao.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ahy.pycfn.com

[Q58] 累计求和
来源：http://aeh.ydjk.org.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://oor.jianghu66.top

[Q59] 分组内累计
来源：http://rtx.chenjidiqi.icu

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://fwv.zhengqikj.top

[Q60] 取上一行 / 下一行
来源：http://pou.zhoulong.xyz

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://oqb.sweek.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://lva.yfazqb.com

[Q61] 移动平均
来源：http://sij.xuanzx.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mkv.zhiwuduotai.top

[Q62] 分组占比
来源：http://yqr.bbcook.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://kgo.iojbl.cn

[Q63] 开启事务
来源：http://euy.shzxlz.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://srk.jinqigufen.top

[Q64] 提交事务
来源：http://dqq.fktsv.cn

COMMIT;
来源：http://bem.xuanzx.com

[Q65] 回滚事务
来源：http://ofa.hammf.cn

ROLLBACK;
来源：http://vno.bbcook.cn

[Q66] 行锁查询
来源：http://nlm.ybcxt.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://enn.shanyushiyangtech.top

[Q67] 设置隔离级别
来源：http://rio.yangfankeji.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://elt.cashguo.top

[Q68] 保存点
来源：http://ksi.zhoulong.xyz

SAVEPOINT sp1;
来源：http://ipf.hfpthk.cn

ROLLBACK TO sp1;
来源：http://ifo.tanke756.top

[Q69] 查看执行计划
来源：http://jes.jlsjyb.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://glg.xinyue.icu

[Q70] 更新统计信息
来源：http://rzn.cqqwz.cn

ANALYZE TABLE users;
来源：http://srp.pycfn.com

[Q71] 查看建表语句
来源：http://ajb.yfazqb.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://gst.ywan-chungtsiang.top

[Q72] 查看索引
来源：http://tyf.zdqjudy.top

SHOW INDEX FROM users;
来源：http://vci.zycfv.cn

[Q73] 查看表状态
来源：http://ifw.daria6918.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://utd.yj20258.top

[Q74] 强制使用索引
来源：http://syr.nanxuanxn.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://fpi.ppjwa.cn

[Q75] 日期格式化
来源：http://kzh.andypj.xyz

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://grh.zycfv.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://het.yangfankeji.com

[Q76] 按天统计
来源：http://kaw.chenlongwang.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://vuu.mhx1999.top

[Q77] 时间加减
来源：http://ncr.birdmap.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hba.chenjidiqi.icu

[Q78] 当前时间
来源：http://mnp.hnqzz.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://agg.xuetiantiany.cn

[Q79] 字符串拼接
来源：http://agg.tanke756.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ocu.bbcook.cn

[Q80] 字符串截取
来源：http://lry.52xcode.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://pqv.jinqigufen.top

[Q81] 字符串替换
来源：http://ajv.zhixingplan.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://jkl.cheryme.top

[Q82] 字符长度与字节长度
来源：http://mng.shuidangran.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mct.sysykeji.top

[Q83] 大小写转换
来源：http://nfz.redwolf501.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://aeh.shanyushiyangtech.top

[Q84] 去除首尾空格
来源：http://vhz.nanxuanxn.top

SELECT TRIM(name) FROM users;
来源：http://tby.iojbl.cn

[Q85] 数值取整
来源：http://cdu.jqgufenzy.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://tdw.ydzc1.top

[Q86] 读取 JSON 字段
来源：http://gsk.snrcjt.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://owj.zhaomingkeji.xyz

[Q87] JSON 字段做条件
来源：http://hbo.guannengcc.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://pyt.zhijiandao.cn

[Q88] 行转列（条件聚合）
来源：http://psi.nwbrower.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://lfa.nanxuanxn.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://epn.chenjidiqi.icu

[Q89] 判断表是否存在
来源：http://muc.iojbl.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://fth.shanyushiyangtech.top

[Q90] 生成序号列
来源：http://iiz.shzxlz.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://qrl.fehbvm.com

================================================================================
来源：http://tkk.yvedp.cn

R. Bash 专题
来源：http://szn.pengpengdd.cyou

================================================================================
来源：http://vgh.ehwqpu.com

[R01] shebang 与严格模式
来源：http://sef.chenjidiqi.icu

#!/usr/bin/env bash
来源：http://kna.wangdashe.top

set -euo pipefail
来源：http://clp.guannengcc.top

[R02] 变量赋值与使用
来源：http://gyg.zycfv.cn

name="Tom"; echo "$name"
来源：http://pqg.gaohongyu789.top

[R03] 只读变量
来源：http://czq.gzhubu.top

readonly PI=3.14
来源：http://bwu.316326.xyz

[R04] 位置参数
来源：http://pjq.yongpay.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://kzf.xinyue.icu

[R05] 参数默认值
来源：http://tte.nwbrower.top

name="${1:-default}"
来源：http://oxr.yanxiufei.cn

[R06] 判断命令是否存在
来源：http://zha.yongpay.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wnt.zdqjudy.top

[R07] if 判断文件
来源：http://nib.nanxuanxn.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://npy.hcnkem.com

[R08] 数值比较
来源：http://cmc.jinghuilouyu.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://qhk.hysaishi.cn

[R09] 字符串比较
来源：http://zll.jinyuanbaomall.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://vgs.yongpay.top

[R10] 正则匹配
来源：http://sbx.tianlin.xyz

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://vak.xingfuxueyuan.xyz

[R11] case 多分支
来源：http://bxf.0kj1m.cn

case "$1" in
来源：http://hro.yj20258888.top

start) echo "启动" ;;
来源：http://bwn.gotoacloud.top

stop)  echo "停止" ;;
来源：http://bup.fehbvm.com

*)     echo "未知命令" ;;
来源：http://pdx.zhoulong.xyz

esac
来源：http://gbm.yueranfly.top

[R12] for 遍历文件
来源：http://qyz.yanxiufei.cn

for f in *.txt; do echo "$f"; done
来源：http://auc.gogol.net.cn

[R13] for 计数循环
来源：http://dxs.cqqwz.cn

for i in {1..10}; do echo "$i"; done
来源：http://ngt.bbcook.cn

[R14] C 风格 for
来源：http://xdx.andypj.xyz

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ifp.gogol.net.cn

[R15] while 逐行读文件
来源：http://hpc.ybcxt.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://eme.zhengqikj.top

[R16] until 等待条件
来源：http://whi.hammf.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mcj.hcnkem.com

[R17] 数组定义与取值
来源：http://ehg.zdbjq.cn

arr=(a b c); echo "${arr[0]}"
来源：http://zyx.jinghuilouyu.cn

[R18] 遍历数组
来源：http://xtj.daxiang520.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://vmq.gaohongyu789.top

[R19] 数组长度
来源：http://jvt.xziqi.cn

echo "${#arr[@]}"
来源：http://mjs.zdqjudy.top

[R20] 关联数组（字典）
来源：http://yds.hnqzz.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://vof.hcnkem.com

[R21] 字符串长度
来源：http://sbz.meibo888.top

echo "${#s}"
来源：http://foe.jyoumei.cn

[R22] 截取子串
来源：http://kvn.tarul.cn

echo "${s:0:5}"
来源：http://cke.chenlongwang.top

[R23] 字符串替换
来源：http://sfw.daxiang520.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://tsw.hnqzz.top

[R24] 大小写转换
来源：http://fon.meibo888.top

echo "${s^^}"; echo "${s,,}"
来源：http://flt.zhongyouzk.top

[R25] 去后缀 / 去前缀
来源：http://oes.yueranfly.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://vow.chenzaomai.com

[R26] 命令替换
来源：http://ofg.guowangkeji.top

now=$(date +%F); echo "$now"
来源：http://wqm.hammf.cn

[R27] 算术展开
来源：http://ncv.dashuyun.cn

echo $((1 + 2 * 3))
来源：http://gfx.meibo888.top

[R28] 浮点运算
来源：http://cqf.yueranfly.top

echo "scale=2; 10/3" | bc
来源：http://cjz.xuetiantiany.cn

[R29] 定义函数
来源：http://lhp.shzxlz.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://gct.guowangkeji.top

[R30] 函数返回状态码
来源：http://qsb.cucudq.cn

f() { return 0; }; f || echo "失败了"
来源：http://gvc.tianlin.xyz

[R31] 局部变量
来源：http://qms.yonumen.top

f() { local x=1; echo "$x"; }
来源：http://ddw.zhijiandao.cn

[R32] 参数个数校验
来源：http://jbm.zycfv.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://zsu.dashuyun.cn

[R33] 捕获错误并提示行号
来源：http://tjg.shzxlz.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://esq.tanke756.top

[R34] 退出时清理
来源：http://yzy.sysykeji.top

trap 'rm -f "$tmp"' EXIT
来源：http://ilo.sjlbkw.cn

[R35] 后台执行并等待
来源：http://ooq.yongpay.top

sleep 5 & pid=$!; wait "$pid"
来源：http://wzu.zycfv.cn

[R36] 并发执行多个任务
来源：http://mnt.hongshengwenyu.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://yvw.zhengqikj.top

[R37] 把输出赋给变量
来源：http://nsn.shangyingyoupin.top

files=$(ls -1)
来源：http://xkc.chenzaomai.com

[R38] 管道串联
来源：http://cow.guannengcc.top

cat a.txt | grep -i error | wc -l
来源：http://vcw.nanxuanxn.top

[R39] 重定向标准输出与错误
来源：http://vup.jianghu66.top

cmd > out.log 2>&1
来源：http://kpn.yanxiufei.cn

[R40] 追加写日志
来源：http://yob.sufxvd.cn

echo "log" >> out.log
来源：http://uxw.feifeiyinyue.top

[R41] 丢弃输出
来源：http://yhs.zhaomingkeji.xyz

cmd >/dev/null 2>&1
来源：http://xsl.wangdashe.top

[R42] 输入重定向
来源：http://wwk.wangdashe.top

wc -l < a.txt
来源：http://mnh.yangfankeji.com

[R43] 按名字查找文件
来源：http://sfm.ppjwa.cn

find . -name "*.log" -type f
来源：http://owd.hammf.cn

[R44] 按修改时间查找
来源：http://ijr.tanke756.top

find . -mtime -7 -type f
来源：http://wvh.zhixingplan.top

[R45] 批量删除
来源：http://wbb.jianghu66.top

find . -name "*.tmp" -delete
来源：http://ljg.yangfankeji.com

[R46] 递归替换文件内容
来源：http://xqp.meibo888.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://zeb.svipenyu.cn

[R47] sed 单行替换
来源：http://gtp.gaohongyu789.top

sed -i 's/foo/bar/g' a.txt
来源：http://mgv.gotoacloud.top

[R48] awk 取指定列
来源：http://aql.pengpengdd.cyou

awk '{print $1, $3}' a.txt
来源：http://pxc.quarkkingdee.top

[R49] awk 带条件
来源：http://xil.nanxinkj.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://otx.epnwcf.com

[R50] awk 求和
来源：http://apl.yangfankeji.com

awk '{s += $2} END {print s}' a.txt
来源：http://dsl.cashguo.top

[R51] 排序去重取前几
来源：http://hss.ivvv.top

sort a.txt | uniq -c | sort -rn | head
来源：http://kqx.fzhhl.top

[R52] 统计行数
来源：http://xvo.316326.xyz

wc -l a.txt
来源：http://sqw.wangdashe.top

[R53] 查看文件头与实时尾
来源：http://rcq.gzhubu.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://djd.gogol.net.cn

[R54] 比较两个文件
来源：http://dug.sweek.top

diff a.txt b.txt
来源：http://gdu.dianchejie.cn

[R55] 压缩与解压
来源：http://sdu.shangyingyoupin.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://pbn.sweek.top

[R56] 远程拷贝
来源：http://tim.316326.xyz

scp file user@host:/path/
来源：http://jqb.zhixingplan.top

[R57] 远程执行命令
来源：http://tsj.sxryk.cn

ssh user@host 'uptime'
来源：http://hof.jlsjyb.cn

[R58] 下载文件
来源：http://kmw.xinyue.icu

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hbi.daxiang520.top

[R59] 发 POST JSON
来源：http://teb.jinghuilouyu.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ahp.hesvh.cn

[R60] 只看 HTTP 状态码
来源：http://qym.shuidangran.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://odd.haohaochexian.top

[R61] 磁盘占用
来源：http://ilq.jyoumei.cn

df -h;  du -sh *
来源：http://waa.jianghu66.top

[R62] 找最占空间的文件
来源：http://plz.hesvh.cn

du -ah . | sort -rh | head -10
来源：http://ujl.tianlin.xyz

[R63] 内存与进程
来源：http://lge.zdbjq.cn

free -h;  ps aux | grep nginx
来源：http://bto.xingfuxueyuan.xyz

[R64] 结束进程
来源：http://ukq.gogol.net.cn

kill -9 $(pgrep -f app.py)
来源：http://pll.cheryme.top

[R65] 查看端口占用
来源：http://ezs.pycfn.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wlx.sufxvd.cn

[R66] 定时任务
来源：http://dnf.yanxiufei.cn

crontab -e;  crontab -l
来源：http://vec.0kj1m.cn

[R67] 生成随机十六进制串
来源：http://heo.vqdsnc.cn

openssl rand -hex 16
来源：http://rwm.epnwcf.com

[R68] 计算文件校验值
来源：http://kte.zdbjq.cn

sha256sum a.txt;  md5sum a.txt
来源：http://vvh.gaohongyu789.top

[R69] 生成随机密码
来源：http://fuo.fktsv.cn

head -c 16 /dev/urandom | base64
来源：http://lae.fktsv.cn

[R70] 时间戳与互转
来源：http://zdx.jqgufenzy.top

date +%s;  date -d @1700000000
来源：http://lms.xinyue.icu

[R71] 日期格式化
来源：http://kyp.fehbvm.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://fbt.zhijiandao.cn

[R72] 等待端口就绪
来源：http://aev.epnwcf.com

until nc -z localhost 3306; do sleep 1; done
来源：http://bzn.tarul.cn

[R73] 分割大日志
来源：http://jlv.daria6918.cn

split -l 1000 big.log part_
来源：http://njg.ctjpmb.com

[R74] 批量重命名
来源：http://taq.hfpthk.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://etn.xuanzx.com

[R75] 导出环境变量
来源：http://pzs.ppjwa.cn

export PATH="$HOME/bin:$PATH"
来源：http://tuj.gogol.net.cn

[R76] 使用临时文件
来源：http://odl.aizwys.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://jms.yonumen.top

[R77] 读取用户输入
来源：http://hiq.zhijiandao.cn

read -rp "请输入: " ans
来源：http://tou.yuxming.cn

[R78] 交互式菜单
来源：http://gup.bjfxy.top

select opt in a b c; do echo "$opt"; break; done
来源：http://gyg.bbcook.cn

[R79] 解析命令行选项
来源：http://znu.kuanghao11.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hnu.ydzc1.top

[R80] 查看脚本执行耗时
来源：http://hzm.shangyingyoupin.top

time ./run.sh
来源：http://cib.aibaodan.cn

================================================================================
来源：http://bjr.yanxiufei.cn


<!-- 参考信息 -->