代发 wailian999

[Q36] 左连接
来源：http://cgj.jinghuilouyu.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hok.xinyue.icu

[Q37] 右连接
来源：http://txg.aizwys.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://muj.wangdashe.top

[Q38] 全外连接（PostgreSQL）
来源：http://rhu.hysaishi.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://csl.nanxinkj.top

[Q39] 自连接（查上下级）
来源：http://daz.ivvv.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://mor.mhx1999.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ptn.hysaishi.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://xfj.yuanzhike.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ssm.ydzc1.top

[Q41] 多表连接
来源：http://eqd.ivvv.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://chy.tian-w.cn

JOIN users u ON u.id = o.user_id
来源：http://jgw.hfpthk.cn

JOIN products p ON p.id = o.product_id;
来源：http://nfe.shuidangran.top

[Q42] 连接条件附加过滤
来源：http://wzy.xuetiantiany.cn

SELECT u.name, o.amount FROM users u
来源：http://xoj.sweek.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ykv.shzxlz.cn

[Q43] 标量子查询
来源：http://miz.shanyushiyangtech.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://imh.jinqigfzy.top

[Q44] IN 子查询
来源：http://bhv.c1oappe.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://zqt.vqdsnc.cn

[Q45] EXISTS 判断存在
来源：http://tqi.svipenyu.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://iik.cucudq.cn

[Q46] NOT EXISTS 判断不存在
来源：http://lpn.zhixingplan.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ucs.zhiwuduotai.top

[Q47] 与平均值比较
来源：http://tfr.0kj1m.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ryf.zhoulong.xyz

[Q48] CTE 公用表表达式
来源：http://sqs.shanyushiyangtech.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mgx.snrcjt.cn

SELECT * FROM t WHERE c > 5;
来源：http://gep.zhiwuduotai.top

[Q49] 更新单行
来源：http://rxu.tanke756.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://iqf.ivvv.top

[Q50] 批量更新
来源：http://zqm.sxryk.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://xda.hywenlv.cn

[Q51] 用子查询更新
来源：http://szz.yj20258.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://sql.jinqigufen.top

[Q52] 删除指定行
来源：http://qsc.xziqi.cn

DELETE FROM users WHERE id = 10;
来源：http://uzv.vqdsnc.cn

[Q53] 按条件删除
来源：http://gcu.c1oappe.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://kjr.aibaodan.cn

[Q54] 清空表
来源：http://dbh.uphjek.com

TRUNCATE TABLE logs;
来源：http://jcn.epnwcf.com

[Q55] 排名（并列占位）
来源：http://jum.gogol.net.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hvq.aizwys.cn

[Q56] 密集排名（并列不占位）
来源：http://nos.nanxinkj.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://brt.gogol.net.cn

[Q57] 行号
来源：http://bim.sysykeji.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://cwo.cqqwz.cn

[Q58] 累计求和
来源：http://ali.bbcook.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ogy.yvedp.cn

[Q59] 分组内累计
来源：http://bwq.ydjk.org.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://rra.snrcjt.cn

[Q60] 取上一行 / 下一行
来源：http://ild.hcnkem.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wkd.yanxiufei.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://olt.bjfxy.top

[Q61] 移动平均
来源：http://bmc.cucudq.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://epf.nwbrower.top

[Q62] 分组占比
来源：http://dec.tarul.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://liy.shangyingyoupin.top

[Q63] 开启事务
来源：http://iyv.epnwcf.com

START TRANSACTION;                -- 或 BEGIN
来源：http://vft.zhongyouzk.top

[Q64] 提交事务
来源：http://wmf.zhixingplan.top

COMMIT;
来源：http://ijx.cashguo.top

[Q65] 回滚事务
来源：http://xtf.ppjwa.cn

ROLLBACK;
来源：http://lir.ydjk.org.cn

[Q66] 行锁查询
来源：http://qgd.zhiwuduotai.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://xxm.jianghu66.top

[Q67] 设置隔离级别
来源：http://cfp.jiagoushi.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://idw.fktsv.cn

[Q68] 保存点
来源：http://kjw.xinyue.icu

SAVEPOINT sp1;
来源：http://eow.chenlongwang.top

ROLLBACK TO sp1;
来源：http://aro.fanxiaobao.xyz

[Q69] 查看执行计划
来源：http://ghf.tianlin.xyz

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://eja.zdqjudy.top

[Q70] 更新统计信息
来源：http://ijy.jinghuilouyu.cn

ANALYZE TABLE users;
来源：http://zop.9152youxi.cn

[Q71] 查看建表语句
来源：http://nhm.xuetiantiany.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://zel.dianchejie.cn

[Q72] 查看索引
来源：http://kxe.fengsongda.top

SHOW INDEX FROM users;
来源：http://jln.sufxvd.cn

[Q73] 查看表状态
来源：http://adf.haohaochexian.top

SHOW TABLE STATUS LIKE 'users';
来源：http://mbp.jyoumei.cn

[Q74] 强制使用索引
来源：http://ktp.ivvv.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://zmk.ydjk.org.cn

[Q75] 日期格式化
来源：http://zpx.pengpengdd.cyou

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://bpg.jyoumei.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://scg.zhaomingkeji.xyz

[Q76] 按天统计
来源：http://jyf.hongshengwenyu.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://yig.iojbl.cn

[Q77] 时间加减
来源：http://rxq.redwolf501.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://fbs.0kj1m.cn

[Q78] 当前时间
来源：http://kar.jqgfzy.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://lzp.uphjek.com

[Q79] 字符串拼接
来源：http://obq.cqqwz.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://gtc.jqgufenzy.top

[Q80] 字符串截取
来源：http://pjd.yuanzhike.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://kvo.yuanzhike.top

[Q81] 字符串替换
来源：http://vnr.cdnleiting.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ykp.yonumen.top

[Q82] 字符长度与字节长度
来源：http://smj.birdmap.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://dub.hesvh.cn

[Q83] 大小写转换
来源：http://axt.daxiang520.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mld.chenjidiqi.icu

[Q84] 去除首尾空格
来源：http://szp.yj202588.top

SELECT TRIM(name) FROM users;
来源：http://rjd.smart0.xyz

[Q85] 数值取整
来源：http://ckc.hywenlv.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ceh.ppjwa.cn

[Q86] 读取 JSON 字段
来源：http://edo.quarkkingdee.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://voc.ctjpmb.com

[Q87] JSON 字段做条件
来源：http://yaa.xylfe.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hsj.jqgufenzy.top

[Q88] 行转列（条件聚合）
来源：http://vlk.meibo888.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://kpm.jinyuanbaomall.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://dry.xziqi.cn

[Q89] 判断表是否存在
来源：http://vyf.9152youxi.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://xmt.redwolf501.top

[Q90] 生成序号列
来源：http://czs.bbcook.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://tiz.smart0.xyz

================================================================================
来源：http://rcs.zdqjudy.top

R. Bash 专题
来源：http://zqf.hnqzz.top

================================================================================
来源：http://knc.tianlin.xyz

[R01] shebang 与严格模式
来源：http://acx.tanke756.top

#!/usr/bin/env bash
来源：http://byg.quarkkingdee.top

set -euo pipefail
来源：http://jmy.andypj.xyz

[R02] 变量赋值与使用
来源：http://wvb.cucudq.cn

name="Tom"; echo "$name"
来源：http://nla.yanxiufei.cn

[R03] 只读变量
来源：http://eku.jlsjyb.cn

readonly PI=3.14
来源：http://wvy.hfpthk.cn

[R04] 位置参数
来源：http://lbp.uphjek.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://kcd.hnxiangtu.top

[R05] 参数默认值
来源：http://jwa.fzhhl.top

name="${1:-default}"
来源：http://gjn.hcnkem.com

[R06] 判断命令是否存在
来源：http://dat.wangshuangyany.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://xop.svipenyu.cn

[R07] if 判断文件
来源：http://rjz.shuidangran.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://itv.sysykeji.top

[R08] 数值比较
来源：http://ecw.hnxiangtu.top

if (( a > b )); then echo "a 更大"; fi
来源：http://jvz.jqgfzy.top

[R09] 字符串比较
来源：http://arx.cucudq.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://onx.gaohongyu789.top

[R10] 正则匹配
来源：http://lkg.dianchejie.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ymc.yanxiufei.cn

[R11] case 多分支
来源：http://fdi.sjlbkw.cn

case "$1" in
来源：http://yet.tarul.cn

start) echo "启动" ;;
来源：http://xbd.havefunace.top

stop)  echo "停止" ;;
来源：http://aev.chenjidiqi.icu

*)     echo "未知命令" ;;
来源：http://dxu.hesvh.cn

esac
来源：http://orx.sweek.top

[R12] for 遍历文件
来源：http://qed.sweek.top

for f in *.txt; do echo "$f"; done
来源：http://gfo.hongshengwenyu.top

[R13] for 计数循环
来源：http://apt.cqqwz.cn

for i in {1..10}; do echo "$i"; done
来源：http://wwv.hesvh.cn

[R14] C 风格 for
来源：http://anu.aibaodan.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://nqw.yanxiufei.cn

[R15] while 逐行读文件
来源：http://byw.shangyingyoupin.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://lev.xylfe.cn

[R16] until 等待条件
来源：http://okx.c1oappe.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://pqc.gogol.net.cn

[R17] 数组定义与取值
来源：http://joy.cashguo.top

arr=(a b c); echo "${arr[0]}"
来源：http://cam.9152youxi.cn

[R18] 遍历数组
来源：http://quj.zhaomingkeji.xyz

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ctn.sysykeji.top

[R19] 数组长度
来源：http://bui.nanxinkj.top

echo "${#arr[@]}"
来源：http://ebz.hesvh.cn

[R20] 关联数组（字典）
来源：http://nlh.gogol.net.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://xpq.chenjidiqi.icu

[R21] 字符串长度
来源：http://jld.yuxming.cn

echo "${#s}"
来源：http://hkp.ehwqpu.com

[R22] 截取子串
来源：http://yyj.birdmap.top

echo "${s:0:5}"
来源：http://wyc.shanyushiyangtech.top

[R23] 字符串替换
来源：http://ncj.ehwqpu.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ikf.yuxming.cn

[R24] 大小写转换
来源：http://rme.bjfxy.top

echo "${s^^}"; echo "${s,,}"
来源：http://zjv.zhoulong.xyz

[R25] 去后缀 / 去前缀
来源：http://hsv.jqgufenzy.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://iqa.cashguo.top

[R26] 命令替换
来源：http://qhf.tanke756.top

now=$(date +%F); echo "$now"
来源：http://fku.9152youxi.cn

[R27] 算术展开
来源：http://xmp.jlsjyb.cn

echo $((1 + 2 * 3))
来源：http://edg.zycfv.cn

[R28] 浮点运算
来源：http://okz.fktsv.cn

echo "scale=2; 10/3" | bc
来源：http://ibj.birdmap.top

[R29] 定义函数
来源：http://wsf.sxryk.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://rla.haohaochexian.top

[R30] 函数返回状态码
来源：http://lpe.yuxming.cn

f() { return 0; }; f || echo "失败了"
来源：http://bvh.chenzaomai.com

[R31] 局部变量
来源：http://nms.hfpthk.cn

f() { local x=1; echo "$x"; }
来源：http://csi.zhaomingkeji.xyz

[R32] 参数个数校验
来源：http://ple.hnxiangtu.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://oge.iojbl.cn

[R33] 捕获错误并提示行号
来源：http://rmk.hnxiangtu.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ngc.hammf.cn

[R34] 退出时清理
来源：http://zqk.cucudq.cn

trap 'rm -f "$tmp"' EXIT
来源：http://iml.xingfuxueyuan.xyz

[R35] 后台执行并等待
来源：http://jvt.ppjwa.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://dqn.jyoumei.cn

[R36] 并发执行多个任务
来源：http://sfp.zdbjq.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://csm.hnqzz.top

[R37] 把输出赋给变量
来源：http://pjh.shuidangran.top

files=$(ls -1)
来源：http://fpi.kuanghao11.cn

[R38] 管道串联
来源：http://vhv.iojbl.cn

cat a.txt | grep -i error | wc -l
来源：http://jqg.316326.xyz

[R39] 重定向标准输出与错误
来源：http://tqs.iojbl.cn

cmd > out.log 2>&1
来源：http://vuo.daxiang520.top

[R40] 追加写日志
来源：http://kcx.nanxuanxn.top

echo "log" >> out.log
来源：http://qdj.cqqwz.cn

[R41] 丢弃输出
来源：http://pbm.gotoacloud.top

cmd >/dev/null 2>&1
来源：http://tjq.tian-w.cn

[R42] 输入重定向
来源：http://ryl.cqqwz.cn

wc -l < a.txt
来源：http://sty.sweek.top

[R43] 按名字查找文件
来源：http://uya.pycfn.com

find . -name "*.log" -type f
来源：http://ybo.jinqigfzy.top

[R44] 按修改时间查找
来源：http://wff.pycfn.com

find . -mtime -7 -type f
来源：http://kpj.meibo888.top

[R45] 批量删除
来源：http://plm.bjfxy.top

find . -name "*.tmp" -delete
来源：http://fmi.jinghuilouyu.cn

[R46] 递归替换文件内容
来源：http://ukc.chenjidiqi.icu

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://kdx.ppjwa.cn

[R47] sed 单行替换
来源：http://vnm.tanke756.top

sed -i 's/foo/bar/g' a.txt
来源：http://atz.pycfn.com

[R48] awk 取指定列
来源：http://lps.daxiang520.top

awk '{print $1, $3}' a.txt
来源：http://wzq.xylfe.cn

[R49] awk 带条件
来源：http://pog.xinyue.icu

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wlx.9152youxi.cn

[R50] awk 求和
来源：http://bnd.aibaodan.cn

awk '{s += $2} END {print s}' a.txt
来源：http://qfv.shzxlz.cn

[R51] 排序去重取前几
来源：http://czs.vehdjk.com

sort a.txt | uniq -c | sort -rn | head
来源：http://xaq.hfpthk.cn

[R52] 统计行数
来源：http://bpt.wangdashe.top

wc -l a.txt
来源：http://ogv.wangshuangyany.cn

[R53] 查看文件头与实时尾
来源：http://ilv.hesvh.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://qsp.tian-w.cn

[R54] 比较两个文件
来源：http://uud.zhiwuduotai.top

diff a.txt b.txt
来源：http://amp.ybcxt.top

[R55] 压缩与解压
来源：http://iiy.hongshengwenyu.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://peh.zhengqikj.top

[R56] 远程拷贝
来源：http://nvt.52xcode.cn

scp file user@host:/path/
来源：http://snj.bbcook.cn

[R57] 远程执行命令
来源：http://cqb.52xcode.cn

ssh user@host 'uptime'
来源：http://ctu.zycfv.cn

[R58] 下载文件
来源：http://iun.jinghuilouyu.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://bso.zdqjudy.top

[R59] 发 POST JSON
来源：http://unz.aizwys.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ejp.jianghu66.top

[R60] 只看 HTTP 状态码
来源：http://syk.meibo888.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://pms.fengsongda.top

[R61] 磁盘占用
来源：http://icc.sjlbkw.cn

df -h;  du -sh *
来源：http://wpz.zhongyouzk.top

[R62] 找最占空间的文件
来源：http://sdn.xingfuxueyuan.xyz

du -ah . | sort -rh | head -10
来源：http://ufi.sjlbkw.cn

[R63] 内存与进程
来源：http://iqh.shangyingyoupin.top

free -h;  ps aux | grep nginx
来源：http://rkf.jinqigufen.top

[R64] 结束进程
来源：http://fme.jlsjyb.cn

kill -9 $(pgrep -f app.py)
来源：http://gzd.yj20258888.top

[R65] 查看端口占用
来源：http://lkx.fzhhl.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://jrh.xziqi.cn

[R66] 定时任务
来源：http://kur.pengpengdd.cyou

crontab -e;  crontab -l
来源：http://ujx.shanyushiyangtech.top

[R67] 生成随机十六进制串
来源：http://ocs.tianlin.xyz

openssl rand -hex 16
来源：http://goi.haohaochexian.top

[R68] 计算文件校验值
来源：http://bav.yfazqb.com

sha256sum a.txt;  md5sum a.txt
来源：http://myp.hfpthk.cn

[R69] 生成随机密码
来源：http://upk.daxiang520.top

head -c 16 /dev/urandom | base64
来源：http://blz.gotoacloud.top

[R70] 时间戳与互转
来源：http://izv.fengsongda.top

date +%s;  date -d @1700000000
来源：http://agu.ydjk.org.cn

[R71] 日期格式化
来源：http://ehs.ydzc1.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://qgw.ivvv.top

[R72] 等待端口就绪
来源：http://aoj.dianchejie.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://nuk.fanxiaobao.xyz

[R73] 分割大日志
来源：http://axf.ydjk.org.cn

split -l 1000 big.log part_
来源：http://qab.zhixingplan.top

[R74] 批量重命名
来源：http://nxv.yj20258888.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://una.tarul.cn

[R75] 导出环境变量
来源：http://dhg.fanxiaobao.xyz

export PATH="$HOME/bin:$PATH"
来源：http://bcg.xuetiantiany.cn

[R76] 使用临时文件
来源：http://cdv.zycfv.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://eaq.sysykeji.top

[R77] 读取用户输入
来源：http://aof.aibaodan.cn

read -rp "请输入: " ans
来源：http://jls.yj20258.top

[R78] 交互式菜单
来源：http://jhr.hesvh.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://zsd.yuanzhike.top

[R79] 解析命令行选项
来源：http://mpg.xinyue.icu

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ivj.jinqigufen.top

[R80] 查看脚本执行耗时
来源：http://kos.jiagoushi.top

time ./run.sh
来源：http://qoi.xingfuxueyuan.xyz

================================================================================
来源：http://ggm.c1oappe.top

S. C / C++ 专题
来源：http://kgq.tarul.cn

================================================================================
来源：http://xkc.9152youxi.cn

[S01] C：Hello World
来源：http://hco.wangdashe.top

#include <stdio.h>
来源：http://lhk.cheryme.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://flw.yongpay.top

[S02] C：变量与格式化输出
来源：http://psd.0kj1m.cn

int a = 10; printf("%d\n", a);
来源：http://gnc.jiagoushi.top

[S03] C：读入整数
来源：http://koh.hammf.cn

int x; scanf("%d", &x);
来源：http://qex.jiagoushi.top

[S04] C：字符串复制
来源：http://iaw.daria6918.cn

char dst[32]; strcpy(dst, "hi");
来源：http://jqb.9152youxi.cn

[S05] C：字符串长度
来源：http://bbd.ehwqpu.com


<!-- 参考信息 -->