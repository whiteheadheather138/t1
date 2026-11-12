代发 wailian999

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://oxn.svipenyu.cn

) t WHERE rn = 1;
来源：http://fav.andypj.xyz

[Q35] 内连接
来源：http://dni.ctjpmb.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mtl.xuetiantiany.cn

[Q36] 左连接
来源：http://snq.yuxming.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://agy.hywenlv.cn

[Q37] 右连接
来源：http://bdg.shuidangran.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ygt.9152youxi.cn

[Q38] 全外连接（PostgreSQL）
来源：http://nga.yueranfly.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://iep.yueranfly.top

[Q39] 自连接（查上下级）
来源：http://hky.nwbrower.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://ucz.andypj.xyz

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ydr.hywenlv.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://pvs.316326.xyz

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mdw.hysaishi.cn

[Q41] 多表连接
来源：http://ybb.hnxiangtu.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://mtq.andypj.xyz

JOIN users u ON u.id = o.user_id
来源：http://ygd.cashguo.top

JOIN products p ON p.id = o.product_id;
来源：http://rjz.quarkkingdee.top

[Q42] 连接条件附加过滤
来源：http://joj.ehwqpu.com

SELECT u.name, o.amount FROM users u
来源：http://hay.redwolf501.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://rjm.fanxiaobao.xyz

[Q43] 标量子查询
来源：http://qfq.jiagoushi.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://yhw.hfpthk.cn

[Q44] IN 子查询
来源：http://ojp.meibo888.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://pjr.hongshengwenyu.top

[Q45] EXISTS 判断存在
来源：http://xon.snrcjt.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://twh.zdqjudy.top

[Q46] NOT EXISTS 判断不存在
来源：http://aag.zhaomingkeji.xyz

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://yqs.ctjpmb.com

[Q47] 与平均值比较
来源：http://nxh.feifeiyinyue.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://zab.zhijiandao.cn

[Q48] CTE 公用表表达式
来源：http://kcf.sufxvd.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://qcx.yuxming.cn

SELECT * FROM t WHERE c > 5;
来源：http://obe.zycfv.cn

[Q49] 更新单行
来源：http://zws.jinqigfzy.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ofu.sufxvd.cn

[Q50] 批量更新
来源：http://bbp.zdqjudy.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://tcc.jyoumei.cn

[Q51] 用子查询更新
来源：http://cnl.yuxming.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://nzj.zhijiandao.cn

[Q52] 删除指定行
来源：http://uwc.cqqwz.cn

DELETE FROM users WHERE id = 10;
来源：http://rgh.smart0.xyz

[Q53] 按条件删除
来源：http://rpl.epnwcf.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hko.xuanzx.com

[Q54] 清空表
来源：http://wxr.jlsjyb.cn

TRUNCATE TABLE logs;
来源：http://ddt.chenlongwang.top

[Q55] 排名（并列占位）
来源：http://uvx.nwbrower.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://msx.vqdsnc.cn

[Q56] 密集排名（并列不占位）
来源：http://snw.zhongyouzk.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://diq.yj20258.top

[Q57] 行号
来源：http://kaa.yueranfly.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://cgo.yueranfly.top

[Q58] 累计求和
来源：http://yxn.kuanghao11.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://cnd.tian-w.cn

[Q59] 分组内累计
来源：http://thm.yvedp.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ahw.yj20258.top

[Q60] 取上一行 / 下一行
来源：http://taa.bbcook.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ivc.shanyushiyangkeji.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://puf.zhixingplan.top

[Q61] 移动平均
来源：http://cnl.ywan-chungtsiang.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://qel.bjfxy.top

[Q62] 分组占比
来源：http://kwz.tarul.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://dpg.jinyuanbaomall.cn

[Q63] 开启事务
来源：http://cnu.ybcxt.top

START TRANSACTION;                -- 或 BEGIN
来源：http://odx.fktsv.cn

[Q64] 提交事务
来源：http://bzg.yfazqb.com

COMMIT;
来源：http://yis.316326.xyz

[Q65] 回滚事务
来源：http://dfl.vqdsnc.cn

ROLLBACK;
来源：http://upp.hfpthk.cn

[Q66] 行锁查询
来源：http://xcc.chenlongwang.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hyz.gotoacloud.top

[Q67] 设置隔离级别
来源：http://skt.aibaodan.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://off.fehbvm.com

[Q68] 保存点
来源：http://ymz.tian-w.cn

SAVEPOINT sp1;
来源：http://eyt.yongpay.top

ROLLBACK TO sp1;
来源：http://ddd.ydjk.org.cn

[Q69] 查看执行计划
来源：http://hqv.9152youxi.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://lcm.0kj1m.cn

[Q70] 更新统计信息
来源：http://cja.bbcook.cn

ANALYZE TABLE users;
来源：http://vmw.zhongyouzk.top

[Q71] 查看建表语句
来源：http://ypj.yj202588.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ech.jlsjyb.cn

[Q72] 查看索引
来源：http://nnc.bbcook.cn

SHOW INDEX FROM users;
来源：http://wdc.daxiang520.top

[Q73] 查看表状态
来源：http://sva.fengsongda.top

SHOW TABLE STATUS LIKE 'users';
来源：http://eli.jyoumei.cn

[Q74] 强制使用索引
来源：http://pfm.shuidangran.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://eeo.gogol.net.cn

[Q75] 日期格式化
来源：http://kfa.shanyushiyangtech.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://nvx.52xcode.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wbe.yueranfly.top

[Q76] 按天统计
来源：http://fep.iojbl.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ffe.zhaomingkeji.xyz

[Q77] 时间加减
来源：http://trg.zhijiandao.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ikv.tanke756.top

[Q78] 当前时间
来源：http://zbw.cdnleiting.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://sid.tianlin.xyz

[Q79] 字符串拼接
来源：http://zgz.jlsjyb.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://jik.yvedp.cn

[Q80] 字符串截取
来源：http://rmv.zhiwuduotai.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://epx.hcnkem.com

[Q81] 字符串替换
来源：http://iat.sxryk.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://bmo.jqgfzy.top

[Q82] 字符长度与字节长度
来源：http://fmd.hywenlv.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://uwa.dianchejie.cn

[Q83] 大小写转换
来源：http://psd.sjlbkw.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://kpi.sjlbkw.cn

[Q84] 去除首尾空格
来源：http://srb.sjlbkw.cn

SELECT TRIM(name) FROM users;
来源：http://jdo.wangdashe.top

[Q85] 数值取整
来源：http://ujz.ydjk.org.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wfq.chenzaomai.com

[Q86] 读取 JSON 字段
来源：http://tqg.epnwcf.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://enn.smart0.xyz

[Q87] JSON 字段做条件
来源：http://khc.havefunace.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://igm.tian-w.cn

[Q88] 行转列（条件聚合）
来源：http://mgw.ybcxt.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://kyc.chenzaomai.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://bfr.ppjwa.cn

[Q89] 判断表是否存在
来源：http://lky.chenjidiqi.icu

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://dhx.gaohongyu789.top

[Q90] 生成序号列
来源：http://ars.kuanghao11.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://iog.meibo888.top

================================================================================
来源：http://jbt.sjlbkw.cn

R. Bash 专题
来源：http://ark.hammf.cn

================================================================================
来源：http://anf.c1oappe.top

[R01] shebang 与严格模式
来源：http://rlx.hesvh.cn

#!/usr/bin/env bash
来源：http://ptl.havefunace.top

set -euo pipefail
来源：http://xtc.tarul.cn

[R02] 变量赋值与使用
来源：http://scp.ppjwa.cn

name="Tom"; echo "$name"
来源：http://fdl.fanxiaobao.xyz

[R03] 只读变量
来源：http://iqs.fanxiaobao.xyz

readonly PI=3.14
来源：http://aqn.jinqigufen.top

[R04] 位置参数
来源：http://wcf.nwbrower.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://jek.fehbvm.com

[R05] 参数默认值
来源：http://rnt.andypj.xyz

name="${1:-default}"
来源：http://col.gzhubu.top

[R06] 判断命令是否存在
来源：http://qih.havefunace.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://fvb.yj20258888.top

[R07] if 判断文件
来源：http://jvt.nwbrower.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://flh.yuxming.cn

[R08] 数值比较
来源：http://slq.gzhubu.top

if (( a > b )); then echo "a 更大"; fi
来源：http://djy.yuanzhike.top

[R09] 字符串比较
来源：http://sku.shzxlz.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mmi.cqqwz.cn

[R10] 正则匹配
来源：http://arx.snrcjt.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://kbs.daria6918.cn

[R11] case 多分支
来源：http://mmv.9152youxi.cn

case "$1" in
来源：http://ydo.hcnkem.com

start) echo "启动" ;;
来源：http://ilo.bjfxy.top

stop)  echo "停止" ;;
来源：http://ppu.daria6918.cn

*)     echo "未知命令" ;;
来源：http://wbe.pengpengdd.cyou

esac
来源：http://foh.yangfankeji.com

[R12] for 遍历文件
来源：http://mmm.ppjwa.cn

for f in *.txt; do echo "$f"; done
来源：http://swp.hysaishi.cn

[R13] for 计数循环
来源：http://wxt.jiagoushi.top

for i in {1..10}; do echo "$i"; done
来源：http://phr.ctjpmb.com

[R14] C 风格 for
来源：http://hpr.daria6918.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://zhf.gogol.net.cn

[R15] while 逐行读文件
来源：http://xpn.zhijiandao.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://lcr.gotoacloud.top

[R16] until 等待条件
来源：http://ket.guowangkeji.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://qwq.jinyuanbaomall.cn

[R17] 数组定义与取值
来源：http://avh.fengsongda.top

arr=(a b c); echo "${arr[0]}"
来源：http://jed.zhaomingkeji.xyz

[R18] 遍历数组
来源：http://bqf.sysykeji.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ges.cdnleiting.top

[R19] 数组长度
来源：http://jgu.zhixingplan.top

echo "${#arr[@]}"
来源：http://mfi.jqgufenzy.top

[R20] 关联数组（字典）
来源：http://ysx.gogol.net.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://yux.jinqigfzy.top

[R21] 字符串长度
来源：http://sed.sufxvd.cn

echo "${#s}"
来源：http://fmr.jinyuanbaomall.cn

[R22] 截取子串
来源：http://tkq.hesvh.cn

echo "${s:0:5}"
来源：http://war.xingfuxueyuan.xyz

[R23] 字符串替换
来源：http://ulk.haohaochexian.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://xxq.xuanzx.com

[R24] 大小写转换
来源：http://mwe.zhixingplan.top

echo "${s^^}"; echo "${s,,}"
来源：http://gau.yj202588.top

[R25] 去后缀 / 去前缀
来源：http://raw.jyoumei.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://hni.feifeiyinyue.top

[R26] 命令替换
来源：http://ixg.fktsv.cn

now=$(date +%F); echo "$now"
来源：http://mft.andypj.xyz

[R27] 算术展开
来源：http://dwq.jinyuanbaomall.cn

echo $((1 + 2 * 3))
来源：http://kdg.gzhubu.top

[R28] 浮点运算
来源：http://meu.shanyushiyangkeji.top

echo "scale=2; 10/3" | bc
来源：http://toc.hcnkem.com

[R29] 定义函数
来源：http://kwx.zdbjq.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://nma.xuanzx.com

[R30] 函数返回状态码
来源：http://owy.aibaodan.cn

f() { return 0; }; f || echo "失败了"
来源：http://cah.jqgufenzy.top

[R31] 局部变量
来源：http://oel.ydjk.org.cn

f() { local x=1; echo "$x"; }
来源：http://nsv.yongpay.top

[R32] 参数个数校验
来源：http://kkf.ydzc1.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://jvx.dashuyun.cn

[R33] 捕获错误并提示行号
来源：http://ozs.c1oappe.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://uci.sufxvd.cn

[R34] 退出时清理
来源：http://ysh.chenzaomai.com

trap 'rm -f "$tmp"' EXIT
来源：http://qqi.uphjek.com

[R35] 后台执行并等待
来源：http://wgs.zycfv.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://oel.hnxiangtu.top

[R36] 并发执行多个任务
来源：http://dup.yj20258888.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://glf.xinyue.icu

[R37] 把输出赋给变量
来源：http://ytj.vehdjk.com

files=$(ls -1)
来源：http://mvh.wangshuangyany.cn

[R38] 管道串联
来源：http://rmn.jinghuilouyu.cn

cat a.txt | grep -i error | wc -l
来源：http://grp.andypj.xyz

[R39] 重定向标准输出与错误
来源：http://vht.ppjwa.cn

cmd > out.log 2>&1
来源：http://gtr.quarkkingdee.top

[R40] 追加写日志
来源：http://yvx.jinqigfzy.top

echo "log" >> out.log
来源：http://yhp.uphjek.com

[R41] 丢弃输出
来源：http://gii.sxryk.cn

cmd >/dev/null 2>&1
来源：http://gmp.hongshengwenyu.top

[R42] 输入重定向
来源：http://lts.zdbjq.cn

wc -l < a.txt
来源：http://ffj.hammf.cn

[R43] 按名字查找文件
来源：http://fym.c1oappe.top

find . -name "*.log" -type f
来源：http://gmu.fanxiaobao.xyz

[R44] 按修改时间查找
来源：http://krm.smart0.xyz

find . -mtime -7 -type f
来源：http://vsz.ppjwa.cn

[R45] 批量删除
来源：http://iau.jyoumei.cn

find . -name "*.tmp" -delete
来源：http://uox.yanxiufei.cn

[R46] 递归替换文件内容
来源：http://blf.zhoulong.xyz

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://bac.shuidangran.top

[R47] sed 单行替换
来源：http://nff.zhiwuduotai.top

sed -i 's/foo/bar/g' a.txt
来源：http://dck.fengsongda.top

[R48] awk 取指定列
来源：http://cqt.sysykeji.top

awk '{print $1, $3}' a.txt
来源：http://fme.yfazqb.com

[R49] awk 带条件
来源：http://xiv.pengpengdd.cyou

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ybx.tianlin.xyz

[R50] awk 求和
来源：http://rgo.sysykeji.top

awk '{s += $2} END {print s}' a.txt
来源：http://yve.52xcode.cn

[R51] 排序去重取前几
来源：http://nbd.jinqigufen.top

sort a.txt | uniq -c | sort -rn | head
来源：http://elm.birdmap.top

[R52] 统计行数
来源：http://boc.52xcode.cn

wc -l a.txt
来源：http://kse.fktsv.cn

[R53] 查看文件头与实时尾
来源：http://jtu.jqgufenzy.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://tan.zhiwuduotai.top

[R54] 比较两个文件
来源：http://unk.hfpthk.cn

diff a.txt b.txt
来源：http://agq.andypj.xyz

[R55] 压缩与解压
来源：http://mid.zhijiandao.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://tto.52xcode.cn

[R56] 远程拷贝
来源：http://iwy.xinyue.icu

scp file user@host:/path/
来源：http://asl.jyoumei.cn

[R57] 远程执行命令
来源：http://mvv.zdqjudy.top

ssh user@host 'uptime'
来源：http://bgc.zhaomingkeji.xyz

[R58] 下载文件
来源：http://uwz.316326.xyz

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://lnb.hammf.cn

[R59] 发 POST JSON
来源：http://igy.yj20258888.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://xrb.ydjk.org.cn

[R60] 只看 HTTP 状态码
来源：http://chz.guowangkeji.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://nrm.havefunace.top

[R61] 磁盘占用
来源：http://sxy.havefunace.top

df -h;  du -sh *
来源：http://zaq.hongshengwenyu.top

[R62] 找最占空间的文件
来源：http://kzb.shuidangran.top

du -ah . | sort -rh | head -10
来源：http://ooh.nwbrower.top

[R63] 内存与进程
来源：http://gto.jlsjyb.cn

free -h;  ps aux | grep nginx
来源：http://jnp.meibo888.top

[R64] 结束进程
来源：http://uwg.fengsongda.top

kill -9 $(pgrep -f app.py)
来源：http://zxu.gzhubu.top

[R65] 查看端口占用
来源：http://rzr.yangfankeji.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://see.jyoumei.cn

[R66] 定时任务
来源：http://nmq.xziqi.cn

crontab -e;  crontab -l
来源：http://rch.meibo888.top

[R67] 生成随机十六进制串
来源：http://nhy.mhx1999.top

openssl rand -hex 16
来源：http://ctq.xziqi.cn

[R68] 计算文件校验值
来源：http://xdq.jianghu66.top

sha256sum a.txt;  md5sum a.txt
来源：http://lov.jinyuanbaomall.cn

[R69] 生成随机密码
来源：http://mbo.bjfxy.top

head -c 16 /dev/urandom | base64
来源：http://frv.meibo888.top

[R70] 时间戳与互转
来源：http://vuq.c1oappe.top

date +%s;  date -d @1700000000
来源：http://biu.nanxuanxn.top

[R71] 日期格式化
来源：http://wwo.redwolf501.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://uci.ywan-chungtsiang.top

[R72] 等待端口就绪
来源：http://mjq.gzhubu.top

until nc -z localhost 3306; do sleep 1; done
来源：http://eug.9152youxi.cn

[R73] 分割大日志
来源：http://voe.haohaochexian.top

split -l 1000 big.log part_
来源：http://dqo.jqgufenzy.top

[R74] 批量重命名
来源：http://qao.jqgufenzy.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://erp.cdnleiting.top

[R75] 导出环境变量
来源：http://iol.hcnkem.com

export PATH="$HOME/bin:$PATH"
来源：http://lnk.shanyushiyangtech.top

[R76] 使用临时文件
来源：http://cay.nwbrower.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://pgl.yj20258.top

[R77] 读取用户输入
来源：http://tiv.jinqigfzy.top

read -rp "请输入: " ans
来源：http://pjl.shangyingyoupin.top

[R78] 交互式菜单
来源：http://buh.tanke756.top

select opt in a b c; do echo "$opt"; break; done
来源：http://nvr.sysykeji.top

[R79] 解析命令行选项
来源：http://jof.jinqigufen.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://kie.yvedp.cn

[R80] 查看脚本执行耗时
来源：http://wyj.aibaodan.cn

time ./run.sh
来源：http://qpi.zhijiandao.cn

================================================================================
来源：http://bzz.aibaodan.cn

S. C / C++ 专题
来源：http://lqr.yuxming.cn

================================================================================
来源：http://mqd.nwbrower.top

[S01] C：Hello World
来源：http://bus.nanxuanxn.top

#include <stdio.h>
来源：http://mmr.hammf.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://osp.yueranfly.top

[S02] C：变量与格式化输出
来源：http://smm.jiagoushi.top

int a = 10; printf("%d\n", a);
来源：http://qiv.cqqwz.cn

[S03] C：读入整数
来源：http://bhb.svipenyu.cn


<!-- 参考信息 -->