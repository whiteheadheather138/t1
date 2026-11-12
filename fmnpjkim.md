代发 wailian999

[Q33] 多列分组
来源：http://gbs.ppjwa.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://cua.daria6918.cn

[Q34] 每组取第一条
来源：http://luz.yj202588.top

SELECT * FROM (
来源：http://ffp.zhixingplan.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hif.zycfv.cn

) t WHERE rn = 1;
来源：http://joh.jianghu66.top

[Q35] 内连接
来源：http://sek.chenlongwang.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://xyr.shanyushiyangtech.top

[Q36] 左连接
来源：http://fjo.meibo888.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://lri.wangdashe.top

[Q37] 右连接
来源：http://loa.guannengcc.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hnu.aibaodan.cn

[Q38] 全外连接（PostgreSQL）
来源：http://aao.hfpthk.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://yqn.zhixingplan.top

[Q39] 自连接（查上下级）
来源：http://pxv.hnqzz.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://abc.hesvh.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://dpb.gzhubu.top

[Q40] 交叉连接（笛卡尔积）
来源：http://grz.zhengqikj.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://jno.jinyuanbaomall.cn

[Q41] 多表连接
来源：http://kds.guannengcc.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://bsb.xingfuxueyuan.xyz

JOIN users u ON u.id = o.user_id
来源：http://vaw.ydzc1.top

JOIN products p ON p.id = o.product_id;
来源：http://vok.dashuyun.cn

[Q42] 连接条件附加过滤
来源：http://euu.hammf.cn

SELECT u.name, o.amount FROM users u
来源：http://inx.zhijiandao.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hou.hongshengwenyu.top

[Q43] 标量子查询
来源：http://mpj.xylfe.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://vwo.gotoacloud.top

[Q44] IN 子查询
来源：http://ejv.jiagoushi.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://bgf.xuetiantiany.cn

[Q45] EXISTS 判断存在
来源：http://qcm.haohaochexian.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://eif.tarul.cn

[Q46] NOT EXISTS 判断不存在
来源：http://zqt.316326.xyz

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bmw.jiagoushi.top

[Q47] 与平均值比较
来源：http://tqw.nwbrower.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ver.gaohongyu789.top

[Q48] CTE 公用表表达式
来源：http://dnd.guowangkeji.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://qus.pengpengdd.cyou

SELECT * FROM t WHERE c > 5;
来源：http://fbg.yuxming.cn

[Q49] 更新单行
来源：http://ohb.fengsongda.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ugp.hesvh.cn

[Q50] 批量更新
来源：http://ttf.guannengcc.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://xco.ydjk.org.cn

[Q51] 用子查询更新
来源：http://uce.jinghuilouyu.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://vcf.cdnleiting.top

[Q52] 删除指定行
来源：http://jmq.nanxinkj.top

DELETE FROM users WHERE id = 10;
来源：http://khl.zdbjq.cn

[Q53] 按条件删除
来源：http://ntz.cucudq.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://khw.pycfn.com

[Q54] 清空表
来源：http://sro.jqgufenzy.top

TRUNCATE TABLE logs;
来源：http://ilq.jqgfzy.top

[Q55] 排名（并列占位）
来源：http://aec.zhixingplan.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://qlp.yfazqb.com

[Q56] 密集排名（并列不占位）
来源：http://ujq.jinyuanbaomall.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://urz.iojbl.cn

[Q57] 行号
来源：http://wve.yvedp.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://oqd.ybcxt.top

[Q58] 累计求和
来源：http://vwl.bbcook.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://lfc.bbcook.cn

[Q59] 分组内累计
来源：http://xja.hywenlv.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://lrv.iojbl.cn

[Q60] 取上一行 / 下一行
来源：http://dca.hesvh.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://jvm.yonumen.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://soa.ybcxt.top

[Q61] 移动平均
来源：http://iqb.yj202588.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ajz.zhiwuduotai.top

[Q62] 分组占比
来源：http://rog.cucudq.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://kpx.zhongyouzk.top

[Q63] 开启事务
来源：http://zhg.fktsv.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://uvy.tanke756.top

[Q64] 提交事务
来源：http://daq.bjfxy.top

COMMIT;
来源：http://yxw.ehwqpu.com

[Q65] 回滚事务
来源：http://pvt.gaohongyu789.top

ROLLBACK;
来源：http://orv.c1oappe.top

[Q66] 行锁查询
来源：http://luf.hesvh.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mvt.xylfe.cn

[Q67] 设置隔离级别
来源：http://qae.shuidangran.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://pvz.feifeiyinyue.top

[Q68] 保存点
来源：http://sek.snrcjt.cn

SAVEPOINT sp1;
来源：http://gzp.pengpengdd.cyou

ROLLBACK TO sp1;
来源：http://rzv.zhijiandao.cn

[Q69] 查看执行计划
来源：http://blq.fengsongda.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://agr.smart0.xyz

[Q70] 更新统计信息
来源：http://ixr.fehbvm.com

ANALYZE TABLE users;
来源：http://qib.shzxlz.cn

[Q71] 查看建表语句
来源：http://qss.hcnkem.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://qqq.zhixingplan.top

[Q72] 查看索引
来源：http://cej.ydzc1.top

SHOW INDEX FROM users;
来源：http://ywf.tian-w.cn

[Q73] 查看表状态
来源：http://kcr.smart0.xyz

SHOW TABLE STATUS LIKE 'users';
来源：http://nux.iojbl.cn

[Q74] 强制使用索引
来源：http://ggy.dashuyun.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ias.chenjidiqi.icu

[Q75] 日期格式化
来源：http://nns.zhoulong.xyz

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://oau.0kj1m.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://zov.mhx1999.top

[Q76] 按天统计
来源：http://wjz.dashuyun.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://cqv.cashguo.top

[Q77] 时间加减
来源：http://nww.andypj.xyz

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://jal.hammf.cn

[Q78] 当前时间
来源：http://bwd.zycfv.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://uia.hammf.cn

[Q79] 字符串拼接
来源：http://sts.sysykeji.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://yeg.sufxvd.cn

[Q80] 字符串截取
来源：http://ggo.tian-w.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://czu.guannengcc.top

[Q81] 字符串替换
来源：http://bmh.ivvv.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hij.9152youxi.cn

[Q82] 字符长度与字节长度
来源：http://vdh.bjfxy.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ilc.gogol.net.cn

[Q83] 大小写转换
来源：http://fti.bbcook.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://tzi.ybcxt.top

[Q84] 去除首尾空格
来源：http://kff.feifeiyinyue.top

SELECT TRIM(name) FROM users;
来源：http://qzn.quarkkingdee.top

[Q85] 数值取整
来源：http://yxk.yueranfly.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://abx.yj20258.top

[Q86] 读取 JSON 字段
来源：http://wfb.bbcook.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://tqa.gogol.net.cn

[Q87] JSON 字段做条件
来源：http://qqo.jqgfzy.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://vmi.xziqi.cn

[Q88] 行转列（条件聚合）
来源：http://xeg.ivvv.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://feu.iojbl.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://fdi.sysykeji.top

[Q89] 判断表是否存在
来源：http://nji.yj20258888.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://rog.yanxiufei.cn

[Q90] 生成序号列
来源：http://osb.zdqjudy.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://zyv.zhixingplan.top

================================================================================
来源：http://aal.zhongyouzk.top

R. Bash 专题
来源：http://zck.gogol.net.cn

================================================================================
来源：http://nok.hammf.cn

[R01] shebang 与严格模式
来源：http://sti.ybcxt.top

#!/usr/bin/env bash
来源：http://idx.jqgufenzy.top

set -euo pipefail
来源：http://gsm.shanyushiyangtech.top

[R02] 变量赋值与使用
来源：http://exw.vehdjk.com

name="Tom"; echo "$name"
来源：http://zux.yongpay.top

[R03] 只读变量
来源：http://xcj.vqdsnc.cn

readonly PI=3.14
来源：http://rde.mhx1999.top

[R04] 位置参数
来源：http://ggk.redwolf501.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://pzg.zdbjq.cn

[R05] 参数默认值
来源：http://mnj.jlsjyb.cn

name="${1:-default}"
来源：http://lxi.gogol.net.cn

[R06] 判断命令是否存在
来源：http://tdz.chenzaomai.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://rty.jinyuanbaomall.cn

[R07] if 判断文件
来源：http://ydp.shzxlz.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://nsd.shuidangran.top

[R08] 数值比较
来源：http://ejc.tianlin.xyz

if (( a > b )); then echo "a 更大"; fi
来源：http://hrg.hysaishi.cn

[R09] 字符串比较
来源：http://riw.pycfn.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://qso.tanke756.top

[R10] 正则匹配
来源：http://zly.dashuyun.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://rac.316326.xyz

[R11] case 多分支
来源：http://nwp.yuxming.cn

case "$1" in
来源：http://hrk.birdmap.top

start) echo "启动" ;;
来源：http://txs.0kj1m.cn

stop)  echo "停止" ;;
来源：http://yty.dashuyun.cn

*)     echo "未知命令" ;;
来源：http://dnr.wangshuangyany.cn

esac
来源：http://dab.sxryk.cn

[R12] for 遍历文件
来源：http://lyw.mhx1999.top

for f in *.txt; do echo "$f"; done
来源：http://dtr.ybcxt.top

[R13] for 计数循环
来源：http://iua.zhengqikj.top

for i in {1..10}; do echo "$i"; done
来源：http://uvq.shzxlz.cn

[R14] C 风格 for
来源：http://liu.gaohongyu789.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://qfr.ivvv.top

[R15] while 逐行读文件
来源：http://fhf.svipenyu.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://xlb.wangdashe.top

[R16] until 等待条件
来源：http://jif.wangshuangyany.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://cep.gzhubu.top

[R17] 数组定义与取值
来源：http://kxc.fzhhl.top

arr=(a b c); echo "${arr[0]}"
来源：http://laz.uphjek.com

[R18] 遍历数组
来源：http://peb.xinyue.icu

for x in "${arr[@]}"; do echo "$x"; done
来源：http://jiy.9152youxi.cn

[R19] 数组长度
来源：http://kcm.shuidangran.top

echo "${#arr[@]}"
来源：http://rhx.jinyuanbaomall.cn

[R20] 关联数组（字典）
来源：http://yfs.yj20258888.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://why.chenzaomai.com

[R21] 字符串长度
来源：http://csl.gzhubu.top

echo "${#s}"
来源：http://wob.yuxming.cn

[R22] 截取子串
来源：http://guw.jqgufenzy.top

echo "${s:0:5}"
来源：http://ldz.cqqwz.cn

[R23] 字符串替换
来源：http://tep.c1oappe.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://rzu.nwbrower.top

[R24] 大小写转换
来源：http://vru.zdbjq.cn

echo "${s^^}"; echo "${s,,}"
来源：http://pdf.ctjpmb.com

[R25] 去后缀 / 去前缀
来源：http://koe.hnqzz.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://pmz.aizwys.cn

[R26] 命令替换
来源：http://kik.zhijiandao.cn

now=$(date +%F); echo "$now"
来源：http://gjl.shzxlz.cn

[R27] 算术展开
来源：http://wbt.tanke756.top

echo $((1 + 2 * 3))
来源：http://wpi.xuetiantiany.cn

[R28] 浮点运算
来源：http://aus.daxiang520.top

echo "scale=2; 10/3" | bc
来源：http://koz.daxiang520.top

[R29] 定义函数
来源：http://lwx.jlsjyb.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://aim.shanyushiyangtech.top

[R30] 函数返回状态码
来源：http://nfk.ydzc1.top

f() { return 0; }; f || echo "失败了"
来源：http://xhi.chenlongwang.top

[R31] 局部变量
来源：http://xpw.daria6918.cn

f() { local x=1; echo "$x"; }
来源：http://eiv.shuidangran.top

[R32] 参数个数校验
来源：http://acm.jinqigfzy.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://vqb.xinyue.icu

[R33] 捕获错误并提示行号
来源：http://tmv.fzhhl.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://lev.jyoumei.cn

[R34] 退出时清理
来源：http://jxi.shanyushiyangtech.top

trap 'rm -f "$tmp"' EXIT
来源：http://xua.vqdsnc.cn

[R35] 后台执行并等待
来源：http://vid.fzhhl.top

sleep 5 & pid=$!; wait "$pid"
来源：http://ami.jinqigfzy.top

[R36] 并发执行多个任务
来源：http://wsq.ivvv.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://rhq.jinqigufen.top

[R37] 把输出赋给变量
来源：http://paa.chenjidiqi.icu

files=$(ls -1)
来源：http://ygo.fanxiaobao.xyz

[R38] 管道串联
来源：http://mlw.jinqigfzy.top

cat a.txt | grep -i error | wc -l
来源：http://cly.hongshengwenyu.top

[R39] 重定向标准输出与错误
来源：http://rxc.yongpay.top

cmd > out.log 2>&1
来源：http://ndq.yj20258.top

[R40] 追加写日志
来源：http://wbd.haohaochexian.top

echo "log" >> out.log
来源：http://rss.daria6918.cn

[R41] 丢弃输出
来源：http://sjw.hesvh.cn

cmd >/dev/null 2>&1
来源：http://npb.havefunace.top

[R42] 输入重定向
来源：http://jax.fengsongda.top

wc -l < a.txt
来源：http://ovt.316326.xyz

[R43] 按名字查找文件
来源：http://ann.c1oappe.top

find . -name "*.log" -type f
来源：http://nqv.chenlongwang.top

[R44] 按修改时间查找
来源：http://exa.yfazqb.com

find . -mtime -7 -type f
来源：http://tud.vqdsnc.cn

[R45] 批量删除
来源：http://jsg.fehbvm.com

find . -name "*.tmp" -delete
来源：http://shq.cashguo.top

[R46] 递归替换文件内容
来源：http://fwq.haohaochexian.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mms.jinyuanbaomall.cn

[R47] sed 单行替换
来源：http://qac.xylfe.cn

sed -i 's/foo/bar/g' a.txt
来源：http://qjw.yfazqb.com

[R48] awk 取指定列
来源：http://frx.sweek.top

awk '{print $1, $3}' a.txt
来源：http://xsj.yfazqb.com

[R49] awk 带条件
来源：http://tat.yj20258.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ezp.feifeiyinyue.top

[R50] awk 求和
来源：http://spy.birdmap.top

awk '{s += $2} END {print s}' a.txt
来源：http://yqq.dashuyun.cn

[R51] 排序去重取前几
来源：http://gij.sjlbkw.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://nws.c1oappe.top

[R52] 统计行数
来源：http://jgn.bjfxy.top

wc -l a.txt
来源：http://gop.hcnkem.com

[R53] 查看文件头与实时尾
来源：http://bhl.yanxiufei.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://zye.dashuyun.cn

[R54] 比较两个文件
来源：http://uro.bbcook.cn

diff a.txt b.txt
来源：http://krw.xziqi.cn

[R55] 压缩与解压
来源：http://bvm.yonumen.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://yft.wangdashe.top

[R56] 远程拷贝
来源：http://wlb.hnqzz.top

scp file user@host:/path/
来源：http://grr.fengsongda.top

[R57] 远程执行命令
来源：http://jce.ybcxt.top

ssh user@host 'uptime'
来源：http://pdk.chenjidiqi.icu

[R58] 下载文件
来源：http://ang.snrcjt.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://dvd.cheryme.top

[R59] 发 POST JSON
来源：http://whk.jinqigfzy.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ytm.fzhhl.top

[R60] 只看 HTTP 状态码
来源：http://bde.xinyue.icu

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://xtm.meibo888.top

[R61] 磁盘占用
来源：http://zvk.shanyushiyangtech.top

df -h;  du -sh *
来源：http://nae.yj20258888.top

[R62] 找最占空间的文件
来源：http://hjb.ctjpmb.com

du -ah . | sort -rh | head -10
来源：http://zdn.wangshuangyany.cn

[R63] 内存与进程
来源：http://glq.jqgfzy.top

free -h;  ps aux | grep nginx
来源：http://qag.bbcook.cn

[R64] 结束进程
来源：http://hjt.jinqigufen.top

kill -9 $(pgrep -f app.py)
来源：http://bym.hnxiangtu.top

[R65] 查看端口占用
来源：http://dyz.tianlin.xyz

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://tqm.yj20258888.top

[R66] 定时任务
来源：http://zgr.quarkkingdee.top

crontab -e;  crontab -l
来源：http://qbs.zhixingplan.top

[R67] 生成随机十六进制串
来源：http://aai.jianghu66.top

openssl rand -hex 16
来源：http://bla.quarkkingdee.top

[R68] 计算文件校验值
来源：http://vdl.nwbrower.top

sha256sum a.txt;  md5sum a.txt
来源：http://jvd.redwolf501.top

[R69] 生成随机密码
来源：http://znz.ivvv.top

head -c 16 /dev/urandom | base64
来源：http://ats.fktsv.cn

[R70] 时间戳与互转
来源：http://oxz.wangshuangyany.cn

date +%s;  date -d @1700000000
来源：http://nrm.svipenyu.cn

[R71] 日期格式化
来源：http://idc.jiagoushi.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://ckq.nanxuanxn.top

[R72] 等待端口就绪
来源：http://cql.iojbl.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://buw.zdbjq.cn

[R73] 分割大日志
来源：http://cfh.bjfxy.top

split -l 1000 big.log part_
来源：http://saw.epnwcf.com

[R74] 批量重命名
来源：http://nck.jlsjyb.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hmk.zhixingplan.top

[R75] 导出环境变量
来源：http://esv.nanxuanxn.top

export PATH="$HOME/bin:$PATH"
来源：http://yur.yj20258.top

[R76] 使用临时文件
来源：http://yys.fanxiaobao.xyz

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://maw.tarul.cn

[R77] 读取用户输入
来源：http://wyt.sufxvd.cn

read -rp "请输入: " ans
来源：http://roz.tarul.cn

[R78] 交互式菜单
来源：http://upq.0kj1m.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://hgj.cqqwz.cn

[R79] 解析命令行选项
来源：http://uuh.yonumen.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://fsu.hesvh.cn

[R80] 查看脚本执行耗时
来源：http://drs.yvedp.cn

time ./run.sh
来源：http://iei.vehdjk.com

================================================================================
来源：http://tyi.zhoulong.xyz

S. C / C++ 专题
来源：http://zbu.shuidangran.top

================================================================================
来源：http://tlj.hysaishi.cn

[S01] C：Hello World
来源：http://dgz.yj202588.top

#include <stdio.h>
来源：http://dju.xylfe.cn


<!-- 参考信息 -->