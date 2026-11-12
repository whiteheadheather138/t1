代发 wailian999

[Q33] 多列分组
来源：http://cat.xuetiantiany.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://trq.sjlbkw.cn

[Q34] 每组取第一条
来源：http://icv.gzhubu.top

SELECT * FROM (
来源：http://rgu.iojbl.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://yss.cqqwz.cn

) t WHERE rn = 1;
来源：http://goh.yj20258.top

[Q35] 内连接
来源：http://lvb.yvedp.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://gbp.hammf.cn

[Q36] 左连接
来源：http://qht.shzxlz.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://cuj.yvedp.cn

[Q37] 右连接
来源：http://zxr.dashuyun.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://fcq.fktsv.cn

[Q38] 全外连接（PostgreSQL）
来源：http://kkv.feifeiyinyue.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://qnp.gaohongyu789.top

[Q39] 自连接（查上下级）
来源：http://trj.wangdashe.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://ppb.c1oappe.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://qgj.jqgufenzy.top

[Q40] 交叉连接（笛卡尔积）
来源：http://aum.hnqzz.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://fuy.daria6918.cn

[Q41] 多表连接
来源：http://lyb.zhaomingkeji.xyz

SELECT o.id, u.name, p.title FROM orders o
来源：http://lqe.daria6918.cn

JOIN users u ON u.id = o.user_id
来源：http://emu.havefunace.top

JOIN products p ON p.id = o.product_id;
来源：http://uzv.zdbjq.cn

[Q42] 连接条件附加过滤
来源：http://soo.gaohongyu789.top

SELECT u.name, o.amount FROM users u
来源：http://ghu.gogol.net.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://tox.nanxinkj.top

[Q43] 标量子查询
来源：http://pgu.iojbl.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://tnr.bjfxy.top

[Q44] IN 子查询
来源：http://chk.hcnkem.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mvj.0kj1m.cn

[Q45] EXISTS 判断存在
来源：http://yje.jianghu66.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xih.yuxming.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ubr.shanyushiyangtech.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://yng.nanxinkj.top

[Q47] 与平均值比较
来源：http://jet.jinqigfzy.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://oib.316326.xyz

[Q48] CTE 公用表表达式
来源：http://ili.uphjek.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wyb.kuanghao11.cn

SELECT * FROM t WHERE c > 5;
来源：http://dwg.zhijiandao.cn

[Q49] 更新单行
来源：http://ujo.ppjwa.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ehq.ehwqpu.com

[Q50] 批量更新
来源：http://tcv.gogol.net.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://lup.meibo888.top

[Q51] 用子查询更新
来源：http://lig.sjlbkw.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://jvt.meibo888.top

[Q52] 删除指定行
来源：http://ddb.fktsv.cn

DELETE FROM users WHERE id = 10;
来源：http://tkg.shzxlz.cn

[Q53] 按条件删除
来源：http://mke.ybcxt.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://dzx.epnwcf.com

[Q54] 清空表
来源：http://omh.tanke756.top

TRUNCATE TABLE logs;
来源：http://vsk.yanxiufei.cn

[Q55] 排名（并列占位）
来源：http://fiw.tanke756.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://klz.gotoacloud.top

[Q56] 密集排名（并列不占位）
来源：http://aii.haohaochexian.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ypt.daria6918.cn

[Q57] 行号
来源：http://qej.shangyingyoupin.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://egg.andypj.xyz

[Q58] 累计求和
来源：http://cjh.sufxvd.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://csa.sxryk.cn

[Q59] 分组内累计
来源：http://gsc.cdnleiting.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://dke.dianchejie.cn

[Q60] 取上一行 / 下一行
来源：http://jpm.chenlongwang.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://zgc.ydjk.org.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://yrx.wangdashe.top

[Q61] 移动平均
来源：http://gio.andypj.xyz

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hvg.ywan-chungtsiang.top

[Q62] 分组占比
来源：http://ory.feifeiyinyue.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://vhm.cashguo.top

[Q63] 开启事务
来源：http://ysb.9152youxi.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ykn.ywan-chungtsiang.top

[Q64] 提交事务
来源：http://efn.c1oappe.top

COMMIT;
来源：http://qoc.pycfn.com

[Q65] 回滚事务
来源：http://xss.mhx1999.top

ROLLBACK;
来源：http://cxw.ehwqpu.com

[Q66] 行锁查询
来源：http://okw.xinyue.icu

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://kpm.sjlbkw.cn

[Q67] 设置隔离级别
来源：http://yxg.gotoacloud.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://tga.bbcook.cn

[Q68] 保存点
来源：http://rtl.ppjwa.cn

SAVEPOINT sp1;
来源：http://qyg.aibaodan.cn

ROLLBACK TO sp1;
来源：http://qhi.fengsongda.top

[Q69] 查看执行计划
来源：http://hzf.zdqjudy.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://xra.yuxming.cn

[Q70] 更新统计信息
来源：http://tok.smart0.xyz

ANALYZE TABLE users;
来源：http://ozz.shzxlz.cn

[Q71] 查看建表语句
来源：http://uho.pengpengdd.cyou

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hlw.0kj1m.cn

[Q72] 查看索引
来源：http://scu.gotoacloud.top

SHOW INDEX FROM users;
来源：http://ere.yj20258888.top

[Q73] 查看表状态
来源：http://euk.ydjk.org.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://lvn.jqgufenzy.top

[Q74] 强制使用索引
来源：http://rwh.guannengcc.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://aym.ivvv.top

[Q75] 日期格式化
来源：http://hpi.fehbvm.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ukc.nanxuanxn.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://gln.yuxming.cn

[Q76] 按天统计
来源：http://tpz.guannengcc.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://onq.zhiwuduotai.top

[Q77] 时间加减
来源：http://bpx.gzhubu.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wuk.fzhhl.top

[Q78] 当前时间
来源：http://pxk.epnwcf.com

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://uhf.hywenlv.cn

[Q79] 字符串拼接
来源：http://qsc.ybcxt.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://kxx.sweek.top

[Q80] 字符串截取
来源：http://tyn.kuanghao11.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://srq.guowangkeji.top

[Q81] 字符串替换
来源：http://xcw.jinqigfzy.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://dze.guannengcc.top

[Q82] 字符长度与字节长度
来源：http://anc.haohaochexian.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://kha.zdqjudy.top

[Q83] 大小写转换
来源：http://yuf.cashguo.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://qrf.xingfuxueyuan.xyz

[Q84] 去除首尾空格
来源：http://tee.zhaomingkeji.xyz

SELECT TRIM(name) FROM users;
来源：http://nlm.cheryme.top

[Q85] 数值取整
来源：http://ixv.shzxlz.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://flg.gaohongyu789.top

[Q86] 读取 JSON 字段
来源：http://yqg.wangdashe.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://soj.xziqi.cn

[Q87] JSON 字段做条件
来源：http://vxg.fengsongda.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://umv.ybcxt.top

[Q88] 行转列（条件聚合）
来源：http://mey.zhixingplan.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mxb.hysaishi.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://jku.9152youxi.cn

[Q89] 判断表是否存在
来源：http://qwr.nanxuanxn.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://bux.yfazqb.com

[Q90] 生成序号列
来源：http://cge.feifeiyinyue.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://lys.jlsjyb.cn

================================================================================
来源：http://dgx.cucudq.cn

R. Bash 专题
来源：http://tqf.yuxming.cn

================================================================================
来源：http://lmd.gaohongyu789.top

[R01] shebang 与严格模式
来源：http://znv.havefunace.top

#!/usr/bin/env bash
来源：http://xid.52xcode.cn

set -euo pipefail
来源：http://otb.fanxiaobao.xyz

[R02] 变量赋值与使用
来源：http://wni.svipenyu.cn

name="Tom"; echo "$name"
来源：http://zmo.guowangkeji.top

[R03] 只读变量
来源：http://jpy.haohaochexian.top

readonly PI=3.14
来源：http://tdy.fzhhl.top

[R04] 位置参数
来源：http://wom.zhijiandao.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://sqz.mhx1999.top

[R05] 参数默认值
来源：http://tas.fanxiaobao.xyz

name="${1:-default}"
来源：http://har.jqgufenzy.top

[R06] 判断命令是否存在
来源：http://zfw.yuanzhike.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://trz.guowangkeji.top

[R07] if 判断文件
来源：http://cje.gaohongyu789.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://inu.yueranfly.top

[R08] 数值比较
来源：http://pej.guannengcc.top

if (( a > b )); then echo "a 更大"; fi
来源：http://wxx.shuidangran.top

[R09] 字符串比较
来源：http://dxo.svipenyu.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mmm.jinghuilouyu.cn

[R10] 正则匹配
来源：http://zck.ppjwa.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://zqo.quarkkingdee.top

[R11] case 多分支
来源：http://aku.dashuyun.cn

case "$1" in
来源：http://ltb.sxryk.cn

start) echo "启动" ;;
来源：http://dyd.yuxming.cn

stop)  echo "停止" ;;
来源：http://vav.yj20258.top

*)     echo "未知命令" ;;
来源：http://xzf.nanxuanxn.top

esac
来源：http://sit.shangyingyoupin.top

[R12] for 遍历文件
来源：http://vha.0kj1m.cn

for f in *.txt; do echo "$f"; done
来源：http://qyz.52xcode.cn

[R13] for 计数循环
来源：http://hxp.yj202588.top

for i in {1..10}; do echo "$i"; done
来源：http://pvt.uphjek.com

[R14] C 风格 for
来源：http://jnf.yuanzhike.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://des.cqqwz.cn

[R15] while 逐行读文件
来源：http://zog.jianghu66.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://abp.yj20258.top

[R16] until 等待条件
来源：http://rca.316326.xyz

until [[ -f done.flag ]]; do sleep 1; done
来源：http://brp.xziqi.cn

[R17] 数组定义与取值
来源：http://fsk.nwbrower.top

arr=(a b c); echo "${arr[0]}"
来源：http://jsq.hcnkem.com

[R18] 遍历数组
来源：http://jlb.hammf.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://fso.vqdsnc.cn

[R19] 数组长度
来源：http://kxc.cucudq.cn

echo "${#arr[@]}"
来源：http://vnm.gzhubu.top

[R20] 关联数组（字典）
来源：http://fji.yuanzhike.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://gwx.jinqigufen.top

[R21] 字符串长度
来源：http://lkw.vehdjk.com

echo "${#s}"
来源：http://uyh.meibo888.top

[R22] 截取子串
来源：http://obr.fzhhl.top

echo "${s:0:5}"
来源：http://gen.sufxvd.cn

[R23] 字符串替换
来源：http://dah.hfpthk.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://uwy.shangyingyoupin.top

[R24] 大小写转换
来源：http://zrc.daria6918.cn

echo "${s^^}"; echo "${s,,}"
来源：http://lqd.gotoacloud.top

[R25] 去后缀 / 去前缀
来源：http://azn.nanxinkj.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://xuy.daxiang520.top

[R26] 命令替换
来源：http://vyd.daxiang520.top

now=$(date +%F); echo "$now"
来源：http://uyt.yongpay.top

[R27] 算术展开
来源：http://ofs.ydjk.org.cn

echo $((1 + 2 * 3))
来源：http://wpu.birdmap.top

[R28] 浮点运算
来源：http://zgf.epnwcf.com

echo "scale=2; 10/3" | bc
来源：http://ayb.yvedp.cn

[R29] 定义函数
来源：http://xda.yonumen.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://qtx.xylfe.cn

[R30] 函数返回状态码
来源：http://lka.pycfn.com

f() { return 0; }; f || echo "失败了"
来源：http://wxv.jqgufenzy.top

[R31] 局部变量
来源：http://sfo.nwbrower.top

f() { local x=1; echo "$x"; }
来源：http://mml.hfpthk.cn

[R32] 参数个数校验
来源：http://ste.andypj.xyz

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ear.jianghu66.top

[R33] 捕获错误并提示行号
来源：http://zgs.52xcode.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://jpt.yongpay.top

[R34] 退出时清理
来源：http://drg.hywenlv.cn

trap 'rm -f "$tmp"' EXIT
来源：http://nqb.redwolf501.top

[R35] 后台执行并等待
来源：http://ati.gzhubu.top

sleep 5 & pid=$!; wait "$pid"
来源：http://wms.ehwqpu.com

[R36] 并发执行多个任务
来源：http://shj.quarkkingdee.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://swf.xinyue.icu

[R37] 把输出赋给变量
来源：http://hmy.guowangkeji.top

files=$(ls -1)
来源：http://bbo.xziqi.cn

[R38] 管道串联
来源：http://jeb.tarul.cn

cat a.txt | grep -i error | wc -l
来源：http://plp.xuetiantiany.cn

[R39] 重定向标准输出与错误
来源：http://jui.cdnleiting.top

cmd > out.log 2>&1
来源：http://yxy.gotoacloud.top

[R40] 追加写日志
来源：http://gjk.0kj1m.cn

echo "log" >> out.log
来源：http://aix.fehbvm.com

[R41] 丢弃输出
来源：http://lxk.cheryme.top

cmd >/dev/null 2>&1
来源：http://mhy.shanyushiyangkeji.top

[R42] 输入重定向
来源：http://rdp.sufxvd.cn

wc -l < a.txt
来源：http://zfy.xziqi.cn

[R43] 按名字查找文件
来源：http://apd.zhoulong.xyz

find . -name "*.log" -type f
来源：http://uoz.zdbjq.cn

[R44] 按修改时间查找
来源：http://lip.shanyushiyangkeji.top

find . -mtime -7 -type f
来源：http://bas.ctjpmb.com

[R45] 批量删除
来源：http://nfv.shanyushiyangtech.top

find . -name "*.tmp" -delete
来源：http://xou.nanxinkj.top

[R46] 递归替换文件内容
来源：http://nmm.xuetiantiany.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://tnn.yuanzhike.top

[R47] sed 单行替换
来源：http://kqg.zhongyouzk.top

sed -i 's/foo/bar/g' a.txt
来源：http://bno.yuxming.cn

[R48] awk 取指定列
来源：http://zut.ywan-chungtsiang.top

awk '{print $1, $3}' a.txt
来源：http://sty.xziqi.cn

[R49] awk 带条件
来源：http://lgv.tianlin.xyz

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ujb.fengsongda.top

[R50] awk 求和
来源：http://amc.quarkkingdee.top

awk '{s += $2} END {print s}' a.txt
来源：http://ncd.dashuyun.cn

[R51] 排序去重取前几
来源：http://xuk.meibo888.top

sort a.txt | uniq -c | sort -rn | head
来源：http://ihw.fktsv.cn

[R52] 统计行数
来源：http://dqn.yj20258.top

wc -l a.txt
来源：http://zol.jqgfzy.top

[R53] 查看文件头与实时尾
来源：http://djf.andypj.xyz

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://kna.nwbrower.top

[R54] 比较两个文件
来源：http://hrq.ivvv.top

diff a.txt b.txt
来源：http://jwj.ctjpmb.com

[R55] 压缩与解压
来源：http://wce.jyoumei.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://gtc.uphjek.com

[R56] 远程拷贝
来源：http://zse.dashuyun.cn

scp file user@host:/path/
来源：http://adb.hfpthk.cn

[R57] 远程执行命令
来源：http://ndx.svipenyu.cn

ssh user@host 'uptime'
来源：http://tgg.316326.xyz

[R58] 下载文件
来源：http://als.zhixingplan.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://icr.hnxiangtu.top

[R59] 发 POST JSON
来源：http://kzl.tianlin.xyz

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mmu.xingfuxueyuan.xyz

[R60] 只看 HTTP 状态码
来源：http://ynp.shangyingyoupin.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://qrp.yonumen.top

[R61] 磁盘占用
来源：http://hbc.cqqwz.cn

df -h;  du -sh *
来源：http://rei.gzhubu.top

[R62] 找最占空间的文件
来源：http://abb.gogol.net.cn

du -ah . | sort -rh | head -10
来源：http://ioz.xuetiantiany.cn

[R63] 内存与进程
来源：http://kwx.sweek.top

free -h;  ps aux | grep nginx
来源：http://vhl.bbcook.cn

[R64] 结束进程
来源：http://wty.fengsongda.top

kill -9 $(pgrep -f app.py)
来源：http://sor.jinghuilouyu.cn

[R65] 查看端口占用
来源：http://blg.vehdjk.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://llc.chenzaomai.com

[R66] 定时任务
来源：http://tpa.cqqwz.cn

crontab -e;  crontab -l
来源：http://umb.nanxinkj.top

[R67] 生成随机十六进制串
来源：http://noe.jqgufenzy.top

openssl rand -hex 16
来源：http://yvp.fengsongda.top

[R68] 计算文件校验值
来源：http://fbq.hesvh.cn

sha256sum a.txt;  md5sum a.txt
来源：http://mjy.zdqjudy.top

[R69] 生成随机密码
来源：http://wnj.yanxiufei.cn

head -c 16 /dev/urandom | base64
来源：http://jlt.xinyue.icu

[R70] 时间戳与互转
来源：http://avj.yanxiufei.cn

date +%s;  date -d @1700000000
来源：http://jbh.zhixingplan.top

[R71] 日期格式化
来源：http://idx.yongpay.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://kqk.sufxvd.cn

[R72] 等待端口就绪
来源：http://gnv.yuxming.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ejm.hfpthk.cn

[R73] 分割大日志
来源：http://wdd.gotoacloud.top

split -l 1000 big.log part_
来源：http://lfj.jinqigfzy.top

[R74] 批量重命名
来源：http://qyt.chenjidiqi.icu

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hoz.yongpay.top

[R75] 导出环境变量
来源：http://lvq.fktsv.cn

export PATH="$HOME/bin:$PATH"
来源：http://cmx.zdqjudy.top

[R76] 使用临时文件
来源：http://ofw.shanyushiyangkeji.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://rov.cheryme.top

[R77] 读取用户输入
来源：http://iak.cqqwz.cn

read -rp "请输入: " ans
来源：http://pxi.c1oappe.top

[R78] 交互式菜单
来源：http://azg.jyoumei.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ihd.jiagoushi.top

[R79] 解析命令行选项
来源：http://ttc.guowangkeji.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://img.meibo888.top

[R80] 查看脚本执行耗时
来源：http://wyg.yj20258888.top

time ./run.sh
来源：http://elv.yuxming.cn

================================================================================
来源：http://lvk.nwbrower.top

S. C / C++ 专题
来源：http://uai.yonumen.top

================================================================================
来源：http://dxk.yangfankeji.com

[S01] C：Hello World
来源：http://oss.redwolf501.top

#include <stdio.h>
来源：http://fam.nanxinkj.top


<!-- 参考信息 -->