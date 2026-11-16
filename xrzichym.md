代发 wailian999

[Q33] 多列分组
来源：http://jex.vehdjk.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://jaj.shzxlz.cn

[Q34] 每组取第一条
来源：http://nlr.zhongyouzk.top

SELECT * FROM (
来源：http://tyc.jyoumei.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://pvw.tianlin.xyz

) t WHERE rn = 1;
来源：http://wir.tian-w.cn

[Q35] 内连接
来源：http://xnd.jqgfzy.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://eza.vehdjk.com

[Q36] 左连接
来源：http://zer.zycfv.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://djn.shanyushiyangkeji.top

[Q37] 右连接
来源：http://glw.yvedp.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://jlt.guannengcc.top

[Q38] 全外连接（PostgreSQL）
来源：http://siy.meibo888.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wzg.hcnkem.com

[Q39] 自连接（查上下级）
来源：http://kjo.yfazqb.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://sro.pycfn.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://kzn.gotoacloud.top

[Q40] 交叉连接（笛卡尔积）
来源：http://qjp.zhengqikj.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://tgs.smart0.xyz

[Q41] 多表连接
来源：http://kwu.vehdjk.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://cks.ctjpmb.com

JOIN users u ON u.id = o.user_id
来源：http://ryz.zhengqikj.top

JOIN products p ON p.id = o.product_id;
来源：http://swe.shuidangran.top

[Q42] 连接条件附加过滤
来源：http://uhy.nanxuanxn.top

SELECT u.name, o.amount FROM users u
来源：http://bba.hywenlv.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hno.smart0.xyz

[Q43] 标量子查询
来源：http://azn.9152youxi.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hax.shanyushiyangkeji.top

[Q44] IN 子查询
来源：http://ewc.gogol.net.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://buo.zhoulong.xyz

[Q45] EXISTS 判断存在
来源：http://auf.ppjwa.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://pbs.vehdjk.com

[Q46] NOT EXISTS 判断不存在
来源：http://zno.zhaomingkeji.xyz

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vmc.zdqjudy.top

[Q47] 与平均值比较
来源：http://kyo.ppjwa.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://jfa.xziqi.cn

[Q48] CTE 公用表表达式
来源：http://rzq.sxryk.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://urt.hongshengwenyu.top

SELECT * FROM t WHERE c > 5;
来源：http://pup.daria6918.cn

[Q49] 更新单行
来源：http://nck.chenlongwang.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://cdt.zhiwuduotai.top

[Q50] 批量更新
来源：http://rpy.hongshengwenyu.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://lwd.zdqjudy.top

[Q51] 用子查询更新
来源：http://kkh.aibaodan.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ffg.hammf.cn

[Q52] 删除指定行
来源：http://fyk.zycfv.cn

DELETE FROM users WHERE id = 10;
来源：http://xbt.shanyushiyangkeji.top

[Q53] 按条件删除
来源：http://nqm.xziqi.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://rdi.mhx1999.top

[Q54] 清空表
来源：http://wwn.yuxming.cn

TRUNCATE TABLE logs;
来源：http://wwi.zdqjudy.top

[Q55] 排名（并列占位）
来源：http://ezc.sweek.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://sxz.ehwqpu.com

[Q56] 密集排名（并列不占位）
来源：http://uuw.xingfuxueyuan.xyz

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://jqr.daria6918.cn

[Q57] 行号
来源：http://ybd.9152youxi.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://cmj.jiagoushi.top

[Q58] 累计求和
来源：http://lhp.yangfankeji.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://qlh.shanyushiyangtech.top

[Q59] 分组内累计
来源：http://wly.yangfankeji.com

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://auy.ctjpmb.com

[Q60] 取上一行 / 下一行
来源：http://iyn.jinqigfzy.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://vpi.wangdashe.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://haa.zhengqikj.top

[Q61] 移动平均
来源：http://iue.iojbl.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://dwa.xingfuxueyuan.xyz

[Q62] 分组占比
来源：http://zst.yueranfly.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://rkb.tianlin.xyz

[Q63] 开启事务
来源：http://raw.ivvv.top

START TRANSACTION;                -- 或 BEGIN
来源：http://rpd.gotoacloud.top

[Q64] 提交事务
来源：http://gzn.xuetiantiany.cn

COMMIT;
来源：http://bsl.fktsv.cn

[Q65] 回滚事务
来源：http://nbf.ydjk.org.cn

ROLLBACK;
来源：http://koy.quarkkingdee.top

[Q66] 行锁查询
来源：http://lgg.nwbrower.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://nlp.ywan-chungtsiang.top

[Q67] 设置隔离级别
来源：http://tdk.svipenyu.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://zhg.nanxuanxn.top

[Q68] 保存点
来源：http://jll.wangdashe.top

SAVEPOINT sp1;
来源：http://yla.c1oappe.top

ROLLBACK TO sp1;
来源：http://ute.bbcook.cn

[Q69] 查看执行计划
来源：http://dpz.jiagoushi.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://jna.gotoacloud.top

[Q70] 更新统计信息
来源：http://coy.xuanzx.com

ANALYZE TABLE users;
来源：http://raa.zhoulong.xyz

[Q71] 查看建表语句
来源：http://gno.chenjidiqi.icu

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://zkr.bjfxy.top

[Q72] 查看索引
来源：http://jsr.wangdashe.top

SHOW INDEX FROM users;
来源：http://tfl.gaohongyu789.top

[Q73] 查看表状态
来源：http://dch.0kj1m.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://doe.chenjidiqi.icu

[Q74] 强制使用索引
来源：http://ags.svipenyu.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wqn.zdqjudy.top

[Q75] 日期格式化
来源：http://gbw.jinqigfzy.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://nby.fengsongda.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://vjh.hammf.cn

[Q76] 按天统计
来源：http://fwy.ivvv.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://nnw.pycfn.com

[Q77] 时间加减
来源：http://ooy.sjlbkw.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://qcw.hesvh.cn

[Q78] 当前时间
来源：http://gjx.nanxuanxn.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hid.yanxiufei.cn

[Q79] 字符串拼接
来源：http://gmj.hfpthk.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://plw.yueranfly.top

[Q80] 字符串截取
来源：http://fax.yj202588.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://lgr.dianchejie.cn

[Q81] 字符串替换
来源：http://tqw.ybcxt.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://phr.havefunace.top

[Q82] 字符长度与字节长度
来源：http://xts.jinqigfzy.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ozf.shanyushiyangkeji.top

[Q83] 大小写转换
来源：http://iio.gzhubu.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://aph.tanke756.top

[Q84] 去除首尾空格
来源：http://zjh.meibo888.top

SELECT TRIM(name) FROM users;
来源：http://pbi.sjlbkw.cn

[Q85] 数值取整
来源：http://ixy.jinqigufen.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wjk.yvedp.cn

[Q86] 读取 JSON 字段
来源：http://xwj.feifeiyinyue.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://omk.jqgfzy.top

[Q87] JSON 字段做条件
来源：http://qeg.sweek.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://zfv.ydjk.org.cn

[Q88] 行转列（条件聚合）
来源：http://szn.shanyushiyangkeji.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://pwh.yfazqb.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://gom.xziqi.cn

[Q89] 判断表是否存在
来源：http://ege.yuanzhike.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ybi.xingfuxueyuan.xyz

[Q90] 生成序号列
来源：http://rqo.vqdsnc.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://oot.feifeiyinyue.top

================================================================================
来源：http://nlc.yonumen.top

R. Bash 专题
来源：http://cyc.yj202588.top

================================================================================
来源：http://sar.yueranfly.top

[R01] shebang 与严格模式
来源：http://hni.c1oappe.top

#!/usr/bin/env bash
来源：http://hif.hcnkem.com

set -euo pipefail
来源：http://qds.xuetiantiany.cn

[R02] 变量赋值与使用
来源：http://isa.fehbvm.com

name="Tom"; echo "$name"
来源：http://tho.daxiang520.top

[R03] 只读变量
来源：http://rua.yanxiufei.cn

readonly PI=3.14
来源：http://clb.havefunace.top

[R04] 位置参数
来源：http://ous.snrcjt.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://lyi.hesvh.cn

[R05] 参数默认值
来源：http://yaf.haohaochexian.top

name="${1:-default}"
来源：http://vwi.cheryme.top

[R06] 判断命令是否存在
来源：http://nas.yj20258888.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://tym.xinyue.icu

[R07] if 判断文件
来源：http://grv.yonumen.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://vhd.sysykeji.top

[R08] 数值比较
来源：http://mws.redwolf501.top

if (( a > b )); then echo "a 更大"; fi
来源：http://ayz.yanxiufei.cn

[R09] 字符串比较
来源：http://bjg.daria6918.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://rpe.sxryk.cn

[R10] 正则匹配
来源：http://hke.meibo888.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://jjt.iojbl.cn

[R11] case 多分支
来源：http://fdt.jinqigufen.top

case "$1" in
来源：http://hax.yj202588.top

start) echo "启动" ;;
来源：http://zgm.xinyue.icu

stop)  echo "停止" ;;
来源：http://hhl.zdqjudy.top

*)     echo "未知命令" ;;
来源：http://gdx.yj202588.top

esac
来源：http://iyi.gzhubu.top

[R12] for 遍历文件
来源：http://fed.zhaomingkeji.xyz

for f in *.txt; do echo "$f"; done
来源：http://ucj.hnxiangtu.top

[R13] for 计数循环
来源：http://gmv.snrcjt.cn

for i in {1..10}; do echo "$i"; done
来源：http://san.zhiwuduotai.top

[R14] C 风格 for
来源：http://ppx.hongshengwenyu.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://tlb.guannengcc.top

[R15] while 逐行读文件
来源：http://xmo.yueranfly.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ewf.guowangkeji.top

[R16] until 等待条件
来源：http://xmd.jinqigfzy.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://bgq.uphjek.com

[R17] 数组定义与取值
来源：http://dcf.fehbvm.com

arr=(a b c); echo "${arr[0]}"
来源：http://nqd.vqdsnc.cn

[R18] 遍历数组
来源：http://bwl.yuanzhike.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://cqo.dashuyun.cn

[R19] 数组长度
来源：http://nef.yueranfly.top

echo "${#arr[@]}"
来源：http://pyv.fehbvm.com

[R20] 关联数组（字典）
来源：http://eoz.pengpengdd.cyou

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://uhu.jlsjyb.cn

[R21] 字符串长度
来源：http://cdk.yuxming.cn

echo "${#s}"
来源：http://ftn.tanke756.top

[R22] 截取子串
来源：http://kwh.chenzaomai.com

echo "${s:0:5}"
来源：http://qqs.gogol.net.cn

[R23] 字符串替换
来源：http://unz.jinqigufen.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://oph.xuanzx.com

[R24] 大小写转换
来源：http://gqy.hywenlv.cn

echo "${s^^}"; echo "${s,,}"
来源：http://sro.xuanzx.com

[R25] 去后缀 / 去前缀
来源：http://hqk.yonumen.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://ljn.zdbjq.cn

[R26] 命令替换
来源：http://uwd.svipenyu.cn

now=$(date +%F); echo "$now"
来源：http://inm.dianchejie.cn

[R27] 算术展开
来源：http://tic.fengsongda.top

echo $((1 + 2 * 3))
来源：http://gzx.ctjpmb.com

[R28] 浮点运算
来源：http://fmp.wangdashe.top

echo "scale=2; 10/3" | bc
来源：http://yqj.vqdsnc.cn

[R29] 定义函数
来源：http://wky.fzhhl.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://duy.haohaochexian.top

[R30] 函数返回状态码
来源：http://cjd.cheryme.top

f() { return 0; }; f || echo "失败了"
来源：http://kqo.shanyushiyangtech.top

[R31] 局部变量
来源：http://vfm.zycfv.cn

f() { local x=1; echo "$x"; }
来源：http://wni.jiagoushi.top

[R32] 参数个数校验
来源：http://udm.daria6918.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ijn.c1oappe.top

[R33] 捕获错误并提示行号
来源：http://zuk.ydzc1.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://naw.yuanzhike.top

[R34] 退出时清理
来源：http://lsz.ppjwa.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ptj.zhijiandao.cn

[R35] 后台执行并等待
来源：http://mpg.ywan-chungtsiang.top

sleep 5 & pid=$!; wait "$pid"
来源：http://kst.yj20258.top

[R36] 并发执行多个任务
来源：http://uty.zhijiandao.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wdl.hongshengwenyu.top

[R37] 把输出赋给变量
来源：http://res.quarkkingdee.top

files=$(ls -1)
来源：http://nrb.fanxiaobao.xyz

[R38] 管道串联
来源：http://ztn.chenjidiqi.icu

cat a.txt | grep -i error | wc -l
来源：http://rae.fengsongda.top

[R39] 重定向标准输出与错误
来源：http://oar.guannengcc.top

cmd > out.log 2>&1
来源：http://bir.fehbvm.com

[R40] 追加写日志
来源：http://hrd.fanxiaobao.xyz

echo "log" >> out.log
来源：http://nfh.shuidangran.top

[R41] 丢弃输出
来源：http://ebd.redwolf501.top

cmd >/dev/null 2>&1
来源：http://spo.nanxuanxn.top

[R42] 输入重定向
来源：http://ioh.sweek.top

wc -l < a.txt
来源：http://upn.yj20258.top

[R43] 按名字查找文件
来源：http://iyh.shanyushiyangtech.top

find . -name "*.log" -type f
来源：http://bsa.fzhhl.top

[R44] 按修改时间查找
来源：http://guy.zdbjq.cn

find . -mtime -7 -type f
来源：http://rhf.zhiwuduotai.top

[R45] 批量删除
来源：http://hra.yfazqb.com

find . -name "*.tmp" -delete
来源：http://xla.shzxlz.cn

[R46] 递归替换文件内容
来源：http://cfc.cdnleiting.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ihi.iojbl.cn

[R47] sed 单行替换
来源：http://xnc.xuetiantiany.cn

sed -i 's/foo/bar/g' a.txt
来源：http://xbv.jinghuilouyu.cn

[R48] awk 取指定列
来源：http://dza.sufxvd.cn

awk '{print $1, $3}' a.txt
来源：http://une.gaohongyu789.top

[R49] awk 带条件
来源：http://nqw.hcnkem.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://xja.aibaodan.cn

[R50] awk 求和
来源：http://dxj.chenlongwang.top

awk '{s += $2} END {print s}' a.txt
来源：http://kgp.fzhhl.top

[R51] 排序去重取前几
来源：http://dai.ivvv.top

sort a.txt | uniq -c | sort -rn | head
来源：http://ics.nanxinkj.top

[R52] 统计行数
来源：http://zhr.dianchejie.cn

wc -l a.txt
来源：http://lqi.sweek.top

[R53] 查看文件头与实时尾
来源：http://tde.hongshengwenyu.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://aqq.ppjwa.cn

[R54] 比较两个文件
来源：http://jhj.fengsongda.top

diff a.txt b.txt
来源：http://akz.zhiwuduotai.top

[R55] 压缩与解压
来源：http://hee.zdqjudy.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://dia.chenjidiqi.icu

[R56] 远程拷贝
来源：http://jxs.guowangkeji.top

scp file user@host:/path/
来源：http://yeg.xingfuxueyuan.xyz

[R57] 远程执行命令
来源：http://ogf.nanxuanxn.top

ssh user@host 'uptime'
来源：http://xhd.wangdashe.top

[R58] 下载文件
来源：http://iup.yfazqb.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://xwn.bjfxy.top

[R59] 发 POST JSON
来源：http://mfa.cdnleiting.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://bdc.xuanzx.com

[R60] 只看 HTTP 状态码
来源：http://qmq.daria6918.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://iwd.bbcook.cn

[R61] 磁盘占用
来源：http://mic.nanxuanxn.top

df -h;  du -sh *
来源：http://rmh.epnwcf.com

[R62] 找最占空间的文件
来源：http://gav.yanxiufei.cn

du -ah . | sort -rh | head -10
来源：http://ehs.cashguo.top

[R63] 内存与进程
来源：http://tjz.52xcode.cn

free -h;  ps aux | grep nginx
来源：http://obe.9152youxi.cn

[R64] 结束进程
来源：http://gad.aibaodan.cn

kill -9 $(pgrep -f app.py)
来源：http://yex.mhx1999.top

[R65] 查看端口占用
来源：http://eia.andypj.xyz

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://els.shuidangran.top

[R66] 定时任务
来源：http://qor.fzhhl.top

crontab -e;  crontab -l
来源：http://bng.tanke756.top

[R67] 生成随机十六进制串
来源：http://rpr.ydjk.org.cn

openssl rand -hex 16
来源：http://obe.hongshengwenyu.top

[R68] 计算文件校验值
来源：http://xqs.shuidangran.top

sha256sum a.txt;  md5sum a.txt
来源：http://ebj.yj202588.top

[R69] 生成随机密码
来源：http://vir.havefunace.top

head -c 16 /dev/urandom | base64
来源：http://skk.havefunace.top

[R70] 时间戳与互转
来源：http://fnh.tarul.cn

date +%s;  date -d @1700000000
来源：http://gtf.hywenlv.cn

[R71] 日期格式化
来源：http://sae.zhengqikj.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://vhw.aibaodan.cn

[R72] 等待端口就绪
来源：http://qhr.guowangkeji.top

until nc -z localhost 3306; do sleep 1; done
来源：http://pax.yuxming.cn

[R73] 分割大日志
来源：http://tot.yuxming.cn

split -l 1000 big.log part_
来源：http://eqp.fanxiaobao.xyz

[R74] 批量重命名
来源：http://arr.kuanghao11.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://gjn.hfpthk.cn

[R75] 导出环境变量
来源：http://azg.0kj1m.cn

export PATH="$HOME/bin:$PATH"
来源：http://fsn.xuanzx.com

[R76] 使用临时文件
来源：http://buu.yuxming.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://plb.tarul.cn

[R77] 读取用户输入
来源：http://ofr.ivvv.top

read -rp "请输入: " ans
来源：http://rvr.jqgufenzy.top

[R78] 交互式菜单
来源：http://xdw.daria6918.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://qtt.cdnleiting.top

[R79] 解析命令行选项
来源：http://abh.yj20258.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://jav.wangshuangyany.cn

[R80] 查看脚本执行耗时
来源：http://gwj.zhijiandao.cn

time ./run.sh
来源：http://ixk.dianchejie.cn

================================================================================
来源：http://rnc.gogol.net.cn

S. C / C++ 专题
来源：http://asd.nanxinkj.top

================================================================================
来源：http://ppy.guannengcc.top

[S01] C：Hello World
来源：http://ler.bjfxy.top

#include <stdio.h>
来源：http://mhf.tarul.cn


<!-- 参考信息 -->