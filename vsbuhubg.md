代发 wailian999

SELECT MAX(age), MIN(age) FROM users;
来源：http://onx.wangdashe.top

[Q30] 分组统计
来源：http://xne.tarul.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ito.hammf.cn

[Q31] 分组后过滤
来源：http://fmo.bbcook.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://khr.vqdsnc.cn

[Q32] 分组拼接字符串
来源：http://xes.iojbl.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://xyt.nanxinkj.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mpk.xuetiantiany.cn

[Q33] 多列分组
来源：http://nyl.pycfn.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://spq.fzhhl.top

[Q34] 每组取第一条
来源：http://enw.sysykeji.top

SELECT * FROM (
来源：http://ntl.jqgufenzy.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mci.hfpthk.cn

) t WHERE rn = 1;
来源：http://xmj.yangfankeji.com

[Q35] 内连接
来源：http://zrd.52xcode.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://gwr.cheryme.top

[Q36] 左连接
来源：http://nwe.ydzc1.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://yza.jinqigfzy.top

[Q37] 右连接
来源：http://wup.nanxinkj.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mfk.hammf.cn

[Q38] 全外连接（PostgreSQL）
来源：http://opw.chenjidiqi.icu

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://dso.ehwqpu.com

[Q39] 自连接（查上下级）
来源：http://bmh.yj20258.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://keb.yj20258.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ytv.tarul.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://rgn.xziqi.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://pwr.bbcook.cn

[Q41] 多表连接
来源：http://wtb.yongpay.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://lnc.svipenyu.cn

JOIN users u ON u.id = o.user_id
来源：http://pme.sweek.top

JOIN products p ON p.id = o.product_id;
来源：http://vtq.shuidangran.top

[Q42] 连接条件附加过滤
来源：http://acb.jinyuanbaomall.cn

SELECT u.name, o.amount FROM users u
来源：http://dvd.xylfe.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://xrs.nanxuanxn.top

[Q43] 标量子查询
来源：http://fff.zycfv.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ylf.guowangkeji.top

[Q44] IN 子查询
来源：http://gok.quarkkingdee.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://fnu.zycfv.cn

[Q45] EXISTS 判断存在
来源：http://jvx.yangfankeji.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kpc.fehbvm.com

[Q46] NOT EXISTS 判断不存在
来源：http://oxg.chenjidiqi.icu

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hiq.yonumen.top

[Q47] 与平均值比较
来源：http://vfh.aizwys.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://skp.iojbl.cn

[Q48] CTE 公用表表达式
来源：http://hdf.chenlongwang.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://sga.zdbjq.cn

SELECT * FROM t WHERE c > 5;
来源：http://men.andypj.xyz

[Q49] 更新单行
来源：http://iei.fktsv.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://nmk.jianghu66.top

[Q50] 批量更新
来源：http://rcc.nanxinkj.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://bzn.jiagoushi.top

[Q51] 用子查询更新
来源：http://ikq.9152youxi.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hkz.haohaochexian.top

[Q52] 删除指定行
来源：http://frb.zdqjudy.top

DELETE FROM users WHERE id = 10;
来源：http://lxx.ctjpmb.com

[Q53] 按条件删除
来源：http://qaw.meibo888.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ley.zycfv.cn

[Q54] 清空表
来源：http://gjw.yanxiufei.cn

TRUNCATE TABLE logs;
来源：http://wpp.daria6918.cn

[Q55] 排名（并列占位）
来源：http://ufb.zycfv.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://xit.hysaishi.cn

[Q56] 密集排名（并列不占位）
来源：http://xmg.snrcjt.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://zvz.guannengcc.top

[Q57] 行号
来源：http://ylt.zhixingplan.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://pgz.316326.xyz

[Q58] 累计求和
来源：http://veq.nwbrower.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wql.meibo888.top

[Q59] 分组内累计
来源：http://vtd.tarul.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://szi.fengsongda.top

[Q60] 取上一行 / 下一行
来源：http://pty.yj202588.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://vxj.pengpengdd.cyou

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://qeb.feifeiyinyue.top

[Q61] 移动平均
来源：http://sxd.gaohongyu789.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://qrs.fzhhl.top

[Q62] 分组占比
来源：http://xrd.tanke756.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://zzm.dianchejie.cn

[Q63] 开启事务
来源：http://qdv.haohaochexian.top

START TRANSACTION;                -- 或 BEGIN
来源：http://kpt.9152youxi.cn

[Q64] 提交事务
来源：http://bhb.feifeiyinyue.top

COMMIT;
来源：http://plx.birdmap.top

[Q65] 回滚事务
来源：http://zoc.zhaomingkeji.xyz

ROLLBACK;
来源：http://mwf.yongpay.top

[Q66] 行锁查询
来源：http://lgc.cdnleiting.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://oys.ywan-chungtsiang.top

[Q67] 设置隔离级别
来源：http://yye.hnqzz.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://cuk.shuidangran.top

[Q68] 保存点
来源：http://pil.cdnleiting.top

SAVEPOINT sp1;
来源：http://lor.dianchejie.cn

ROLLBACK TO sp1;
来源：http://fjh.mhx1999.top

[Q69] 查看执行计划
来源：http://udh.hongshengwenyu.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ael.yuanzhike.top

[Q70] 更新统计信息
来源：http://wwk.316326.xyz

ANALYZE TABLE users;
来源：http://vcq.shzxlz.cn

[Q71] 查看建表语句
来源：http://sak.0kj1m.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://yyk.zhaomingkeji.xyz

[Q72] 查看索引
来源：http://wry.pengpengdd.cyou

SHOW INDEX FROM users;
来源：http://uvt.cucudq.cn

[Q73] 查看表状态
来源：http://inv.bjfxy.top

SHOW TABLE STATUS LIKE 'users';
来源：http://bvz.jinqigfzy.top

[Q74] 强制使用索引
来源：http://yhg.ivvv.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://omd.gogol.net.cn

[Q75] 日期格式化
来源：http://tju.0kj1m.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://cko.yueranfly.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://bnx.52xcode.cn

[Q76] 按天统计
来源：http://eah.sufxvd.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mxc.pycfn.com

[Q77] 时间加减
来源：http://tzl.xinyue.icu

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ygx.gogol.net.cn

[Q78] 当前时间
来源：http://uxo.jianghu66.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://yrt.sjlbkw.cn

[Q79] 字符串拼接
来源：http://dls.jinqigufen.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://uyx.zhoulong.xyz

[Q80] 字符串截取
来源：http://shi.nanxinkj.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://rwj.hammf.cn

[Q81] 字符串替换
来源：http://cyz.zhijiandao.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wtg.jinqigfzy.top

[Q82] 字符长度与字节长度
来源：http://jws.hfpthk.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mzb.sweek.top

[Q83] 大小写转换
来源：http://dog.cashguo.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://kys.tarul.cn

[Q84] 去除首尾空格
来源：http://ecj.yueranfly.top

SELECT TRIM(name) FROM users;
来源：http://jti.zycfv.cn

[Q85] 数值取整
来源：http://jxd.snrcjt.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://rba.cashguo.top

[Q86] 读取 JSON 字段
来源：http://whf.xylfe.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://nhg.ywan-chungtsiang.top

[Q87] JSON 字段做条件
来源：http://hqj.andypj.xyz

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://jai.vqdsnc.cn

[Q88] 行转列（条件聚合）
来源：http://ecb.gogol.net.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://kxd.shanyushiyangtech.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://nzv.cashguo.top

[Q89] 判断表是否存在
来源：http://toq.wangdashe.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ane.meibo888.top

[Q90] 生成序号列
来源：http://wic.yj20258.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://cdi.havefunace.top

================================================================================
来源：http://col.yuanzhike.top

R. Bash 专题
来源：http://ufn.jinyuanbaomall.cn

================================================================================
来源：http://txl.cashguo.top

[R01] shebang 与严格模式
来源：http://dvh.epnwcf.com

#!/usr/bin/env bash
来源：http://nfr.hnqzz.top

set -euo pipefail
来源：http://ukb.havefunace.top

[R02] 变量赋值与使用
来源：http://mie.shuidangran.top

name="Tom"; echo "$name"
来源：http://nzd.uphjek.com

[R03] 只读变量
来源：http://gzj.sjlbkw.cn

readonly PI=3.14
来源：http://mxv.zhaomingkeji.xyz

[R04] 位置参数
来源：http://qzj.hywenlv.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://faf.yj202588.top

[R05] 参数默认值
来源：http://avq.cdnleiting.top

name="${1:-default}"
来源：http://eqz.yuxming.cn

[R06] 判断命令是否存在
来源：http://pwb.daxiang520.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://euq.yanxiufei.cn

[R07] if 判断文件
来源：http://his.tianlin.xyz

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://qvg.smart0.xyz

[R08] 数值比较
来源：http://lzx.sxryk.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://sjc.shanyushiyangtech.top

[R09] 字符串比较
来源：http://xvj.ctjpmb.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://zrv.yonumen.top

[R10] 正则匹配
来源：http://jic.gaohongyu789.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://jhw.gaohongyu789.top

[R11] case 多分支
来源：http://oep.epnwcf.com

case "$1" in
来源：http://fgk.zhijiandao.cn

start) echo "启动" ;;
来源：http://yra.fanxiaobao.xyz

stop)  echo "停止" ;;
来源：http://htq.yj20258.top

*)     echo "未知命令" ;;
来源：http://pqd.yfazqb.com

esac
来源：http://egz.hnxiangtu.top

[R12] for 遍历文件
来源：http://roy.shanyushiyangkeji.top

for f in *.txt; do echo "$f"; done
来源：http://uhp.yj202588.top

[R13] for 计数循环
来源：http://xrd.shangyingyoupin.top

for i in {1..10}; do echo "$i"; done
来源：http://sae.feifeiyinyue.top

[R14] C 风格 for
来源：http://wut.bjfxy.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://qiw.ctjpmb.com

[R15] while 逐行读文件
来源：http://bfb.guannengcc.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://fqb.sjlbkw.cn

[R16] until 等待条件
来源：http://aha.chenzaomai.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wlq.chenzaomai.com

[R17] 数组定义与取值
来源：http://xcg.vehdjk.com

arr=(a b c); echo "${arr[0]}"
来源：http://udv.ppjwa.cn

[R18] 遍历数组
来源：http://fdw.yanxiufei.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://rkh.316326.xyz

[R19] 数组长度
来源：http://oia.sufxvd.cn

echo "${#arr[@]}"
来源：http://zdb.hesvh.cn

[R20] 关联数组（字典）
来源：http://byx.jyoumei.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ijj.yonumen.top

[R21] 字符串长度
来源：http://zqs.ehwqpu.com

echo "${#s}"
来源：http://zyi.shuidangran.top

[R22] 截取子串
来源：http://yhw.xingfuxueyuan.xyz

echo "${s:0:5}"
来源：http://xxb.yongpay.top

[R23] 字符串替换
来源：http://ckv.gzhubu.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://jlf.xuanzx.com

[R24] 大小写转换
来源：http://tgd.zdqjudy.top

echo "${s^^}"; echo "${s,,}"
来源：http://bgn.feifeiyinyue.top

[R25] 去后缀 / 去前缀
来源：http://mvf.dashuyun.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://gwp.cucudq.cn

[R26] 命令替换
来源：http://mmi.nwbrower.top

now=$(date +%F); echo "$now"
来源：http://gtf.tianlin.xyz

[R27] 算术展开
来源：http://ucm.chenzaomai.com

echo $((1 + 2 * 3))
来源：http://ort.zdqjudy.top

[R28] 浮点运算
来源：http://uel.zycfv.cn

echo "scale=2; 10/3" | bc
来源：http://xhy.52xcode.cn

[R29] 定义函数
来源：http://nlp.dianchejie.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mcc.pengpengdd.cyou

[R30] 函数返回状态码
来源：http://bjj.vehdjk.com

f() { return 0; }; f || echo "失败了"
来源：http://hth.c1oappe.top

[R31] 局部变量
来源：http://vas.fengsongda.top

f() { local x=1; echo "$x"; }
来源：http://ifg.fehbvm.com

[R32] 参数个数校验
来源：http://mta.dashuyun.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://qug.ydjk.org.cn

[R33] 捕获错误并提示行号
来源：http://unk.mhx1999.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hdp.nanxuanxn.top

[R34] 退出时清理
来源：http://phd.fzhhl.top

trap 'rm -f "$tmp"' EXIT
来源：http://yhc.nanxinkj.top

[R35] 后台执行并等待
来源：http://nxx.sjlbkw.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://soh.wangdashe.top

[R36] 并发执行多个任务
来源：http://jmb.fengsongda.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://thu.chenzaomai.com

[R37] 把输出赋给变量
来源：http://qsm.52xcode.cn

files=$(ls -1)
来源：http://jgq.pycfn.com

[R38] 管道串联
来源：http://pik.hesvh.cn

cat a.txt | grep -i error | wc -l
来源：http://rjc.hesvh.cn

[R39] 重定向标准输出与错误
来源：http://jab.shangyingyoupin.top

cmd > out.log 2>&1
来源：http://ziu.pycfn.com

[R40] 追加写日志
来源：http://ljg.ehwqpu.com

echo "log" >> out.log
来源：http://hog.yj20258888.top

[R41] 丢弃输出
来源：http://nqd.hysaishi.cn

cmd >/dev/null 2>&1
来源：http://sma.shzxlz.cn

[R42] 输入重定向
来源：http://vjt.hammf.cn

wc -l < a.txt
来源：http://dvh.ctjpmb.com

[R43] 按名字查找文件
来源：http://oek.tian-w.cn

find . -name "*.log" -type f
来源：http://clp.pycfn.com

[R44] 按修改时间查找
来源：http://oyq.zhaomingkeji.xyz

find . -mtime -7 -type f
来源：http://bjk.hnxiangtu.top

[R45] 批量删除
来源：http://bsy.ybcxt.top

find . -name "*.tmp" -delete
来源：http://lzf.zhiwuduotai.top

[R46] 递归替换文件内容
来源：http://pyb.zdqjudy.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wbv.ctjpmb.com

[R47] sed 单行替换
来源：http://dys.cqqwz.cn

sed -i 's/foo/bar/g' a.txt
来源：http://llm.daria6918.cn

[R48] awk 取指定列
来源：http://hnx.daria6918.cn

awk '{print $1, $3}' a.txt
来源：http://kyy.zhoulong.xyz

[R49] awk 带条件
来源：http://gvb.sysykeji.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://tep.snrcjt.cn

[R50] awk 求和
来源：http://wmu.kuanghao11.cn

awk '{s += $2} END {print s}' a.txt
来源：http://axf.hammf.cn

[R51] 排序去重取前几
来源：http://nlh.jinqigfzy.top

sort a.txt | uniq -c | sort -rn | head
来源：http://eoj.birdmap.top

[R52] 统计行数
来源：http://avg.feifeiyinyue.top

wc -l a.txt
来源：http://wus.jinqigfzy.top

[R53] 查看文件头与实时尾
来源：http://hmq.jqgfzy.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://uig.sysykeji.top

[R54] 比较两个文件
来源：http://pwr.pycfn.com

diff a.txt b.txt
来源：http://xbz.hnqzz.top

[R55] 压缩与解压
来源：http://kql.epnwcf.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://bca.chenzaomai.com

[R56] 远程拷贝
来源：http://dnl.jinyuanbaomall.cn

scp file user@host:/path/
来源：http://hfo.fanxiaobao.xyz

[R57] 远程执行命令
来源：http://pnx.vehdjk.com

ssh user@host 'uptime'
来源：http://uve.jianghu66.top

[R58] 下载文件
来源：http://hrh.fengsongda.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://tcy.hfpthk.cn

[R59] 发 POST JSON
来源：http://qnm.zhongyouzk.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://art.cheryme.top

[R60] 只看 HTTP 状态码
来源：http://sqz.jinqigufen.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://may.hfpthk.cn

[R61] 磁盘占用
来源：http://qha.dashuyun.cn

df -h;  du -sh *
来源：http://ogq.jlsjyb.cn

[R62] 找最占空间的文件
来源：http://gpx.nwbrower.top

du -ah . | sort -rh | head -10
来源：http://jky.yj202588.top

[R63] 内存与进程
来源：http://joj.ydzc1.top

free -h;  ps aux | grep nginx
来源：http://tdu.pycfn.com

[R64] 结束进程
来源：http://wjj.zhoulong.xyz

kill -9 $(pgrep -f app.py)
来源：http://ipu.smart0.xyz

[R65] 查看端口占用
来源：http://jwm.ybcxt.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://boa.dianchejie.cn

[R66] 定时任务
来源：http://jaz.zhiwuduotai.top

crontab -e;  crontab -l
来源：http://aow.xylfe.cn

[R67] 生成随机十六进制串
来源：http://mxl.meibo888.top

openssl rand -hex 16
来源：http://nib.9152youxi.cn

[R68] 计算文件校验值
来源：http://jxi.iojbl.cn

sha256sum a.txt;  md5sum a.txt
来源：http://yzc.yfazqb.com

[R69] 生成随机密码
来源：http://rpa.yuanzhike.top

head -c 16 /dev/urandom | base64
来源：http://gto.yvedp.cn

[R70] 时间戳与互转
来源：http://wph.yfazqb.com

date +%s;  date -d @1700000000
来源：http://lqp.ydjk.org.cn

[R71] 日期格式化
来源：http://ncq.jqgfzy.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://irn.sjlbkw.cn

[R72] 等待端口就绪
来源：http://mkh.ehwqpu.com

until nc -z localhost 3306; do sleep 1; done
来源：http://wvg.yueranfly.top

[R73] 分割大日志
来源：http://dka.shangyingyoupin.top

split -l 1000 big.log part_
来源：http://duv.52xcode.cn

[R74] 批量重命名
来源：http://adw.shzxlz.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://kbp.gaohongyu789.top

[R75] 导出环境变量
来源：http://hkp.quarkkingdee.top

export PATH="$HOME/bin:$PATH"
来源：http://wcg.hnxiangtu.top

[R76] 使用临时文件
来源：http://ogu.nanxuanxn.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://znk.nanxinkj.top

[R77] 读取用户输入
来源：http://qov.pengpengdd.cyou

read -rp "请输入: " ans
来源：http://tyo.shanyushiyangkeji.top

[R78] 交互式菜单
来源：http://xsa.sxryk.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://hjn.zdqjudy.top

[R79] 解析命令行选项
来源：http://kwl.iojbl.cn


<!-- 参考信息 -->