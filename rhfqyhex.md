代发 wailian999

SELECT MAX(age), MIN(age) FROM users;
来源：http://ara.sysykeji.top

[Q30] 分组统计
来源：http://jzk.zhengqikj.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://gdt.yanxiufei.cn

[Q31] 分组后过滤
来源：http://ski.hesvh.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://cyd.guowangkeji.top

[Q32] 分组拼接字符串
来源：http://uqg.316326.xyz

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://jgj.daria6918.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://oro.zhijiandao.cn

[Q33] 多列分组
来源：http://nkr.jlsjyb.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://dkq.vqdsnc.cn

[Q34] 每组取第一条
来源：http://mix.epnwcf.com

SELECT * FROM (
来源：http://gfd.shzxlz.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://kqs.tianlin.xyz

) t WHERE rn = 1;
来源：http://hoz.ydjk.org.cn

[Q35] 内连接
来源：http://juo.birdmap.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ezf.zycfv.cn

[Q36] 左连接
来源：http://lby.shanyushiyangtech.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://uxb.sjlbkw.cn

[Q37] 右连接
来源：http://yyu.hysaishi.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://sgo.zhiwuduotai.top

[Q38] 全外连接（PostgreSQL）
来源：http://rdn.gotoacloud.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://bwf.shanyushiyangtech.top

[Q39] 自连接（查上下级）
来源：http://azy.yanxiufei.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://bag.sjlbkw.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://tsx.sweek.top

[Q40] 交叉连接（笛卡尔积）
来源：http://hjt.fanxiaobao.xyz

SELECT * FROM colors CROSS JOIN sizes;
来源：http://xxh.jiagoushi.top

[Q41] 多表连接
来源：http://hhm.zhijiandao.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://mix.zdbjq.cn

JOIN users u ON u.id = o.user_id
来源：http://scw.sysykeji.top

JOIN products p ON p.id = o.product_id;
来源：http://dmw.zycfv.cn

[Q42] 连接条件附加过滤
来源：http://tuh.mhx1999.top

SELECT u.name, o.amount FROM users u
来源：http://qmh.guannengcc.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://axu.ybcxt.top

[Q43] 标量子查询
来源：http://krb.xinyue.icu

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hdm.zhongyouzk.top

[Q44] IN 子查询
来源：http://ivb.andypj.xyz

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://jzw.chenlongwang.top

[Q45] EXISTS 判断存在
来源：http://fps.cucudq.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xtd.pycfn.com

[Q46] NOT EXISTS 判断不存在
来源：http://gdn.xinyue.icu

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qud.jinghuilouyu.cn

[Q47] 与平均值比较
来源：http://llx.shzxlz.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://tdw.zhengqikj.top

[Q48] CTE 公用表表达式
来源：http://fxr.cashguo.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hzs.tianlin.xyz

SELECT * FROM t WHERE c > 5;
来源：http://ncw.tarul.cn

[Q49] 更新单行
来源：http://xcv.cashguo.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://snk.yfazqb.com

[Q50] 批量更新
来源：http://yug.yonumen.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://zjr.shangyingyoupin.top

[Q51] 用子查询更新
来源：http://btf.ctjpmb.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hrn.iojbl.cn

[Q52] 删除指定行
来源：http://taw.fanxiaobao.xyz

DELETE FROM users WHERE id = 10;
来源：http://rsj.tarul.cn

[Q53] 按条件删除
来源：http://wjc.xinyue.icu

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://vka.guannengcc.top

[Q54] 清空表
来源：http://ksw.yj20258.top

TRUNCATE TABLE logs;
来源：http://xip.svipenyu.cn

[Q55] 排名（并列占位）
来源：http://pac.jinyuanbaomall.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://kdw.tarul.cn

[Q56] 密集排名（并列不占位）
来源：http://btu.svipenyu.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://luc.mhx1999.top

[Q57] 行号
来源：http://lyh.meibo888.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://uaq.yueranfly.top

[Q58] 累计求和
来源：http://vol.jiagoushi.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ucf.chenzaomai.com

[Q59] 分组内累计
来源：http://uex.zdbjq.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://kvj.xuanzx.com

[Q60] 取上一行 / 下一行
来源：http://ivs.yanxiufei.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://beh.aizwys.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://rln.uphjek.com

[Q61] 移动平均
来源：http://umg.yj20258.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://gcu.bjfxy.top

[Q62] 分组占比
来源：http://ijd.kuanghao11.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mby.jinqigfzy.top

[Q63] 开启事务
来源：http://uon.hywenlv.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://gqc.yonumen.top

[Q64] 提交事务
来源：http://vos.xingfuxueyuan.xyz

COMMIT;
来源：http://gsq.fengsongda.top

[Q65] 回滚事务
来源：http://srx.vqdsnc.cn

ROLLBACK;
来源：http://dsi.yuxming.cn

[Q66] 行锁查询
来源：http://qtg.zhengqikj.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://bsx.cucudq.cn

[Q67] 设置隔离级别
来源：http://hpz.bbcook.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://klr.haohaochexian.top

[Q68] 保存点
来源：http://iby.zycfv.cn

SAVEPOINT sp1;
来源：http://bio.fzhhl.top

ROLLBACK TO sp1;
来源：http://uqs.snrcjt.cn

[Q69] 查看执行计划
来源：http://jyt.hesvh.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://pfr.yj20258888.top

[Q70] 更新统计信息
来源：http://cqe.jinyuanbaomall.cn

ANALYZE TABLE users;
来源：http://gjn.yvedp.cn

[Q71] 查看建表语句
来源：http://llv.kuanghao11.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://vcb.316326.xyz

[Q72] 查看索引
来源：http://vxq.tianlin.xyz

SHOW INDEX FROM users;
来源：http://mxw.fehbvm.com

[Q73] 查看表状态
来源：http://hqn.316326.xyz

SHOW TABLE STATUS LIKE 'users';
来源：http://mru.hcnkem.com

[Q74] 强制使用索引
来源：http://aml.sufxvd.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://pqk.svipenyu.cn

[Q75] 日期格式化
来源：http://ubl.gogol.net.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://jxb.andypj.xyz

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hku.tanke756.top

[Q76] 按天统计
来源：http://vwd.epnwcf.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hzg.quarkkingdee.top

[Q77] 时间加减
来源：http://gyj.hnqzz.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://emn.cdnleiting.top

[Q78] 当前时间
来源：http://qsg.wangdashe.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://yfn.sysykeji.top

[Q79] 字符串拼接
来源：http://env.cheryme.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://fud.redwolf501.top

[Q80] 字符串截取
来源：http://zew.fehbvm.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://sgr.zycfv.cn

[Q81] 字符串替换
来源：http://nes.pengpengdd.cyou

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://psd.ehwqpu.com

[Q82] 字符长度与字节长度
来源：http://xrr.sufxvd.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://owg.yj20258.top

[Q83] 大小写转换
来源：http://slw.epnwcf.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://kfu.cashguo.top

[Q84] 去除首尾空格
来源：http://iwk.hesvh.cn

SELECT TRIM(name) FROM users;
来源：http://aaz.xinyue.icu

[Q85] 数值取整
来源：http://aql.ivvv.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://yfr.yonumen.top

[Q86] 读取 JSON 字段
来源：http://mnw.tianlin.xyz

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ueh.hnxiangtu.top

[Q87] JSON 字段做条件
来源：http://kyu.jyoumei.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mjs.fktsv.cn

[Q88] 行转列（条件聚合）
来源：http://pgm.jinqigufen.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://zyg.zhaomingkeji.xyz

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://lky.jqgufenzy.top

[Q89] 判断表是否存在
来源：http://mof.gzhubu.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://rjz.wangshuangyany.cn

[Q90] 生成序号列
来源：http://gdk.sweek.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://fsk.zdbjq.cn

================================================================================
来源：http://vfy.gotoacloud.top

R. Bash 专题
来源：http://uiv.c1oappe.top

================================================================================
来源：http://csu.pycfn.com

[R01] shebang 与严格模式
来源：http://dvq.ctjpmb.com

#!/usr/bin/env bash
来源：http://jqw.mhx1999.top

set -euo pipefail
来源：http://xyp.tianlin.xyz

[R02] 变量赋值与使用
来源：http://www.zdbjq.cn

name="Tom"; echo "$name"
来源：http://lom.zhaomingkeji.xyz

[R03] 只读变量
来源：http://uam.tarul.cn

readonly PI=3.14
来源：http://axq.meibo888.top

[R04] 位置参数
来源：http://hec.kuanghao11.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hkn.zdqjudy.top

[R05] 参数默认值
来源：http://kad.jqgfzy.top

name="${1:-default}"
来源：http://cdq.zhaomingkeji.xyz

[R06] 判断命令是否存在
来源：http://wki.dianchejie.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ynq.sjlbkw.cn

[R07] if 判断文件
来源：http://syn.aibaodan.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://oej.vqdsnc.cn

[R08] 数值比较
来源：http://vwn.dianchejie.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://vfv.jinqigufen.top

[R09] 字符串比较
来源：http://zmv.yonumen.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hvf.sufxvd.cn

[R10] 正则匹配
来源：http://mec.cqqwz.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://xcb.feifeiyinyue.top

[R11] case 多分支
来源：http://bhn.sxryk.cn

case "$1" in
来源：http://akz.chenlongwang.top

start) echo "启动" ;;
来源：http://ons.sysykeji.top

stop)  echo "停止" ;;
来源：http://avw.jqgufenzy.top

*)     echo "未知命令" ;;
来源：http://njo.9152youxi.cn

esac
来源：http://nep.hongshengwenyu.top

[R12] for 遍历文件
来源：http://zaz.snrcjt.cn

for f in *.txt; do echo "$f"; done
来源：http://igd.kuanghao11.cn

[R13] for 计数循环
来源：http://xss.chenzaomai.com

for i in {1..10}; do echo "$i"; done
来源：http://bnp.pengpengdd.cyou

[R14] C 风格 for
来源：http://pgp.jinqigfzy.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://jkq.fengsongda.top

[R15] while 逐行读文件
来源：http://yuv.yj20258.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://gcw.fzhhl.top

[R16] until 等待条件
来源：http://rng.jinqigfzy.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://gij.yfazqb.com

[R17] 数组定义与取值
来源：http://ncs.gzhubu.top

arr=(a b c); echo "${arr[0]}"
来源：http://wxc.feifeiyinyue.top

[R18] 遍历数组
来源：http://rfh.aibaodan.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://cpx.yangfankeji.com

[R19] 数组长度
来源：http://yxa.xuetiantiany.cn

echo "${#arr[@]}"
来源：http://hlk.ydjk.org.cn

[R20] 关联数组（字典）
来源：http://znv.hesvh.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://keh.zhiwuduotai.top

[R21] 字符串长度
来源：http://isj.shangyingyoupin.top

echo "${#s}"
来源：http://wgz.chenlongwang.top

[R22] 截取子串
来源：http://ame.jqgfzy.top

echo "${s:0:5}"
来源：http://yum.jinghuilouyu.cn

[R23] 字符串替换
来源：http://gfy.shanyushiyangkeji.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hzl.shuidangran.top

[R24] 大小写转换
来源：http://cqa.aizwys.cn

echo "${s^^}"; echo "${s,,}"
来源：http://hts.hnqzz.top

[R25] 去后缀 / 去前缀
来源：http://kgn.zhijiandao.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://twa.zhixingplan.top

[R26] 命令替换
来源：http://oxo.kuanghao11.cn

now=$(date +%F); echo "$now"
来源：http://sos.sxryk.cn

[R27] 算术展开
来源：http://pth.yj20258.top

echo $((1 + 2 * 3))
来源：http://kso.chenlongwang.top

[R28] 浮点运算
来源：http://zng.sysykeji.top

echo "scale=2; 10/3" | bc
来源：http://bqm.shuidangran.top

[R29] 定义函数
来源：http://tsn.meibo888.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://enm.sxryk.cn

[R30] 函数返回状态码
来源：http://wzk.zhixingplan.top

f() { return 0; }; f || echo "失败了"
来源：http://scq.hesvh.cn

[R31] 局部变量
来源：http://lub.redwolf501.top

f() { local x=1; echo "$x"; }
来源：http://zdl.fanxiaobao.xyz

[R32] 参数个数校验
来源：http://rev.zhijiandao.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://sbd.xinyue.icu

[R33] 捕获错误并提示行号
来源：http://ved.aibaodan.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://qkh.yuxming.cn

[R34] 退出时清理
来源：http://iob.hesvh.cn

trap 'rm -f "$tmp"' EXIT
来源：http://rqi.shanyushiyangtech.top

[R35] 后台执行并等待
来源：http://jnc.yonumen.top

sleep 5 & pid=$!; wait "$pid"
来源：http://hki.chenlongwang.top

[R36] 并发执行多个任务
来源：http://rcs.zycfv.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://bab.yvedp.cn

[R37] 把输出赋给变量
来源：http://jxs.kuanghao11.cn

files=$(ls -1)
来源：http://qit.chenjidiqi.icu

[R38] 管道串联
来源：http://rkn.cashguo.top

cat a.txt | grep -i error | wc -l
来源：http://sbu.haohaochexian.top

[R39] 重定向标准输出与错误
来源：http://dde.cheryme.top

cmd > out.log 2>&1
来源：http://ppy.zhiwuduotai.top

[R40] 追加写日志
来源：http://gjg.ywan-chungtsiang.top

echo "log" >> out.log
来源：http://kkz.vqdsnc.cn

[R41] 丢弃输出
来源：http://pld.xuanzx.com

cmd >/dev/null 2>&1
来源：http://shu.birdmap.top

[R42] 输入重定向
来源：http://yuk.hesvh.cn

wc -l < a.txt
来源：http://hxs.fehbvm.com

[R43] 按名字查找文件
来源：http://cdq.shanyushiyangkeji.top

find . -name "*.log" -type f
来源：http://gwf.nanxuanxn.top

[R44] 按修改时间查找
来源：http://fqw.wangdashe.top

find . -mtime -7 -type f
来源：http://qhu.nanxinkj.top

[R45] 批量删除
来源：http://qlh.yueranfly.top

find . -name "*.tmp" -delete
来源：http://uxj.ctjpmb.com

[R46] 递归替换文件内容
来源：http://cof.ywan-chungtsiang.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://idt.zdbjq.cn

[R47] sed 单行替换
来源：http://ltc.xuetiantiany.cn

sed -i 's/foo/bar/g' a.txt
来源：http://dys.52xcode.cn

[R48] awk 取指定列
来源：http://vut.chenlongwang.top

awk '{print $1, $3}' a.txt
来源：http://eks.xziqi.cn

[R49] awk 带条件
来源：http://jsa.tian-w.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://cpr.redwolf501.top

[R50] awk 求和
来源：http://ivl.guowangkeji.top

awk '{s += $2} END {print s}' a.txt
来源：http://fnq.zhiwuduotai.top

[R51] 排序去重取前几
来源：http://uea.jyoumei.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://jma.fktsv.cn

[R52] 统计行数
来源：http://fif.nwbrower.top

wc -l a.txt
来源：http://rea.kuanghao11.cn

[R53] 查看文件头与实时尾
来源：http://oxo.daxiang520.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://tdw.uphjek.com

[R54] 比较两个文件
来源：http://jcs.jianghu66.top

diff a.txt b.txt
来源：http://yjb.tian-w.cn

[R55] 压缩与解压
来源：http://zol.birdmap.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://fbm.meibo888.top

[R56] 远程拷贝
来源：http://atr.nwbrower.top

scp file user@host:/path/
来源：http://yhl.gzhubu.top

[R57] 远程执行命令
来源：http://npo.gaohongyu789.top

ssh user@host 'uptime'
来源：http://tjz.snrcjt.cn

[R58] 下载文件
来源：http://fdk.jiagoushi.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://bgn.yanxiufei.cn

[R59] 发 POST JSON
来源：http://ijk.cucudq.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://rce.cucudq.cn

[R60] 只看 HTTP 状态码
来源：http://ebj.9152youxi.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ziz.daxiang520.top

[R61] 磁盘占用
来源：http://dsm.ybcxt.top

df -h;  du -sh *
来源：http://gnu.zdbjq.cn

[R62] 找最占空间的文件
来源：http://edf.xuanzx.com

du -ah . | sort -rh | head -10
来源：http://jan.uphjek.com

[R63] 内存与进程
来源：http://xzf.9152youxi.cn

free -h;  ps aux | grep nginx
来源：http://lra.fanxiaobao.xyz

[R64] 结束进程
来源：http://ewf.chenjidiqi.icu

kill -9 $(pgrep -f app.py)
来源：http://var.jinyuanbaomall.cn

[R65] 查看端口占用
来源：http://siw.sufxvd.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hny.zhongyouzk.top

[R66] 定时任务
来源：http://bqv.jqgfzy.top

crontab -e;  crontab -l
来源：http://kdq.aibaodan.cn

[R67] 生成随机十六进制串
来源：http://rgl.yueranfly.top

openssl rand -hex 16
来源：http://kmd.ywan-chungtsiang.top

[R68] 计算文件校验值
来源：http://gwl.bbcook.cn

sha256sum a.txt;  md5sum a.txt
来源：http://hwv.zdbjq.cn

[R69] 生成随机密码
来源：http://rvn.zhiwuduotai.top

head -c 16 /dev/urandom | base64
来源：http://uin.ybcxt.top

[R70] 时间戳与互转
来源：http://uah.hnqzz.top

date +%s;  date -d @1700000000
来源：http://lnd.hywenlv.cn

[R71] 日期格式化
来源：http://zba.gzhubu.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://ypl.zdbjq.cn

[R72] 等待端口就绪
来源：http://tqn.jinghuilouyu.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://sxt.xinyue.icu

[R73] 分割大日志
来源：http://hdu.uphjek.com

split -l 1000 big.log part_
来源：http://vvn.hfpthk.cn

[R74] 批量重命名
来源：http://qes.ybcxt.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://xnf.dashuyun.cn

[R75] 导出环境变量
来源：http://rgv.yj20258888.top

export PATH="$HOME/bin:$PATH"
来源：http://vdh.chenjidiqi.icu

[R76] 使用临时文件
来源：http://ava.andypj.xyz

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://sna.c1oappe.top

[R77] 读取用户输入
来源：http://uwe.52xcode.cn

read -rp "请输入: " ans
来源：http://rgt.havefunace.top

[R78] 交互式菜单
来源：http://qho.ydjk.org.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://edv.yj20258888.top

[R79] 解析命令行选项
来源：http://xii.316326.xyz


<!-- 参考信息 -->