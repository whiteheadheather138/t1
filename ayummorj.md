代发 wailian999

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://poi.sjlbkw.cn

[Q28] 求和与平均
来源：http://utx.ivvv.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://kie.hcnkem.com

[Q29] 最大最小值
来源：http://yzh.hongshengwenyu.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://fui.fengsongda.top

[Q30] 分组统计
来源：http://ixk.jinghuilouyu.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://zsr.cashguo.top

[Q31] 分组后过滤
来源：http://msg.tarul.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hnh.yj20258888.top

[Q32] 分组拼接字符串
来源：http://lnd.zhongyouzk.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://amu.jinqigufen.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://euo.chenlongwang.top

[Q33] 多列分组
来源：http://ggh.zhijiandao.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://okh.guannengcc.top

[Q34] 每组取第一条
来源：http://aky.chenlongwang.top

SELECT * FROM (
来源：http://idt.xinyue.icu

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://syw.316326.xyz

) t WHERE rn = 1;
来源：http://ant.fanxiaobao.xyz

[Q35] 内连接
来源：http://bwo.birdmap.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ari.yuanzhike.top

[Q36] 左连接
来源：http://yfh.yongpay.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://lnr.zhongyouzk.top

[Q37] 右连接
来源：http://zfk.hywenlv.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://lib.shzxlz.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ifk.cucudq.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://pgt.hesvh.cn

[Q39] 自连接（查上下级）
来源：http://awf.hammf.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ffi.sjlbkw.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://xwu.wangdashe.top

[Q40] 交叉连接（笛卡尔积）
来源：http://voo.zhoulong.xyz

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ehd.zycfv.cn

[Q41] 多表连接
来源：http://wgt.zhixingplan.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://vya.wangshuangyany.cn

JOIN users u ON u.id = o.user_id
来源：http://ywb.zhijiandao.cn

JOIN products p ON p.id = o.product_id;
来源：http://hdc.yj202588.top

[Q42] 连接条件附加过滤
来源：http://jft.jinqigufen.top

SELECT u.name, o.amount FROM users u
来源：http://ygl.ydzc1.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://lpy.guannengcc.top

[Q43] 标量子查询
来源：http://lif.bbcook.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hah.hysaishi.cn

[Q44] IN 子查询
来源：http://pnh.c1oappe.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://glh.9152youxi.cn

[Q45] EXISTS 判断存在
来源：http://vcu.sufxvd.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://nsi.pycfn.com

[Q46] NOT EXISTS 判断不存在
来源：http://ttl.sufxvd.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://put.zhengqikj.top

[Q47] 与平均值比较
来源：http://bpz.aibaodan.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://iql.fzhhl.top

[Q48] CTE 公用表表达式
来源：http://asv.yonumen.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://pwk.xylfe.cn

SELECT * FROM t WHERE c > 5;
来源：http://ald.bbcook.cn

[Q49] 更新单行
来源：http://zta.316326.xyz

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ndt.jyoumei.cn

[Q50] 批量更新
来源：http://xph.sjlbkw.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://jqz.hywenlv.cn

[Q51] 用子查询更新
来源：http://xqm.yueranfly.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://zcz.quarkkingdee.top

[Q52] 删除指定行
来源：http://nwz.mhx1999.top

DELETE FROM users WHERE id = 10;
来源：http://hqd.nwbrower.top

[Q53] 按条件删除
来源：http://jot.hywenlv.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://xbt.svipenyu.cn

[Q54] 清空表
来源：http://bre.xylfe.cn

TRUNCATE TABLE logs;
来源：http://rrd.kuanghao11.cn

[Q55] 排名（并列占位）
来源：http://tff.jinghuilouyu.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mwf.aizwys.cn

[Q56] 密集排名（并列不占位）
来源：http://jcd.gaohongyu789.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://bbf.ctjpmb.com

[Q57] 行号
来源：http://hgg.zhengqikj.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://nud.xingfuxueyuan.xyz

[Q58] 累计求和
来源：http://wau.zycfv.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://nej.kuanghao11.cn

[Q59] 分组内累计
来源：http://ygd.ybcxt.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://xod.vehdjk.com

[Q60] 取上一行 / 下一行
来源：http://nru.hnxiangtu.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://jam.yongpay.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://jki.dianchejie.cn

[Q61] 移动平均
来源：http://ubu.fehbvm.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://uyj.fehbvm.com

[Q62] 分组占比
来源：http://pci.quarkkingdee.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://vmy.gogol.net.cn

[Q63] 开启事务
来源：http://umy.jinyuanbaomall.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://kjy.gogol.net.cn

[Q64] 提交事务
来源：http://rrc.xuetiantiany.cn

COMMIT;
来源：http://dig.yj20258888.top

[Q65] 回滚事务
来源：http://vhv.ivvv.top

ROLLBACK;
来源：http://tej.hysaishi.cn

[Q66] 行锁查询
来源：http://rnd.tian-w.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://uxx.gotoacloud.top

[Q67] 设置隔离级别
来源：http://oob.uphjek.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://qcm.yongpay.top

[Q68] 保存点
来源：http://zgr.sxryk.cn

SAVEPOINT sp1;
来源：http://bii.ivvv.top

ROLLBACK TO sp1;
来源：http://acd.jinyuanbaomall.cn

[Q69] 查看执行计划
来源：http://qog.zhixingplan.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://vtv.meibo888.top

[Q70] 更新统计信息
来源：http://apv.cqqwz.cn

ANALYZE TABLE users;
来源：http://sqp.yongpay.top

[Q71] 查看建表语句
来源：http://sfx.guowangkeji.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://kju.svipenyu.cn

[Q72] 查看索引
来源：http://xek.andypj.xyz

SHOW INDEX FROM users;
来源：http://nqw.shangyingyoupin.top

[Q73] 查看表状态
来源：http://sgv.dashuyun.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://fqk.cucudq.cn

[Q74] 强制使用索引
来源：http://ili.xuanzx.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://got.chenlongwang.top

[Q75] 日期格式化
来源：http://hga.0kj1m.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ydx.nanxinkj.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://cwu.tanke756.top

[Q76] 按天统计
来源：http://fes.xingfuxueyuan.xyz

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://sfd.fktsv.cn

[Q77] 时间加减
来源：http://lgu.vqdsnc.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://soj.feifeiyinyue.top

[Q78] 当前时间
来源：http://rcn.hywenlv.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://iqa.52xcode.cn

[Q79] 字符串拼接
来源：http://rft.gaohongyu789.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://gwx.daxiang520.top

[Q80] 字符串截取
来源：http://glu.sxryk.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wln.snrcjt.cn

[Q81] 字符串替换
来源：http://gyi.9152youxi.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mdo.9152youxi.cn

[Q82] 字符长度与字节长度
来源：http://bxr.xingfuxueyuan.xyz

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ioo.xingfuxueyuan.xyz

[Q83] 大小写转换
来源：http://dgj.zhaomingkeji.xyz

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://rha.hysaishi.cn

[Q84] 去除首尾空格
来源：http://xlw.hcnkem.com

SELECT TRIM(name) FROM users;
来源：http://cth.iojbl.cn

[Q85] 数值取整
来源：http://rxz.jinghuilouyu.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://pia.0kj1m.cn

[Q86] 读取 JSON 字段
来源：http://gvs.chenjidiqi.icu

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://bst.xingfuxueyuan.xyz

[Q87] JSON 字段做条件
来源：http://ofg.zhengqikj.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://dcq.chenzaomai.com

[Q88] 行转列（条件聚合）
来源：http://ics.pengpengdd.cyou

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://aec.guannengcc.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://fdu.nanxuanxn.top

[Q89] 判断表是否存在
来源：http://sow.meibo888.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ifp.hnqzz.top

[Q90] 生成序号列
来源：http://xrb.guowangkeji.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://cfb.ywan-chungtsiang.top

================================================================================
来源：http://aqi.tarul.cn

R. Bash 专题
来源：http://cvn.daxiang520.top

================================================================================
来源：http://eqt.yongpay.top

[R01] shebang 与严格模式
来源：http://ypt.zhongyouzk.top

#!/usr/bin/env bash
来源：http://gbh.jqgfzy.top

set -euo pipefail
来源：http://sri.fanxiaobao.xyz

[R02] 变量赋值与使用
来源：http://urg.guowangkeji.top

name="Tom"; echo "$name"
来源：http://jdl.wangshuangyany.cn

[R03] 只读变量
来源：http://uex.yj202588.top

readonly PI=3.14
来源：http://mjm.yangfankeji.com

[R04] 位置参数
来源：http://hzl.vehdjk.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://isv.jianghu66.top

[R05] 参数默认值
来源：http://uck.zhixingplan.top

name="${1:-default}"
来源：http://rbt.ywan-chungtsiang.top

[R06] 判断命令是否存在
来源：http://tyh.xuetiantiany.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wbn.fzhhl.top

[R07] if 判断文件
来源：http://rhw.vehdjk.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://rxi.yvedp.cn

[R08] 数值比较
来源：http://dmv.yuanzhike.top

if (( a > b )); then echo "a 更大"; fi
来源：http://utp.guowangkeji.top

[R09] 字符串比较
来源：http://jkw.cashguo.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://oks.yonumen.top

[R10] 正则匹配
来源：http://yah.gaohongyu789.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://tye.shanyushiyangtech.top

[R11] case 多分支
来源：http://agu.yj20258888.top

case "$1" in
来源：http://ohx.kuanghao11.cn

start) echo "启动" ;;
来源：http://zun.zdbjq.cn

stop)  echo "停止" ;;
来源：http://hpw.smart0.xyz

*)     echo "未知命令" ;;
来源：http://fil.gotoacloud.top

esac
来源：http://ivw.yueranfly.top

[R12] for 遍历文件
来源：http://mut.shanyushiyangtech.top

for f in *.txt; do echo "$f"; done
来源：http://khv.yueranfly.top

[R13] for 计数循环
来源：http://asi.jyoumei.cn

for i in {1..10}; do echo "$i"; done
来源：http://ddc.fzhhl.top

[R14] C 风格 for
来源：http://axh.epnwcf.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://xaa.chenzaomai.com

[R15] while 逐行读文件
来源：http://nqk.fktsv.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ewa.tarul.cn

[R16] until 等待条件
来源：http://nzv.yongpay.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://lvb.ctjpmb.com

[R17] 数组定义与取值
来源：http://eds.tian-w.cn

arr=(a b c); echo "${arr[0]}"
来源：http://bif.xingfuxueyuan.xyz

[R18] 遍历数组
来源：http://chx.svipenyu.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://dzj.cqqwz.cn

[R19] 数组长度
来源：http://wmo.yj20258888.top

echo "${#arr[@]}"
来源：http://zwg.hfpthk.cn

[R20] 关联数组（字典）
来源：http://nct.cheryme.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://aoa.yueranfly.top

[R21] 字符串长度
来源：http://gal.dianchejie.cn

echo "${#s}"
来源：http://rdx.svipenyu.cn

[R22] 截取子串
来源：http://dij.tianlin.xyz

echo "${s:0:5}"
来源：http://aqv.ydjk.org.cn

[R23] 字符串替换
来源：http://dma.nwbrower.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://pgl.tianlin.xyz

[R24] 大小写转换
来源：http://tel.cqqwz.cn

echo "${s^^}"; echo "${s,,}"
来源：http://pkz.zdqjudy.top

[R25] 去后缀 / 去前缀
来源：http://yfy.xziqi.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://stk.hnqzz.top

[R26] 命令替换
来源：http://tqf.zdbjq.cn

now=$(date +%F); echo "$now"
来源：http://scw.zhaomingkeji.xyz

[R27] 算术展开
来源：http://zun.mhx1999.top

echo $((1 + 2 * 3))
来源：http://xhc.havefunace.top

[R28] 浮点运算
来源：http://dvl.chenzaomai.com

echo "scale=2; 10/3" | bc
来源：http://ryr.meibo888.top

[R29] 定义函数
来源：http://bpu.jqgfzy.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://zix.aibaodan.cn

[R30] 函数返回状态码
来源：http://hiq.nanxuanxn.top

f() { return 0; }; f || echo "失败了"
来源：http://htl.hnxiangtu.top

[R31] 局部变量
来源：http://wca.zhiwuduotai.top

f() { local x=1; echo "$x"; }
来源：http://wgt.zhengqikj.top

[R32] 参数个数校验
来源：http://sin.fanxiaobao.xyz

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ojm.zhongyouzk.top

[R33] 捕获错误并提示行号
来源：http://txm.gaohongyu789.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://fjj.fktsv.cn

[R34] 退出时清理
来源：http://voi.jqgfzy.top

trap 'rm -f "$tmp"' EXIT
来源：http://sjs.pycfn.com

[R35] 后台执行并等待
来源：http://nfp.yj20258888.top

sleep 5 & pid=$!; wait "$pid"
来源：http://dbb.svipenyu.cn

[R36] 并发执行多个任务
来源：http://jol.hnqzz.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ncs.nanxinkj.top

[R37] 把输出赋给变量
来源：http://okn.yuxming.cn

files=$(ls -1)
来源：http://yca.tarul.cn

[R38] 管道串联
来源：http://kdz.gaohongyu789.top

cat a.txt | grep -i error | wc -l
来源：http://lfz.yongpay.top

[R39] 重定向标准输出与错误
来源：http://zzz.zhiwuduotai.top

cmd > out.log 2>&1
来源：http://awd.shanyushiyangtech.top

[R40] 追加写日志
来源：http://aoj.gogol.net.cn

echo "log" >> out.log
来源：http://vdy.jlsjyb.cn

[R41] 丢弃输出
来源：http://cyp.xingfuxueyuan.xyz

cmd >/dev/null 2>&1
来源：http://pdf.jinghuilouyu.cn

[R42] 输入重定向
来源：http://apl.jinqigfzy.top

wc -l < a.txt
来源：http://pkp.sysykeji.top

[R43] 按名字查找文件
来源：http://dln.0kj1m.cn

find . -name "*.log" -type f
来源：http://xpa.jqgufenzy.top

[R44] 按修改时间查找
来源：http://vpj.jqgfzy.top

find . -mtime -7 -type f
来源：http://pfo.jiagoushi.top

[R45] 批量删除
来源：http://vyd.nwbrower.top

find . -name "*.tmp" -delete
来源：http://qpi.jqgfzy.top

[R46] 递归替换文件内容
来源：http://amz.gaohongyu789.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ojf.quarkkingdee.top

[R47] sed 单行替换
来源：http://elh.xuanzx.com

sed -i 's/foo/bar/g' a.txt
来源：http://ukf.hysaishi.cn

[R48] awk 取指定列
来源：http://vqg.sjlbkw.cn

awk '{print $1, $3}' a.txt
来源：http://bsb.hysaishi.cn

[R49] awk 带条件
来源：http://tfv.ehwqpu.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://uzb.hnxiangtu.top

[R50] awk 求和
来源：http://aqe.hysaishi.cn

awk '{s += $2} END {print s}' a.txt
来源：http://iot.nwbrower.top

[R51] 排序去重取前几
来源：http://wjh.ybcxt.top

sort a.txt | uniq -c | sort -rn | head
来源：http://ryg.sufxvd.cn

[R52] 统计行数
来源：http://wsg.ppjwa.cn

wc -l a.txt
来源：http://sjs.hcnkem.com

[R53] 查看文件头与实时尾
来源：http://mii.hongshengwenyu.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://njw.sjlbkw.cn

[R54] 比较两个文件
来源：http://htk.yfazqb.com

diff a.txt b.txt
来源：http://bhv.uphjek.com

[R55] 压缩与解压
来源：http://adj.jinqigfzy.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mai.yuxming.cn

[R56] 远程拷贝
来源：http://yon.xuetiantiany.cn

scp file user@host:/path/
来源：http://hgq.yj202588.top

[R57] 远程执行命令
来源：http://foa.hysaishi.cn

ssh user@host 'uptime'
来源：http://vqk.chenlongwang.top

[R58] 下载文件
来源：http://anv.sysykeji.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mxy.birdmap.top

[R59] 发 POST JSON
来源：http://gtr.gogol.net.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://rbc.svipenyu.cn

[R60] 只看 HTTP 状态码
来源：http://ymi.feifeiyinyue.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://adz.mhx1999.top

[R61] 磁盘占用
来源：http://ysh.yj20258.top

df -h;  du -sh *
来源：http://lsd.cdnleiting.top

[R62] 找最占空间的文件
来源：http://rpt.jinyuanbaomall.cn

du -ah . | sort -rh | head -10
来源：http://rhx.jinghuilouyu.cn

[R63] 内存与进程
来源：http://dka.9152youxi.cn

free -h;  ps aux | grep nginx
来源：http://mqn.ydzc1.top

[R64] 结束进程
来源：http://igy.yangfankeji.com

kill -9 $(pgrep -f app.py)
来源：http://fmm.vqdsnc.cn

[R65] 查看端口占用
来源：http://fmk.yongpay.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://oha.ybcxt.top

[R66] 定时任务
来源：http://oxb.gaohongyu789.top

crontab -e;  crontab -l
来源：http://jfj.jinqigufen.top

[R67] 生成随机十六进制串
来源：http://avx.yfazqb.com

openssl rand -hex 16
来源：http://fzt.dashuyun.cn

[R68] 计算文件校验值
来源：http://dxp.ydjk.org.cn

sha256sum a.txt;  md5sum a.txt
来源：http://xcg.meibo888.top

[R69] 生成随机密码
来源：http://plk.xziqi.cn

head -c 16 /dev/urandom | base64
来源：http://ddv.0kj1m.cn

[R70] 时间戳与互转
来源：http://veu.vehdjk.com

date +%s;  date -d @1700000000
来源：http://ggi.redwolf501.top

[R71] 日期格式化
来源：http://zxq.tanke756.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://gpg.zhoulong.xyz

[R72] 等待端口就绪
来源：http://nbw.316326.xyz

until nc -z localhost 3306; do sleep 1; done
来源：http://tlk.ydzc1.top

[R73] 分割大日志
来源：http://hpa.snrcjt.cn

split -l 1000 big.log part_
来源：http://atb.ywan-chungtsiang.top

[R74] 批量重命名
来源：http://wum.jlsjyb.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wzx.bbcook.cn

[R75] 导出环境变量
来源：http://iwq.sweek.top

export PATH="$HOME/bin:$PATH"
来源：http://qzm.xingfuxueyuan.xyz

[R76] 使用临时文件
来源：http://qds.9152youxi.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://auq.nanxinkj.top

[R77] 读取用户输入
来源：http://zah.jinqigfzy.top


<!-- 参考信息 -->