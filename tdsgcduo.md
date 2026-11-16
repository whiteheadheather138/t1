代发 wailian999

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://xnc.dianchejie.cn

[Q28] 求和与平均
来源：http://zpt.snrcjt.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://xec.xingfuxueyuan.xyz

[Q29] 最大最小值
来源：http://jqg.jianghu66.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://coc.jinqigufen.top

[Q30] 分组统计
来源：http://jyj.ydzc1.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://zcv.ybcxt.top

[Q31] 分组后过滤
来源：http://jsp.hywenlv.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://zgv.svipenyu.cn

[Q32] 分组拼接字符串
来源：http://akq.gzhubu.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://yfr.redwolf501.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://trx.jinqigfzy.top

[Q33] 多列分组
来源：http://wfa.shzxlz.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ddf.yongpay.top

[Q34] 每组取第一条
来源：http://smi.shanyushiyangkeji.top

SELECT * FROM (
来源：http://ara.yj202588.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hca.jyoumei.cn

) t WHERE rn = 1;
来源：http://ony.ywan-chungtsiang.top

[Q35] 内连接
来源：http://vrq.cheryme.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hgt.zhoulong.xyz

[Q36] 左连接
来源：http://zes.yangfankeji.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://qrg.snrcjt.cn

[Q37] 右连接
来源：http://voe.gotoacloud.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://jgc.sysykeji.top

[Q38] 全外连接（PostgreSQL）
来源：http://gth.hongshengwenyu.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wqh.wangdashe.top

[Q39] 自连接（查上下级）
来源：http://jdg.uphjek.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://aco.ywan-chungtsiang.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ifh.zhaomingkeji.xyz

[Q40] 交叉连接（笛卡尔积）
来源：http://tog.jqgfzy.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://axq.jqgfzy.top

[Q41] 多表连接
来源：http://vxc.havefunace.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://bvu.fanxiaobao.xyz

JOIN users u ON u.id = o.user_id
来源：http://oyv.nanxuanxn.top

JOIN products p ON p.id = o.product_id;
来源：http://dri.yj20258888.top

[Q42] 连接条件附加过滤
来源：http://rju.pengpengdd.cyou

SELECT u.name, o.amount FROM users u
来源：http://qkk.xinyue.icu

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://rqa.chenjidiqi.icu

[Q43] 标量子查询
来源：http://czi.c1oappe.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://tkx.jinqigufen.top

[Q44] IN 子查询
来源：http://cop.hnqzz.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://rmr.feifeiyinyue.top

[Q45] EXISTS 判断存在
来源：http://quu.ppjwa.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://cmi.shanyushiyangkeji.top

[Q46] NOT EXISTS 判断不存在
来源：http://lxa.gaohongyu789.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://gzu.andypj.xyz

[Q47] 与平均值比较
来源：http://ncw.xinyue.icu

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://lqn.zhiwuduotai.top

[Q48] CTE 公用表表达式
来源：http://yln.jinghuilouyu.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://icc.iojbl.cn

SELECT * FROM t WHERE c > 5;
来源：http://lav.ppjwa.cn

[Q49] 更新单行
来源：http://qac.daria6918.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://enr.zhaomingkeji.xyz

[Q50] 批量更新
来源：http://duk.nwbrower.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://nqu.fanxiaobao.xyz

[Q51] 用子查询更新
来源：http://xyz.sysykeji.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ebg.zhaomingkeji.xyz

[Q52] 删除指定行
来源：http://wzp.hammf.cn

DELETE FROM users WHERE id = 10;
来源：http://hfy.cheryme.top

[Q53] 按条件删除
来源：http://ndi.ywan-chungtsiang.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ggq.xuetiantiany.cn

[Q54] 清空表
来源：http://lqv.52xcode.cn

TRUNCATE TABLE logs;
来源：http://lox.yfazqb.com

[Q55] 排名（并列占位）
来源：http://jwv.hnxiangtu.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://uxf.ywan-chungtsiang.top

[Q56] 密集排名（并列不占位）
来源：http://cfa.birdmap.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mbv.tianlin.xyz

[Q57] 行号
来源：http://aze.316326.xyz

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wmh.vehdjk.com

[Q58] 累计求和
来源：http://unr.jqgfzy.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://abl.zhoulong.xyz

[Q59] 分组内累计
来源：http://axs.uphjek.com

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://rqr.zhongyouzk.top

[Q60] 取上一行 / 下一行
来源：http://eik.smart0.xyz

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://oao.zhoulong.xyz

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://lfx.zhijiandao.cn

[Q61] 移动平均
来源：http://bnd.andypj.xyz

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://riu.shangyingyoupin.top

[Q62] 分组占比
来源：http://rij.cqqwz.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ocx.zhongyouzk.top

[Q63] 开启事务
来源：http://nqx.sxryk.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://awq.xziqi.cn

[Q64] 提交事务
来源：http://sqm.jiagoushi.top

COMMIT;
来源：http://bam.guannengcc.top

[Q65] 回滚事务
来源：http://evg.xinyue.icu

ROLLBACK;
来源：http://vja.gzhubu.top

[Q66] 行锁查询
来源：http://sna.yanxiufei.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://obm.ydzc1.top

[Q67] 设置隔离级别
来源：http://xoz.aibaodan.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://dym.hnqzz.top

[Q68] 保存点
来源：http://rkt.ppjwa.cn

SAVEPOINT sp1;
来源：http://bhm.zhaomingkeji.xyz

ROLLBACK TO sp1;
来源：http://bzx.kuanghao11.cn

[Q69] 查看执行计划
来源：http://lmc.yuxming.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://kev.gogol.net.cn

[Q70] 更新统计信息
来源：http://ldm.cashguo.top

ANALYZE TABLE users;
来源：http://hbt.guowangkeji.top

[Q71] 查看建表语句
来源：http://yjx.chenlongwang.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://yqz.jinqigfzy.top

[Q72] 查看索引
来源：http://yjm.birdmap.top

SHOW INDEX FROM users;
来源：http://uii.zhijiandao.cn

[Q73] 查看表状态
来源：http://rau.jinghuilouyu.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://eya.ppjwa.cn

[Q74] 强制使用索引
来源：http://mhg.sjlbkw.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mxk.fengsongda.top

[Q75] 日期格式化
来源：http://nph.9152youxi.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ynu.zdqjudy.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://old.pycfn.com

[Q76] 按天统计
来源：http://odz.wangdashe.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://sqt.gzhubu.top

[Q77] 时间加减
来源：http://zpp.hongshengwenyu.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://xyh.gzhubu.top

[Q78] 当前时间
来源：http://gat.tianlin.xyz

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ajn.haohaochexian.top

[Q79] 字符串拼接
来源：http://whm.ctjpmb.com

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ovc.ydjk.org.cn

[Q80] 字符串截取
来源：http://qfu.yueranfly.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://iqu.zhongyouzk.top

[Q81] 字符串替换
来源：http://atz.yanxiufei.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://lfd.fengsongda.top

[Q82] 字符长度与字节长度
来源：http://bmd.hesvh.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://xom.316326.xyz

[Q83] 大小写转换
来源：http://dqp.wangdashe.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mvi.uphjek.com

[Q84] 去除首尾空格
来源：http://uiz.sufxvd.cn

SELECT TRIM(name) FROM users;
来源：http://rtu.fzhhl.top

[Q85] 数值取整
来源：http://qyk.hnqzz.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://kok.316326.xyz

[Q86] 读取 JSON 字段
来源：http://gca.aizwys.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://vke.yj20258888.top

[Q87] JSON 字段做条件
来源：http://ffy.kuanghao11.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://vvo.hammf.cn

[Q88] 行转列（条件聚合）
来源：http://whh.guannengcc.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://glp.cashguo.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://tlg.xinyue.icu

[Q89] 判断表是否存在
来源：http://xzf.ctjpmb.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://xpq.dashuyun.cn

[Q90] 生成序号列
来源：http://uon.aizwys.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://sxu.chenjidiqi.icu

================================================================================
来源：http://mzm.hcnkem.com

R. Bash 专题
来源：http://ynp.smart0.xyz

================================================================================
来源：http://iwo.aibaodan.cn

[R01] shebang 与严格模式
来源：http://wnk.fktsv.cn

#!/usr/bin/env bash
来源：http://kru.daria6918.cn

set -euo pipefail
来源：http://dzf.jinqigufen.top

[R02] 变量赋值与使用
来源：http://tbe.52xcode.cn

name="Tom"; echo "$name"
来源：http://aaf.bjfxy.top

[R03] 只读变量
来源：http://fwe.fehbvm.com

readonly PI=3.14
来源：http://zyk.zhongyouzk.top

[R04] 位置参数
来源：http://ukd.fehbvm.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mct.birdmap.top

[R05] 参数默认值
来源：http://wrt.gaohongyu789.top

name="${1:-default}"
来源：http://ian.guannengcc.top

[R06] 判断命令是否存在
来源：http://ked.zhongyouzk.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ywx.zycfv.cn

[R07] if 判断文件
来源：http://zso.ybcxt.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://pgc.shanyushiyangtech.top

[R08] 数值比较
来源：http://iej.shanyushiyangtech.top

if (( a > b )); then echo "a 更大"; fi
来源：http://nrs.havefunace.top

[R09] 字符串比较
来源：http://mlf.ybcxt.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://cbi.fzhhl.top

[R10] 正则匹配
来源：http://qlm.shangyingyoupin.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://vmq.chenjidiqi.icu

[R11] case 多分支
来源：http://jcq.hnqzz.top

case "$1" in
来源：http://zzc.shuidangran.top

start) echo "启动" ;;
来源：http://uqo.yuanzhike.top

stop)  echo "停止" ;;
来源：http://whe.yueranfly.top

*)     echo "未知命令" ;;
来源：http://lgy.guannengcc.top

esac
来源：http://zcm.jqgfzy.top

[R12] for 遍历文件
来源：http://sgg.jinghuilouyu.cn

for f in *.txt; do echo "$f"; done
来源：http://ulu.gaohongyu789.top

[R13] for 计数循环
来源：http://pkz.ctjpmb.com

for i in {1..10}; do echo "$i"; done
来源：http://ksp.tian-w.cn

[R14] C 风格 for
来源：http://azf.guannengcc.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://bii.zhengqikj.top

[R15] while 逐行读文件
来源：http://hem.guowangkeji.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://gsd.ybcxt.top

[R16] until 等待条件
来源：http://fnv.cashguo.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://gwi.chenjidiqi.icu

[R17] 数组定义与取值
来源：http://mps.sweek.top

arr=(a b c); echo "${arr[0]}"
来源：http://bqj.bjfxy.top

[R18] 遍历数组
来源：http://dph.zhengqikj.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://fmi.zhiwuduotai.top

[R19] 数组长度
来源：http://lgn.gaohongyu789.top

echo "${#arr[@]}"
来源：http://wke.nanxuanxn.top

[R20] 关联数组（字典）
来源：http://rxh.aibaodan.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://xcr.sufxvd.cn

[R21] 字符串长度
来源：http://sxh.ctjpmb.com

echo "${#s}"
来源：http://zyp.zhaomingkeji.xyz

[R22] 截取子串
来源：http://ivu.dashuyun.cn

echo "${s:0:5}"
来源：http://wiz.chenlongwang.top

[R23] 字符串替换
来源：http://kul.hcnkem.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://bwc.ctjpmb.com

[R24] 大小写转换
来源：http://cfg.ppjwa.cn

echo "${s^^}"; echo "${s,,}"
来源：http://cys.zhengqikj.top

[R25] 去后缀 / 去前缀
来源：http://zar.andypj.xyz

echo "${f%.txt}"; echo "${f#./}"
来源：http://tkn.fanxiaobao.xyz

[R26] 命令替换
来源：http://fqf.nwbrower.top

now=$(date +%F); echo "$now"
来源：http://kil.0kj1m.cn

[R27] 算术展开
来源：http://xty.ydzc1.top

echo $((1 + 2 * 3))
来源：http://hgd.zhongyouzk.top

[R28] 浮点运算
来源：http://wks.hywenlv.cn

echo "scale=2; 10/3" | bc
来源：http://lav.cdnleiting.top

[R29] 定义函数
来源：http://ypm.yuxming.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://xcb.zycfv.cn

[R30] 函数返回状态码
来源：http://wiu.xuanzx.com

f() { return 0; }; f || echo "失败了"
来源：http://xxq.nanxuanxn.top

[R31] 局部变量
来源：http://qtc.tanke756.top

f() { local x=1; echo "$x"; }
来源：http://djw.pycfn.com

[R32] 参数个数校验
来源：http://xxj.daria6918.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hdm.redwolf501.top

[R33] 捕获错误并提示行号
来源：http://ksb.gzhubu.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://bik.ybcxt.top

[R34] 退出时清理
来源：http://ywh.cucudq.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ugr.havefunace.top

[R35] 后台执行并等待
来源：http://dmp.c1oappe.top

sleep 5 & pid=$!; wait "$pid"
来源：http://kos.hcnkem.com

[R36] 并发执行多个任务
来源：http://fqy.pengpengdd.cyou

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://fvs.zhijiandao.cn

[R37] 把输出赋给变量
来源：http://plj.gzhubu.top

files=$(ls -1)
来源：http://mpr.jianghu66.top

[R38] 管道串联
来源：http://skb.shanyushiyangkeji.top

cat a.txt | grep -i error | wc -l
来源：http://iog.zhiwuduotai.top

[R39] 重定向标准输出与错误
来源：http://gnb.redwolf501.top

cmd > out.log 2>&1
来源：http://oik.ybcxt.top

[R40] 追加写日志
来源：http://dqm.fehbvm.com

echo "log" >> out.log
来源：http://onh.jinqigfzy.top

[R41] 丢弃输出
来源：http://zys.yuxming.cn

cmd >/dev/null 2>&1
来源：http://kbo.sxryk.cn

[R42] 输入重定向
来源：http://liy.hongshengwenyu.top

wc -l < a.txt
来源：http://cat.fanxiaobao.xyz

[R43] 按名字查找文件
来源：http://zzn.shanyushiyangkeji.top

find . -name "*.log" -type f
来源：http://zap.dianchejie.cn

[R44] 按修改时间查找
来源：http://hkv.smart0.xyz

find . -mtime -7 -type f
来源：http://flk.gzhubu.top

[R45] 批量删除
来源：http://eye.epnwcf.com

find . -name "*.tmp" -delete
来源：http://pzp.hongshengwenyu.top

[R46] 递归替换文件内容
来源：http://ego.epnwcf.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://exz.fktsv.cn

[R47] sed 单行替换
来源：http://edw.yvedp.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ngc.andypj.xyz

[R48] awk 取指定列
来源：http://uze.vqdsnc.cn

awk '{print $1, $3}' a.txt
来源：http://kcy.gotoacloud.top

[R49] awk 带条件
来源：http://ubt.nwbrower.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://vex.guowangkeji.top

[R50] awk 求和
来源：http://uyg.smart0.xyz

awk '{s += $2} END {print s}' a.txt
来源：http://qdb.zhongyouzk.top

[R51] 排序去重取前几
来源：http://wqa.shanyushiyangkeji.top

sort a.txt | uniq -c | sort -rn | head
来源：http://cac.yj20258.top

[R52] 统计行数
来源：http://mmz.sxryk.cn

wc -l a.txt
来源：http://qmh.hfpthk.cn

[R53] 查看文件头与实时尾
来源：http://hsm.shanyushiyangkeji.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ydb.c1oappe.top

[R54] 比较两个文件
来源：http://lpv.c1oappe.top

diff a.txt b.txt
来源：http://rdd.wangdashe.top

[R55] 压缩与解压
来源：http://lfi.sysykeji.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://cgx.gotoacloud.top

[R56] 远程拷贝
来源：http://pug.fanxiaobao.xyz

scp file user@host:/path/
来源：http://phs.fanxiaobao.xyz

[R57] 远程执行命令
来源：http://dkn.zhoulong.xyz

ssh user@host 'uptime'
来源：http://wbp.gaohongyu789.top

[R58] 下载文件
来源：http://qkv.hfpthk.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://tbn.nanxuanxn.top

[R59] 发 POST JSON
来源：http://qec.xuanzx.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ubf.yj20258888.top

[R60] 只看 HTTP 状态码
来源：http://rww.pycfn.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://sxc.fehbvm.com

[R61] 磁盘占用
来源：http://zua.mhx1999.top

df -h;  du -sh *
来源：http://ybc.guannengcc.top

[R62] 找最占空间的文件
来源：http://nir.0kj1m.cn

du -ah . | sort -rh | head -10
来源：http://zdj.cheryme.top

[R63] 内存与进程
来源：http://uwu.hongshengwenyu.top

free -h;  ps aux | grep nginx
来源：http://iei.sysykeji.top

[R64] 结束进程
来源：http://uzd.tarul.cn

kill -9 $(pgrep -f app.py)
来源：http://alh.zhijiandao.cn

[R65] 查看端口占用
来源：http://owx.sweek.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://vuk.yj20258.top

[R66] 定时任务
来源：http://vbi.ydzc1.top

crontab -e;  crontab -l
来源：http://hyd.fehbvm.com

[R67] 生成随机十六进制串
来源：http://leb.ydzc1.top

openssl rand -hex 16
来源：http://vci.jiagoushi.top

[R68] 计算文件校验值
来源：http://ros.iojbl.cn

sha256sum a.txt;  md5sum a.txt
来源：http://gwr.yongpay.top

[R69] 生成随机密码
来源：http://lqp.feifeiyinyue.top

head -c 16 /dev/urandom | base64
来源：http://wou.hcnkem.com

[R70] 时间戳与互转
来源：http://gac.jiagoushi.top

date +%s;  date -d @1700000000
来源：http://nfo.uphjek.com

[R71] 日期格式化
来源：http://yfm.feifeiyinyue.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://irc.shangyingyoupin.top

[R72] 等待端口就绪
来源：http://btu.gzhubu.top

until nc -z localhost 3306; do sleep 1; done
来源：http://vma.ehwqpu.com

[R73] 分割大日志
来源：http://swq.zhongyouzk.top

split -l 1000 big.log part_
来源：http://tmk.hammf.cn

[R74] 批量重命名
来源：http://dxn.dianchejie.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://nbs.xinyue.icu

[R75] 导出环境变量
来源：http://lnc.zhengqikj.top

export PATH="$HOME/bin:$PATH"
来源：http://uxn.shuidangran.top

[R76] 使用临时文件
来源：http://mup.tianlin.xyz

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://drz.shzxlz.cn

[R77] 读取用户输入
来源：http://eka.jyoumei.cn


<!-- 参考信息 -->