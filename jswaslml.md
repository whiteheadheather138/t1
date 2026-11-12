代发 wailian999

SELECT MAX(age), MIN(age) FROM users;
来源：http://wfu.nanxinkj.top

[Q30] 分组统计
来源：http://vgt.uphjek.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ban.jiagoushi.top

[Q31] 分组后过滤
来源：http://uus.hnqzz.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://vvq.xuanzx.com

[Q32] 分组拼接字符串
来源：http://lrd.xinyue.icu

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://rpq.dashuyun.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://vel.fanxiaobao.xyz

[Q33] 多列分组
来源：http://jzu.fzhhl.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://gdx.tianlin.xyz

[Q34] 每组取第一条
来源：http://mhc.zhijiandao.cn

SELECT * FROM (
来源：http://fqs.tian-w.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://jgt.yuanzhike.top

) t WHERE rn = 1;
来源：http://zqc.shanyushiyangtech.top

[Q35] 内连接
来源：http://lpe.yongpay.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://gmj.gogol.net.cn

[Q36] 左连接
来源：http://wjq.gzhubu.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://cyp.shuidangran.top

[Q37] 右连接
来源：http://vlj.cucudq.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mjc.0kj1m.cn

[Q38] 全外连接（PostgreSQL）
来源：http://gxa.ydjk.org.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://rbb.fzhhl.top

[Q39] 自连接（查上下级）
来源：http://waf.meibo888.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://jox.gotoacloud.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hnv.aibaodan.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://dlx.hongshengwenyu.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://vce.snrcjt.cn

[Q41] 多表连接
来源：http://nvu.zhaomingkeji.xyz

SELECT o.id, u.name, p.title FROM orders o
来源：http://mtu.chenlongwang.top

JOIN users u ON u.id = o.user_id
来源：http://kvm.316326.xyz

JOIN products p ON p.id = o.product_id;
来源：http://pdk.yueranfly.top

[Q42] 连接条件附加过滤
来源：http://yec.epnwcf.com

SELECT u.name, o.amount FROM users u
来源：http://kfj.ybcxt.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://xrp.yvedp.cn

[Q43] 标量子查询
来源：http://snv.gaohongyu789.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://cbl.fanxiaobao.xyz

[Q44] IN 子查询
来源：http://qrl.tanke756.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hah.aizwys.cn

[Q45] EXISTS 判断存在
来源：http://qxs.gotoacloud.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xoq.chenlongwang.top

[Q46] NOT EXISTS 判断不存在
来源：http://uas.wangshuangyany.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vua.gzhubu.top

[Q47] 与平均值比较
来源：http://lwi.yfazqb.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://zjm.yanxiufei.cn

[Q48] CTE 公用表表达式
来源：http://yus.snrcjt.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://dtp.daxiang520.top

SELECT * FROM t WHERE c > 5;
来源：http://nnq.meibo888.top

[Q49] 更新单行
来源：http://fie.feifeiyinyue.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://pkv.cqqwz.cn

[Q50] 批量更新
来源：http://zxq.jyoumei.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://xjj.zhaomingkeji.xyz

[Q51] 用子查询更新
来源：http://ovb.hesvh.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://kxi.svipenyu.cn

[Q52] 删除指定行
来源：http://zhe.ydjk.org.cn

DELETE FROM users WHERE id = 10;
来源：http://ifn.mhx1999.top

[Q53] 按条件删除
来源：http://sgx.jianghu66.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ykb.yanxiufei.cn

[Q54] 清空表
来源：http://djo.sysykeji.top

TRUNCATE TABLE logs;
来源：http://zov.jianghu66.top

[Q55] 排名（并列占位）
来源：http://wor.9152youxi.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://oqs.yueranfly.top

[Q56] 密集排名（并列不占位）
来源：http://imo.hfpthk.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://kfx.birdmap.top

[Q57] 行号
来源：http://ajv.svipenyu.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wtx.smart0.xyz

[Q58] 累计求和
来源：http://pyo.smart0.xyz

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://zhd.zhengqikj.top

[Q59] 分组内累计
来源：http://azy.hfpthk.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://onn.dashuyun.cn

[Q60] 取上一行 / 下一行
来源：http://uym.gzhubu.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://xfa.fktsv.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://tae.zhiwuduotai.top

[Q61] 移动平均
来源：http://phd.ybcxt.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://weq.316326.xyz

[Q62] 分组占比
来源：http://ndj.gotoacloud.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hxq.shuidangran.top

[Q63] 开启事务
来源：http://spk.birdmap.top

START TRANSACTION;                -- 或 BEGIN
来源：http://kwy.jinyuanbaomall.cn

[Q64] 提交事务
来源：http://bji.havefunace.top

COMMIT;
来源：http://asl.jyoumei.cn

[Q65] 回滚事务
来源：http://bot.jinghuilouyu.cn

ROLLBACK;
来源：http://jlm.nanxuanxn.top

[Q66] 行锁查询
来源：http://xev.wangdashe.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://lro.xylfe.cn

[Q67] 设置隔离级别
来源：http://pkd.wangdashe.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://lay.9152youxi.cn

[Q68] 保存点
来源：http://nlx.cdnleiting.top

SAVEPOINT sp1;
来源：http://fst.zhongyouzk.top

ROLLBACK TO sp1;
来源：http://zml.316326.xyz

[Q69] 查看执行计划
来源：http://ezl.hfpthk.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ekw.tianlin.xyz

[Q70] 更新统计信息
来源：http://ilo.gogol.net.cn

ANALYZE TABLE users;
来源：http://wjd.fktsv.cn

[Q71] 查看建表语句
来源：http://zze.0kj1m.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://uoy.jinqigfzy.top

[Q72] 查看索引
来源：http://jkh.yj20258.top

SHOW INDEX FROM users;
来源：http://pxk.feifeiyinyue.top

[Q73] 查看表状态
来源：http://esq.zhongyouzk.top

SHOW TABLE STATUS LIKE 'users';
来源：http://dtc.zhongyouzk.top

[Q74] 强制使用索引
来源：http://wug.haohaochexian.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://yab.andypj.xyz

[Q75] 日期格式化
来源：http://bhe.aibaodan.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mme.snrcjt.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://xki.daxiang520.top

[Q76] 按天统计
来源：http://evl.yuanzhike.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wvr.hammf.cn

[Q77] 时间加减
来源：http://vjy.guowangkeji.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hbs.zhijiandao.cn

[Q78] 当前时间
来源：http://pwc.ctjpmb.com

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://etg.gzhubu.top

[Q79] 字符串拼接
来源：http://pez.gaohongyu789.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://zwc.tianlin.xyz

[Q80] 字符串截取
来源：http://dvf.sxryk.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://utt.haohaochexian.top

[Q81] 字符串替换
来源：http://mih.ppjwa.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://awk.c1oappe.top

[Q82] 字符长度与字节长度
来源：http://zoo.jinghuilouyu.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ric.dashuyun.cn

[Q83] 大小写转换
来源：http://qyu.gotoacloud.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://lfl.tanke756.top

[Q84] 去除首尾空格
来源：http://ifh.chenlongwang.top

SELECT TRIM(name) FROM users;
来源：http://pmh.shanyushiyangtech.top

[Q85] 数值取整
来源：http://wnt.hysaishi.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://daw.zhongyouzk.top

[Q86] 读取 JSON 字段
来源：http://xnr.guannengcc.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wqo.hywenlv.cn

[Q87] JSON 字段做条件
来源：http://hph.zhiwuduotai.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://bjh.daria6918.cn

[Q88] 行转列（条件聚合）
来源：http://gex.daxiang520.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://vct.52xcode.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://whl.zhengqikj.top

[Q89] 判断表是否存在
来源：http://gpx.yanxiufei.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://uyw.dashuyun.cn

[Q90] 生成序号列
来源：http://rnh.fzhhl.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://dus.mhx1999.top

================================================================================
来源：http://uhy.sjlbkw.cn

R. Bash 专题
来源：http://sqp.vehdjk.com

================================================================================
来源：http://xyo.jiagoushi.top

[R01] shebang 与严格模式
来源：http://pyn.316326.xyz

#!/usr/bin/env bash
来源：http://urg.yfazqb.com

set -euo pipefail
来源：http://qzq.haohaochexian.top

[R02] 变量赋值与使用
来源：http://msy.zhaomingkeji.xyz

name="Tom"; echo "$name"
来源：http://atf.xylfe.cn

[R03] 只读变量
来源：http://syw.zdqjudy.top

readonly PI=3.14
来源：http://edx.yj202588.top

[R04] 位置参数
来源：http://ecu.vehdjk.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mjr.hnxiangtu.top

[R05] 参数默认值
来源：http://vez.zycfv.cn

name="${1:-default}"
来源：http://kle.hysaishi.cn

[R06] 判断命令是否存在
来源：http://pak.yfazqb.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://cxt.yuxming.cn

[R07] if 判断文件
来源：http://ivq.ctjpmb.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://kml.yvedp.cn

[R08] 数值比较
来源：http://uvk.sweek.top

if (( a > b )); then echo "a 更大"; fi
来源：http://cym.yvedp.cn

[R09] 字符串比较
来源：http://mub.haohaochexian.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mtd.tianlin.xyz

[R10] 正则匹配
来源：http://dsp.jlsjyb.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://dyh.yvedp.cn

[R11] case 多分支
来源：http://tjh.chenjidiqi.icu

case "$1" in
来源：http://mfp.snrcjt.cn

start) echo "启动" ;;
来源：http://meh.zhiwuduotai.top

stop)  echo "停止" ;;
来源：http://xce.jianghu66.top

*)     echo "未知命令" ;;
来源：http://jka.yueranfly.top

esac
来源：http://uby.tarul.cn

[R12] for 遍历文件
来源：http://ymg.vehdjk.com

for f in *.txt; do echo "$f"; done
来源：http://ptv.yj202588.top

[R13] for 计数循环
来源：http://mlx.yongpay.top

for i in {1..10}; do echo "$i"; done
来源：http://kih.shanyushiyangkeji.top

[R14] C 风格 for
来源：http://zpl.jqgfzy.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://jym.ctjpmb.com

[R15] while 逐行读文件
来源：http://vuk.yj20258888.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mub.guannengcc.top

[R16] until 等待条件
来源：http://tla.fanxiaobao.xyz

until [[ -f done.flag ]]; do sleep 1; done
来源：http://kxp.epnwcf.com

[R17] 数组定义与取值
来源：http://zer.hysaishi.cn

arr=(a b c); echo "${arr[0]}"
来源：http://rsb.hysaishi.cn

[R18] 遍历数组
来源：http://iam.chenzaomai.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://lne.uphjek.com

[R19] 数组长度
来源：http://ifj.chenjidiqi.icu

echo "${#arr[@]}"
来源：http://luu.yonumen.top

[R20] 关联数组（字典）
来源：http://enc.havefunace.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://kpl.aibaodan.cn

[R21] 字符串长度
来源：http://ngt.uphjek.com

echo "${#s}"
来源：http://sll.tian-w.cn

[R22] 截取子串
来源：http://bpi.pycfn.com

echo "${s:0:5}"
来源：http://ehx.fzhhl.top

[R23] 字符串替换
来源：http://rxw.xinyue.icu

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://asp.zhixingplan.top

[R24] 大小写转换
来源：http://rbx.smart0.xyz

echo "${s^^}"; echo "${s,,}"
来源：http://rgj.snrcjt.cn

[R25] 去后缀 / 去前缀
来源：http://isi.jinghuilouyu.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://shz.vqdsnc.cn

[R26] 命令替换
来源：http://cgu.redwolf501.top

now=$(date +%F); echo "$now"
来源：http://lyg.zhongyouzk.top

[R27] 算术展开
来源：http://omm.vehdjk.com

echo $((1 + 2 * 3))
来源：http://xzh.tanke756.top

[R28] 浮点运算
来源：http://yya.vqdsnc.cn

echo "scale=2; 10/3" | bc
来源：http://ntl.ybcxt.top

[R29] 定义函数
来源：http://hmp.cheryme.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://lxq.ywan-chungtsiang.top

[R30] 函数返回状态码
来源：http://uwf.52xcode.cn

f() { return 0; }; f || echo "失败了"
来源：http://ezf.epnwcf.com

[R31] 局部变量
来源：http://dlz.ybcxt.top

f() { local x=1; echo "$x"; }
来源：http://cqi.xingfuxueyuan.xyz

[R32] 参数个数校验
来源：http://wue.wangshuangyany.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://nbb.xylfe.cn

[R33] 捕获错误并提示行号
来源：http://waf.pycfn.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ray.tian-w.cn

[R34] 退出时清理
来源：http://hwl.shanyushiyangtech.top

trap 'rm -f "$tmp"' EXIT
来源：http://ehk.uphjek.com

[R35] 后台执行并等待
来源：http://fqs.bjfxy.top

sleep 5 & pid=$!; wait "$pid"
来源：http://ttx.shanyushiyangkeji.top

[R36] 并发执行多个任务
来源：http://vae.smart0.xyz

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ugk.hesvh.cn

[R37] 把输出赋给变量
来源：http://adk.shzxlz.cn

files=$(ls -1)
来源：http://jus.yongpay.top

[R38] 管道串联
来源：http://wwf.ywan-chungtsiang.top

cat a.txt | grep -i error | wc -l
来源：http://jvd.0kj1m.cn

[R39] 重定向标准输出与错误
来源：http://ddk.hnxiangtu.top

cmd > out.log 2>&1
来源：http://rtd.gzhubu.top

[R40] 追加写日志
来源：http://jqt.chenzaomai.com

echo "log" >> out.log
来源：http://ohx.dashuyun.cn

[R41] 丢弃输出
来源：http://zsy.sysykeji.top

cmd >/dev/null 2>&1
来源：http://jcg.yvedp.cn

[R42] 输入重定向
来源：http://rzm.ehwqpu.com

wc -l < a.txt
来源：http://zct.sysykeji.top

[R43] 按名字查找文件
来源：http://vwu.iojbl.cn

find . -name "*.log" -type f
来源：http://czc.nanxinkj.top

[R44] 按修改时间查找
来源：http://rbc.meibo888.top

find . -mtime -7 -type f
来源：http://mvr.bbcook.cn

[R45] 批量删除
来源：http://btl.shangyingyoupin.top

find . -name "*.tmp" -delete
来源：http://pge.ybcxt.top

[R46] 递归替换文件内容
来源：http://azf.zhoulong.xyz

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ugv.zdbjq.cn

[R47] sed 单行替换
来源：http://gsb.uphjek.com

sed -i 's/foo/bar/g' a.txt
来源：http://wqu.xylfe.cn

[R48] awk 取指定列
来源：http://lmp.quarkkingdee.top

awk '{print $1, $3}' a.txt
来源：http://exx.jlsjyb.cn

[R49] awk 带条件
来源：http://zgd.guowangkeji.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://koe.zhaomingkeji.xyz

[R50] awk 求和
来源：http://otp.0kj1m.cn

awk '{s += $2} END {print s}' a.txt
来源：http://zzg.tarul.cn

[R51] 排序去重取前几
来源：http://jdl.smart0.xyz

sort a.txt | uniq -c | sort -rn | head
来源：http://ove.hfpthk.cn

[R52] 统计行数
来源：http://krh.yonumen.top

wc -l a.txt
来源：http://rpx.0kj1m.cn

[R53] 查看文件头与实时尾
来源：http://wgv.pengpengdd.cyou

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://vmm.ctjpmb.com

[R54] 比较两个文件
来源：http://wbr.316326.xyz

diff a.txt b.txt
来源：http://dng.jiagoushi.top

[R55] 压缩与解压
来源：http://oiw.0kj1m.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wvz.jinqigfzy.top

[R56] 远程拷贝
来源：http://ldn.xingfuxueyuan.xyz

scp file user@host:/path/
来源：http://bxv.mhx1999.top

[R57] 远程执行命令
来源：http://wbs.fengsongda.top

ssh user@host 'uptime'
来源：http://jra.aibaodan.cn

[R58] 下载文件
来源：http://twt.tanke756.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://izn.hnqzz.top

[R59] 发 POST JSON
来源：http://zkg.cdnleiting.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://tsg.yj202588.top

[R60] 只看 HTTP 状态码
来源：http://omi.52xcode.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hxp.fzhhl.top

[R61] 磁盘占用
来源：http://gze.hammf.cn

df -h;  du -sh *
来源：http://wss.bjfxy.top

[R62] 找最占空间的文件
来源：http://sij.sxryk.cn

du -ah . | sort -rh | head -10
来源：http://kvx.xuetiantiany.cn

[R63] 内存与进程
来源：http://rfu.zhaomingkeji.xyz

free -h;  ps aux | grep nginx
来源：http://mgq.xuanzx.com

[R64] 结束进程
来源：http://vgh.jqgufenzy.top

kill -9 $(pgrep -f app.py)
来源：http://jvy.kuanghao11.cn

[R65] 查看端口占用
来源：http://goy.jianghu66.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://bwr.yueranfly.top

[R66] 定时任务
来源：http://qlq.jiagoushi.top

crontab -e;  crontab -l
来源：http://ram.shanyushiyangtech.top

[R67] 生成随机十六进制串
来源：http://nrf.nanxuanxn.top

openssl rand -hex 16
来源：http://mws.gaohongyu789.top

[R68] 计算文件校验值
来源：http://sor.kuanghao11.cn

sha256sum a.txt;  md5sum a.txt
来源：http://onv.dianchejie.cn

[R69] 生成随机密码
来源：http://hji.fanxiaobao.xyz

head -c 16 /dev/urandom | base64
来源：http://jyn.vehdjk.com

[R70] 时间戳与互转
来源：http://xwy.hywenlv.cn

date +%s;  date -d @1700000000
来源：http://hau.gaohongyu789.top

[R71] 日期格式化
来源：http://kte.svipenyu.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://gvj.wangshuangyany.cn

[R72] 等待端口就绪
来源：http://rnz.tianlin.xyz

until nc -z localhost 3306; do sleep 1; done
来源：http://nzq.svipenyu.cn

[R73] 分割大日志
来源：http://psm.chenzaomai.com

split -l 1000 big.log part_
来源：http://qxc.zycfv.cn

[R74] 批量重命名
来源：http://ocw.shangyingyoupin.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://atw.shanyushiyangtech.top

[R75] 导出环境变量
来源：http://wcm.zhoulong.xyz

export PATH="$HOME/bin:$PATH"
来源：http://lbh.sjlbkw.cn

[R76] 使用临时文件
来源：http://fdm.hammf.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ykg.yonumen.top

[R77] 读取用户输入
来源：http://sll.bbcook.cn

read -rp "请输入: " ans
来源：http://cug.bbcook.cn

[R78] 交互式菜单
来源：http://lla.quarkkingdee.top

select opt in a b c; do echo "$opt"; break; done
来源：http://agj.hysaishi.cn

[R79] 解析命令行选项
来源：http://vlg.daxiang520.top


<!-- 参考信息 -->