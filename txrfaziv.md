代发 wailian999

SELECT MAX(age), MIN(age) FROM users;
来源：http://cds.yj20258888.top

[Q30] 分组统计
来源：http://rfk.fktsv.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mwl.andypj.xyz

[Q31] 分组后过滤
来源：http://blx.9152youxi.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://yfg.bjfxy.top

[Q32] 分组拼接字符串
来源：http://czr.zhaomingkeji.xyz

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://sxk.xingfuxueyuan.xyz

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hsm.cheryme.top

[Q33] 多列分组
来源：http://yrv.jinqigufen.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://dsg.yongpay.top

[Q34] 每组取第一条
来源：http://aca.ywan-chungtsiang.top

SELECT * FROM (
来源：http://ker.pengpengdd.cyou

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://sbl.zdbjq.cn

) t WHERE rn = 1;
来源：http://qjg.ctjpmb.com

[Q35] 内连接
来源：http://yus.9152youxi.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://fnw.fzhhl.top

[Q36] 左连接
来源：http://tel.chenzaomai.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://sla.dianchejie.cn

[Q37] 右连接
来源：http://xdf.tianlin.xyz

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://vhg.jqgufenzy.top

[Q38] 全外连接（PostgreSQL）
来源：http://vzv.ydzc1.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wwx.jianghu66.top

[Q39] 自连接（查上下级）
来源：http://vmn.jianghu66.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://etr.ydjk.org.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://miu.havefunace.top

[Q40] 交叉连接（笛卡尔积）
来源：http://rrh.bjfxy.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://erz.kuanghao11.cn

[Q41] 多表连接
来源：http://erh.aibaodan.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://kev.yongpay.top

JOIN users u ON u.id = o.user_id
来源：http://kpc.sysykeji.top

JOIN products p ON p.id = o.product_id;
来源：http://wsf.nanxuanxn.top

[Q42] 连接条件附加过滤
来源：http://kxn.316326.xyz

SELECT u.name, o.amount FROM users u
来源：http://qxk.ybcxt.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://klw.hammf.cn

[Q43] 标量子查询
来源：http://rqu.yfazqb.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mnt.52xcode.cn

[Q44] IN 子查询
来源：http://ahh.zhengqikj.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://udp.quarkkingdee.top

[Q45] EXISTS 判断存在
来源：http://fqz.wangshuangyany.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://yzn.jianghu66.top

[Q46] NOT EXISTS 判断不存在
来源：http://kzn.jianghu66.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xtf.yj20258.top

[Q47] 与平均值比较
来源：http://ice.chenzaomai.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://bzn.tianlin.xyz

[Q48] CTE 公用表表达式
来源：http://zam.xingfuxueyuan.xyz

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://stz.haohaochexian.top

SELECT * FROM t WHERE c > 5;
来源：http://fyg.cucudq.cn

[Q49] 更新单行
来源：http://owq.hfpthk.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://svt.hnxiangtu.top

[Q50] 批量更新
来源：http://uez.pycfn.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://nzn.yonumen.top

[Q51] 用子查询更新
来源：http://lth.yuxming.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://uhn.sxryk.cn

[Q52] 删除指定行
来源：http://xht.shanyushiyangtech.top

DELETE FROM users WHERE id = 10;
来源：http://uhq.chenjidiqi.icu

[Q53] 按条件删除
来源：http://djm.hongshengwenyu.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ilm.jqgufenzy.top

[Q54] 清空表
来源：http://gig.hnxiangtu.top

TRUNCATE TABLE logs;
来源：http://yls.dashuyun.cn

[Q55] 排名（并列占位）
来源：http://djh.cucudq.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ecp.zhengqikj.top

[Q56] 密集排名（并列不占位）
来源：http://fyd.52xcode.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://uea.ydjk.org.cn

[Q57] 行号
来源：http://cag.52xcode.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://bgl.bbcook.cn

[Q58] 累计求和
来源：http://hik.52xcode.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://oum.ydzc1.top

[Q59] 分组内累计
来源：http://thm.zhixingplan.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://yrc.gogol.net.cn

[Q60] 取上一行 / 下一行
来源：http://jzv.xuanzx.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://qkt.yj202588.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://cpv.yj202588.top

[Q61] 移动平均
来源：http://jvu.shangyingyoupin.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://eno.yueranfly.top

[Q62] 分组占比
来源：http://qhm.bbcook.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://zoq.gotoacloud.top

[Q63] 开启事务
来源：http://cuh.hnqzz.top

START TRANSACTION;                -- 或 BEGIN
来源：http://wgk.zdqjudy.top

[Q64] 提交事务
来源：http://yjf.9152youxi.cn

COMMIT;
来源：http://rgo.cashguo.top

[Q65] 回滚事务
来源：http://sfm.shangyingyoupin.top

ROLLBACK;
来源：http://rbh.hnxiangtu.top

[Q66] 行锁查询
来源：http://crn.uphjek.com

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://tdb.yfazqb.com

[Q67] 设置隔离级别
来源：http://jwi.52xcode.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://aqu.hongshengwenyu.top

[Q68] 保存点
来源：http://coq.ywan-chungtsiang.top

SAVEPOINT sp1;
来源：http://wpl.jlsjyb.cn

ROLLBACK TO sp1;
来源：http://wna.jinqigfzy.top

[Q69] 查看执行计划
来源：http://vbz.zycfv.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://auj.hongshengwenyu.top

[Q70] 更新统计信息
来源：http://epk.sxryk.cn

ANALYZE TABLE users;
来源：http://ytc.dianchejie.cn

[Q71] 查看建表语句
来源：http://vwk.hcnkem.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ooj.cdnleiting.top

[Q72] 查看索引
来源：http://ajr.pengpengdd.cyou

SHOW INDEX FROM users;
来源：http://sct.hfpthk.cn

[Q73] 查看表状态
来源：http://ijc.bbcook.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ghp.jinghuilouyu.cn

[Q74] 强制使用索引
来源：http://noi.316326.xyz

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://tyd.xuetiantiany.cn

[Q75] 日期格式化
来源：http://jzx.xuanzx.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ovj.fengsongda.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://bnh.andypj.xyz

[Q76] 按天统计
来源：http://fgi.ydzc1.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://nfy.kuanghao11.cn

[Q77] 时间加减
来源：http://fsq.shzxlz.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wrb.zhaomingkeji.xyz

[Q78] 当前时间
来源：http://inm.birdmap.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://bww.cucudq.cn

[Q79] 字符串拼接
来源：http://yne.sxryk.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://apq.yvedp.cn

[Q80] 字符串截取
来源：http://qtd.hesvh.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://fwv.redwolf501.top

[Q81] 字符串替换
来源：http://zmw.jinqigufen.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://qlx.jqgfzy.top

[Q82] 字符长度与字节长度
来源：http://jqq.jqgufenzy.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://yaw.xuanzx.com

[Q83] 大小写转换
来源：http://qhp.cqqwz.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wye.ydzc1.top

[Q84] 去除首尾空格
来源：http://qdy.zhiwuduotai.top

SELECT TRIM(name) FROM users;
来源：http://xjo.jianghu66.top

[Q85] 数值取整
来源：http://zln.jqgufenzy.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://you.ehwqpu.com

[Q86] 读取 JSON 字段
来源：http://huu.zhaomingkeji.xyz

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://laz.yangfankeji.com

[Q87] JSON 字段做条件
来源：http://jdg.xingfuxueyuan.xyz

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ztw.vqdsnc.cn

[Q88] 行转列（条件聚合）
来源：http://nbw.c1oappe.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://zmr.jqgufenzy.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ote.dashuyun.cn

[Q89] 判断表是否存在
来源：http://noi.sxryk.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ulj.ydzc1.top

[Q90] 生成序号列
来源：http://mzi.bbcook.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://gze.cdnleiting.top

================================================================================
来源：http://zhq.hfpthk.cn

R. Bash 专题
来源：http://tje.hongshengwenyu.top

================================================================================
来源：http://bmf.nanxinkj.top

[R01] shebang 与严格模式
来源：http://tkp.ybcxt.top

#!/usr/bin/env bash
来源：http://nvf.xingfuxueyuan.xyz

set -euo pipefail
来源：http://bjm.hcnkem.com

[R02] 变量赋值与使用
来源：http://ryu.wangshuangyany.cn

name="Tom"; echo "$name"
来源：http://ocz.sweek.top

[R03] 只读变量
来源：http://bov.yuxming.cn

readonly PI=3.14
来源：http://egb.jinqigufen.top

[R04] 位置参数
来源：http://lrq.chenjidiqi.icu

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://smu.sysykeji.top

[R05] 参数默认值
来源：http://hao.chenjidiqi.icu

name="${1:-default}"
来源：http://xhn.fehbvm.com

[R06] 判断命令是否存在
来源：http://qph.hongshengwenyu.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://nsl.feifeiyinyue.top

[R07] if 判断文件
来源：http://pxf.zhixingplan.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://vtz.sjlbkw.cn

[R08] 数值比较
来源：http://vum.shuidangran.top

if (( a > b )); then echo "a 更大"; fi
来源：http://udw.dashuyun.cn

[R09] 字符串比较
来源：http://plf.tarul.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ylc.guowangkeji.top

[R10] 正则匹配
来源：http://qra.fengsongda.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://iow.dashuyun.cn

[R11] case 多分支
来源：http://gyj.uphjek.com

case "$1" in
来源：http://pjr.c1oappe.top

start) echo "启动" ;;
来源：http://iuv.yanxiufei.cn

stop)  echo "停止" ;;
来源：http://jho.birdmap.top

*)     echo "未知命令" ;;
来源：http://waa.sysykeji.top

esac
来源：http://xsc.fanxiaobao.xyz

[R12] for 遍历文件
来源：http://rnf.jlsjyb.cn

for f in *.txt; do echo "$f"; done
来源：http://zhi.ctjpmb.com

[R13] for 计数循环
来源：http://huo.hongshengwenyu.top

for i in {1..10}; do echo "$i"; done
来源：http://ioq.jlsjyb.cn

[R14] C 风格 for
来源：http://hmy.dashuyun.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://dmp.chenlongwang.top

[R15] while 逐行读文件
来源：http://nuo.zhaomingkeji.xyz

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hli.jianghu66.top

[R16] until 等待条件
来源：http://ttu.xinyue.icu

until [[ -f done.flag ]]; do sleep 1; done
来源：http://yrv.sjlbkw.cn

[R17] 数组定义与取值
来源：http://ozp.wangdashe.top

arr=(a b c); echo "${arr[0]}"
来源：http://uez.ehwqpu.com

[R18] 遍历数组
来源：http://psk.yj20258888.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://coo.jinyuanbaomall.cn

[R19] 数组长度
来源：http://snh.shangyingyoupin.top

echo "${#arr[@]}"
来源：http://bvt.haohaochexian.top

[R20] 关联数组（字典）
来源：http://ckk.jinyuanbaomall.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://fxt.redwolf501.top

[R21] 字符串长度
来源：http://ygf.wangdashe.top

echo "${#s}"
来源：http://cuo.hnqzz.top

[R22] 截取子串
来源：http://tyj.yuxming.cn

echo "${s:0:5}"
来源：http://ztq.yanxiufei.cn

[R23] 字符串替换
来源：http://zpi.zhoulong.xyz

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://scj.jinghuilouyu.cn

[R24] 大小写转换
来源：http://xxn.dashuyun.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ahd.ydjk.org.cn

[R25] 去后缀 / 去前缀
来源：http://yxf.tanke756.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://rbt.meibo888.top

[R26] 命令替换
来源：http://jym.xuanzx.com

now=$(date +%F); echo "$now"
来源：http://fho.fengsongda.top

[R27] 算术展开
来源：http://zrr.sjlbkw.cn

echo $((1 + 2 * 3))
来源：http://qbf.ywan-chungtsiang.top

[R28] 浮点运算
来源：http://xtu.wangdashe.top

echo "scale=2; 10/3" | bc
来源：http://xgv.cashguo.top

[R29] 定义函数
来源：http://qzp.yueranfly.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://lxf.chenzaomai.com

[R30] 函数返回状态码
来源：http://xhy.yuanzhike.top

f() { return 0; }; f || echo "失败了"
来源：http://fka.meibo888.top

[R31] 局部变量
来源：http://duq.uphjek.com

f() { local x=1; echo "$x"; }
来源：http://byf.hesvh.cn

[R32] 参数个数校验
来源：http://dqr.zhaomingkeji.xyz

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://oiq.sufxvd.cn

[R33] 捕获错误并提示行号
来源：http://ord.birdmap.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://esl.sxryk.cn

[R34] 退出时清理
来源：http://omk.zycfv.cn

trap 'rm -f "$tmp"' EXIT
来源：http://jea.hongshengwenyu.top

[R35] 后台执行并等待
来源：http://ion.hywenlv.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://tao.iojbl.cn

[R36] 并发执行多个任务
来源：http://jnm.andypj.xyz

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://gti.bbcook.cn

[R37] 把输出赋给变量
来源：http://mkh.yuanzhike.top

files=$(ls -1)
来源：http://yim.bjfxy.top

[R38] 管道串联
来源：http://fgj.hysaishi.cn

cat a.txt | grep -i error | wc -l
来源：http://kht.sjlbkw.cn

[R39] 重定向标准输出与错误
来源：http://awf.gotoacloud.top

cmd > out.log 2>&1
来源：http://lbf.yuanzhike.top

[R40] 追加写日志
来源：http://cab.ctjpmb.com

echo "log" >> out.log
来源：http://knn.chenzaomai.com

[R41] 丢弃输出
来源：http://lgd.jinqigfzy.top

cmd >/dev/null 2>&1
来源：http://aqe.jinqigufen.top

[R42] 输入重定向
来源：http://srh.snrcjt.cn

wc -l < a.txt
来源：http://jkp.uphjek.com

[R43] 按名字查找文件
来源：http://yqi.zhijiandao.cn

find . -name "*.log" -type f
来源：http://ttg.aizwys.cn

[R44] 按修改时间查找
来源：http://ood.0kj1m.cn

find . -mtime -7 -type f
来源：http://lak.xziqi.cn

[R45] 批量删除
来源：http://xli.c1oappe.top

find . -name "*.tmp" -delete
来源：http://xdf.yj20258888.top

[R46] 递归替换文件内容
来源：http://rfg.chenlongwang.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://stz.snrcjt.cn

[R47] sed 单行替换
来源：http://acs.ywan-chungtsiang.top

sed -i 's/foo/bar/g' a.txt
来源：http://qyv.zhengqikj.top

[R48] awk 取指定列
来源：http://zzn.dianchejie.cn

awk '{print $1, $3}' a.txt
来源：http://qxz.zdbjq.cn

[R49] awk 带条件
来源：http://mcx.316326.xyz

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wkp.shuidangran.top

[R50] awk 求和
来源：http://aio.tarul.cn

awk '{s += $2} END {print s}' a.txt
来源：http://yfk.fehbvm.com

[R51] 排序去重取前几
来源：http://vst.redwolf501.top

sort a.txt | uniq -c | sort -rn | head
来源：http://pap.jqgfzy.top

[R52] 统计行数
来源：http://uue.shuidangran.top

wc -l a.txt
来源：http://rvr.dianchejie.cn

[R53] 查看文件头与实时尾
来源：http://uga.fengsongda.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://oum.jiagoushi.top

[R54] 比较两个文件
来源：http://con.fktsv.cn

diff a.txt b.txt
来源：http://pyc.tarul.cn

[R55] 压缩与解压
来源：http://emu.kuanghao11.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://pwh.zhiwuduotai.top

[R56] 远程拷贝
来源：http://fcm.chenzaomai.com

scp file user@host:/path/
来源：http://amg.aibaodan.cn

[R57] 远程执行命令
来源：http://kdr.zycfv.cn

ssh user@host 'uptime'
来源：http://lkk.ctjpmb.com

[R58] 下载文件
来源：http://ser.redwolf501.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://fcc.cashguo.top

[R59] 发 POST JSON
来源：http://yhq.zhongyouzk.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://smx.shanyushiyangtech.top

[R60] 只看 HTTP 状态码
来源：http://glj.hnxiangtu.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://fdi.chenjidiqi.icu

[R61] 磁盘占用
来源：http://jyn.yuanzhike.top

df -h;  du -sh *
来源：http://zzr.ydjk.org.cn

[R62] 找最占空间的文件
来源：http://tgh.shangyingyoupin.top

du -ah . | sort -rh | head -10
来源：http://ixp.chenlongwang.top

[R63] 内存与进程
来源：http://fdc.sweek.top

free -h;  ps aux | grep nginx
来源：http://bqg.zhongyouzk.top

[R64] 结束进程
来源：http://jot.jianghu66.top

kill -9 $(pgrep -f app.py)
来源：http://knf.sxryk.cn

[R65] 查看端口占用
来源：http://nzb.cheryme.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ekr.sweek.top

[R66] 定时任务
来源：http://kvw.yangfankeji.com

crontab -e;  crontab -l
来源：http://qnk.xingfuxueyuan.xyz

[R67] 生成随机十六进制串
来源：http://hnx.hfpthk.cn

openssl rand -hex 16
来源：http://fse.yueranfly.top

[R68] 计算文件校验值
来源：http://msj.tianlin.xyz

sha256sum a.txt;  md5sum a.txt
来源：http://kxy.tarul.cn

[R69] 生成随机密码
来源：http://kwg.havefunace.top

head -c 16 /dev/urandom | base64
来源：http://ymu.ivvv.top

[R70] 时间戳与互转
来源：http://cpi.zdbjq.cn

date +%s;  date -d @1700000000
来源：http://jsv.wangshuangyany.cn

[R71] 日期格式化
来源：http://jgi.fehbvm.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://ghl.zycfv.cn

[R72] 等待端口就绪
来源：http://zll.chenzaomai.com

until nc -z localhost 3306; do sleep 1; done
来源：http://eoe.c1oappe.top

[R73] 分割大日志
来源：http://gde.shanyushiyangkeji.top

split -l 1000 big.log part_
来源：http://ueg.cdnleiting.top

[R74] 批量重命名
来源：http://itp.pengpengdd.cyou

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://gvz.shangyingyoupin.top

[R75] 导出环境变量
来源：http://fqh.zhoulong.xyz

export PATH="$HOME/bin:$PATH"
来源：http://dyh.zhijiandao.cn

[R76] 使用临时文件
来源：http://ewh.chenlongwang.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://zln.yuanzhike.top

[R77] 读取用户输入
来源：http://ukw.gotoacloud.top

read -rp "请输入: " ans
来源：http://qyg.zhiwuduotai.top

[R78] 交互式菜单
来源：http://nog.shuidangran.top

select opt in a b c; do echo "$opt"; break; done
来源：http://ntj.ywan-chungtsiang.top

[R79] 解析命令行选项
来源：http://eir.jqgfzy.top


<!-- 参考信息 -->