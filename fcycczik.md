代发 wailian999

[Q36] 左连接
来源：http://dio.xuanzx.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://qyk.wangshuangyany.cn

[Q37] 右连接
来源：http://zps.cashguo.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://pno.vqdsnc.cn

[Q38] 全外连接（PostgreSQL）
来源：http://pka.ctjpmb.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://pps.pycfn.com

[Q39] 自连接（查上下级）
来源：http://ihp.jinqigufen.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://kwu.jlsjyb.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ocm.aibaodan.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://mmd.xziqi.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://grc.tanke756.top

[Q41] 多表连接
来源：http://vda.nwbrower.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://abj.zhongyouzk.top

JOIN users u ON u.id = o.user_id
来源：http://ujm.xylfe.cn

JOIN products p ON p.id = o.product_id;
来源：http://hsf.jinqigufen.top

[Q42] 连接条件附加过滤
来源：http://evu.meibo888.top

SELECT u.name, o.amount FROM users u
来源：http://hxs.mhx1999.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://bmr.yuxming.cn

[Q43] 标量子查询
来源：http://gjc.guannengcc.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://jdv.hongshengwenyu.top

[Q44] IN 子查询
来源：http://tda.bbcook.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://yto.hcnkem.com

[Q45] EXISTS 判断存在
来源：http://tge.ydzc1.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://cuw.zhoulong.xyz

[Q46] NOT EXISTS 判断不存在
来源：http://vny.mhx1999.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hrj.yvedp.cn

[Q47] 与平均值比较
来源：http://sjw.jinqigfzy.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ilf.yongpay.top

[Q48] CTE 公用表表达式
来源：http://shm.yuxming.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://whk.hesvh.cn

SELECT * FROM t WHERE c > 5;
来源：http://tqo.hnxiangtu.top

[Q49] 更新单行
来源：http://olz.ybcxt.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://bye.jiagoushi.top

[Q50] 批量更新
来源：http://tti.sjlbkw.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://kqy.fehbvm.com

[Q51] 用子查询更新
来源：http://phx.vqdsnc.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://jzo.iojbl.cn

[Q52] 删除指定行
来源：http://kcj.cdnleiting.top

DELETE FROM users WHERE id = 10;
来源：http://cix.vqdsnc.cn

[Q53] 按条件删除
来源：http://irg.zhijiandao.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://nlh.xinyue.icu

[Q54] 清空表
来源：http://mre.zhengqikj.top

TRUNCATE TABLE logs;
来源：http://xoe.ppjwa.cn

[Q55] 排名（并列占位）
来源：http://cim.ppjwa.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://lkh.wangdashe.top

[Q56] 密集排名（并列不占位）
来源：http://mca.shanyushiyangkeji.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://uud.yongpay.top

[Q57] 行号
来源：http://vie.ivvv.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://low.yj202588.top

[Q58] 累计求和
来源：http://svg.yj20258888.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://vwl.shzxlz.cn

[Q59] 分组内累计
来源：http://ams.jyoumei.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://qui.jinghuilouyu.cn

[Q60] 取上一行 / 下一行
来源：http://fzp.wangdashe.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://bqa.zycfv.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ogg.xingfuxueyuan.xyz

[Q61] 移动平均
来源：http://mem.iojbl.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://btj.cheryme.top

[Q62] 分组占比
来源：http://hmv.yuanzhike.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://opr.snrcjt.cn

[Q63] 开启事务
来源：http://xjy.svipenyu.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://piz.xingfuxueyuan.xyz

[Q64] 提交事务
来源：http://uhf.tianlin.xyz

COMMIT;
来源：http://vpl.fktsv.cn

[Q65] 回滚事务
来源：http://hvy.epnwcf.com

ROLLBACK;
来源：http://fgi.yuxming.cn

[Q66] 行锁查询
来源：http://gnl.yuxming.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ktz.epnwcf.com

[Q67] 设置隔离级别
来源：http://hnl.xziqi.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ozh.xylfe.cn

[Q68] 保存点
来源：http://bpu.shanyushiyangtech.top

SAVEPOINT sp1;
来源：http://rys.hysaishi.cn

ROLLBACK TO sp1;
来源：http://gye.zycfv.cn

[Q69] 查看执行计划
来源：http://kjm.wangshuangyany.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://jip.hysaishi.cn

[Q70] 更新统计信息
来源：http://epw.yvedp.cn

ANALYZE TABLE users;
来源：http://gyi.guannengcc.top

[Q71] 查看建表语句
来源：http://jbc.jyoumei.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://gzb.gaohongyu789.top

[Q72] 查看索引
来源：http://ymw.jinyuanbaomall.cn

SHOW INDEX FROM users;
来源：http://xzj.jqgfzy.top

[Q73] 查看表状态
来源：http://jit.daxiang520.top

SHOW TABLE STATUS LIKE 'users';
来源：http://kym.hongshengwenyu.top

[Q74] 强制使用索引
来源：http://ukl.hnxiangtu.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://pgj.jqgfzy.top

[Q75] 日期格式化
来源：http://fyl.jiagoushi.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ahs.redwolf501.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mxl.shuidangran.top

[Q76] 按天统计
来源：http://xof.zhijiandao.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://vgf.xuanzx.com

[Q77] 时间加减
来源：http://qia.zhongyouzk.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ell.vehdjk.com

[Q78] 当前时间
来源：http://quu.yanxiufei.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ftu.fengsongda.top

[Q79] 字符串拼接
来源：http://blg.sxryk.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://gby.cqqwz.cn

[Q80] 字符串截取
来源：http://lfn.mhx1999.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://iwg.shangyingyoupin.top

[Q81] 字符串替换
来源：http://erh.mhx1999.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ipc.birdmap.top

[Q82] 字符长度与字节长度
来源：http://gyz.hfpthk.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://tkc.havefunace.top

[Q83] 大小写转换
来源：http://foe.jinqigfzy.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hhp.yj20258.top

[Q84] 去除首尾空格
来源：http://opt.feifeiyinyue.top

SELECT TRIM(name) FROM users;
来源：http://boc.hysaishi.cn

[Q85] 数值取整
来源：http://tna.dianchejie.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://gwu.sxryk.cn

[Q86] 读取 JSON 字段
来源：http://jbv.kuanghao11.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://bbf.yonumen.top

[Q87] JSON 字段做条件
来源：http://mpt.yuanzhike.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hry.yuanzhike.top

[Q88] 行转列（条件聚合）
来源：http://qou.zdqjudy.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wrt.gogol.net.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://opk.sufxvd.cn

[Q89] 判断表是否存在
来源：http://usn.gaohongyu789.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://uib.smart0.xyz

[Q90] 生成序号列
来源：http://uok.zhiwuduotai.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://yie.shzxlz.cn

================================================================================
来源：http://cgm.tarul.cn

R. Bash 专题
来源：http://nba.jiagoushi.top

================================================================================
来源：http://kjz.52xcode.cn

[R01] shebang 与严格模式
来源：http://ott.pycfn.com

#!/usr/bin/env bash
来源：http://bsc.fktsv.cn

set -euo pipefail
来源：http://ysj.tarul.cn

[R02] 变量赋值与使用
来源：http://moc.havefunace.top

name="Tom"; echo "$name"
来源：http://kli.haohaochexian.top

[R03] 只读变量
来源：http://cne.nanxinkj.top

readonly PI=3.14
来源：http://veb.ehwqpu.com

[R04] 位置参数
来源：http://eju.hfpthk.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://lwn.hnxiangtu.top

[R05] 参数默认值
来源：http://vrx.redwolf501.top

name="${1:-default}"
来源：http://nrl.bjfxy.top

[R06] 判断命令是否存在
来源：http://eou.snrcjt.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://tdm.yonumen.top

[R07] if 判断文件
来源：http://cdi.daxiang520.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://bxi.vehdjk.com

[R08] 数值比较
来源：http://rpo.hywenlv.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://xms.andypj.xyz

[R09] 字符串比较
来源：http://lok.gogol.net.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://eqh.shuidangran.top

[R10] 正则匹配
来源：http://rdc.sufxvd.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://fvp.ehwqpu.com

[R11] case 多分支
来源：http://vmy.ppjwa.cn

case "$1" in
来源：http://fes.hywenlv.cn

start) echo "启动" ;;
来源：http://wnq.fanxiaobao.xyz

stop)  echo "停止" ;;
来源：http://vkp.chenzaomai.com

*)     echo "未知命令" ;;
来源：http://eiy.tanke756.top

esac
来源：http://aes.havefunace.top

[R12] for 遍历文件
来源：http://chd.wangdashe.top

for f in *.txt; do echo "$f"; done
来源：http://mcy.zdqjudy.top

[R13] for 计数循环
来源：http://iyp.ywan-chungtsiang.top

for i in {1..10}; do echo "$i"; done
来源：http://rte.shangyingyoupin.top

[R14] C 风格 for
来源：http://ukd.nwbrower.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wza.vqdsnc.cn

[R15] while 逐行读文件
来源：http://sdj.316326.xyz

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://khu.xylfe.cn

[R16] until 等待条件
来源：http://ygn.vehdjk.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://roc.kuanghao11.cn

[R17] 数组定义与取值
来源：http://dpo.yongpay.top

arr=(a b c); echo "${arr[0]}"
来源：http://vgq.zhiwuduotai.top

[R18] 遍历数组
来源：http://yhw.yonumen.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://cgc.cdnleiting.top

[R19] 数组长度
来源：http://zir.52xcode.cn

echo "${#arr[@]}"
来源：http://ptv.fehbvm.com

[R20] 关联数组（字典）
来源：http://amk.tianlin.xyz

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://abw.jlsjyb.cn

[R21] 字符串长度
来源：http://rvy.yongpay.top

echo "${#s}"
来源：http://hze.fzhhl.top

[R22] 截取子串
来源：http://jvv.zycfv.cn

echo "${s:0:5}"
来源：http://scf.52xcode.cn

[R23] 字符串替换
来源：http://fvo.xinyue.icu

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://tbf.xylfe.cn

[R24] 大小写转换
来源：http://phv.iojbl.cn

echo "${s^^}"; echo "${s,,}"
来源：http://asn.wangshuangyany.cn

[R25] 去后缀 / 去前缀
来源：http://pup.jqgufenzy.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://dyl.zhoulong.xyz

[R26] 命令替换
来源：http://pun.nanxinkj.top

now=$(date +%F); echo "$now"
来源：http://pid.shuidangran.top

[R27] 算术展开
来源：http://zvs.quarkkingdee.top

echo $((1 + 2 * 3))
来源：http://xcb.jyoumei.cn

[R28] 浮点运算
来源：http://wqo.ctjpmb.com

echo "scale=2; 10/3" | bc
来源：http://fgb.sufxvd.cn

[R29] 定义函数
来源：http://xym.dashuyun.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://nxi.jinghuilouyu.cn

[R30] 函数返回状态码
来源：http://bwk.cucudq.cn

f() { return 0; }; f || echo "失败了"
来源：http://ejf.jianghu66.top

[R31] 局部变量
来源：http://mgb.zdbjq.cn

f() { local x=1; echo "$x"; }
来源：http://abz.vqdsnc.cn

[R32] 参数个数校验
来源：http://dol.yanxiufei.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://tzz.wangdashe.top

[R33] 捕获错误并提示行号
来源：http://cao.dashuyun.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://xka.ehwqpu.com

[R34] 退出时清理
来源：http://yuu.zdqjudy.top

trap 'rm -f "$tmp"' EXIT
来源：http://qug.xziqi.cn

[R35] 后台执行并等待
来源：http://eug.jinqigfzy.top

sleep 5 & pid=$!; wait "$pid"
来源：http://cxq.xuetiantiany.cn

[R36] 并发执行多个任务
来源：http://tda.jinqigfzy.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://fqr.c1oappe.top

[R37] 把输出赋给变量
来源：http://dvd.ppjwa.cn

files=$(ls -1)
来源：http://jsl.nanxinkj.top

[R38] 管道串联
来源：http://zjc.chenlongwang.top

cat a.txt | grep -i error | wc -l
来源：http://fsu.zycfv.cn

[R39] 重定向标准输出与错误
来源：http://zaa.ehwqpu.com

cmd > out.log 2>&1
来源：http://duj.ctjpmb.com

[R40] 追加写日志
来源：http://egh.dianchejie.cn

echo "log" >> out.log
来源：http://lyz.pycfn.com

[R41] 丢弃输出
来源：http://abt.yuanzhike.top

cmd >/dev/null 2>&1
来源：http://kte.quarkkingdee.top

[R42] 输入重定向
来源：http://lll.yj20258.top

wc -l < a.txt
来源：http://jpa.daria6918.cn

[R43] 按名字查找文件
来源：http://mai.wangshuangyany.cn

find . -name "*.log" -type f
来源：http://woy.nanxinkj.top

[R44] 按修改时间查找
来源：http://ljg.shangyingyoupin.top

find . -mtime -7 -type f
来源：http://qxo.wangdashe.top

[R45] 批量删除
来源：http://xsu.sysykeji.top

find . -name "*.tmp" -delete
来源：http://tnd.tarul.cn

[R46] 递归替换文件内容
来源：http://nxm.ctjpmb.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ahy.hnxiangtu.top

[R47] sed 单行替换
来源：http://pfc.cdnleiting.top

sed -i 's/foo/bar/g' a.txt
来源：http://rsk.cheryme.top

[R48] awk 取指定列
来源：http://qrs.xinyue.icu

awk '{print $1, $3}' a.txt
来源：http://jnj.ywan-chungtsiang.top

[R49] awk 带条件
来源：http://czo.tarul.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ccw.gogol.net.cn

[R50] awk 求和
来源：http://scj.cqqwz.cn

awk '{s += $2} END {print s}' a.txt
来源：http://hwc.redwolf501.top

[R51] 排序去重取前几
来源：http://uyn.sjlbkw.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://pwz.yueranfly.top

[R52] 统计行数
来源：http://hjt.hesvh.cn

wc -l a.txt
来源：http://rps.shuidangran.top

[R53] 查看文件头与实时尾
来源：http://dzr.aibaodan.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mim.haohaochexian.top

[R54] 比较两个文件
来源：http://kze.zhoulong.xyz

diff a.txt b.txt
来源：http://jnl.sxryk.cn

[R55] 压缩与解压
来源：http://ule.aizwys.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ntg.zhoulong.xyz

[R56] 远程拷贝
来源：http://sha.jyoumei.cn

scp file user@host:/path/
来源：http://rwj.hnxiangtu.top

[R57] 远程执行命令
来源：http://yho.jianghu66.top

ssh user@host 'uptime'
来源：http://ycn.yj20258888.top

[R58] 下载文件
来源：http://don.sjlbkw.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://gfq.hnqzz.top

[R59] 发 POST JSON
来源：http://qxg.jyoumei.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://tyq.smart0.xyz

[R60] 只看 HTTP 状态码
来源：http://nht.uphjek.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wie.ydzc1.top

[R61] 磁盘占用
来源：http://lex.ppjwa.cn

df -h;  du -sh *
来源：http://umz.hywenlv.cn

[R62] 找最占空间的文件
来源：http://kex.havefunace.top

du -ah . | sort -rh | head -10
来源：http://wvu.sjlbkw.cn

[R63] 内存与进程
来源：http://kld.ydzc1.top

free -h;  ps aux | grep nginx
来源：http://kqi.0kj1m.cn

[R64] 结束进程
来源：http://dks.zhongyouzk.top

kill -9 $(pgrep -f app.py)
来源：http://ovr.pengpengdd.cyou

[R65] 查看端口占用
来源：http://hav.zhoulong.xyz

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://lhy.chenjidiqi.icu

[R66] 定时任务
来源：http://imr.pycfn.com

crontab -e;  crontab -l
来源：http://lrd.kuanghao11.cn

[R67] 生成随机十六进制串
来源：http://yvp.uphjek.com

openssl rand -hex 16
来源：http://bfa.yuxming.cn

[R68] 计算文件校验值
来源：http://him.pengpengdd.cyou

sha256sum a.txt;  md5sum a.txt
来源：http://xhc.hammf.cn

[R69] 生成随机密码
来源：http://oiu.uphjek.com

head -c 16 /dev/urandom | base64
来源：http://lnh.nanxuanxn.top

[R70] 时间戳与互转
来源：http://uck.hammf.cn

date +%s;  date -d @1700000000
来源：http://zaz.xuanzx.com

[R71] 日期格式化
来源：http://hmw.aizwys.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://atd.daxiang520.top

[R72] 等待端口就绪
来源：http://mpg.zhixingplan.top

until nc -z localhost 3306; do sleep 1; done
来源：http://mum.yueranfly.top

[R73] 分割大日志
来源：http://kkp.zhoulong.xyz

split -l 1000 big.log part_
来源：http://rfj.9152youxi.cn

[R74] 批量重命名
来源：http://omo.yuanzhike.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://pqr.zhongyouzk.top

[R75] 导出环境变量
来源：http://mje.fktsv.cn

export PATH="$HOME/bin:$PATH"
来源：http://xmy.bbcook.cn

[R76] 使用临时文件
来源：http://clc.ywan-chungtsiang.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://fnb.yangfankeji.com

[R77] 读取用户输入
来源：http://oom.nwbrower.top

read -rp "请输入: " ans
来源：http://vep.chenzaomai.com

[R78] 交互式菜单
来源：http://wwv.yuxming.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://btg.sjlbkw.cn

[R79] 解析命令行选项
来源：http://ayz.zhixingplan.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://nga.nanxinkj.top

[R80] 查看脚本执行耗时
来源：http://bzq.xingfuxueyuan.xyz

time ./run.sh
来源：http://mln.dianchejie.cn

================================================================================
来源：http://jfj.cashguo.top

S. C / C++ 专题
来源：http://zyv.havefunace.top

================================================================================
来源：http://ena.kuanghao11.cn

[S01] C：Hello World
来源：http://hat.kuanghao11.cn

#include <stdio.h>
来源：http://unx.sysykeji.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://bwx.gogol.net.cn

[S02] C：变量与格式化输出
来源：http://xpb.aibaodan.cn

int a = 10; printf("%d\n", a);
来源：http://lkp.ehwqpu.com

[S03] C：读入整数
来源：http://dmu.jlsjyb.cn

int x; scanf("%d", &x);
来源：http://ibw.xuetiantiany.cn

[S04] C：字符串复制
来源：http://ajn.jyoumei.cn

char dst[32]; strcpy(dst, "hi");
来源：http://vjm.meibo888.top

[S05] C：字符串长度
来源：http://ctf.jiagoushi.top


<!-- 参考信息 -->