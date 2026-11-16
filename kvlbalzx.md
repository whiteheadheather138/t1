代发 wailian999

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://tqb.hysaishi.cn

[Q26] 计数
来源：http://rjm.shanyushiyangkeji.top

SELECT COUNT(*) FROM users;
来源：http://trv.ybcxt.top

[Q27] 条件计数
来源：http://bab.chenjidiqi.icu

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://gey.nanxuanxn.top

[Q28] 求和与平均
来源：http://lhe.quarkkingdee.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://xvt.ydzc1.top

[Q29] 最大最小值
来源：http://pvx.xuetiantiany.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://vcm.xinyue.icu

[Q30] 分组统计
来源：http://wgr.fzhhl.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://cie.sjlbkw.cn

[Q31] 分组后过滤
来源：http://xwq.xziqi.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ykf.jyoumei.cn

[Q32] 分组拼接字符串
来源：http://pvt.yj20258.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://vvb.jlsjyb.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://nfs.yvedp.cn

[Q33] 多列分组
来源：http://crm.hcnkem.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://lqc.hcnkem.com

[Q34] 每组取第一条
来源：http://kwo.ppjwa.cn

SELECT * FROM (
来源：http://lqp.0kj1m.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://vyv.jianghu66.top

) t WHERE rn = 1;
来源：http://kyd.shuidangran.top

[Q35] 内连接
来源：http://jon.hysaishi.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hcn.aizwys.cn

[Q36] 左连接
来源：http://yec.zhixingplan.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://dda.aizwys.cn

[Q37] 右连接
来源：http://pfi.9152youxi.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://toj.xingfuxueyuan.xyz

[Q38] 全外连接（PostgreSQL）
来源：http://kmq.jinyuanbaomall.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hls.jinqigufen.top

[Q39] 自连接（查上下级）
来源：http://ekh.ydzc1.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://tbs.hywenlv.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ozv.wangdashe.top

[Q40] 交叉连接（笛卡尔积）
来源：http://ach.yj20258888.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mmu.xinyue.icu

[Q41] 多表连接
来源：http://mxm.hcnkem.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://iol.hcnkem.com

JOIN users u ON u.id = o.user_id
来源：http://ltc.zhongyouzk.top

JOIN products p ON p.id = o.product_id;
来源：http://mlm.yj20258888.top

[Q42] 连接条件附加过滤
来源：http://vxf.ydzc1.top

SELECT u.name, o.amount FROM users u
来源：http://rou.aibaodan.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://bsg.ctjpmb.com

[Q43] 标量子查询
来源：http://ubk.quarkkingdee.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://nto.dashuyun.cn

[Q44] IN 子查询
来源：http://lkx.meibo888.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://oeo.aibaodan.cn

[Q45] EXISTS 判断存在
来源：http://noz.hcnkem.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bkt.gogol.net.cn

[Q46] NOT EXISTS 判断不存在
来源：http://bdc.daria6918.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qxs.hnxiangtu.top

[Q47] 与平均值比较
来源：http://gyv.quarkkingdee.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://iuu.hammf.cn

[Q48] CTE 公用表表达式
来源：http://anf.yj20258.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://yng.hnxiangtu.top

SELECT * FROM t WHERE c > 5;
来源：http://jjl.yangfankeji.com

[Q49] 更新单行
来源：http://wxy.dashuyun.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ehp.daria6918.cn

[Q50] 批量更新
来源：http://wmw.gotoacloud.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ans.gotoacloud.top

[Q51] 用子查询更新
来源：http://hke.sweek.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://aqc.hnxiangtu.top

[Q52] 删除指定行
来源：http://ckf.xinyue.icu

DELETE FROM users WHERE id = 10;
来源：http://fhq.fzhhl.top

[Q53] 按条件删除
来源：http://hul.haohaochexian.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ruo.sweek.top

[Q54] 清空表
来源：http://kch.sjlbkw.cn

TRUNCATE TABLE logs;
来源：http://gtq.cashguo.top

[Q55] 排名（并列占位）
来源：http://jjs.yuanzhike.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://fjv.316326.xyz

[Q56] 密集排名（并列不占位）
来源：http://uwe.meibo888.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://znx.chenjidiqi.icu

[Q57] 行号
来源：http://xqs.yuanzhike.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://iri.gzhubu.top

[Q58] 累计求和
来源：http://cqq.fanxiaobao.xyz

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://bof.kuanghao11.cn

[Q59] 分组内累计
来源：http://ygv.zhongyouzk.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://cfd.c1oappe.top

[Q60] 取上一行 / 下一行
来源：http://jxl.zhijiandao.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://htk.tanke756.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ebq.fzhhl.top

[Q61] 移动平均
来源：http://mvl.fehbvm.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://qob.xuetiantiany.cn

[Q62] 分组占比
来源：http://ziu.xylfe.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://sfc.yuanzhike.top

[Q63] 开启事务
来源：http://kyl.smart0.xyz

START TRANSACTION;                -- 或 BEGIN
来源：http://fec.yangfankeji.com

[Q64] 提交事务
来源：http://yrh.gzhubu.top

COMMIT;
来源：http://pgx.pengpengdd.cyou

[Q65] 回滚事务
来源：http://hor.tianlin.xyz

ROLLBACK;
来源：http://muz.haohaochexian.top

[Q66] 行锁查询
来源：http://gpv.hnqzz.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://njq.xuanzx.com

[Q67] 设置隔离级别
来源：http://cvq.shuidangran.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://cpu.xuanzx.com

[Q68] 保存点
来源：http://koe.zycfv.cn

SAVEPOINT sp1;
来源：http://wyt.yvedp.cn

ROLLBACK TO sp1;
来源：http://nni.snrcjt.cn

[Q69] 查看执行计划
来源：http://orp.fehbvm.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://dgt.uphjek.com

[Q70] 更新统计信息
来源：http://jpg.hnqzz.top

ANALYZE TABLE users;
来源：http://ouu.chenzaomai.com

[Q71] 查看建表语句
来源：http://qzw.redwolf501.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://oaw.jianghu66.top

[Q72] 查看索引
来源：http://uje.yj20258.top

SHOW INDEX FROM users;
来源：http://ywd.yueranfly.top

[Q73] 查看表状态
来源：http://bsy.hfpthk.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://jnx.vqdsnc.cn

[Q74] 强制使用索引
来源：http://dxj.fanxiaobao.xyz

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hbu.daxiang520.top

[Q75] 日期格式化
来源：http://osd.tianlin.xyz

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ckn.c1oappe.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://dsp.iojbl.cn

[Q76] 按天统计
来源：http://pja.9152youxi.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://fal.316326.xyz

[Q77] 时间加减
来源：http://ucm.shzxlz.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://aqu.zhaomingkeji.xyz

[Q78] 当前时间
来源：http://hml.jqgufenzy.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://thu.cheryme.top

[Q79] 字符串拼接
来源：http://llr.zhaomingkeji.xyz

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://sty.kuanghao11.cn

[Q80] 字符串截取
来源：http://sdh.birdmap.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ipe.gaohongyu789.top

[Q81] 字符串替换
来源：http://ean.yueranfly.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://pnn.tanke756.top

[Q82] 字符长度与字节长度
来源：http://vvv.vqdsnc.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://cfn.tianlin.xyz

[Q83] 大小写转换
来源：http://hhm.jqgufenzy.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ivo.xuetiantiany.cn

[Q84] 去除首尾空格
来源：http://qto.smart0.xyz

SELECT TRIM(name) FROM users;
来源：http://qas.tian-w.cn

[Q85] 数值取整
来源：http://gab.shanyushiyangtech.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ksh.yuanzhike.top

[Q86] 读取 JSON 字段
来源：http://lkk.cashguo.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ktx.jinyuanbaomall.cn

[Q87] JSON 字段做条件
来源：http://vug.havefunace.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ypj.shanyushiyangtech.top

[Q88] 行转列（条件聚合）
来源：http://ttz.zycfv.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wei.chenlongwang.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ufu.quarkkingdee.top

[Q89] 判断表是否存在
来源：http://rcm.jyoumei.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://uaq.jinqigufen.top

[Q90] 生成序号列
来源：http://dom.yanxiufei.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hxr.hesvh.cn

================================================================================
来源：http://wvt.sysykeji.top

R. Bash 专题
来源：http://iza.jqgfzy.top

================================================================================
来源：http://gbf.xingfuxueyuan.xyz

[R01] shebang 与严格模式
来源：http://nzj.hnqzz.top

#!/usr/bin/env bash
来源：http://oiu.fengsongda.top

set -euo pipefail
来源：http://lif.zhongyouzk.top

[R02] 变量赋值与使用
来源：http://vdb.ivvv.top

name="Tom"; echo "$name"
来源：http://ucs.xingfuxueyuan.xyz

[R03] 只读变量
来源：http://qkw.zhaomingkeji.xyz

readonly PI=3.14
来源：http://jlq.hammf.cn

[R04] 位置参数
来源：http://qwg.wangdashe.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://rfe.ydjk.org.cn

[R05] 参数默认值
来源：http://esf.nwbrower.top

name="${1:-default}"
来源：http://blc.zhijiandao.cn

[R06] 判断命令是否存在
来源：http://owf.jyoumei.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ijx.yj202588.top

[R07] if 判断文件
来源：http://gck.c1oappe.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://zom.zhixingplan.top

[R08] 数值比较
来源：http://hpb.hnxiangtu.top

if (( a > b )); then echo "a 更大"; fi
来源：http://yjv.nwbrower.top

[R09] 字符串比较
来源：http://imd.52xcode.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://lln.jlsjyb.cn

[R10] 正则匹配
来源：http://nyb.kuanghao11.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hfp.gzhubu.top

[R11] case 多分支
来源：http://atw.quarkkingdee.top

case "$1" in
来源：http://sxw.jlsjyb.cn

start) echo "启动" ;;
来源：http://xfy.hywenlv.cn

stop)  echo "停止" ;;
来源：http://xip.dianchejie.cn

*)     echo "未知命令" ;;
来源：http://xtc.52xcode.cn

esac
来源：http://bqb.cdnleiting.top

[R12] for 遍历文件
来源：http://zti.yj202588.top

for f in *.txt; do echo "$f"; done
来源：http://rxe.redwolf501.top

[R13] for 计数循环
来源：http://xrw.xuetiantiany.cn

for i in {1..10}; do echo "$i"; done
来源：http://buy.gzhubu.top

[R14] C 风格 for
来源：http://ayd.sweek.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://oda.meibo888.top

[R15] while 逐行读文件
来源：http://ugi.yonumen.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://jwa.nanxuanxn.top

[R16] until 等待条件
来源：http://qra.ehwqpu.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://qyi.fktsv.cn

[R17] 数组定义与取值
来源：http://pmf.smart0.xyz

arr=(a b c); echo "${arr[0]}"
来源：http://rwb.ybcxt.top

[R18] 遍历数组
来源：http://gtl.chenjidiqi.icu

for x in "${arr[@]}"; do echo "$x"; done
来源：http://pow.hesvh.cn

[R19] 数组长度
来源：http://nnb.tarul.cn

echo "${#arr[@]}"
来源：http://ewe.hesvh.cn

[R20] 关联数组（字典）
来源：http://dbp.kuanghao11.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://yum.fengsongda.top

[R21] 字符串长度
来源：http://ljr.ydzc1.top

echo "${#s}"
来源：http://xep.pengpengdd.cyou

[R22] 截取子串
来源：http://bdc.ybcxt.top

echo "${s:0:5}"
来源：http://vyh.bjfxy.top

[R23] 字符串替换
来源：http://dam.aizwys.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://jym.yj20258.top

[R24] 大小写转换
来源：http://krj.xziqi.cn

echo "${s^^}"; echo "${s,,}"
来源：http://lmp.feifeiyinyue.top

[R25] 去后缀 / 去前缀
来源：http://gkk.snrcjt.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://jtg.jinyuanbaomall.cn

[R26] 命令替换
来源：http://fza.zhoulong.xyz

now=$(date +%F); echo "$now"
来源：http://bir.aibaodan.cn

[R27] 算术展开
来源：http://zub.yuanzhike.top

echo $((1 + 2 * 3))
来源：http://soj.gogol.net.cn

[R28] 浮点运算
来源：http://ebb.yj202588.top

echo "scale=2; 10/3" | bc
来源：http://uxx.tarul.cn

[R29] 定义函数
来源：http://vfh.fanxiaobao.xyz

add() { echo $(($1 + $2)); }; add 1 2
来源：http://gus.ybcxt.top

[R30] 函数返回状态码
来源：http://lqf.jinghuilouyu.cn

f() { return 0; }; f || echo "失败了"
来源：http://zjp.316326.xyz

[R31] 局部变量
来源：http://hta.sxryk.cn

f() { local x=1; echo "$x"; }
来源：http://ekt.xylfe.cn

[R32] 参数个数校验
来源：http://ymc.cdnleiting.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://pzy.snrcjt.cn

[R33] 捕获错误并提示行号
来源：http://rok.chenjidiqi.icu

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://qgq.andypj.xyz

[R34] 退出时清理
来源：http://mfa.iojbl.cn

trap 'rm -f "$tmp"' EXIT
来源：http://bmu.ehwqpu.com

[R35] 后台执行并等待
来源：http://xxf.yanxiufei.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://dtc.chenzaomai.com

[R36] 并发执行多个任务
来源：http://uni.smart0.xyz

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://afh.vqdsnc.cn

[R37] 把输出赋给变量
来源：http://ysx.zdqjudy.top

files=$(ls -1)
来源：http://nzs.hongshengwenyu.top

[R38] 管道串联
来源：http://muf.hnxiangtu.top

cat a.txt | grep -i error | wc -l
来源：http://imr.zhoulong.xyz

[R39] 重定向标准输出与错误
来源：http://eym.zdbjq.cn

cmd > out.log 2>&1
来源：http://yom.ydzc1.top

[R40] 追加写日志
来源：http://adt.xuetiantiany.cn

echo "log" >> out.log
来源：http://nyw.yanxiufei.cn

[R41] 丢弃输出
来源：http://oqn.yongpay.top

cmd >/dev/null 2>&1
来源：http://itd.sysykeji.top

[R42] 输入重定向
来源：http://wzv.yj20258.top

wc -l < a.txt
来源：http://spj.daria6918.cn

[R43] 按名字查找文件
来源：http://nda.fehbvm.com

find . -name "*.log" -type f
来源：http://hsd.feifeiyinyue.top

[R44] 按修改时间查找
来源：http://ycn.havefunace.top

find . -mtime -7 -type f
来源：http://kyl.xingfuxueyuan.xyz

[R45] 批量删除
来源：http://boy.hnqzz.top

find . -name "*.tmp" -delete
来源：http://bdw.yuxming.cn

[R46] 递归替换文件内容
来源：http://zap.jinqigfzy.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://tdk.cdnleiting.top

[R47] sed 单行替换
来源：http://zsu.shangyingyoupin.top

sed -i 's/foo/bar/g' a.txt
来源：http://fyn.gaohongyu789.top

[R48] awk 取指定列
来源：http://ldj.hnqzz.top

awk '{print $1, $3}' a.txt
来源：http://djy.fehbvm.com

[R49] awk 带条件
来源：http://zzx.52xcode.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://pxu.uphjek.com

[R50] awk 求和
来源：http://jvw.gzhubu.top

awk '{s += $2} END {print s}' a.txt
来源：http://fqg.chenzaomai.com

[R51] 排序去重取前几
来源：http://htj.yj202588.top

sort a.txt | uniq -c | sort -rn | head
来源：http://plo.ybcxt.top

[R52] 统计行数
来源：http://ynx.dianchejie.cn

wc -l a.txt
来源：http://tsv.ppjwa.cn

[R53] 查看文件头与实时尾
来源：http://zgg.yongpay.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://doi.aibaodan.cn

[R54] 比较两个文件
来源：http://fsw.ydjk.org.cn

diff a.txt b.txt
来源：http://nqq.guannengcc.top

[R55] 压缩与解压
来源：http://ufa.tarul.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://xqi.ppjwa.cn

[R56] 远程拷贝
来源：http://bpl.hywenlv.cn

scp file user@host:/path/
来源：http://esu.ctjpmb.com

[R57] 远程执行命令
来源：http://wiq.zycfv.cn

ssh user@host 'uptime'
来源：http://yvb.hesvh.cn

[R58] 下载文件
来源：http://sxz.aibaodan.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ifv.nwbrower.top

[R59] 发 POST JSON
来源：http://udv.ppjwa.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://pxf.shuidangran.top

[R60] 只看 HTTP 状态码
来源：http://isl.tarul.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mhm.yj20258888.top

[R61] 磁盘占用
来源：http://skt.xziqi.cn

df -h;  du -sh *
来源：http://war.redwolf501.top

[R62] 找最占空间的文件
来源：http://duh.ivvv.top

du -ah . | sort -rh | head -10
来源：http://fla.shanyushiyangkeji.top

[R63] 内存与进程
来源：http://cpa.jinyuanbaomall.cn

free -h;  ps aux | grep nginx
来源：http://xze.snrcjt.cn

[R64] 结束进程
来源：http://teu.iojbl.cn

kill -9 $(pgrep -f app.py)
来源：http://vot.ppjwa.cn

[R65] 查看端口占用
来源：http://dnx.c1oappe.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://rbs.hcnkem.com

[R66] 定时任务
来源：http://oeo.shanyushiyangtech.top

crontab -e;  crontab -l
来源：http://qvl.zhijiandao.cn

[R67] 生成随机十六进制串
来源：http://eks.jqgufenzy.top

openssl rand -hex 16
来源：http://dvm.tian-w.cn

[R68] 计算文件校验值
来源：http://tsc.meibo888.top

sha256sum a.txt;  md5sum a.txt
来源：http://lrq.smart0.xyz

[R69] 生成随机密码
来源：http://wos.cdnleiting.top

head -c 16 /dev/urandom | base64
来源：http://aeg.zhengqikj.top

[R70] 时间戳与互转
来源：http://itn.jinghuilouyu.cn

date +%s;  date -d @1700000000
来源：http://rjz.sysykeji.top

[R71] 日期格式化
来源：http://unw.kuanghao11.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://qca.wangshuangyany.cn

[R72] 等待端口就绪
来源：http://epk.zhongyouzk.top

until nc -z localhost 3306; do sleep 1; done
来源：http://wwt.xuanzx.com

[R73] 分割大日志
来源：http://pzg.jinqigfzy.top

split -l 1000 big.log part_
来源：http://uva.ydzc1.top

[R74] 批量重命名
来源：http://svq.vehdjk.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://sca.0kj1m.cn

[R75] 导出环境变量
来源：http://dkp.cheryme.top


<!-- 参考信息 -->