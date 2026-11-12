代发 wailian999

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://dle.ehwqpu.com

) t WHERE rn = 1;
来源：http://gxs.cucudq.cn

[Q35] 内连接
来源：http://yto.xylfe.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://vsn.yj20258.top

[Q36] 左连接
来源：http://phx.haohaochexian.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://xsk.hnqzz.top

[Q37] 右连接
来源：http://oae.fktsv.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://djl.redwolf501.top

[Q38] 全外连接（PostgreSQL）
来源：http://gme.redwolf501.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://xus.quarkkingdee.top

[Q39] 自连接（查上下级）
来源：http://fpe.jqgfzy.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://ogx.yj202588.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hkb.zdbjq.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://gok.hammf.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://sur.zhengqikj.top

[Q41] 多表连接
来源：http://xqk.guannengcc.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://etn.yongpay.top

JOIN users u ON u.id = o.user_id
来源：http://kfl.zhengqikj.top

JOIN products p ON p.id = o.product_id;
来源：http://xnf.cdnleiting.top

[Q42] 连接条件附加过滤
来源：http://fll.wangdashe.top

SELECT u.name, o.amount FROM users u
来源：http://ggq.chenlongwang.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mba.xylfe.cn

[Q43] 标量子查询
来源：http://pys.vqdsnc.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://fkm.316326.xyz

[Q44] IN 子查询
来源：http://hez.yj202588.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://nxd.zhengqikj.top

[Q45] EXISTS 判断存在
来源：http://vbd.yangfankeji.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://var.aizwys.cn

[Q46] NOT EXISTS 判断不存在
来源：http://sfz.zhengqikj.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://gsz.hnqzz.top

[Q47] 与平均值比较
来源：http://mrk.ybcxt.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://dlp.xuanzx.com

[Q48] CTE 公用表表达式
来源：http://zfs.fanxiaobao.xyz

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://dib.pengpengdd.cyou

SELECT * FROM t WHERE c > 5;
来源：http://uba.nanxuanxn.top

[Q49] 更新单行
来源：http://ajh.yj20258888.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://boy.hcnkem.com

[Q50] 批量更新
来源：http://cid.jinyuanbaomall.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://dao.sxryk.cn

[Q51] 用子查询更新
来源：http://dvg.xylfe.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://uzg.fzhhl.top

[Q52] 删除指定行
来源：http://jbk.mhx1999.top

DELETE FROM users WHERE id = 10;
来源：http://pzf.jinqigufen.top

[Q53] 按条件删除
来源：http://alr.fehbvm.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://bah.sjlbkw.cn

[Q54] 清空表
来源：http://xqv.daria6918.cn

TRUNCATE TABLE logs;
来源：http://lcc.52xcode.cn

[Q55] 排名（并列占位）
来源：http://jzo.jqgfzy.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wqb.sjlbkw.cn

[Q56] 密集排名（并列不占位）
来源：http://flw.cashguo.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ahu.yfazqb.com

[Q57] 行号
来源：http://zke.uphjek.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://uzs.nanxuanxn.top

[Q58] 累计求和
来源：http://sna.xziqi.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://xxa.zhiwuduotai.top

[Q59] 分组内累计
来源：http://oxh.zhongyouzk.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://xul.xinyue.icu

[Q60] 取上一行 / 下一行
来源：http://arf.jqgufenzy.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://tuv.dashuyun.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://xsu.daxiang520.top

[Q61] 移动平均
来源：http://cso.hnxiangtu.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://weq.jinqigfzy.top

[Q62] 分组占比
来源：http://kpn.bbcook.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://czl.shuidangran.top

[Q63] 开启事务
来源：http://xut.zdqjudy.top

START TRANSACTION;                -- 或 BEGIN
来源：http://aeo.yj202588.top

[Q64] 提交事务
来源：http://rlq.gotoacloud.top

COMMIT;
来源：http://qbi.gzhubu.top

[Q65] 回滚事务
来源：http://bck.jinghuilouyu.cn

ROLLBACK;
来源：http://xnw.zhaomingkeji.xyz

[Q66] 行锁查询
来源：http://vbh.jinqigfzy.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://fzt.xuanzx.com

[Q67] 设置隔离级别
来源：http://zpo.hcnkem.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ssu.bjfxy.top

[Q68] 保存点
来源：http://xqx.shanyushiyangtech.top

SAVEPOINT sp1;
来源：http://cfz.jinghuilouyu.cn

ROLLBACK TO sp1;
来源：http://svn.havefunace.top

[Q69] 查看执行计划
来源：http://ulf.dianchejie.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mdi.hammf.cn

[Q70] 更新统计信息
来源：http://vut.hywenlv.cn

ANALYZE TABLE users;
来源：http://wol.cheryme.top

[Q71] 查看建表语句
来源：http://sxy.sufxvd.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://qjy.hammf.cn

[Q72] 查看索引
来源：http://nyg.snrcjt.cn

SHOW INDEX FROM users;
来源：http://wic.ydzc1.top

[Q73] 查看表状态
来源：http://aub.ydzc1.top

SHOW TABLE STATUS LIKE 'users';
来源：http://bfx.fanxiaobao.xyz

[Q74] 强制使用索引
来源：http://lez.gzhubu.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mhp.hammf.cn

[Q75] 日期格式化
来源：http://ddc.zdqjudy.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://bqy.dianchejie.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://rky.jinghuilouyu.cn

[Q76] 按天统计
来源：http://hmy.ctjpmb.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://uze.zhaomingkeji.xyz

[Q77] 时间加减
来源：http://tfe.ivvv.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://zkv.ctjpmb.com

[Q78] 当前时间
来源：http://rad.fengsongda.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://rcc.xuetiantiany.cn

[Q79] 字符串拼接
来源：http://tak.pengpengdd.cyou

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://kxk.zhongyouzk.top

[Q80] 字符串截取
来源：http://ncd.fktsv.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://tvf.cdnleiting.top

[Q81] 字符串替换
来源：http://tfl.hongshengwenyu.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://fds.yfazqb.com

[Q82] 字符长度与字节长度
来源：http://jjk.fzhhl.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://xru.gzhubu.top

[Q83] 大小写转换
来源：http://kgh.yanxiufei.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wyn.jianghu66.top

[Q84] 去除首尾空格
来源：http://vns.c1oappe.top

SELECT TRIM(name) FROM users;
来源：http://spe.ppjwa.cn

[Q85] 数值取整
来源：http://evs.cucudq.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://utm.zhongyouzk.top

[Q86] 读取 JSON 字段
来源：http://ana.wangdashe.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://nkq.yj20258.top

[Q87] JSON 字段做条件
来源：http://ikg.wangdashe.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://iwi.andypj.xyz

[Q88] 行转列（条件聚合）
来源：http://odg.ywan-chungtsiang.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://dgh.gaohongyu789.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://gdz.zhixingplan.top

[Q89] 判断表是否存在
来源：http://ykc.chenlongwang.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://vte.yuxming.cn

[Q90] 生成序号列
来源：http://jbv.gogol.net.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://svs.hfpthk.cn

================================================================================
来源：http://mru.jqgfzy.top

R. Bash 专题
来源：http://kiq.bjfxy.top

================================================================================
来源：http://zan.hywenlv.cn

[R01] shebang 与严格模式
来源：http://czb.fanxiaobao.xyz

#!/usr/bin/env bash
来源：http://liw.xinyue.icu

set -euo pipefail
来源：http://kms.shuidangran.top

[R02] 变量赋值与使用
来源：http://lpd.cqqwz.cn

name="Tom"; echo "$name"
来源：http://nba.smart0.xyz

[R03] 只读变量
来源：http://mpc.jqgfzy.top

readonly PI=3.14
来源：http://pgd.zycfv.cn

[R04] 位置参数
来源：http://vpc.ywan-chungtsiang.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ivk.svipenyu.cn

[R05] 参数默认值
来源：http://txo.sysykeji.top

name="${1:-default}"
来源：http://vgq.zhiwuduotai.top

[R06] 判断命令是否存在
来源：http://lnp.smart0.xyz

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://bok.yfazqb.com

[R07] if 判断文件
来源：http://sxi.fzhhl.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://vnd.pengpengdd.cyou

[R08] 数值比较
来源：http://zhc.tianlin.xyz

if (( a > b )); then echo "a 更大"; fi
来源：http://lzm.daria6918.cn

[R09] 字符串比较
来源：http://uhu.havefunace.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://tfk.zhaomingkeji.xyz

[R10] 正则匹配
来源：http://vnv.jinqigufen.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://zbk.zhengqikj.top

[R11] case 多分支
来源：http://ifb.xinyue.icu

case "$1" in
来源：http://asl.316326.xyz

start) echo "启动" ;;
来源：http://xho.jiagoushi.top

stop)  echo "停止" ;;
来源：http://xcm.sjlbkw.cn

*)     echo "未知命令" ;;
来源：http://ayt.9152youxi.cn

esac
来源：http://oqe.ydjk.org.cn

[R12] for 遍历文件
来源：http://vxf.fengsongda.top

for f in *.txt; do echo "$f"; done
来源：http://zgc.svipenyu.cn

[R13] for 计数循环
来源：http://zkg.mhx1999.top

for i in {1..10}; do echo "$i"; done
来源：http://ruz.wangdashe.top

[R14] C 风格 for
来源：http://gah.bjfxy.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ayl.hnxiangtu.top

[R15] while 逐行读文件
来源：http://mie.ehwqpu.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://srx.zhaomingkeji.xyz

[R16] until 等待条件
来源：http://cqa.aibaodan.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://pyd.hywenlv.cn

[R17] 数组定义与取值
来源：http://zkm.jinghuilouyu.cn

arr=(a b c); echo "${arr[0]}"
来源：http://duk.epnwcf.com

[R18] 遍历数组
来源：http://ely.bjfxy.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://doi.yj20258.top

[R19] 数组长度
来源：http://gjl.wangshuangyany.cn

echo "${#arr[@]}"
来源：http://kio.fehbvm.com

[R20] 关联数组（字典）
来源：http://bum.hysaishi.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://aij.chenzaomai.com

[R21] 字符串长度
来源：http://jxd.smart0.xyz

echo "${#s}"
来源：http://nry.aizwys.cn

[R22] 截取子串
来源：http://izd.tian-w.cn

echo "${s:0:5}"
来源：http://tus.chenlongwang.top

[R23] 字符串替换
来源：http://lxr.yuanzhike.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://apa.jinqigufen.top

[R24] 大小写转换
来源：http://bpv.hfpthk.cn

echo "${s^^}"; echo "${s,,}"
来源：http://nnn.gogol.net.cn

[R25] 去后缀 / 去前缀
来源：http://qip.zhongyouzk.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://xsm.xuetiantiany.cn

[R26] 命令替换
来源：http://yff.yfazqb.com

now=$(date +%F); echo "$now"
来源：http://djg.sjlbkw.cn

[R27] 算术展开
来源：http://ibc.vehdjk.com

echo $((1 + 2 * 3))
来源：http://cct.dashuyun.cn

[R28] 浮点运算
来源：http://ubk.hywenlv.cn

echo "scale=2; 10/3" | bc
来源：http://ejj.jinghuilouyu.cn

[R29] 定义函数
来源：http://upt.birdmap.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://vbs.jiagoushi.top

[R30] 函数返回状态码
来源：http://hxr.wangdashe.top

f() { return 0; }; f || echo "失败了"
来源：http://rrr.xingfuxueyuan.xyz

[R31] 局部变量
来源：http://rrn.ehwqpu.com

f() { local x=1; echo "$x"; }
来源：http://bqi.yj20258.top

[R32] 参数个数校验
来源：http://hdw.gogol.net.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://pni.hongshengwenyu.top

[R33] 捕获错误并提示行号
来源：http://fyx.gotoacloud.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ygj.uphjek.com

[R34] 退出时清理
来源：http://ujd.pengpengdd.cyou

trap 'rm -f "$tmp"' EXIT
来源：http://snf.0kj1m.cn

[R35] 后台执行并等待
来源：http://wfv.fengsongda.top

sleep 5 & pid=$!; wait "$pid"
来源：http://pji.yueranfly.top

[R36] 并发执行多个任务
来源：http://wcw.kuanghao11.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://vvm.daxiang520.top

[R37] 把输出赋给变量
来源：http://yuo.ywan-chungtsiang.top

files=$(ls -1)
来源：http://zsy.gzhubu.top

[R38] 管道串联
来源：http://xfq.hnqzz.top

cat a.txt | grep -i error | wc -l
来源：http://cgh.ppjwa.cn

[R39] 重定向标准输出与错误
来源：http://ovg.birdmap.top

cmd > out.log 2>&1
来源：http://wak.zycfv.cn

[R40] 追加写日志
来源：http://ftw.bbcook.cn

echo "log" >> out.log
来源：http://nkr.jqgfzy.top

[R41] 丢弃输出
来源：http://vue.nanxinkj.top

cmd >/dev/null 2>&1
来源：http://tta.daria6918.cn

[R42] 输入重定向
来源：http://xkk.zycfv.cn

wc -l < a.txt
来源：http://hcs.zycfv.cn

[R43] 按名字查找文件
来源：http://edd.nanxuanxn.top

find . -name "*.log" -type f
来源：http://rrv.chenzaomai.com

[R44] 按修改时间查找
来源：http://klb.yangfankeji.com

find . -mtime -7 -type f
来源：http://rnb.aizwys.cn

[R45] 批量删除
来源：http://kdb.pengpengdd.cyou

find . -name "*.tmp" -delete
来源：http://zsw.shanyushiyangkeji.top

[R46] 递归替换文件内容
来源：http://tgz.cqqwz.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://dyt.chenzaomai.com

[R47] sed 单行替换
来源：http://xjq.fktsv.cn

sed -i 's/foo/bar/g' a.txt
来源：http://wtz.jianghu66.top

[R48] awk 取指定列
来源：http://mzu.yj202588.top

awk '{print $1, $3}' a.txt
来源：http://rku.tanke756.top

[R49] awk 带条件
来源：http://xzd.shanyushiyangkeji.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://rni.ywan-chungtsiang.top

[R50] awk 求和
来源：http://ctp.chenzaomai.com

awk '{s += $2} END {print s}' a.txt
来源：http://smy.pycfn.com

[R51] 排序去重取前几
来源：http://rgs.ppjwa.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://rrq.jqgufenzy.top

[R52] 统计行数
来源：http://pis.316326.xyz

wc -l a.txt
来源：http://hye.316326.xyz

[R53] 查看文件头与实时尾
来源：http://fdn.epnwcf.com

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://tqe.feifeiyinyue.top

[R54] 比较两个文件
来源：http://dih.xinyue.icu

diff a.txt b.txt
来源：http://afr.jinghuilouyu.cn

[R55] 压缩与解压
来源：http://ver.jyoumei.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://kpn.yfazqb.com

[R56] 远程拷贝
来源：http://ohj.yvedp.cn

scp file user@host:/path/
来源：http://hzi.bbcook.cn

[R57] 远程执行命令
来源：http://bwz.tarul.cn

ssh user@host 'uptime'
来源：http://rnv.mhx1999.top

[R58] 下载文件
来源：http://bhp.zhaomingkeji.xyz

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://aop.yj202588.top

[R59] 发 POST JSON
来源：http://xiy.guannengcc.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://asg.xinyue.icu

[R60] 只看 HTTP 状态码
来源：http://tdi.yj20258888.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ogb.pycfn.com

[R61] 磁盘占用
来源：http://fib.xuanzx.com

df -h;  du -sh *
来源：http://bev.cqqwz.cn

[R62] 找最占空间的文件
来源：http://uhk.pengpengdd.cyou

du -ah . | sort -rh | head -10
来源：http://liw.zdqjudy.top

[R63] 内存与进程
来源：http://wdp.zhengqikj.top

free -h;  ps aux | grep nginx
来源：http://grm.meibo888.top

[R64] 结束进程
来源：http://nhr.nanxinkj.top

kill -9 $(pgrep -f app.py)
来源：http://wdm.xylfe.cn

[R65] 查看端口占用
来源：http://ivy.fengsongda.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://glx.wangshuangyany.cn

[R66] 定时任务
来源：http://smw.sjlbkw.cn

crontab -e;  crontab -l
来源：http://mdq.jqgfzy.top

[R67] 生成随机十六进制串
来源：http://ydo.nwbrower.top

openssl rand -hex 16
来源：http://phv.ivvv.top

[R68] 计算文件校验值
来源：http://txr.dashuyun.cn

sha256sum a.txt;  md5sum a.txt
来源：http://uwi.ywan-chungtsiang.top

[R69] 生成随机密码
来源：http://aum.tian-w.cn

head -c 16 /dev/urandom | base64
来源：http://zhr.mhx1999.top

[R70] 时间戳与互转
来源：http://bdv.zhaomingkeji.xyz

date +%s;  date -d @1700000000
来源：http://wxe.zhiwuduotai.top

[R71] 日期格式化
来源：http://bxa.feifeiyinyue.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://ris.jlsjyb.cn

[R72] 等待端口就绪
来源：http://nae.tarul.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ubk.52xcode.cn

[R73] 分割大日志
来源：http://sxs.hfpthk.cn

split -l 1000 big.log part_
来源：http://qtu.snrcjt.cn

[R74] 批量重命名
来源：http://jcr.jianghu66.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ipt.wangdashe.top

[R75] 导出环境变量
来源：http://jnh.yvedp.cn

export PATH="$HOME/bin:$PATH"
来源：http://uss.zhiwuduotai.top

[R76] 使用临时文件
来源：http://zrt.cucudq.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ard.yj20258.top

[R77] 读取用户输入
来源：http://muc.yanxiufei.cn

read -rp "请输入: " ans
来源：http://zke.zhaomingkeji.xyz

[R78] 交互式菜单
来源：http://pim.shanyushiyangkeji.top

select opt in a b c; do echo "$opt"; break; done
来源：http://vjb.gotoacloud.top

[R79] 解析命令行选项
来源：http://zsz.uphjek.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mva.tian-w.cn

[R80] 查看脚本执行耗时
来源：http://wkh.fanxiaobao.xyz

time ./run.sh
来源：http://ago.xziqi.cn

================================================================================
来源：http://rjl.daria6918.cn

S. C / C++ 专题
来源：http://rbe.gaohongyu789.top

================================================================================
来源：http://zhl.jinyuanbaomall.cn

[S01] C：Hello World
来源：http://lug.shzxlz.cn

#include <stdio.h>
来源：http://aza.uphjek.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://mgg.chenzaomai.com

[S02] C：变量与格式化输出
来源：http://dbq.guowangkeji.top

int a = 10; printf("%d\n", a);
来源：http://spr.ywan-chungtsiang.top

[S03] C：读入整数
来源：http://qri.chenlongwang.top


<!-- 参考信息 -->