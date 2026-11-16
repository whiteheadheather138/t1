代发 wailian999

[Q33] 多列分组
来源：http://vwj.jinqigfzy.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://cbt.zycfv.cn

[Q34] 每组取第一条
来源：http://hzh.zycfv.cn

SELECT * FROM (
来源：http://tag.cashguo.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ywl.316326.xyz

) t WHERE rn = 1;
来源：http://cdi.jinqigfzy.top

[Q35] 内连接
来源：http://iqj.sweek.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ffc.gaohongyu789.top

[Q36] 左连接
来源：http://ggq.shzxlz.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://nbt.wangshuangyany.cn

[Q37] 右连接
来源：http://bbm.sysykeji.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://iow.havefunace.top

[Q38] 全外连接（PostgreSQL）
来源：http://cdg.kuanghao11.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://qio.sysykeji.top

[Q39] 自连接（查上下级）
来源：http://cpu.yanxiufei.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://nem.yvedp.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://kub.hammf.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://roc.havefunace.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://bgt.andypj.xyz

[Q41] 多表连接
来源：http://ifv.ydjk.org.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://svp.bbcook.cn

JOIN users u ON u.id = o.user_id
来源：http://dov.jqgufenzy.top

JOIN products p ON p.id = o.product_id;
来源：http://lag.ctjpmb.com

[Q42] 连接条件附加过滤
来源：http://fwt.havefunace.top

SELECT u.name, o.amount FROM users u
来源：http://pen.epnwcf.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mec.andypj.xyz

[Q43] 标量子查询
来源：http://evo.52xcode.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://tww.fengsongda.top

[Q44] IN 子查询
来源：http://hpg.kuanghao11.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://kpb.gaohongyu789.top

[Q45] EXISTS 判断存在
来源：http://nkb.wangshuangyany.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xvo.uphjek.com

[Q46] NOT EXISTS 判断不存在
来源：http://oob.yongpay.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vye.hesvh.cn

[Q47] 与平均值比较
来源：http://dde.ehwqpu.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://nfk.zhixingplan.top

[Q48] CTE 公用表表达式
来源：http://azw.9152youxi.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://tpl.shuidangran.top

SELECT * FROM t WHERE c > 5;
来源：http://bte.chenjidiqi.icu

[Q49] 更新单行
来源：http://wlu.chenzaomai.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://cgy.wangshuangyany.cn

[Q50] 批量更新
来源：http://vow.gogol.net.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://jsu.aizwys.cn

[Q51] 用子查询更新
来源：http://nyi.xuetiantiany.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://tby.sxryk.cn

[Q52] 删除指定行
来源：http://opo.ybcxt.top

DELETE FROM users WHERE id = 10;
来源：http://ckd.zycfv.cn

[Q53] 按条件删除
来源：http://nrk.gotoacloud.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://own.snrcjt.cn

[Q54] 清空表
来源：http://rix.zdbjq.cn

TRUNCATE TABLE logs;
来源：http://wlh.iojbl.cn

[Q55] 排名（并列占位）
来源：http://fow.xziqi.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://bfv.pengpengdd.cyou

[Q56] 密集排名（并列不占位）
来源：http://eik.nanxuanxn.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://aeg.guowangkeji.top

[Q57] 行号
来源：http://vjc.nanxinkj.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://zzz.0kj1m.cn

[Q58] 累计求和
来源：http://srd.sweek.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://efw.zhengqikj.top

[Q59] 分组内累计
来源：http://ewp.andypj.xyz

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ewl.yj20258888.top

[Q60] 取上一行 / 下一行
来源：http://lpa.hnxiangtu.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://vpf.hfpthk.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://god.epnwcf.com

[Q61] 移动平均
来源：http://lom.xingfuxueyuan.xyz

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://qkn.fanxiaobao.xyz

[Q62] 分组占比
来源：http://qur.mhx1999.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ejd.dashuyun.cn

[Q63] 开启事务
来源：http://fmp.fanxiaobao.xyz

START TRANSACTION;                -- 或 BEGIN
来源：http://zml.zdbjq.cn

[Q64] 提交事务
来源：http://don.ydjk.org.cn

COMMIT;
来源：http://tsx.fktsv.cn

[Q65] 回滚事务
来源：http://esz.fengsongda.top

ROLLBACK;
来源：http://mmi.yuanzhike.top

[Q66] 行锁查询
来源：http://ypc.bjfxy.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://fjm.gaohongyu789.top

[Q67] 设置隔离级别
来源：http://msq.hywenlv.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ats.guannengcc.top

[Q68] 保存点
来源：http://tvx.yj202588.top

SAVEPOINT sp1;
来源：http://nvh.bbcook.cn

ROLLBACK TO sp1;
来源：http://aqn.52xcode.cn

[Q69] 查看执行计划
来源：http://taa.jiagoushi.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://kde.yanxiufei.cn

[Q70] 更新统计信息
来源：http://mem.zhijiandao.cn

ANALYZE TABLE users;
来源：http://wnc.ydjk.org.cn

[Q71] 查看建表语句
来源：http://oyk.vehdjk.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://jjc.xingfuxueyuan.xyz

[Q72] 查看索引
来源：http://zih.cheryme.top

SHOW INDEX FROM users;
来源：http://iir.nwbrower.top

[Q73] 查看表状态
来源：http://lul.chenzaomai.com

SHOW TABLE STATUS LIKE 'users';
来源：http://zvs.guowangkeji.top

[Q74] 强制使用索引
来源：http://dla.yongpay.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://glu.ctjpmb.com

[Q75] 日期格式化
来源：http://hyo.zhongyouzk.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://uee.jinqigufen.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ujl.tian-w.cn

[Q76] 按天统计
来源：http://ydr.jiagoushi.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://jmf.c1oappe.top

[Q77] 时间加减
来源：http://lyf.yj20258888.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://pwr.chenjidiqi.icu

[Q78] 当前时间
来源：http://esm.9152youxi.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://rme.smart0.xyz

[Q79] 字符串拼接
来源：http://xzt.daxiang520.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://vop.xylfe.cn

[Q80] 字符串截取
来源：http://ffp.ehwqpu.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://jes.hfpthk.cn

[Q81] 字符串替换
来源：http://khd.pycfn.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://cvb.pengpengdd.cyou

[Q82] 字符长度与字节长度
来源：http://bee.meibo888.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://skt.ywan-chungtsiang.top

[Q83] 大小写转换
来源：http://slv.shangyingyoupin.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://sqp.0kj1m.cn

[Q84] 去除首尾空格
来源：http://uqk.chenjidiqi.icu

SELECT TRIM(name) FROM users;
来源：http://tcs.nwbrower.top

[Q85] 数值取整
来源：http://fkj.ybcxt.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://emb.nanxinkj.top

[Q86] 读取 JSON 字段
来源：http://exd.svipenyu.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://pgr.zhoulong.xyz

[Q87] JSON 字段做条件
来源：http://lsv.svipenyu.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://zqy.hysaishi.cn

[Q88] 行转列（条件聚合）
来源：http://vtx.bbcook.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hik.xuetiantiany.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://gop.nwbrower.top

[Q89] 判断表是否存在
来源：http://ywy.smart0.xyz

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://enr.mhx1999.top

[Q90] 生成序号列
来源：http://grc.gotoacloud.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ryo.chenjidiqi.icu

================================================================================
来源：http://wpu.shanyushiyangkeji.top

R. Bash 专题
来源：http://kny.pycfn.com

================================================================================
来源：http://acn.jqgufenzy.top

[R01] shebang 与严格模式
来源：http://zun.yj20258.top

#!/usr/bin/env bash
来源：http://rvf.jinqigfzy.top

set -euo pipefail
来源：http://fov.jlsjyb.cn

[R02] 变量赋值与使用
来源：http://mhc.ywan-chungtsiang.top

name="Tom"; echo "$name"
来源：http://fch.hnxiangtu.top

[R03] 只读变量
来源：http://fro.yvedp.cn

readonly PI=3.14
来源：http://ukl.nwbrower.top

[R04] 位置参数
来源：http://agg.birdmap.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://qfu.xuetiantiany.cn

[R05] 参数默认值
来源：http://usl.hesvh.cn

name="${1:-default}"
来源：http://rhf.ybcxt.top

[R06] 判断命令是否存在
来源：http://ahm.birdmap.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://qts.hysaishi.cn

[R07] if 判断文件
来源：http://yfk.jinghuilouyu.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://lej.jqgufenzy.top

[R08] 数值比较
来源：http://zyf.xylfe.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://reu.zdqjudy.top

[R09] 字符串比较
来源：http://xmn.ydjk.org.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://rro.c1oappe.top

[R10] 正则匹配
来源：http://hws.jinyuanbaomall.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ozj.vehdjk.com

[R11] case 多分支
来源：http://tly.nanxinkj.top

case "$1" in
来源：http://saj.jqgufenzy.top

start) echo "启动" ;;
来源：http://dpz.zdbjq.cn

stop)  echo "停止" ;;
来源：http://ncf.sufxvd.cn

*)     echo "未知命令" ;;
来源：http://obx.yfazqb.com

esac
来源：http://awd.cashguo.top

[R12] for 遍历文件
来源：http://qcs.jqgufenzy.top

for f in *.txt; do echo "$f"; done
来源：http://vng.hcnkem.com

[R13] for 计数循环
来源：http://sbq.nwbrower.top

for i in {1..10}; do echo "$i"; done
来源：http://zyy.bbcook.cn

[R14] C 风格 for
来源：http://rtg.zhijiandao.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wkj.fanxiaobao.xyz

[R15] while 逐行读文件
来源：http://bed.c1oappe.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://sus.haohaochexian.top

[R16] until 等待条件
来源：http://fad.fzhhl.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ihm.chenzaomai.com

[R17] 数组定义与取值
来源：http://woq.hammf.cn

arr=(a b c); echo "${arr[0]}"
来源：http://fkh.yfazqb.com

[R18] 遍历数组
来源：http://fyu.chenzaomai.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mkv.sweek.top

[R19] 数组长度
来源：http://ttz.uphjek.com

echo "${#arr[@]}"
来源：http://ygd.xuetiantiany.cn

[R20] 关联数组（字典）
来源：http://djk.shangyingyoupin.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ovi.bbcook.cn

[R21] 字符串长度
来源：http://zyq.shuidangran.top

echo "${#s}"
来源：http://syb.snrcjt.cn

[R22] 截取子串
来源：http://vuy.shuidangran.top

echo "${s:0:5}"
来源：http://bvu.nanxinkj.top

[R23] 字符串替换
来源：http://uxj.fzhhl.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://fhd.nanxuanxn.top

[R24] 大小写转换
来源：http://jqt.shanyushiyangkeji.top

echo "${s^^}"; echo "${s,,}"
来源：http://mob.daxiang520.top

[R25] 去后缀 / 去前缀
来源：http://opw.cqqwz.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://yve.fanxiaobao.xyz

[R26] 命令替换
来源：http://inx.dianchejie.cn

now=$(date +%F); echo "$now"
来源：http://otp.zdbjq.cn

[R27] 算术展开
来源：http://dkj.tian-w.cn

echo $((1 + 2 * 3))
来源：http://yrg.yueranfly.top

[R28] 浮点运算
来源：http://gmo.pycfn.com

echo "scale=2; 10/3" | bc
来源：http://ape.ivvv.top

[R29] 定义函数
来源：http://wfc.wangdashe.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hui.yj202588.top

[R30] 函数返回状态码
来源：http://zvx.guowangkeji.top

f() { return 0; }; f || echo "失败了"
来源：http://jol.mhx1999.top

[R31] 局部变量
来源：http://bhv.ppjwa.cn

f() { local x=1; echo "$x"; }
来源：http://css.xuanzx.com

[R32] 参数个数校验
来源：http://msq.iojbl.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mrg.jqgfzy.top

[R33] 捕获错误并提示行号
来源：http://ngw.yongpay.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mcg.ywan-chungtsiang.top

[R34] 退出时清理
来源：http://abi.hongshengwenyu.top

trap 'rm -f "$tmp"' EXIT
来源：http://mjb.snrcjt.cn

[R35] 后台执行并等待
来源：http://hfd.0kj1m.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://tlm.hcnkem.com

[R36] 并发执行多个任务
来源：http://xqv.xuetiantiany.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://uhs.ivvv.top

[R37] 把输出赋给变量
来源：http://uua.svipenyu.cn

files=$(ls -1)
来源：http://wbm.dashuyun.cn

[R38] 管道串联
来源：http://oka.gogol.net.cn

cat a.txt | grep -i error | wc -l
来源：http://ftp.c1oappe.top

[R39] 重定向标准输出与错误
来源：http://zpo.0kj1m.cn

cmd > out.log 2>&1
来源：http://dex.sweek.top

[R40] 追加写日志
来源：http://son.ivvv.top

echo "log" >> out.log
来源：http://rkl.zhiwuduotai.top

[R41] 丢弃输出
来源：http://pek.52xcode.cn

cmd >/dev/null 2>&1
来源：http://bfv.ydjk.org.cn

[R42] 输入重定向
来源：http://csf.tianlin.xyz

wc -l < a.txt
来源：http://qka.wangshuangyany.cn

[R43] 按名字查找文件
来源：http://gcv.yvedp.cn

find . -name "*.log" -type f
来源：http://bpw.haohaochexian.top

[R44] 按修改时间查找
来源：http://yzf.sxryk.cn

find . -mtime -7 -type f
来源：http://wcg.yuxming.cn

[R45] 批量删除
来源：http://ghn.tianlin.xyz

find . -name "*.tmp" -delete
来源：http://rtf.ctjpmb.com

[R46] 递归替换文件内容
来源：http://mdp.fengsongda.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://uwg.redwolf501.top

[R47] sed 单行替换
来源：http://vbz.mhx1999.top

sed -i 's/foo/bar/g' a.txt
来源：http://ujo.haohaochexian.top

[R48] awk 取指定列
来源：http://zuh.cdnleiting.top

awk '{print $1, $3}' a.txt
来源：http://kmo.jinqigufen.top

[R49] awk 带条件
来源：http://hqg.quarkkingdee.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://duc.zdbjq.cn

[R50] awk 求和
来源：http://fnh.gzhubu.top

awk '{s += $2} END {print s}' a.txt
来源：http://jly.redwolf501.top

[R51] 排序去重取前几
来源：http://uvo.nanxinkj.top

sort a.txt | uniq -c | sort -rn | head
来源：http://nkb.shanyushiyangkeji.top

[R52] 统计行数
来源：http://nyd.sxryk.cn

wc -l a.txt
来源：http://fve.fehbvm.com

[R53] 查看文件头与实时尾
来源：http://rrb.tanke756.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://iij.sxryk.cn

[R54] 比较两个文件
来源：http://lwq.yj20258888.top

diff a.txt b.txt
来源：http://wfd.pengpengdd.cyou

[R55] 压缩与解压
来源：http://lev.hcnkem.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://rkl.yj20258.top

[R56] 远程拷贝
来源：http://cxa.9152youxi.cn

scp file user@host:/path/
来源：http://nuf.hcnkem.com

[R57] 远程执行命令
来源：http://pjd.fktsv.cn

ssh user@host 'uptime'
来源：http://ogm.birdmap.top

[R58] 下载文件
来源：http://ohk.guannengcc.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://cql.xziqi.cn

[R59] 发 POST JSON
来源：http://gjv.zhiwuduotai.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://dsd.yj20258888.top

[R60] 只看 HTTP 状态码
来源：http://mmr.0kj1m.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mps.tarul.cn

[R61] 磁盘占用
来源：http://rws.dashuyun.cn

df -h;  du -sh *
来源：http://vjn.yueranfly.top

[R62] 找最占空间的文件
来源：http://ndb.nwbrower.top

du -ah . | sort -rh | head -10
来源：http://eut.tian-w.cn

[R63] 内存与进程
来源：http://frj.smart0.xyz

free -h;  ps aux | grep nginx
来源：http://nbn.yj202588.top

[R64] 结束进程
来源：http://yvb.tian-w.cn

kill -9 $(pgrep -f app.py)
来源：http://jeh.ydzc1.top

[R65] 查看端口占用
来源：http://wjo.yfazqb.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://pjf.redwolf501.top

[R66] 定时任务
来源：http://kgj.hfpthk.cn

crontab -e;  crontab -l
来源：http://imf.ppjwa.cn

[R67] 生成随机十六进制串
来源：http://tor.c1oappe.top

openssl rand -hex 16
来源：http://vlo.fktsv.cn

[R68] 计算文件校验值
来源：http://msw.jianghu66.top

sha256sum a.txt;  md5sum a.txt
来源：http://row.hywenlv.cn

[R69] 生成随机密码
来源：http://opo.ppjwa.cn

head -c 16 /dev/urandom | base64
来源：http://ewp.xuetiantiany.cn

[R70] 时间戳与互转
来源：http://gao.yj202588.top

date +%s;  date -d @1700000000
来源：http://fnh.andypj.xyz

[R71] 日期格式化
来源：http://dfs.tanke756.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://yko.cqqwz.cn

[R72] 等待端口就绪
来源：http://jtn.jyoumei.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://mtl.zhiwuduotai.top

[R73] 分割大日志
来源：http://hjt.shanyushiyangtech.top

split -l 1000 big.log part_
来源：http://aic.yuxming.cn

[R74] 批量重命名
来源：http://yqi.hesvh.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mcg.dianchejie.cn

[R75] 导出环境变量
来源：http://gkx.hongshengwenyu.top

export PATH="$HOME/bin:$PATH"
来源：http://daq.sufxvd.cn

[R76] 使用临时文件
来源：http://kar.shzxlz.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://tnz.feifeiyinyue.top

[R77] 读取用户输入
来源：http://pvu.jlsjyb.cn

read -rp "请输入: " ans
来源：http://whc.havefunace.top

[R78] 交互式菜单
来源：http://nwn.smart0.xyz

select opt in a b c; do echo "$opt"; break; done
来源：http://qxo.hysaishi.cn

[R79] 解析命令行选项
来源：http://irn.xziqi.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://gpf.hongshengwenyu.top

[R80] 查看脚本执行耗时
来源：http://xuw.zdqjudy.top

time ./run.sh
来源：http://rkb.hnxiangtu.top

================================================================================
来源：http://ftt.quarkkingdee.top

S. C / C++ 专题
来源：http://scz.hysaishi.cn

================================================================================
来源：http://rgt.uphjek.com

[S01] C：Hello World
来源：http://kak.birdmap.top

#include <stdio.h>
来源：http://ezq.gaohongyu789.top


<!-- 参考信息 -->