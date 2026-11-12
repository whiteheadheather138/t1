代发 wailian999

SELECT MAX(age), MIN(age) FROM users;
来源：http://jkj.quarkkingdee.top

[Q30] 分组统计
来源：http://zhe.hfpthk.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://bhc.hnqzz.top

[Q31] 分组后过滤
来源：http://ryh.hammf.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wyu.nanxinkj.top

[Q32] 分组拼接字符串
来源：http://mmr.zhoulong.xyz

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://klu.ybcxt.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ial.ivvv.top

[Q33] 多列分组
来源：http://twb.guannengcc.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://dfm.jiagoushi.top

[Q34] 每组取第一条
来源：http://sqb.chenlongwang.top

SELECT * FROM (
来源：http://nxq.nanxinkj.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hqk.fktsv.cn

) t WHERE rn = 1;
来源：http://vrn.fehbvm.com

[Q35] 内连接
来源：http://tfg.ehwqpu.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ndb.jqgufenzy.top

[Q36] 左连接
来源：http://dfa.c1oappe.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://xku.uphjek.com

[Q37] 右连接
来源：http://dyl.xziqi.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://eco.dashuyun.cn

[Q38] 全外连接（PostgreSQL）
来源：http://npn.jinghuilouyu.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wij.gotoacloud.top

[Q39] 自连接（查上下级）
来源：http://bap.bbcook.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://emd.fehbvm.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://lch.zhoulong.xyz

[Q40] 交叉连接（笛卡尔积）
来源：http://pux.fanxiaobao.xyz

SELECT * FROM colors CROSS JOIN sizes;
来源：http://zek.hongshengwenyu.top

[Q41] 多表连接
来源：http://ozr.cheryme.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://omb.vqdsnc.cn

JOIN users u ON u.id = o.user_id
来源：http://ucn.chenlongwang.top

JOIN products p ON p.id = o.product_id;
来源：http://yjw.tianlin.xyz

[Q42] 连接条件附加过滤
来源：http://tlx.c1oappe.top

SELECT u.name, o.amount FROM users u
来源：http://nky.jinqigufen.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://olm.uphjek.com

[Q43] 标量子查询
来源：http://czg.chenjidiqi.icu

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://nnd.shanyushiyangtech.top

[Q44] IN 子查询
来源：http://dtn.kuanghao11.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://fxj.zhijiandao.cn

[Q45] EXISTS 判断存在
来源：http://ywo.chenzaomai.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://afg.cucudq.cn

[Q46] NOT EXISTS 判断不存在
来源：http://uyw.zdbjq.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://sfe.yangfankeji.com

[Q47] 与平均值比较
来源：http://nle.zhiwuduotai.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://sfv.shzxlz.cn

[Q48] CTE 公用表表达式
来源：http://qxe.fanxiaobao.xyz

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://pjw.daria6918.cn

SELECT * FROM t WHERE c > 5;
来源：http://agq.jyoumei.cn

[Q49] 更新单行
来源：http://qxg.xinyue.icu

UPDATE users SET status = 1 WHERE id = 10;
来源：http://zeg.nwbrower.top

[Q50] 批量更新
来源：http://gvk.cqqwz.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://jpz.tian-w.cn

[Q51] 用子查询更新
来源：http://deo.gzhubu.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://qin.hysaishi.cn

[Q52] 删除指定行
来源：http://myk.vehdjk.com

DELETE FROM users WHERE id = 10;
来源：http://jvq.svipenyu.cn

[Q53] 按条件删除
来源：http://tfd.smart0.xyz

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wcr.wangdashe.top

[Q54] 清空表
来源：http://rbz.zdqjudy.top

TRUNCATE TABLE logs;
来源：http://opi.hcnkem.com

[Q55] 排名（并列占位）
来源：http://gau.fzhhl.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://okd.ydjk.org.cn

[Q56] 密集排名（并列不占位）
来源：http://kvu.jiagoushi.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ybv.hfpthk.cn

[Q57] 行号
来源：http://yht.daria6918.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://cgd.yuxming.cn

[Q58] 累计求和
来源：http://eye.gogol.net.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ihv.uphjek.com

[Q59] 分组内累计
来源：http://jvh.meibo888.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://cgi.fzhhl.top

[Q60] 取上一行 / 下一行
来源：http://mxm.ywan-chungtsiang.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://efh.epnwcf.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://jzk.zhengqikj.top

[Q61] 移动平均
来源：http://lcs.zhixingplan.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://rsj.xinyue.icu

[Q62] 分组占比
来源：http://izc.xziqi.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wtl.yfazqb.com

[Q63] 开启事务
来源：http://xvc.yj20258.top

START TRANSACTION;                -- 或 BEGIN
来源：http://xeg.dashuyun.cn

[Q64] 提交事务
来源：http://nzd.shangyingyoupin.top

COMMIT;
来源：http://xws.jinghuilouyu.cn

[Q65] 回滚事务
来源：http://fhm.aibaodan.cn

ROLLBACK;
来源：http://iei.ydzc1.top

[Q66] 行锁查询
来源：http://fov.hnqzz.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://isx.jqgufenzy.top

[Q67] 设置隔离级别
来源：http://svk.dianchejie.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://uqk.shzxlz.cn

[Q68] 保存点
来源：http://feo.gzhubu.top

SAVEPOINT sp1;
来源：http://unl.jqgfzy.top

ROLLBACK TO sp1;
来源：http://vhg.pycfn.com

[Q69] 查看执行计划
来源：http://iwu.fktsv.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://qgd.hesvh.cn

[Q70] 更新统计信息
来源：http://wsj.xinyue.icu

ANALYZE TABLE users;
来源：http://mkh.xinyue.icu

[Q71] 查看建表语句
来源：http://hdf.gogol.net.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hgu.aibaodan.cn

[Q72] 查看索引
来源：http://mtc.sxryk.cn

SHOW INDEX FROM users;
来源：http://urv.pengpengdd.cyou

[Q73] 查看表状态
来源：http://bll.jyoumei.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://sxa.quarkkingdee.top

[Q74] 强制使用索引
来源：http://jvb.zhaomingkeji.xyz

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ehu.hnxiangtu.top

[Q75] 日期格式化
来源：http://zbn.jqgufenzy.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://bdg.xinyue.icu

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://pbh.wangdashe.top

[Q76] 按天统计
来源：http://vvk.gzhubu.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://nra.zycfv.cn

[Q77] 时间加减
来源：http://qfe.aibaodan.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://kkb.shanyushiyangtech.top

[Q78] 当前时间
来源：http://dar.sxryk.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wtw.xinyue.icu

[Q79] 字符串拼接
来源：http://ngn.dianchejie.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://dug.zycfv.cn

[Q80] 字符串截取
来源：http://nmv.jianghu66.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hoi.hnxiangtu.top

[Q81] 字符串替换
来源：http://lve.iojbl.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://vjp.kuanghao11.cn

[Q82] 字符长度与字节长度
来源：http://ygo.aizwys.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://fdb.chenzaomai.com

[Q83] 大小写转换
来源：http://rco.aibaodan.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hyc.xziqi.cn

[Q84] 去除首尾空格
来源：http://yck.bjfxy.top

SELECT TRIM(name) FROM users;
来源：http://kmr.uphjek.com

[Q85] 数值取整
来源：http://bot.yangfankeji.com

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://yrb.jqgufenzy.top

[Q86] 读取 JSON 字段
来源：http://sqs.zhongyouzk.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://vmm.ydjk.org.cn

[Q87] JSON 字段做条件
来源：http://wjj.jlsjyb.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://cqs.quarkkingdee.top

[Q88] 行转列（条件聚合）
来源：http://xtz.smart0.xyz

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://pah.chenjidiqi.icu

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wkv.0kj1m.cn

[Q89] 判断表是否存在
来源：http://msu.tianlin.xyz

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hau.epnwcf.com

[Q90] 生成序号列
来源：http://cqo.smart0.xyz

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://sga.ybcxt.top

================================================================================
来源：http://ahf.aizwys.cn

R. Bash 专题
来源：http://msv.xziqi.cn

================================================================================
来源：http://jaj.zhixingplan.top

[R01] shebang 与严格模式
来源：http://wfh.cdnleiting.top

#!/usr/bin/env bash
来源：http://djv.snrcjt.cn

set -euo pipefail
来源：http://snv.52xcode.cn

[R02] 变量赋值与使用
来源：http://qto.gotoacloud.top

name="Tom"; echo "$name"
来源：http://hjy.gogol.net.cn

[R03] 只读变量
来源：http://van.hysaishi.cn

readonly PI=3.14
来源：http://wzu.yuanzhike.top

[R04] 位置参数
来源：http://dhj.0kj1m.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wlw.cheryme.top

[R05] 参数默认值
来源：http://wws.hfpthk.cn

name="${1:-default}"
来源：http://osg.xingfuxueyuan.xyz

[R06] 判断命令是否存在
来源：http://pkv.shanyushiyangtech.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://odx.bjfxy.top

[R07] if 判断文件
来源：http://tvf.shuidangran.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://cgb.52xcode.cn

[R08] 数值比较
来源：http://wrn.sjlbkw.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://nkg.chenjidiqi.icu

[R09] 字符串比较
来源：http://onj.shuidangran.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://lrx.cqqwz.cn

[R10] 正则匹配
来源：http://srk.c1oappe.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://cff.birdmap.top

[R11] case 多分支
来源：http://puj.shanyushiyangkeji.top

case "$1" in
来源：http://plv.tianlin.xyz

start) echo "启动" ;;
来源：http://ygw.jiagoushi.top

stop)  echo "停止" ;;
来源：http://jrv.hongshengwenyu.top

*)     echo "未知命令" ;;
来源：http://saf.ydzc1.top

esac
来源：http://zxk.bbcook.cn

[R12] for 遍历文件
来源：http://eqg.jinghuilouyu.cn

for f in *.txt; do echo "$f"; done
来源：http://ldr.yongpay.top

[R13] for 计数循环
来源：http://dvt.hnxiangtu.top

for i in {1..10}; do echo "$i"; done
来源：http://khh.fehbvm.com

[R14] C 风格 for
来源：http://saz.tianlin.xyz

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ldp.guannengcc.top

[R15] while 逐行读文件
来源：http://ujt.xuetiantiany.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://pwr.hcnkem.com

[R16] until 等待条件
来源：http://oea.snrcjt.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://cns.shanyushiyangkeji.top

[R17] 数组定义与取值
来源：http://tfc.zhoulong.xyz

arr=(a b c); echo "${arr[0]}"
来源：http://xoi.fktsv.cn

[R18] 遍历数组
来源：http://lso.dashuyun.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://vtr.0kj1m.cn

[R19] 数组长度
来源：http://ixm.316326.xyz

echo "${#arr[@]}"
来源：http://pwh.gotoacloud.top

[R20] 关联数组（字典）
来源：http://yzn.mhx1999.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ywi.zdbjq.cn

[R21] 字符串长度
来源：http://smg.bbcook.cn

echo "${#s}"
来源：http://fwx.hnqzz.top

[R22] 截取子串
来源：http://kmi.tanke756.top

echo "${s:0:5}"
来源：http://ygm.jlsjyb.cn

[R23] 字符串替换
来源：http://hhl.52xcode.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://tcn.yj20258.top

[R24] 大小写转换
来源：http://tcu.jinqigfzy.top

echo "${s^^}"; echo "${s,,}"
来源：http://nye.ywan-chungtsiang.top

[R25] 去后缀 / 去前缀
来源：http://nhk.hfpthk.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://orf.0kj1m.cn

[R26] 命令替换
来源：http://gyv.quarkkingdee.top

now=$(date +%F); echo "$now"
来源：http://wie.cheryme.top

[R27] 算术展开
来源：http://lnx.jqgfzy.top

echo $((1 + 2 * 3))
来源：http://khd.nwbrower.top

[R28] 浮点运算
来源：http://qbj.yj202588.top

echo "scale=2; 10/3" | bc
来源：http://tvx.daxiang520.top

[R29] 定义函数
来源：http://dhw.52xcode.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://whu.yuanzhike.top

[R30] 函数返回状态码
来源：http://wgt.jiagoushi.top

f() { return 0; }; f || echo "失败了"
来源：http://xim.xziqi.cn

[R31] 局部变量
来源：http://bkg.pengpengdd.cyou

f() { local x=1; echo "$x"; }
来源：http://uvm.bbcook.cn

[R32] 参数个数校验
来源：http://fha.bjfxy.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://lvv.hywenlv.cn

[R33] 捕获错误并提示行号
来源：http://ega.zdbjq.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hhz.chenjidiqi.icu

[R34] 退出时清理
来源：http://pvr.hnxiangtu.top

trap 'rm -f "$tmp"' EXIT
来源：http://pbe.cdnleiting.top

[R35] 后台执行并等待
来源：http://fco.fehbvm.com

sleep 5 & pid=$!; wait "$pid"
来源：http://pfv.sufxvd.cn

[R36] 并发执行多个任务
来源：http://brh.smart0.xyz

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://vqe.shanyushiyangtech.top

[R37] 把输出赋给变量
来源：http://rjq.zycfv.cn

files=$(ls -1)
来源：http://vnk.feifeiyinyue.top

[R38] 管道串联
来源：http://diq.xuetiantiany.cn

cat a.txt | grep -i error | wc -l
来源：http://wkh.52xcode.cn

[R39] 重定向标准输出与错误
来源：http://hyz.yvedp.cn

cmd > out.log 2>&1
来源：http://vwl.daria6918.cn

[R40] 追加写日志
来源：http://tim.jiagoushi.top

echo "log" >> out.log
来源：http://gjf.shanyushiyangkeji.top

[R41] 丢弃输出
来源：http://fnc.shuidangran.top

cmd >/dev/null 2>&1
来源：http://lgt.xziqi.cn

[R42] 输入重定向
来源：http://rwr.sjlbkw.cn

wc -l < a.txt
来源：http://ztu.cdnleiting.top

[R43] 按名字查找文件
来源：http://gvt.shanyushiyangtech.top

find . -name "*.log" -type f
来源：http://jfl.shangyingyoupin.top

[R44] 按修改时间查找
来源：http://psp.chenjidiqi.icu

find . -mtime -7 -type f
来源：http://var.ppjwa.cn

[R45] 批量删除
来源：http://rua.yj20258.top

find . -name "*.tmp" -delete
来源：http://anc.yvedp.cn

[R46] 递归替换文件内容
来源：http://lhu.quarkkingdee.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ryb.fktsv.cn

[R47] sed 单行替换
来源：http://yep.gotoacloud.top

sed -i 's/foo/bar/g' a.txt
来源：http://xuu.cashguo.top

[R48] awk 取指定列
来源：http://qfl.quarkkingdee.top

awk '{print $1, $3}' a.txt
来源：http://uif.iojbl.cn

[R49] awk 带条件
来源：http://sca.yj202588.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://eim.yueranfly.top

[R50] awk 求和
来源：http://vhy.nanxinkj.top

awk '{s += $2} END {print s}' a.txt
来源：http://sdf.52xcode.cn

[R51] 排序去重取前几
来源：http://syp.yongpay.top

sort a.txt | uniq -c | sort -rn | head
来源：http://uwf.nwbrower.top

[R52] 统计行数
来源：http://xyt.nwbrower.top

wc -l a.txt
来源：http://jif.zhiwuduotai.top

[R53] 查看文件头与实时尾
来源：http://cjx.tian-w.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://pfl.yj202588.top

[R54] 比较两个文件
来源：http://vrv.zhiwuduotai.top

diff a.txt b.txt
来源：http://kbo.dianchejie.cn

[R55] 压缩与解压
来源：http://yog.zdqjudy.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://owx.zhixingplan.top

[R56] 远程拷贝
来源：http://mlj.zhijiandao.cn

scp file user@host:/path/
来源：http://tbp.sysykeji.top

[R57] 远程执行命令
来源：http://jjo.wangdashe.top

ssh user@host 'uptime'
来源：http://euo.yongpay.top

[R58] 下载文件
来源：http://cos.sysykeji.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://sta.jinghuilouyu.cn

[R59] 发 POST JSON
来源：http://yjt.gogol.net.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://yfj.hnqzz.top

[R60] 只看 HTTP 状态码
来源：http://vmv.ybcxt.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://cwr.yueranfly.top

[R61] 磁盘占用
来源：http://fdq.cheryme.top

df -h;  du -sh *
来源：http://gqp.fengsongda.top

[R62] 找最占空间的文件
来源：http://tnx.gzhubu.top

du -ah . | sort -rh | head -10
来源：http://xhw.jiagoushi.top

[R63] 内存与进程
来源：http://jss.shanyushiyangtech.top

free -h;  ps aux | grep nginx
来源：http://fqq.zdbjq.cn

[R64] 结束进程
来源：http://glf.svipenyu.cn

kill -9 $(pgrep -f app.py)
来源：http://clg.nanxinkj.top

[R65] 查看端口占用
来源：http://ybd.ehwqpu.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hxp.bjfxy.top

[R66] 定时任务
来源：http://dng.52xcode.cn

crontab -e;  crontab -l
来源：http://lty.ppjwa.cn

[R67] 生成随机十六进制串
来源：http://sgo.havefunace.top

openssl rand -hex 16
来源：http://hcz.cqqwz.cn

[R68] 计算文件校验值
来源：http://app.meibo888.top

sha256sum a.txt;  md5sum a.txt
来源：http://tby.aizwys.cn

[R69] 生成随机密码
来源：http://qov.zycfv.cn

head -c 16 /dev/urandom | base64
来源：http://bvh.jinqigfzy.top

[R70] 时间戳与互转
来源：http://ioi.hcnkem.com

date +%s;  date -d @1700000000
来源：http://roe.chenjidiqi.icu

[R71] 日期格式化
来源：http://muj.c1oappe.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://khz.zhixingplan.top

[R72] 等待端口就绪
来源：http://usv.jinghuilouyu.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://xqa.wangdashe.top

[R73] 分割大日志
来源：http://ghm.tianlin.xyz

split -l 1000 big.log part_
来源：http://fko.shanyushiyangtech.top

[R74] 批量重命名
来源：http://zqm.jianghu66.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://zqf.shanyushiyangtech.top

[R75] 导出环境变量
来源：http://uen.9152youxi.cn

export PATH="$HOME/bin:$PATH"
来源：http://dkx.ppjwa.cn

[R76] 使用临时文件
来源：http://knm.bjfxy.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ecz.ctjpmb.com

[R77] 读取用户输入
来源：http://kwy.wangshuangyany.cn

read -rp "请输入: " ans
来源：http://lfp.hywenlv.cn

[R78] 交互式菜单
来源：http://ghk.wangdashe.top

select opt in a b c; do echo "$opt"; break; done
来源：http://nbv.sxryk.cn

[R79] 解析命令行选项
来源：http://rmg.ehwqpu.com


<!-- 参考信息 -->