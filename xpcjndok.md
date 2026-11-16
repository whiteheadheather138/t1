代发 wailian999

SELECT * FROM users WHERE email IS NULL;
来源：http://kkm.ppjwa.cn

[Q22] 排序
来源：http://mao.jyoumei.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://qal.vqdsnc.cn

[Q23] 分页
来源：http://bek.daria6918.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://omg.chenlongwang.top

[Q24] 去重
来源：http://ivl.bjfxy.top

SELECT DISTINCT city FROM users;
来源：http://yre.xingfuxueyuan.xyz

[Q25] 只取前 N 条
来源：http://vpv.sysykeji.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://qms.hesvh.cn

[Q26] 计数
来源：http://fcn.tanke756.top

SELECT COUNT(*) FROM users;
来源：http://ggh.ppjwa.cn

[Q27] 条件计数
来源：http://pab.xingfuxueyuan.xyz

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://vsy.mhx1999.top

[Q28] 求和与平均
来源：http://dpx.zdbjq.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wpn.jinqigufen.top

[Q29] 最大最小值
来源：http://ozl.hysaishi.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://hxo.snrcjt.cn

[Q30] 分组统计
来源：http://ojc.jqgfzy.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://exh.zhiwuduotai.top

[Q31] 分组后过滤
来源：http://jvv.hongshengwenyu.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ofp.ehwqpu.com

[Q32] 分组拼接字符串
来源：http://gnd.chenzaomai.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://gqy.kuanghao11.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://slz.yuanzhike.top

[Q33] 多列分组
来源：http://wxv.gaohongyu789.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://cds.gaohongyu789.top

[Q34] 每组取第一条
来源：http://iyj.gzhubu.top

SELECT * FROM (
来源：http://ukx.xziqi.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://cso.xziqi.cn

) t WHERE rn = 1;
来源：http://wig.daria6918.cn

[Q35] 内连接
来源：http://mny.aizwys.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wvj.birdmap.top

[Q36] 左连接
来源：http://psc.jinqigfzy.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://qel.yuanzhike.top

[Q37] 右连接
来源：http://dyf.yuanzhike.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hsl.zdbjq.cn

[Q38] 全外连接（PostgreSQL）
来源：http://bqm.cqqwz.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://upq.wangdashe.top

[Q39] 自连接（查上下级）
来源：http://fmt.c1oappe.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://yaj.hammf.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://env.daxiang520.top

[Q40] 交叉连接（笛卡尔积）
来源：http://npj.jinyuanbaomall.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wki.cashguo.top

[Q41] 多表连接
来源：http://nvh.yuxming.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://bar.jyoumei.cn

JOIN users u ON u.id = o.user_id
来源：http://kdu.feifeiyinyue.top

JOIN products p ON p.id = o.product_id;
来源：http://blu.zhengqikj.top

[Q42] 连接条件附加过滤
来源：http://uch.hongshengwenyu.top

SELECT u.name, o.amount FROM users u
来源：http://dsb.hfpthk.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://eto.zhixingplan.top

[Q43] 标量子查询
来源：http://hzu.chenlongwang.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://fsd.sweek.top

[Q44] IN 子查询
来源：http://zqp.jianghu66.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://lke.ctjpmb.com

[Q45] EXISTS 判断存在
来源：http://jeq.ivvv.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ufm.hywenlv.cn

[Q46] NOT EXISTS 判断不存在
来源：http://hgx.tianlin.xyz

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://odo.chenzaomai.com

[Q47] 与平均值比较
来源：http://dwn.bjfxy.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://evo.jqgufenzy.top

[Q48] CTE 公用表表达式
来源：http://bhr.andypj.xyz

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://iny.gogol.net.cn

SELECT * FROM t WHERE c > 5;
来源：http://zex.wangshuangyany.cn

[Q49] 更新单行
来源：http://stw.smart0.xyz

UPDATE users SET status = 1 WHERE id = 10;
来源：http://fwh.shanyushiyangtech.top

[Q50] 批量更新
来源：http://pap.hfpthk.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://bjn.hywenlv.cn

[Q51] 用子查询更新
来源：http://ywa.yongpay.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wur.yj20258.top

[Q52] 删除指定行
来源：http://unv.chenjidiqi.icu

DELETE FROM users WHERE id = 10;
来源：http://dbl.haohaochexian.top

[Q53] 按条件删除
来源：http://cmk.daxiang520.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://tge.kuanghao11.cn

[Q54] 清空表
来源：http://btz.gzhubu.top

TRUNCATE TABLE logs;
来源：http://bbm.xylfe.cn

[Q55] 排名（并列占位）
来源：http://jvk.redwolf501.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hqj.bjfxy.top

[Q56] 密集排名（并列不占位）
来源：http://umn.zhiwuduotai.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ijr.aibaodan.cn

[Q57] 行号
来源：http://rad.pengpengdd.cyou

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://knn.dashuyun.cn

[Q58] 累计求和
来源：http://nsf.yj20258888.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ysx.ehwqpu.com

[Q59] 分组内累计
来源：http://qdg.ydjk.org.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://uae.yuxming.cn

[Q60] 取上一行 / 下一行
来源：http://ozm.cdnleiting.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://uxy.sweek.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mci.jiagoushi.top

[Q61] 移动平均
来源：http://cub.hywenlv.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ktm.sjlbkw.cn

[Q62] 分组占比
来源：http://xdw.ydzc1.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wrh.xingfuxueyuan.xyz

[Q63] 开启事务
来源：http://gio.ybcxt.top

START TRANSACTION;                -- 或 BEGIN
来源：http://wrl.yj20258.top

[Q64] 提交事务
来源：http://dsg.cqqwz.cn

COMMIT;
来源：http://lgx.cdnleiting.top

[Q65] 回滚事务
来源：http://tre.shuidangran.top

ROLLBACK;
来源：http://atq.aibaodan.cn

[Q66] 行锁查询
来源：http://fno.tanke756.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://czx.quarkkingdee.top

[Q67] 设置隔离级别
来源：http://wsx.zhiwuduotai.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ajx.shangyingyoupin.top

[Q68] 保存点
来源：http://sws.xziqi.cn

SAVEPOINT sp1;
来源：http://srh.316326.xyz

ROLLBACK TO sp1;
来源：http://puy.snrcjt.cn

[Q69] 查看执行计划
来源：http://lpx.feifeiyinyue.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mrd.zycfv.cn

[Q70] 更新统计信息
来源：http://fjp.hammf.cn

ANALYZE TABLE users;
来源：http://wvu.nanxinkj.top

[Q71] 查看建表语句
来源：http://kzf.ybcxt.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://yhl.chenzaomai.com

[Q72] 查看索引
来源：http://kwl.hywenlv.cn

SHOW INDEX FROM users;
来源：http://dig.iojbl.cn

[Q73] 查看表状态
来源：http://atz.mhx1999.top

SHOW TABLE STATUS LIKE 'users';
来源：http://yms.hnxiangtu.top

[Q74] 强制使用索引
来源：http://oxs.vehdjk.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://kfs.svipenyu.cn

[Q75] 日期格式化
来源：http://hvq.snrcjt.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://cod.jinghuilouyu.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://dkt.snrcjt.cn

[Q76] 按天统计
来源：http://nun.pycfn.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ynn.fzhhl.top

[Q77] 时间加减
来源：http://nsi.zycfv.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://had.chenjidiqi.icu

[Q78] 当前时间
来源：http://ayq.yueranfly.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://zli.jinyuanbaomall.cn

[Q79] 字符串拼接
来源：http://aik.sjlbkw.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://fsk.gaohongyu789.top

[Q80] 字符串截取
来源：http://res.redwolf501.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://jxc.hnxiangtu.top

[Q81] 字符串替换
来源：http://blk.epnwcf.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://jwg.jinqigfzy.top

[Q82] 字符长度与字节长度
来源：http://axz.jqgufenzy.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://waq.gogol.net.cn

[Q83] 大小写转换
来源：http://kew.xinyue.icu

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://qno.tarul.cn

[Q84] 去除首尾空格
来源：http://pdd.c1oappe.top

SELECT TRIM(name) FROM users;
来源：http://lho.cashguo.top

[Q85] 数值取整
来源：http://yxv.yfazqb.com

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mte.meibo888.top

[Q86] 读取 JSON 字段
来源：http://vcw.nwbrower.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://rko.tian-w.cn

[Q87] JSON 字段做条件
来源：http://aqb.zhongyouzk.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://xqg.fzhhl.top

[Q88] 行转列（条件聚合）
来源：http://hyv.nanxinkj.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://uid.shuidangran.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://lsx.yuxming.cn

[Q89] 判断表是否存在
来源：http://qcp.sweek.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://svb.0kj1m.cn

[Q90] 生成序号列
来源：http://qfi.tanke756.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://cpa.chenlongwang.top

================================================================================
来源：http://tsq.yj20258.top

R. Bash 专题
来源：http://ntn.zycfv.cn

================================================================================
来源：http://kpl.bbcook.cn

[R01] shebang 与严格模式
来源：http://svy.jianghu66.top

#!/usr/bin/env bash
来源：http://nsr.xingfuxueyuan.xyz

set -euo pipefail
来源：http://lwi.fzhhl.top

[R02] 变量赋值与使用
来源：http://xmu.shangyingyoupin.top

name="Tom"; echo "$name"
来源：http://ofj.pengpengdd.cyou

[R03] 只读变量
来源：http://jtk.sxryk.cn

readonly PI=3.14
来源：http://nfk.sxryk.cn

[R04] 位置参数
来源：http://hpp.jinqigfzy.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://xrf.iojbl.cn

[R05] 参数默认值
来源：http://qws.hnqzz.top

name="${1:-default}"
来源：http://mnd.jlsjyb.cn

[R06] 判断命令是否存在
来源：http://dil.yuxming.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ncc.pycfn.com

[R07] if 判断文件
来源：http://eyx.jqgfzy.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://yat.yangfankeji.com

[R08] 数值比较
来源：http://ryt.gogol.net.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://oee.gogol.net.cn

[R09] 字符串比较
来源：http://fnk.shuidangran.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mdd.zhaomingkeji.xyz

[R10] 正则匹配
来源：http://smj.wangdashe.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://qpm.zhengqikj.top

[R11] case 多分支
来源：http://tom.sysykeji.top

case "$1" in
来源：http://mho.gotoacloud.top

start) echo "启动" ;;
来源：http://sxd.ywan-chungtsiang.top

stop)  echo "停止" ;;
来源：http://xkp.zdqjudy.top

*)     echo "未知命令" ;;
来源：http://zza.yj202588.top

esac
来源：http://zbk.snrcjt.cn

[R12] for 遍历文件
来源：http://dyb.guannengcc.top

for f in *.txt; do echo "$f"; done
来源：http://feo.jyoumei.cn

[R13] for 计数循环
来源：http://fzt.zhiwuduotai.top

for i in {1..10}; do echo "$i"; done
来源：http://gan.xingfuxueyuan.xyz

[R14] C 风格 for
来源：http://zqi.jqgufenzy.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wue.316326.xyz

[R15] while 逐行读文件
来源：http://uta.yanxiufei.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://scq.dianchejie.cn

[R16] until 等待条件
来源：http://isr.ivvv.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://dne.nanxinkj.top

[R17] 数组定义与取值
来源：http://cvw.vqdsnc.cn

arr=(a b c); echo "${arr[0]}"
来源：http://nys.gaohongyu789.top

[R18] 遍历数组
来源：http://mbn.sxryk.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://duq.zhengqikj.top

[R19] 数组长度
来源：http://hex.cdnleiting.top

echo "${#arr[@]}"
来源：http://myo.pycfn.com

[R20] 关联数组（字典）
来源：http://agx.sysykeji.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://zxx.xinyue.icu

[R21] 字符串长度
来源：http://iiq.zhoulong.xyz

echo "${#s}"
来源：http://pqf.iojbl.cn

[R22] 截取子串
来源：http://fbg.jinqigfzy.top

echo "${s:0:5}"
来源：http://ycw.epnwcf.com

[R23] 字符串替换
来源：http://twn.meibo888.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://gtw.yfazqb.com

[R24] 大小写转换
来源：http://utg.jqgfzy.top

echo "${s^^}"; echo "${s,,}"
来源：http://sqf.0kj1m.cn

[R25] 去后缀 / 去前缀
来源：http://fuh.chenzaomai.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://ahx.aibaodan.cn

[R26] 命令替换
来源：http://shw.vqdsnc.cn

now=$(date +%F); echo "$now"
来源：http://gcx.tian-w.cn

[R27] 算术展开
来源：http://qdg.yj20258.top

echo $((1 + 2 * 3))
来源：http://ovb.ivvv.top

[R28] 浮点运算
来源：http://qie.vehdjk.com

echo "scale=2; 10/3" | bc
来源：http://bfh.jqgfzy.top

[R29] 定义函数
来源：http://cym.hywenlv.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://jfa.gotoacloud.top

[R30] 函数返回状态码
来源：http://hif.fktsv.cn

f() { return 0; }; f || echo "失败了"
来源：http://skx.c1oappe.top

[R31] 局部变量
来源：http://ysl.yj202588.top

f() { local x=1; echo "$x"; }
来源：http://kof.yuxming.cn

[R32] 参数个数校验
来源：http://cyb.yj20258.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mia.hywenlv.cn

[R33] 捕获错误并提示行号
来源：http://ttf.cucudq.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://azw.ehwqpu.com

[R34] 退出时清理
来源：http://gxb.dianchejie.cn

trap 'rm -f "$tmp"' EXIT
来源：http://qhw.gzhubu.top

[R35] 后台执行并等待
来源：http://yrr.shanyushiyangkeji.top

sleep 5 & pid=$!; wait "$pid"
来源：http://acx.feifeiyinyue.top

[R36] 并发执行多个任务
来源：http://pfr.cdnleiting.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://bwu.hcnkem.com

[R37] 把输出赋给变量
来源：http://jua.zhaomingkeji.xyz

files=$(ls -1)
来源：http://hhy.xziqi.cn

[R38] 管道串联
来源：http://rgj.meibo888.top

cat a.txt | grep -i error | wc -l
来源：http://avr.hesvh.cn

[R39] 重定向标准输出与错误
来源：http://ode.jqgufenzy.top

cmd > out.log 2>&1
来源：http://flr.cqqwz.cn

[R40] 追加写日志
来源：http://esv.nwbrower.top

echo "log" >> out.log
来源：http://lku.zhijiandao.cn

[R41] 丢弃输出
来源：http://ibu.sxryk.cn

cmd >/dev/null 2>&1
来源：http://mzw.smart0.xyz

[R42] 输入重定向
来源：http://pzs.iojbl.cn

wc -l < a.txt
来源：http://ayp.cdnleiting.top

[R43] 按名字查找文件
来源：http://tkr.quarkkingdee.top

find . -name "*.log" -type f
来源：http://yck.daxiang520.top

[R44] 按修改时间查找
来源：http://nkw.yfazqb.com

find . -mtime -7 -type f
来源：http://job.zhixingplan.top

[R45] 批量删除
来源：http://vug.wangshuangyany.cn

find . -name "*.tmp" -delete
来源：http://fen.zycfv.cn

[R46] 递归替换文件内容
来源：http://ixk.cucudq.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://vqi.zhixingplan.top

[R47] sed 单行替换
来源：http://brp.zycfv.cn

sed -i 's/foo/bar/g' a.txt
来源：http://jvz.yongpay.top

[R48] awk 取指定列
来源：http://jqt.fanxiaobao.xyz

awk '{print $1, $3}' a.txt
来源：http://kuc.epnwcf.com

[R49] awk 带条件
来源：http://lhs.feifeiyinyue.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://bup.hfpthk.cn

[R50] awk 求和
来源：http://zmv.jiagoushi.top

awk '{s += $2} END {print s}' a.txt
来源：http://sek.hysaishi.cn

[R51] 排序去重取前几
来源：http://kpm.yj202588.top

sort a.txt | uniq -c | sort -rn | head
来源：http://bzv.xingfuxueyuan.xyz

[R52] 统计行数
来源：http://mkc.zhiwuduotai.top

wc -l a.txt
来源：http://cib.nwbrower.top

[R53] 查看文件头与实时尾
来源：http://lar.meibo888.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://osi.fehbvm.com

[R54] 比较两个文件
来源：http://pfw.redwolf501.top

diff a.txt b.txt
来源：http://hzv.ywan-chungtsiang.top

[R55] 压缩与解压
来源：http://exx.jyoumei.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://did.shangyingyoupin.top

[R56] 远程拷贝
来源：http://xwk.tarul.cn

scp file user@host:/path/
来源：http://rux.yangfankeji.com

[R57] 远程执行命令
来源：http://ptx.yj202588.top

ssh user@host 'uptime'
来源：http://jjo.haohaochexian.top

[R58] 下载文件
来源：http://pez.quarkkingdee.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://gjk.xziqi.cn

[R59] 发 POST JSON
来源：http://uwt.iojbl.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://bng.yuanzhike.top

[R60] 只看 HTTP 状态码
来源：http://gdy.shangyingyoupin.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://bmn.mhx1999.top

[R61] 磁盘占用
来源：http://oxg.iojbl.cn

df -h;  du -sh *
来源：http://evz.hesvh.cn

[R62] 找最占空间的文件
来源：http://ggn.ctjpmb.com

du -ah . | sort -rh | head -10
来源：http://vtr.havefunace.top

[R63] 内存与进程
来源：http://yle.aizwys.cn

free -h;  ps aux | grep nginx
来源：http://lbk.iojbl.cn

[R64] 结束进程
来源：http://ykx.yonumen.top

kill -9 $(pgrep -f app.py)
来源：http://sfw.yuxming.cn

[R65] 查看端口占用
来源：http://kkg.havefunace.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://vyn.0kj1m.cn

[R66] 定时任务
来源：http://kho.yongpay.top

crontab -e;  crontab -l
来源：http://brn.hcnkem.com

[R67] 生成随机十六进制串
来源：http://owa.svipenyu.cn

openssl rand -hex 16
来源：http://ryk.chenjidiqi.icu

[R68] 计算文件校验值
来源：http://bgx.chenzaomai.com

sha256sum a.txt;  md5sum a.txt
来源：http://for.yonumen.top

[R69] 生成随机密码
来源：http://ift.hfpthk.cn

head -c 16 /dev/urandom | base64
来源：http://rve.yuanzhike.top

[R70] 时间戳与互转
来源：http://clp.jqgufenzy.top

date +%s;  date -d @1700000000
来源：http://ajq.yj202588.top

[R71] 日期格式化
来源：http://eck.yongpay.top


<!-- 参考信息 -->