代发 wailian999

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://qou.tarul.cn

[Q28] 求和与平均
来源：http://atq.52xcode.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://omt.sysykeji.top

[Q29] 最大最小值
来源：http://bbl.sjlbkw.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://wqv.aibaodan.cn

[Q30] 分组统计
来源：http://guz.zdbjq.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://pje.zhoulong.xyz

[Q31] 分组后过滤
来源：http://jwl.jinqigfzy.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://egj.hysaishi.cn

[Q32] 分组拼接字符串
来源：http://nxd.yangfankeji.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://eet.guannengcc.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ule.cucudq.cn

[Q33] 多列分组
来源：http://mdc.sufxvd.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://sug.zhaomingkeji.xyz

[Q34] 每组取第一条
来源：http://gqq.sufxvd.cn

SELECT * FROM (
来源：http://iuk.ehwqpu.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ama.ydzc1.top

) t WHERE rn = 1;
来源：http://uty.cqqwz.cn

[Q35] 内连接
来源：http://cpr.jyoumei.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://yfh.hnqzz.top

[Q36] 左连接
来源：http://chg.chenlongwang.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://jgy.havefunace.top

[Q37] 右连接
来源：http://lrs.yanxiufei.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://bzp.yongpay.top

[Q38] 全外连接（PostgreSQL）
来源：http://mcl.fanxiaobao.xyz

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://eal.guowangkeji.top

[Q39] 自连接（查上下级）
来源：http://cmq.sxryk.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://lql.guowangkeji.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://xbl.zhixingplan.top

[Q40] 交叉连接（笛卡尔积）
来源：http://uap.wangdashe.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://xhi.zhaomingkeji.xyz

[Q41] 多表连接
来源：http://ewf.yueranfly.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://exg.wangshuangyany.cn

JOIN users u ON u.id = o.user_id
来源：http://viz.vqdsnc.cn

JOIN products p ON p.id = o.product_id;
来源：http://mrv.mhx1999.top

[Q42] 连接条件附加过滤
来源：http://yli.zhaomingkeji.xyz

SELECT u.name, o.amount FROM users u
来源：http://ugz.smart0.xyz

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ozl.xuetiantiany.cn

[Q43] 标量子查询
来源：http://fjr.jinyuanbaomall.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://vij.gogol.net.cn

[Q44] IN 子查询
来源：http://nmv.yj20258888.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://xnb.yj202588.top

[Q45] EXISTS 判断存在
来源：http://xib.cqqwz.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://nuq.tian-w.cn

[Q46] NOT EXISTS 判断不存在
来源：http://hox.yongpay.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vjt.zhoulong.xyz

[Q47] 与平均值比较
来源：http://ukf.sxryk.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://niw.zhongyouzk.top

[Q48] CTE 公用表表达式
来源：http://ccr.hfpthk.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://dzd.hfpthk.cn

SELECT * FROM t WHERE c > 5;
来源：http://gcm.jinqigfzy.top

[Q49] 更新单行
来源：http://vxq.gaohongyu789.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://uoz.pengpengdd.cyou

[Q50] 批量更新
来源：http://vrs.hongshengwenyu.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://qno.bjfxy.top

[Q51] 用子查询更新
来源：http://bqn.jlsjyb.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://bwm.mhx1999.top

[Q52] 删除指定行
来源：http://uli.bbcook.cn

DELETE FROM users WHERE id = 10;
来源：http://rzn.hysaishi.cn

[Q53] 按条件删除
来源：http://mvq.jinqigfzy.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://vsh.xingfuxueyuan.xyz

[Q54] 清空表
来源：http://alz.yj20258888.top

TRUNCATE TABLE logs;
来源：http://ira.vehdjk.com

[Q55] 排名（并列占位）
来源：http://mwh.zhiwuduotai.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hrm.jinghuilouyu.cn

[Q56] 密集排名（并列不占位）
来源：http://lbk.birdmap.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://fiy.vehdjk.com

[Q57] 行号
来源：http://xzh.wangshuangyany.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://dlp.shanyushiyangkeji.top

[Q58] 累计求和
来源：http://uls.gaohongyu789.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ikw.smart0.xyz

[Q59] 分组内累计
来源：http://qog.cashguo.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wjc.hfpthk.cn

[Q60] 取上一行 / 下一行
来源：http://yxp.bbcook.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://zni.sweek.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mhz.0kj1m.cn

[Q61] 移动平均
来源：http://ron.jinqigfzy.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://fnu.xuetiantiany.cn

[Q62] 分组占比
来源：http://jwk.shanyushiyangtech.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://qjj.ywan-chungtsiang.top

[Q63] 开启事务
来源：http://mtt.xuanzx.com

START TRANSACTION;                -- 或 BEGIN
来源：http://yah.fanxiaobao.xyz

[Q64] 提交事务
来源：http://fwd.yangfankeji.com

COMMIT;
来源：http://guo.svipenyu.cn

[Q65] 回滚事务
来源：http://ymn.jyoumei.cn

ROLLBACK;
来源：http://tqp.cdnleiting.top

[Q66] 行锁查询
来源：http://edc.wangdashe.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://fog.yvedp.cn

[Q67] 设置隔离级别
来源：http://pxv.sysykeji.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ncz.wangdashe.top

[Q68] 保存点
来源：http://srl.guannengcc.top

SAVEPOINT sp1;
来源：http://ssv.redwolf501.top

ROLLBACK TO sp1;
来源：http://jvs.havefunace.top

[Q69] 查看执行计划
来源：http://qzf.hesvh.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://tiv.fengsongda.top

[Q70] 更新统计信息
来源：http://kka.yongpay.top

ANALYZE TABLE users;
来源：http://eyd.hongshengwenyu.top

[Q71] 查看建表语句
来源：http://sev.ctjpmb.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://zcm.mhx1999.top

[Q72] 查看索引
来源：http://yqu.tarul.cn

SHOW INDEX FROM users;
来源：http://elk.zycfv.cn

[Q73] 查看表状态
来源：http://lgn.feifeiyinyue.top

SHOW TABLE STATUS LIKE 'users';
来源：http://rso.yuanzhike.top

[Q74] 强制使用索引
来源：http://fho.tianlin.xyz

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blr.hcnkem.com

[Q75] 日期格式化
来源：http://rxg.9152youxi.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://pcr.ywan-chungtsiang.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://veb.quarkkingdee.top

[Q76] 按天统计
来源：http://oxw.zdbjq.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://bpv.feifeiyinyue.top

[Q77] 时间加减
来源：http://iel.yanxiufei.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hpk.sxryk.cn

[Q78] 当前时间
来源：http://poi.xinyue.icu

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://plx.dianchejie.cn

[Q79] 字符串拼接
来源：http://fwk.jyoumei.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://lhz.zhaomingkeji.xyz

[Q80] 字符串截取
来源：http://cqg.sxryk.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://dub.xuanzx.com

[Q81] 字符串替换
来源：http://oqu.aibaodan.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://pdv.cashguo.top

[Q82] 字符长度与字节长度
来源：http://zwg.quarkkingdee.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ooj.jlsjyb.cn

[Q83] 大小写转换
来源：http://awl.pycfn.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://gxa.yj20258.top

[Q84] 去除首尾空格
来源：http://tdd.yj20258.top

SELECT TRIM(name) FROM users;
来源：http://fpz.pycfn.com

[Q85] 数值取整
来源：http://rfm.yvedp.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://bnr.jlsjyb.cn

[Q86] 读取 JSON 字段
来源：http://hyg.sysykeji.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://eeo.zhengqikj.top

[Q87] JSON 字段做条件
来源：http://mat.hnxiangtu.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://doq.hfpthk.cn

[Q88] 行转列（条件聚合）
来源：http://zhl.jlsjyb.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://cjd.aizwys.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://jvd.yonumen.top

[Q89] 判断表是否存在
来源：http://juv.redwolf501.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mhz.cqqwz.cn

[Q90] 生成序号列
来源：http://oit.shanyushiyangkeji.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://tuu.mhx1999.top

================================================================================
来源：http://ldx.fengsongda.top

R. Bash 专题
来源：http://tku.hesvh.cn

================================================================================
来源：http://ecg.sxryk.cn

[R01] shebang 与严格模式
来源：http://liy.shanyushiyangtech.top

#!/usr/bin/env bash
来源：http://hce.nwbrower.top

set -euo pipefail
来源：http://suf.shanyushiyangkeji.top

[R02] 变量赋值与使用
来源：http://wfu.guowangkeji.top

name="Tom"; echo "$name"
来源：http://ooc.jinqigfzy.top

[R03] 只读变量
来源：http://psr.hnxiangtu.top

readonly PI=3.14
来源：http://jxg.snrcjt.cn

[R04] 位置参数
来源：http://xnu.sweek.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://gcr.ehwqpu.com

[R05] 参数默认值
来源：http://kdl.zhijiandao.cn

name="${1:-default}"
来源：http://gso.quarkkingdee.top

[R06] 判断命令是否存在
来源：http://mrz.zycfv.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ibk.cqqwz.cn

[R07] if 判断文件
来源：http://nmv.aibaodan.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mef.zhengqikj.top

[R08] 数值比较
来源：http://are.gaohongyu789.top

if (( a > b )); then echo "a 更大"; fi
来源：http://pas.gaohongyu789.top

[R09] 字符串比较
来源：http://ezo.cdnleiting.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://jvv.havefunace.top

[R10] 正则匹配
来源：http://xvc.52xcode.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://xgx.zhaomingkeji.xyz

[R11] case 多分支
来源：http://izh.zhongyouzk.top

case "$1" in
来源：http://fxr.hfpthk.cn

start) echo "启动" ;;
来源：http://jow.xinyue.icu

stop)  echo "停止" ;;
来源：http://avq.uphjek.com

*)     echo "未知命令" ;;
来源：http://ulw.wangshuangyany.cn

esac
来源：http://ivd.sweek.top

[R12] for 遍历文件
来源：http://rdh.chenzaomai.com

for f in *.txt; do echo "$f"; done
来源：http://ell.chenlongwang.top

[R13] for 计数循环
来源：http://gwj.snrcjt.cn

for i in {1..10}; do echo "$i"; done
来源：http://hfu.xuanzx.com

[R14] C 风格 for
来源：http://vgy.daxiang520.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://xjz.hysaishi.cn

[R15] while 逐行读文件
来源：http://gge.cucudq.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://cge.fktsv.cn

[R16] until 等待条件
来源：http://zlp.yanxiufei.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://jdo.zhixingplan.top

[R17] 数组定义与取值
来源：http://mwh.yj20258888.top

arr=(a b c); echo "${arr[0]}"
来源：http://aou.dianchejie.cn

[R18] 遍历数组
来源：http://ysy.ivvv.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wgd.redwolf501.top

[R19] 数组长度
来源：http://kbx.zhengqikj.top

echo "${#arr[@]}"
来源：http://ukz.xuetiantiany.cn

[R20] 关联数组（字典）
来源：http://tnc.yuxming.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ujw.cqqwz.cn

[R21] 字符串长度
来源：http://cyr.andypj.xyz

echo "${#s}"
来源：http://pat.9152youxi.cn

[R22] 截取子串
来源：http://tjr.gotoacloud.top

echo "${s:0:5}"
来源：http://gkr.sysykeji.top

[R23] 字符串替换
来源：http://tmm.ctjpmb.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://eil.vqdsnc.cn

[R24] 大小写转换
来源：http://xfe.bbcook.cn

echo "${s^^}"; echo "${s,,}"
来源：http://jwj.tian-w.cn

[R25] 去后缀 / 去前缀
来源：http://tsd.cdnleiting.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://tdr.iojbl.cn

[R26] 命令替换
来源：http://jva.jinghuilouyu.cn

now=$(date +%F); echo "$now"
来源：http://nbd.hongshengwenyu.top

[R27] 算术展开
来源：http://iws.fanxiaobao.xyz

echo $((1 + 2 * 3))
来源：http://umz.bjfxy.top

[R28] 浮点运算
来源：http://mme.yvedp.cn

echo "scale=2; 10/3" | bc
来源：http://fsl.havefunace.top

[R29] 定义函数
来源：http://vwc.hywenlv.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://inj.snrcjt.cn

[R30] 函数返回状态码
来源：http://vhj.hcnkem.com

f() { return 0; }; f || echo "失败了"
来源：http://irq.ywan-chungtsiang.top

[R31] 局部变量
来源：http://pqt.ydzc1.top

f() { local x=1; echo "$x"; }
来源：http://dzv.chenjidiqi.icu

[R32] 参数个数校验
来源：http://uoc.hnqzz.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mko.xylfe.cn

[R33] 捕获错误并提示行号
来源：http://vad.fehbvm.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://xre.zhongyouzk.top

[R34] 退出时清理
来源：http://ffi.xingfuxueyuan.xyz

trap 'rm -f "$tmp"' EXIT
来源：http://rjy.tianlin.xyz

[R35] 后台执行并等待
来源：http://wcj.gogol.net.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://clw.hywenlv.cn

[R36] 并发执行多个任务
来源：http://oqr.52xcode.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://pkr.jinyuanbaomall.cn

[R37] 把输出赋给变量
来源：http://vgv.zhijiandao.cn

files=$(ls -1)
来源：http://cjk.yfazqb.com

[R38] 管道串联
来源：http://yts.yj20258888.top

cat a.txt | grep -i error | wc -l
来源：http://amr.yfazqb.com

[R39] 重定向标准输出与错误
来源：http://rdp.hywenlv.cn

cmd > out.log 2>&1
来源：http://uuy.jqgufenzy.top

[R40] 追加写日志
来源：http://mld.redwolf501.top

echo "log" >> out.log
来源：http://aju.andypj.xyz

[R41] 丢弃输出
来源：http://pkv.zhiwuduotai.top

cmd >/dev/null 2>&1
来源：http://yzo.yangfankeji.com

[R42] 输入重定向
来源：http://noq.uphjek.com

wc -l < a.txt
来源：http://fnw.shanyushiyangtech.top

[R43] 按名字查找文件
来源：http://anq.jiagoushi.top

find . -name "*.log" -type f
来源：http://fom.c1oappe.top

[R44] 按修改时间查找
来源：http://chg.birdmap.top

find . -mtime -7 -type f
来源：http://pam.hammf.cn

[R45] 批量删除
来源：http://tua.sxryk.cn

find . -name "*.tmp" -delete
来源：http://rwx.pengpengdd.cyou

[R46] 递归替换文件内容
来源：http://bpv.dianchejie.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://zsr.uphjek.com

[R47] sed 单行替换
来源：http://xzk.sweek.top

sed -i 's/foo/bar/g' a.txt
来源：http://boz.zhoulong.xyz

[R48] awk 取指定列
来源：http://ozh.jinyuanbaomall.cn

awk '{print $1, $3}' a.txt
来源：http://xln.xingfuxueyuan.xyz

[R49] awk 带条件
来源：http://krv.jinqigfzy.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://fqp.hcnkem.com

[R50] awk 求和
来源：http://bpb.daxiang520.top

awk '{s += $2} END {print s}' a.txt
来源：http://ogu.jinghuilouyu.cn

[R51] 排序去重取前几
来源：http://wrw.daxiang520.top

sort a.txt | uniq -c | sort -rn | head
来源：http://vzr.aizwys.cn

[R52] 统计行数
来源：http://nmm.xinyue.icu

wc -l a.txt
来源：http://ukk.ydzc1.top

[R53] 查看文件头与实时尾
来源：http://xul.shanyushiyangtech.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://qyh.cdnleiting.top

[R54] 比较两个文件
来源：http://haf.vehdjk.com

diff a.txt b.txt
来源：http://lmy.hesvh.cn

[R55] 压缩与解压
来源：http://ljr.ctjpmb.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://iqx.vehdjk.com

[R56] 远程拷贝
来源：http://izb.sxryk.cn

scp file user@host:/path/
来源：http://fxx.yongpay.top

[R57] 远程执行命令
来源：http://ura.shzxlz.cn

ssh user@host 'uptime'
来源：http://wyo.yongpay.top

[R58] 下载文件
来源：http://vpy.xziqi.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://nkr.jinqigufen.top

[R59] 发 POST JSON
来源：http://dkf.chenlongwang.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://crn.andypj.xyz

[R60] 只看 HTTP 状态码
来源：http://xab.9152youxi.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://yps.jinyuanbaomall.cn

[R61] 磁盘占用
来源：http://vnt.feifeiyinyue.top

df -h;  du -sh *
来源：http://orv.ivvv.top

[R62] 找最占空间的文件
来源：http://aop.dianchejie.cn

du -ah . | sort -rh | head -10
来源：http://oyu.ppjwa.cn

[R63] 内存与进程
来源：http://jws.hnxiangtu.top

free -h;  ps aux | grep nginx
来源：http://rkn.yonumen.top

[R64] 结束进程
来源：http://hgb.jinqigfzy.top

kill -9 $(pgrep -f app.py)
来源：http://xlt.shuidangran.top

[R65] 查看端口占用
来源：http://leb.sjlbkw.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://qqr.yonumen.top

[R66] 定时任务
来源：http://rch.haohaochexian.top

crontab -e;  crontab -l
来源：http://auq.yanxiufei.cn

[R67] 生成随机十六进制串
来源：http://lhr.cqqwz.cn

openssl rand -hex 16
来源：http://moz.wangdashe.top

[R68] 计算文件校验值
来源：http://foq.yj202588.top

sha256sum a.txt;  md5sum a.txt
来源：http://och.hnxiangtu.top

[R69] 生成随机密码
来源：http://hsv.yanxiufei.cn

head -c 16 /dev/urandom | base64
来源：http://jtq.hywenlv.cn

[R70] 时间戳与互转
来源：http://fnp.shanyushiyangtech.top

date +%s;  date -d @1700000000
来源：http://hel.yfazqb.com

[R71] 日期格式化
来源：http://wie.yongpay.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://iee.pycfn.com

[R72] 等待端口就绪
来源：http://bmj.fehbvm.com

until nc -z localhost 3306; do sleep 1; done
来源：http://qgf.chenjidiqi.icu

[R73] 分割大日志
来源：http://xar.svipenyu.cn

split -l 1000 big.log part_
来源：http://nzg.shuidangran.top

[R74] 批量重命名
来源：http://mrf.cucudq.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://guz.yj20258888.top

[R75] 导出环境变量
来源：http://dwq.tian-w.cn

export PATH="$HOME/bin:$PATH"
来源：http://plt.yj20258.top

[R76] 使用临时文件
来源：http://xef.jlsjyb.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mre.yuxming.cn

[R77] 读取用户输入
来源：http://orw.zhongyouzk.top


<!-- 参考信息 -->