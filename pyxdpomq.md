代发 wailian999

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://axg.haohaochexian.top

) t WHERE rn = 1;
来源：http://qkx.ywan-chungtsiang.top

[Q35] 内连接
来源：http://apt.jqgufenzy.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://cry.cheryme.top

[Q36] 左连接
来源：http://gdl.fktsv.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://zkm.jqgfzy.top

[Q37] 右连接
来源：http://yox.shuidangran.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://rci.fehbvm.com

[Q38] 全外连接（PostgreSQL）
来源：http://lui.nanxinkj.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://nzl.yongpay.top

[Q39] 自连接（查上下级）
来源：http://uyf.chenzaomai.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://gpj.ywan-chungtsiang.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://gcc.dianchejie.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://uoh.cdnleiting.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hop.chenlongwang.top

[Q41] 多表连接
来源：http://yay.ydzc1.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://lpp.yuanzhike.top

JOIN users u ON u.id = o.user_id
来源：http://wov.shangyingyoupin.top

JOIN products p ON p.id = o.product_id;
来源：http://jxl.xuetiantiany.cn

[Q42] 连接条件附加过滤
来源：http://bni.sweek.top

SELECT u.name, o.amount FROM users u
来源：http://dfy.vehdjk.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://kkv.yonumen.top

[Q43] 标量子查询
来源：http://zil.jinghuilouyu.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mhc.vqdsnc.cn

[Q44] IN 子查询
来源：http://jjx.cqqwz.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://bzy.hnqzz.top

[Q45] EXISTS 判断存在
来源：http://mlb.zhongyouzk.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ypv.zhengqikj.top

[Q46] NOT EXISTS 判断不存在
来源：http://omj.yvedp.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ggq.yonumen.top

[Q47] 与平均值比较
来源：http://owr.fengsongda.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://vcw.gogol.net.cn

[Q48] CTE 公用表表达式
来源：http://kyu.nwbrower.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://zwr.zycfv.cn

SELECT * FROM t WHERE c > 5;
来源：http://axv.zhijiandao.cn

[Q49] 更新单行
来源：http://kfc.jqgufenzy.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://fch.haohaochexian.top

[Q50] 批量更新
来源：http://hyx.hfpthk.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://rlr.guowangkeji.top

[Q51] 用子查询更新
来源：http://jev.9152youxi.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ybt.fengsongda.top

[Q52] 删除指定行
来源：http://tqd.ivvv.top

DELETE FROM users WHERE id = 10;
来源：http://ofx.chenzaomai.com

[Q53] 按条件删除
来源：http://pxn.wangdashe.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://rdn.zhengqikj.top

[Q54] 清空表
来源：http://mvb.fehbvm.com

TRUNCATE TABLE logs;
来源：http://rgj.tianlin.xyz

[Q55] 排名（并列占位）
来源：http://xco.birdmap.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://iaf.xuanzx.com

[Q56] 密集排名（并列不占位）
来源：http://zmt.meibo888.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://par.redwolf501.top

[Q57] 行号
来源：http://enq.chenjidiqi.icu

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://rdm.fzhhl.top

[Q58] 累计求和
来源：http://jfk.andypj.xyz

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://jva.52xcode.cn

[Q59] 分组内累计
来源：http://dph.hammf.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ykh.wangshuangyany.cn

[Q60] 取上一行 / 下一行
来源：http://oug.cashguo.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://doo.sjlbkw.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://xxl.shzxlz.cn

[Q61] 移动平均
来源：http://rae.sufxvd.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://gzk.gotoacloud.top

[Q62] 分组占比
来源：http://nrf.chenjidiqi.icu

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://txb.pycfn.com

[Q63] 开启事务
来源：http://ozc.xinyue.icu

START TRANSACTION;                -- 或 BEGIN
来源：http://ffn.vehdjk.com

[Q64] 提交事务
来源：http://jgm.yfazqb.com

COMMIT;
来源：http://ozo.kuanghao11.cn

[Q65] 回滚事务
来源：http://ayt.gaohongyu789.top

ROLLBACK;
来源：http://vlw.316326.xyz

[Q66] 行锁查询
来源：http://ywc.shanyushiyangtech.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://bnq.haohaochexian.top

[Q67] 设置隔离级别
来源：http://tfp.dashuyun.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://lis.birdmap.top

[Q68] 保存点
来源：http://thi.vqdsnc.cn

SAVEPOINT sp1;
来源：http://ftp.aizwys.cn

ROLLBACK TO sp1;
来源：http://ubg.andypj.xyz

[Q69] 查看执行计划
来源：http://gvg.iojbl.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://rsn.gzhubu.top

[Q70] 更新统计信息
来源：http://ybg.gzhubu.top

ANALYZE TABLE users;
来源：http://evx.uphjek.com

[Q71] 查看建表语句
来源：http://fxk.hnqzz.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://weq.smart0.xyz

[Q72] 查看索引
来源：http://igg.tian-w.cn

SHOW INDEX FROM users;
来源：http://sjy.9152youxi.cn

[Q73] 查看表状态
来源：http://kbe.xuetiantiany.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://lui.gotoacloud.top

[Q74] 强制使用索引
来源：http://mbw.xziqi.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://gbw.bbcook.cn

[Q75] 日期格式化
来源：http://ixb.meibo888.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://lho.yongpay.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://rei.andypj.xyz

[Q76] 按天统计
来源：http://ala.tanke756.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://duk.kuanghao11.cn

[Q77] 时间加减
来源：http://tup.guowangkeji.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mhy.yonumen.top

[Q78] 当前时间
来源：http://gdt.fehbvm.com

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://eex.hcnkem.com

[Q79] 字符串拼接
来源：http://tpn.sjlbkw.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://rrw.vqdsnc.cn

[Q80] 字符串截取
来源：http://ffp.svipenyu.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://vnb.wangdashe.top

[Q81] 字符串替换
来源：http://gdl.shuidangran.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://kvy.smart0.xyz

[Q82] 字符长度与字节长度
来源：http://jjs.nwbrower.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://jgd.mhx1999.top

[Q83] 大小写转换
来源：http://krn.316326.xyz

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://iur.meibo888.top

[Q84] 去除首尾空格
来源：http://pkf.hysaishi.cn

SELECT TRIM(name) FROM users;
来源：http://gck.yangfankeji.com

[Q85] 数值取整
来源：http://gwx.hnqzz.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://vqi.hammf.cn

[Q86] 读取 JSON 字段
来源：http://ams.yj20258888.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ofj.sufxvd.cn

[Q87] JSON 字段做条件
来源：http://san.iojbl.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://xti.pengpengdd.cyou

[Q88] 行转列（条件聚合）
来源：http://iew.hammf.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://rny.shangyingyoupin.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://myd.hongshengwenyu.top

[Q89] 判断表是否存在
来源：http://mtw.snrcjt.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://uvr.kuanghao11.cn

[Q90] 生成序号列
来源：http://ekp.ctjpmb.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://kms.feifeiyinyue.top

================================================================================
来源：http://ijr.fengsongda.top

R. Bash 专题
来源：http://tpn.jinqigufen.top

================================================================================
来源：http://ecg.fanxiaobao.xyz

[R01] shebang 与严格模式
来源：http://fsg.iojbl.cn

#!/usr/bin/env bash
来源：http://hfm.epnwcf.com

set -euo pipefail
来源：http://zkw.yueranfly.top

[R02] 变量赋值与使用
来源：http://tpl.9152youxi.cn

name="Tom"; echo "$name"
来源：http://mfb.sjlbkw.cn

[R03] 只读变量
来源：http://ndw.xylfe.cn

readonly PI=3.14
来源：http://wfj.jqgufenzy.top

[R04] 位置参数
来源：http://lwn.meibo888.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://aby.sufxvd.cn

[R05] 参数默认值
来源：http://mxe.cdnleiting.top

name="${1:-default}"
来源：http://yza.cdnleiting.top

[R06] 判断命令是否存在
来源：http://cez.yj202588.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ltz.chenjidiqi.icu

[R07] if 判断文件
来源：http://ims.iojbl.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://cfp.nanxinkj.top

[R08] 数值比较
来源：http://zeu.fehbvm.com

if (( a > b )); then echo "a 更大"; fi
来源：http://dqb.xylfe.cn

[R09] 字符串比较
来源：http://eln.jqgfzy.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://zxo.gaohongyu789.top

[R10] 正则匹配
来源：http://vyx.jlsjyb.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ima.zdqjudy.top

[R11] case 多分支
来源：http://qxy.hnxiangtu.top

case "$1" in
来源：http://gkx.fktsv.cn

start) echo "启动" ;;
来源：http://bvb.shuidangran.top

stop)  echo "停止" ;;
来源：http://eed.fzhhl.top

*)     echo "未知命令" ;;
来源：http://urj.tanke756.top

esac
来源：http://hmp.vehdjk.com

[R12] for 遍历文件
来源：http://qxf.quarkkingdee.top

for f in *.txt; do echo "$f"; done
来源：http://ufy.shangyingyoupin.top

[R13] for 计数循环
来源：http://rbo.cashguo.top

for i in {1..10}; do echo "$i"; done
来源：http://vep.shanyushiyangkeji.top

[R14] C 风格 for
来源：http://bmg.fanxiaobao.xyz

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ahc.ivvv.top

[R15] while 逐行读文件
来源：http://jjg.zdqjudy.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://bvv.guannengcc.top

[R16] until 等待条件
来源：http://wgc.yfazqb.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://elz.zhijiandao.cn

[R17] 数组定义与取值
来源：http://xit.havefunace.top

arr=(a b c); echo "${arr[0]}"
来源：http://ucn.sysykeji.top

[R18] 遍历数组
来源：http://kjq.ydjk.org.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://qrb.bbcook.cn

[R19] 数组长度
来源：http://kia.hfpthk.cn

echo "${#arr[@]}"
来源：http://lbb.uphjek.com

[R20] 关联数组（字典）
来源：http://vut.sxryk.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://qpe.wangdashe.top

[R21] 字符串长度
来源：http://ivt.shzxlz.cn

echo "${#s}"
来源：http://hek.guowangkeji.top

[R22] 截取子串
来源：http://dzs.nanxinkj.top

echo "${s:0:5}"
来源：http://roq.dashuyun.cn

[R23] 字符串替换
来源：http://sod.redwolf501.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://kdu.316326.xyz

[R24] 大小写转换
来源：http://bjn.cucudq.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ggw.cashguo.top

[R25] 去后缀 / 去前缀
来源：http://yeb.xziqi.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://gwi.jinqigufen.top

[R26] 命令替换
来源：http://vym.yj202588.top

now=$(date +%F); echo "$now"
来源：http://pqh.yongpay.top

[R27] 算术展开
来源：http://yeh.gaohongyu789.top

echo $((1 + 2 * 3))
来源：http://yij.ybcxt.top

[R28] 浮点运算
来源：http://pxg.yanxiufei.cn

echo "scale=2; 10/3" | bc
来源：http://hgb.9152youxi.cn

[R29] 定义函数
来源：http://mow.zhengqikj.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://rzs.fengsongda.top

[R30] 函数返回状态码
来源：http://ofd.gaohongyu789.top

f() { return 0; }; f || echo "失败了"
来源：http://ieu.yongpay.top

[R31] 局部变量
来源：http://omc.tianlin.xyz

f() { local x=1; echo "$x"; }
来源：http://qnq.xylfe.cn

[R32] 参数个数校验
来源：http://yvx.jqgufenzy.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://sqi.fengsongda.top

[R33] 捕获错误并提示行号
来源：http://rew.chenjidiqi.icu

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://pxk.aizwys.cn

[R34] 退出时清理
来源：http://ufp.jinghuilouyu.cn

trap 'rm -f "$tmp"' EXIT
来源：http://nqq.xingfuxueyuan.xyz

[R35] 后台执行并等待
来源：http://ryy.zycfv.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://svr.feifeiyinyue.top

[R36] 并发执行多个任务
来源：http://qaz.kuanghao11.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://eaf.vehdjk.com

[R37] 把输出赋给变量
来源：http://znf.chenzaomai.com

files=$(ls -1)
来源：http://syo.hywenlv.cn

[R38] 管道串联
来源：http://tqx.daxiang520.top

cat a.txt | grep -i error | wc -l
来源：http://xij.tian-w.cn

[R39] 重定向标准输出与错误
来源：http://agv.gotoacloud.top

cmd > out.log 2>&1
来源：http://rxp.jinyuanbaomall.cn

[R40] 追加写日志
来源：http://uxe.chenjidiqi.icu

echo "log" >> out.log
来源：http://feg.hongshengwenyu.top

[R41] 丢弃输出
来源：http://qhp.guannengcc.top

cmd >/dev/null 2>&1
来源：http://naw.tianlin.xyz

[R42] 输入重定向
来源：http://lli.shuidangran.top

wc -l < a.txt
来源：http://aev.zhaomingkeji.xyz

[R43] 按名字查找文件
来源：http://tkz.fzhhl.top

find . -name "*.log" -type f
来源：http://smn.9152youxi.cn

[R44] 按修改时间查找
来源：http://uim.tarul.cn

find . -mtime -7 -type f
来源：http://obk.gotoacloud.top

[R45] 批量删除
来源：http://vtx.tanke756.top

find . -name "*.tmp" -delete
来源：http://vzx.0kj1m.cn

[R46] 递归替换文件内容
来源：http://hbf.birdmap.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://qoe.zhongyouzk.top

[R47] sed 单行替换
来源：http://mct.nanxinkj.top

sed -i 's/foo/bar/g' a.txt
来源：http://vnb.jqgufenzy.top

[R48] awk 取指定列
来源：http://nqu.xuetiantiany.cn

awk '{print $1, $3}' a.txt
来源：http://rpl.birdmap.top

[R49] awk 带条件
来源：http://cpp.xuetiantiany.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://khv.bjfxy.top

[R50] awk 求和
来源：http://jen.cheryme.top

awk '{s += $2} END {print s}' a.txt
来源：http://sly.fehbvm.com

[R51] 排序去重取前几
来源：http://ril.gogol.net.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://kdm.vqdsnc.cn

[R52] 统计行数
来源：http://zyt.aibaodan.cn

wc -l a.txt
来源：http://sxa.sufxvd.cn

[R53] 查看文件头与实时尾
来源：http://wig.mhx1999.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://cvw.pycfn.com

[R54] 比较两个文件
来源：http://shk.tanke756.top

diff a.txt b.txt
来源：http://axw.shanyushiyangtech.top

[R55] 压缩与解压
来源：http://wnd.jinqigufen.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ugb.316326.xyz

[R56] 远程拷贝
来源：http://wsv.haohaochexian.top

scp file user@host:/path/
来源：http://nru.shangyingyoupin.top

[R57] 远程执行命令
来源：http://dxp.zdqjudy.top

ssh user@host 'uptime'
来源：http://kxd.sjlbkw.cn

[R58] 下载文件
来源：http://zwq.svipenyu.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ujn.tanke756.top

[R59] 发 POST JSON
来源：http://azr.feifeiyinyue.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://iwd.yonumen.top

[R60] 只看 HTTP 状态码
来源：http://mau.pengpengdd.cyou

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://sss.fehbvm.com

[R61] 磁盘占用
来源：http://zew.meibo888.top

df -h;  du -sh *
来源：http://ztw.dianchejie.cn

[R62] 找最占空间的文件
来源：http://tfq.zdqjudy.top

du -ah . | sort -rh | head -10
来源：http://cor.smart0.xyz

[R63] 内存与进程
来源：http://gew.hcnkem.com

free -h;  ps aux | grep nginx
来源：http://nky.epnwcf.com

[R64] 结束进程
来源：http://kfd.hammf.cn

kill -9 $(pgrep -f app.py)
来源：http://oao.hfpthk.cn

[R65] 查看端口占用
来源：http://nbk.fehbvm.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://yvc.zhiwuduotai.top

[R66] 定时任务
来源：http://jik.yfazqb.com

crontab -e;  crontab -l
来源：http://xlo.nanxuanxn.top

[R67] 生成随机十六进制串
来源：http://dvt.feifeiyinyue.top

openssl rand -hex 16
来源：http://qdm.havefunace.top

[R68] 计算文件校验值
来源：http://zze.shzxlz.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ywb.mhx1999.top

[R69] 生成随机密码
来源：http://vid.xziqi.cn

head -c 16 /dev/urandom | base64
来源：http://qyz.52xcode.cn

[R70] 时间戳与互转
来源：http://owg.yj20258.top

date +%s;  date -d @1700000000
来源：http://fgg.jiagoushi.top

[R71] 日期格式化
来源：http://kdo.52xcode.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://hvz.sweek.top

[R72] 等待端口就绪
来源：http://opj.yonumen.top

until nc -z localhost 3306; do sleep 1; done
来源：http://skd.bbcook.cn

[R73] 分割大日志
来源：http://rkl.jyoumei.cn

split -l 1000 big.log part_
来源：http://ujq.ydjk.org.cn

[R74] 批量重命名
来源：http://jfi.xylfe.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://gfn.jqgufenzy.top

[R75] 导出环境变量
来源：http://yed.fengsongda.top

export PATH="$HOME/bin:$PATH"
来源：http://yfw.cucudq.cn

[R76] 使用临时文件
来源：http://fco.hysaishi.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://sxv.vehdjk.com

[R77] 读取用户输入
来源：http://ieu.pengpengdd.cyou

read -rp "请输入: " ans
来源：http://wza.nanxinkj.top

[R78] 交互式菜单
来源：http://efz.birdmap.top

select opt in a b c; do echo "$opt"; break; done
来源：http://cwh.zdbjq.cn

[R79] 解析命令行选项
来源：http://fxc.yj20258888.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://kjb.xuetiantiany.cn

[R80] 查看脚本执行耗时
来源：http://tsr.0kj1m.cn

time ./run.sh
来源：http://neb.jianghu66.top

================================================================================
来源：http://hxy.shanyushiyangkeji.top

S. C / C++ 专题
来源：http://owg.xylfe.cn

================================================================================
来源：http://jcv.gaohongyu789.top

[S01] C：Hello World
来源：http://wcr.chenjidiqi.icu

#include <stdio.h>
来源：http://zyh.gotoacloud.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://jhf.jianghu66.top

[S02] C：变量与格式化输出
来源：http://von.tian-w.cn

int a = 10; printf("%d\n", a);
来源：http://zxv.xinyue.icu

[S03] C：读入整数
来源：http://pys.xziqi.cn


<!-- 参考信息 -->