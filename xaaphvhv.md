代发 wailian999

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://nep.cucudq.cn

[Q26] 计数
来源：http://cdq.hesvh.cn

SELECT COUNT(*) FROM users;
来源：http://ihv.zycfv.cn

[Q27] 条件计数
来源：http://uzj.mhx1999.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://yvg.cucudq.cn

[Q28] 求和与平均
来源：http://bve.yueranfly.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://eib.shzxlz.cn

[Q29] 最大最小值
来源：http://qex.hesvh.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ukp.hesvh.cn

[Q30] 分组统计
来源：http://tkh.c1oappe.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://txb.shanyushiyangkeji.top

[Q31] 分组后过滤
来源：http://rzp.zhongyouzk.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hyv.andypj.xyz

[Q32] 分组拼接字符串
来源：http://ops.kuanghao11.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ohy.redwolf501.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ayo.zdqjudy.top

[Q33] 多列分组
来源：http://olx.tianlin.xyz

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://kki.yuanzhike.top

[Q34] 每组取第一条
来源：http://cxo.chenzaomai.com

SELECT * FROM (
来源：http://jri.zhixingplan.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://nja.yangfankeji.com

) t WHERE rn = 1;
来源：http://gsn.316326.xyz

[Q35] 内连接
来源：http://tzt.zhongyouzk.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hxh.birdmap.top

[Q36] 左连接
来源：http://zsl.svipenyu.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://gnt.fehbvm.com

[Q37] 右连接
来源：http://xbk.yj202588.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wkq.sufxvd.cn

[Q38] 全外连接（PostgreSQL）
来源：http://cvl.hnqzz.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://kcl.nanxinkj.top

[Q39] 自连接（查上下级）
来源：http://cdv.fehbvm.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://aid.shangyingyoupin.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://fhm.jqgfzy.top

[Q40] 交叉连接（笛卡尔积）
来源：http://aoh.hnqzz.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://tjq.tian-w.cn

[Q41] 多表连接
来源：http://aas.aizwys.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://pkl.yuxming.cn

JOIN users u ON u.id = o.user_id
来源：http://bwb.xingfuxueyuan.xyz

JOIN products p ON p.id = o.product_id;
来源：http://tin.ybcxt.top

[Q42] 连接条件附加过滤
来源：http://lhl.gogol.net.cn

SELECT u.name, o.amount FROM users u
来源：http://ian.ivvv.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://zlx.feifeiyinyue.top

[Q43] 标量子查询
来源：http://kiv.sxryk.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://rhf.yanxiufei.cn

[Q44] IN 子查询
来源：http://lmj.zdbjq.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://yat.316326.xyz

[Q45] EXISTS 判断存在
来源：http://jii.sysykeji.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ako.sxryk.cn

[Q46] NOT EXISTS 判断不存在
来源：http://qok.shanyushiyangkeji.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jsn.yj202588.top

[Q47] 与平均值比较
来源：http://rpl.nanxinkj.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://lyt.zhijiandao.cn

[Q48] CTE 公用表表达式
来源：http://frh.quarkkingdee.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://vql.andypj.xyz

SELECT * FROM t WHERE c > 5;
来源：http://hqn.tarul.cn

[Q49] 更新单行
来源：http://dxe.yangfankeji.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://oja.xuanzx.com

[Q50] 批量更新
来源：http://njk.xingfuxueyuan.xyz

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://cyg.xinyue.icu

[Q51] 用子查询更新
来源：http://txr.yvedp.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://dxs.haohaochexian.top

[Q52] 删除指定行
来源：http://xpn.sjlbkw.cn

DELETE FROM users WHERE id = 10;
来源：http://ijo.yj20258888.top

[Q53] 按条件删除
来源：http://vzx.jlsjyb.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://lhk.gaohongyu789.top

[Q54] 清空表
来源：http://uvw.quarkkingdee.top

TRUNCATE TABLE logs;
来源：http://qbs.redwolf501.top

[Q55] 排名（并列占位）
来源：http://yot.jinyuanbaomall.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://jpc.guannengcc.top

[Q56] 密集排名（并列不占位）
来源：http://tgj.cucudq.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://abo.jyoumei.cn

[Q57] 行号
来源：http://jzr.zhixingplan.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://tmy.sufxvd.cn

[Q58] 累计求和
来源：http://rnn.sufxvd.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://dvt.hnqzz.top

[Q59] 分组内累计
来源：http://lsu.ctjpmb.com

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ekz.xuanzx.com

[Q60] 取上一行 / 下一行
来源：http://fdt.zhijiandao.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://tcn.svipenyu.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://jiv.ehwqpu.com

[Q61] 移动平均
来源：http://wep.yangfankeji.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://kzt.c1oappe.top

[Q62] 分组占比
来源：http://ghj.chenzaomai.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://zas.ctjpmb.com

[Q63] 开启事务
来源：http://yvs.jinqigufen.top

START TRANSACTION;                -- 或 BEGIN
来源：http://ozt.andypj.xyz

[Q64] 提交事务
来源：http://tka.zhixingplan.top

COMMIT;
来源：http://yop.andypj.xyz

[Q65] 回滚事务
来源：http://qib.havefunace.top

ROLLBACK;
来源：http://owu.jianghu66.top

[Q66] 行锁查询
来源：http://bhq.ybcxt.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://qwm.cheryme.top

[Q67] 设置隔离级别
来源：http://qtb.fktsv.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://gkf.yj20258888.top

[Q68] 保存点
来源：http://lsd.yj20258888.top

SAVEPOINT sp1;
来源：http://oxq.aibaodan.cn

ROLLBACK TO sp1;
来源：http://klo.ywan-chungtsiang.top

[Q69] 查看执行计划
来源：http://mmo.zycfv.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://jyl.ybcxt.top

[Q70] 更新统计信息
来源：http://rry.mhx1999.top

ANALYZE TABLE users;
来源：http://mkg.cucudq.cn

[Q71] 查看建表语句
来源：http://kbj.jinyuanbaomall.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://aal.xziqi.cn

[Q72] 查看索引
来源：http://nov.tanke756.top

SHOW INDEX FROM users;
来源：http://kfx.zhaomingkeji.xyz

[Q73] 查看表状态
来源：http://asd.ydzc1.top

SHOW TABLE STATUS LIKE 'users';
来源：http://wgg.ydjk.org.cn

[Q74] 强制使用索引
来源：http://bzp.nanxuanxn.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://efc.yangfankeji.com

[Q75] 日期格式化
来源：http://ooo.cqqwz.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hom.ctjpmb.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://etl.jqgfzy.top

[Q76] 按天统计
来源：http://gxf.fanxiaobao.xyz

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://xhm.ivvv.top

[Q77] 时间加减
来源：http://hft.xingfuxueyuan.xyz

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://koc.zhengqikj.top

[Q78] 当前时间
来源：http://sye.jqgfzy.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mus.sxryk.cn

[Q79] 字符串拼接
来源：http://tbo.pycfn.com

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://yah.mhx1999.top

[Q80] 字符串截取
来源：http://zkr.jinqigfzy.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://smn.mhx1999.top

[Q81] 字符串替换
来源：http://rgh.tianlin.xyz

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://qrn.dashuyun.cn

[Q82] 字符长度与字节长度
来源：http://bah.vehdjk.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://vqu.bjfxy.top

[Q83] 大小写转换
来源：http://egn.hesvh.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ouh.wangshuangyany.cn

[Q84] 去除首尾空格
来源：http://wsu.yj202588.top

SELECT TRIM(name) FROM users;
来源：http://hlq.chenjidiqi.icu

[Q85] 数值取整
来源：http://ezn.nanxuanxn.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://bfr.fehbvm.com

[Q86] 读取 JSON 字段
来源：http://akr.nanxinkj.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://zln.pengpengdd.cyou

[Q87] JSON 字段做条件
来源：http://syu.feifeiyinyue.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://jkg.ybcxt.top

[Q88] 行转列（条件聚合）
来源：http://ive.tanke756.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hff.jinyuanbaomall.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://fnw.sysykeji.top

[Q89] 判断表是否存在
来源：http://jrm.tian-w.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://fgk.fehbvm.com

[Q90] 生成序号列
来源：http://plz.hywenlv.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://kjl.316326.xyz

================================================================================
来源：http://tzi.dianchejie.cn

R. Bash 专题
来源：http://wtv.havefunace.top

================================================================================
来源：http://rim.yfazqb.com

[R01] shebang 与严格模式
来源：http://rwf.andypj.xyz

#!/usr/bin/env bash
来源：http://pcg.andypj.xyz

set -euo pipefail
来源：http://jjf.tian-w.cn

[R02] 变量赋值与使用
来源：http://xgk.jinqigufen.top

name="Tom"; echo "$name"
来源：http://gyb.fehbvm.com

[R03] 只读变量
来源：http://nwp.quarkkingdee.top

readonly PI=3.14
来源：http://ikm.nanxuanxn.top

[R04] 位置参数
来源：http://jla.cdnleiting.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://edy.yfazqb.com

[R05] 参数默认值
来源：http://qgo.jianghu66.top

name="${1:-default}"
来源：http://imy.pycfn.com

[R06] 判断命令是否存在
来源：http://hzd.tanke756.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://esf.shangyingyoupin.top

[R07] if 判断文件
来源：http://gjt.shuidangran.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://vjf.xinyue.icu

[R08] 数值比较
来源：http://ymb.chenjidiqi.icu

if (( a > b )); then echo "a 更大"; fi
来源：http://gws.sufxvd.cn

[R09] 字符串比较
来源：http://idq.bbcook.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ozc.zdqjudy.top

[R10] 正则匹配
来源：http://ebv.andypj.xyz

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://lzv.quarkkingdee.top

[R11] case 多分支
来源：http://vqa.wangdashe.top

case "$1" in
来源：http://zor.kuanghao11.cn

start) echo "启动" ;;
来源：http://oyl.bjfxy.top

stop)  echo "停止" ;;
来源：http://dob.zdqjudy.top

*)     echo "未知命令" ;;
来源：http://lek.meibo888.top

esac
来源：http://xws.c1oappe.top

[R12] for 遍历文件
来源：http://pqd.cdnleiting.top

for f in *.txt; do echo "$f"; done
来源：http://rkb.vqdsnc.cn

[R13] for 计数循环
来源：http://kiq.316326.xyz

for i in {1..10}; do echo "$i"; done
来源：http://yaw.zhijiandao.cn

[R14] C 风格 for
来源：http://hav.ybcxt.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ohs.xingfuxueyuan.xyz

[R15] while 逐行读文件
来源：http://dzx.tian-w.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wow.zhengqikj.top

[R16] until 等待条件
来源：http://dml.xuanzx.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://xcu.yongpay.top

[R17] 数组定义与取值
来源：http://srj.ehwqpu.com

arr=(a b c); echo "${arr[0]}"
来源：http://bke.hysaishi.cn

[R18] 遍历数组
来源：http://yld.nwbrower.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://yfy.zhengqikj.top

[R19] 数组长度
来源：http://bpx.vqdsnc.cn

echo "${#arr[@]}"
来源：http://ddp.sweek.top

[R20] 关联数组（字典）
来源：http://kcl.c1oappe.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://dvv.hysaishi.cn

[R21] 字符串长度
来源：http://epa.gaohongyu789.top

echo "${#s}"
来源：http://uqn.tian-w.cn

[R22] 截取子串
来源：http://his.yfazqb.com

echo "${s:0:5}"
来源：http://bqp.haohaochexian.top

[R23] 字符串替换
来源：http://jiw.zdqjudy.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://gpg.ivvv.top

[R24] 大小写转换
来源：http://qdr.cucudq.cn

echo "${s^^}"; echo "${s,,}"
来源：http://sww.aibaodan.cn

[R25] 去后缀 / 去前缀
来源：http://bux.bjfxy.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://wgw.yangfankeji.com

[R26] 命令替换
来源：http://hok.daria6918.cn

now=$(date +%F); echo "$now"
来源：http://eqb.cashguo.top

[R27] 算术展开
来源：http://dun.birdmap.top

echo $((1 + 2 * 3))
来源：http://tuv.hnqzz.top

[R28] 浮点运算
来源：http://lot.jinqigfzy.top

echo "scale=2; 10/3" | bc
来源：http://nmm.jinghuilouyu.cn

[R29] 定义函数
来源：http://uot.fanxiaobao.xyz

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wif.hnqzz.top

[R30] 函数返回状态码
来源：http://sir.uphjek.com

f() { return 0; }; f || echo "失败了"
来源：http://tgn.gaohongyu789.top

[R31] 局部变量
来源：http://rjc.hysaishi.cn

f() { local x=1; echo "$x"; }
来源：http://wvp.xuanzx.com

[R32] 参数个数校验
来源：http://qeb.bjfxy.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://cse.mhx1999.top

[R33] 捕获错误并提示行号
来源：http://qjb.zhixingplan.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://lsk.tian-w.cn

[R34] 退出时清理
来源：http://fyi.bbcook.cn

trap 'rm -f "$tmp"' EXIT
来源：http://cla.xinyue.icu

[R35] 后台执行并等待
来源：http://doy.ppjwa.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://dtv.daxiang520.top

[R36] 并发执行多个任务
来源：http://awi.fzhhl.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://qan.sufxvd.cn

[R37] 把输出赋给变量
来源：http://ijr.vehdjk.com

files=$(ls -1)
来源：http://rpi.yj20258888.top

[R38] 管道串联
来源：http://gbm.316326.xyz

cat a.txt | grep -i error | wc -l
来源：http://tvr.hongshengwenyu.top

[R39] 重定向标准输出与错误
来源：http://iwk.zhaomingkeji.xyz

cmd > out.log 2>&1
来源：http://jtr.fzhhl.top

[R40] 追加写日志
来源：http://hww.zhixingplan.top

echo "log" >> out.log
来源：http://hbp.bbcook.cn

[R41] 丢弃输出
来源：http://fqc.jqgfzy.top

cmd >/dev/null 2>&1
来源：http://vyq.cheryme.top

[R42] 输入重定向
来源：http://ikj.yuanzhike.top

wc -l < a.txt
来源：http://zxe.ppjwa.cn

[R43] 按名字查找文件
来源：http://jbl.shanyushiyangkeji.top

find . -name "*.log" -type f
来源：http://vpz.cashguo.top

[R44] 按修改时间查找
来源：http://cgl.cucudq.cn

find . -mtime -7 -type f
来源：http://qlp.ydzc1.top

[R45] 批量删除
来源：http://vki.nwbrower.top

find . -name "*.tmp" -delete
来源：http://fyd.dashuyun.cn

[R46] 递归替换文件内容
来源：http://xkx.daria6918.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ngf.havefunace.top

[R47] sed 单行替换
来源：http://xog.pengpengdd.cyou

sed -i 's/foo/bar/g' a.txt
来源：http://tld.chenzaomai.com

[R48] awk 取指定列
来源：http://ilc.nanxinkj.top

awk '{print $1, $3}' a.txt
来源：http://dxo.fengsongda.top

[R49] awk 带条件
来源：http://tmj.birdmap.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://gsk.tanke756.top

[R50] awk 求和
来源：http://jqm.hywenlv.cn

awk '{s += $2} END {print s}' a.txt
来源：http://lcb.cucudq.cn

[R51] 排序去重取前几
来源：http://sbt.fehbvm.com

sort a.txt | uniq -c | sort -rn | head
来源：http://sjs.gogol.net.cn

[R52] 统计行数
来源：http://dzm.ybcxt.top

wc -l a.txt
来源：http://ybq.daxiang520.top

[R53] 查看文件头与实时尾
来源：http://saa.sysykeji.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ykn.jiagoushi.top

[R54] 比较两个文件
来源：http://pyr.svipenyu.cn

diff a.txt b.txt
来源：http://xvb.bbcook.cn

[R55] 压缩与解压
来源：http://xur.jqgfzy.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://nnx.ydzc1.top

[R56] 远程拷贝
来源：http://xws.xuetiantiany.cn

scp file user@host:/path/
来源：http://zag.hfpthk.cn

[R57] 远程执行命令
来源：http://sfg.yangfankeji.com

ssh user@host 'uptime'
来源：http://khs.gotoacloud.top

[R58] 下载文件
来源：http://bjr.zhixingplan.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wnb.chenzaomai.com

[R59] 发 POST JSON
来源：http://oxd.9152youxi.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://nym.havefunace.top

[R60] 只看 HTTP 状态码
来源：http://jwl.shanyushiyangtech.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ltj.yangfankeji.com

[R61] 磁盘占用
来源：http://ilm.yongpay.top

df -h;  du -sh *
来源：http://jbi.uphjek.com

[R62] 找最占空间的文件
来源：http://wsm.shanyushiyangtech.top

du -ah . | sort -rh | head -10
来源：http://xne.jqgufenzy.top

[R63] 内存与进程
来源：http://vzl.svipenyu.cn

free -h;  ps aux | grep nginx
来源：http://kxv.yonumen.top

[R64] 结束进程
来源：http://jkr.zhongyouzk.top

kill -9 $(pgrep -f app.py)
来源：http://kbp.tanke756.top

[R65] 查看端口占用
来源：http://rze.aizwys.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ykf.guannengcc.top

[R66] 定时任务
来源：http://iur.zdbjq.cn

crontab -e;  crontab -l
来源：http://kqe.hesvh.cn

[R67] 生成随机十六进制串
来源：http://cap.jqgufenzy.top

openssl rand -hex 16
来源：http://xfy.smart0.xyz

[R68] 计算文件校验值
来源：http://lbb.svipenyu.cn

sha256sum a.txt;  md5sum a.txt
来源：http://hce.havefunace.top

[R69] 生成随机密码
来源：http://jxv.fktsv.cn

head -c 16 /dev/urandom | base64
来源：http://shk.tian-w.cn

[R70] 时间戳与互转
来源：http://kua.daria6918.cn

date +%s;  date -d @1700000000
来源：http://yfz.zhijiandao.cn

[R71] 日期格式化
来源：http://ybl.guowangkeji.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://uey.sysykeji.top

[R72] 等待端口就绪
来源：http://bnz.yonumen.top

until nc -z localhost 3306; do sleep 1; done
来源：http://ifl.birdmap.top

[R73] 分割大日志
来源：http://flo.tian-w.cn

split -l 1000 big.log part_
来源：http://kox.sxryk.cn

[R74] 批量重命名
来源：http://bxk.tian-w.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://jro.sjlbkw.cn

[R75] 导出环境变量
来源：http://fqx.nanxinkj.top


<!-- 参考信息 -->