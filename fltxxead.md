代发 wailian999

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://yfk.havefunace.top

[Q24] 去重
来源：http://zdc.xuanzx.com

SELECT DISTINCT city FROM users;
来源：http://dcu.wangshuangyany.cn

[Q25] 只取前 N 条
来源：http://hjm.hywenlv.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://vqm.ywan-chungtsiang.top

[Q26] 计数
来源：http://slk.jinghuilouyu.cn

SELECT COUNT(*) FROM users;
来源：http://kex.zhoulong.xyz

[Q27] 条件计数
来源：http://mgq.fktsv.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://boe.0kj1m.cn

[Q28] 求和与平均
来源：http://nkh.iojbl.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://qgk.zhengqikj.top

[Q29] 最大最小值
来源：http://hvr.ctjpmb.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://did.fengsongda.top

[Q30] 分组统计
来源：http://wri.shzxlz.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://gab.bjfxy.top

[Q31] 分组后过滤
来源：http://mhl.zdbjq.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hpy.yfazqb.com

[Q32] 分组拼接字符串
来源：http://smp.haohaochexian.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wsg.xingfuxueyuan.xyz

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ehm.zhongyouzk.top

[Q33] 多列分组
来源：http://iap.fehbvm.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://pqs.vehdjk.com

[Q34] 每组取第一条
来源：http://xnh.wangdashe.top

SELECT * FROM (
来源：http://cfg.ydzc1.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://fjv.hnxiangtu.top

) t WHERE rn = 1;
来源：http://gzw.epnwcf.com

[Q35] 内连接
来源：http://tio.hongshengwenyu.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://vtc.daria6918.cn

[Q36] 左连接
来源：http://fst.snrcjt.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://shw.xylfe.cn

[Q37] 右连接
来源：http://vws.shzxlz.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://nhz.316326.xyz

[Q38] 全外连接（PostgreSQL）
来源：http://tqb.ydjk.org.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mpo.bbcook.cn

[Q39] 自连接（查上下级）
来源：http://dov.xuetiantiany.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ktt.cashguo.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://yqr.hesvh.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://oaq.zhoulong.xyz

SELECT * FROM colors CROSS JOIN sizes;
来源：http://uxo.zdbjq.cn

[Q41] 多表连接
来源：http://xfx.svipenyu.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ydf.cdnleiting.top

JOIN users u ON u.id = o.user_id
来源：http://tgy.snrcjt.cn

JOIN products p ON p.id = o.product_id;
来源：http://diw.0kj1m.cn

[Q42] 连接条件附加过滤
来源：http://jpm.daxiang520.top

SELECT u.name, o.amount FROM users u
来源：http://whx.gzhubu.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://bdm.jianghu66.top

[Q43] 标量子查询
来源：http://lms.cucudq.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ldp.meibo888.top

[Q44] IN 子查询
来源：http://hlf.tanke756.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://aqb.xuetiantiany.cn

[Q45] EXISTS 判断存在
来源：http://wup.jianghu66.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://dgd.zdqjudy.top

[Q46] NOT EXISTS 判断不存在
来源：http://nmu.bjfxy.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hpg.ybcxt.top

[Q47] 与平均值比较
来源：http://rkh.mhx1999.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ujo.birdmap.top

[Q48] CTE 公用表表达式
来源：http://fpg.ydzc1.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://gcj.hywenlv.cn

SELECT * FROM t WHERE c > 5;
来源：http://ftn.ydjk.org.cn

[Q49] 更新单行
来源：http://kpp.snrcjt.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://rnc.pycfn.com

[Q50] 批量更新
来源：http://rfi.pengpengdd.cyou

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://byk.guowangkeji.top

[Q51] 用子查询更新
来源：http://bgx.zhiwuduotai.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wil.ydjk.org.cn

[Q52] 删除指定行
来源：http://uzs.nanxinkj.top

DELETE FROM users WHERE id = 10;
来源：http://cmh.yvedp.cn

[Q53] 按条件删除
来源：http://jdm.guannengcc.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://elg.nanxuanxn.top

[Q54] 清空表
来源：http://ksy.0kj1m.cn

TRUNCATE TABLE logs;
来源：http://mes.zhoulong.xyz

[Q55] 排名（并列占位）
来源：http://xbo.tanke756.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://tpo.yongpay.top

[Q56] 密集排名（并列不占位）
来源：http://iwh.0kj1m.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://itl.quarkkingdee.top

[Q57] 行号
来源：http://wbj.hesvh.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ngw.sweek.top

[Q58] 累计求和
来源：http://qjl.cdnleiting.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wdv.fehbvm.com

[Q59] 分组内累计
来源：http://opi.zhongyouzk.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://tln.mhx1999.top

[Q60] 取上一行 / 下一行
来源：http://kxk.zhaomingkeji.xyz

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://dbu.mhx1999.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://kmm.yfazqb.com

[Q61] 移动平均
来源：http://zre.wangshuangyany.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://iqt.cdnleiting.top

[Q62] 分组占比
来源：http://vxm.c1oappe.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://gdb.tianlin.xyz

[Q63] 开启事务
来源：http://jps.jinghuilouyu.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://nje.pengpengdd.cyou

[Q64] 提交事务
来源：http://lcy.jinqigufen.top

COMMIT;
来源：http://rft.jinyuanbaomall.cn

[Q65] 回滚事务
来源：http://qlr.jinyuanbaomall.cn

ROLLBACK;
来源：http://wrb.xylfe.cn

[Q66] 行锁查询
来源：http://qjw.aizwys.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://vlt.ydzc1.top

[Q67] 设置隔离级别
来源：http://ngn.zhiwuduotai.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://vhn.yfazqb.com

[Q68] 保存点
来源：http://zdr.quarkkingdee.top

SAVEPOINT sp1;
来源：http://uqj.cheryme.top

ROLLBACK TO sp1;
来源：http://wrg.jiagoushi.top

[Q69] 查看执行计划
来源：http://ofc.316326.xyz

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://tto.chenzaomai.com

[Q70] 更新统计信息
来源：http://npw.xuetiantiany.cn

ANALYZE TABLE users;
来源：http://bfi.9152youxi.cn

[Q71] 查看建表语句
来源：http://gdb.zhaomingkeji.xyz

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wzx.jinghuilouyu.cn

[Q72] 查看索引
来源：http://dlf.yonumen.top

SHOW INDEX FROM users;
来源：http://uhm.sweek.top

[Q73] 查看表状态
来源：http://daw.zhijiandao.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://obo.ppjwa.cn

[Q74] 强制使用索引
来源：http://qap.gogol.net.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://jpw.yj20258888.top

[Q75] 日期格式化
来源：http://gkt.sjlbkw.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://dul.fehbvm.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://egk.yuanzhike.top

[Q76] 按天统计
来源：http://jrj.andypj.xyz

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ujj.havefunace.top

[Q77] 时间加减
来源：http://cnf.jinyuanbaomall.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://cew.meibo888.top

[Q78] 当前时间
来源：http://zdc.zhoulong.xyz

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://nrb.yonumen.top

[Q79] 字符串拼接
来源：http://qxf.yueranfly.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://tgu.ctjpmb.com

[Q80] 字符串截取
来源：http://jof.chenlongwang.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://shr.sufxvd.cn

[Q81] 字符串替换
来源：http://uqw.pycfn.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://sgl.hfpthk.cn

[Q82] 字符长度与字节长度
来源：http://fci.svipenyu.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://urv.zhijiandao.cn

[Q83] 大小写转换
来源：http://aza.zhongyouzk.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://jgi.gotoacloud.top

[Q84] 去除首尾空格
来源：http://tsu.yanxiufei.cn

SELECT TRIM(name) FROM users;
来源：http://jdn.havefunace.top

[Q85] 数值取整
来源：http://zwt.shzxlz.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://nha.xingfuxueyuan.xyz

[Q86] 读取 JSON 字段
来源：http://xhd.yongpay.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ojc.bjfxy.top

[Q87] JSON 字段做条件
来源：http://rjq.aizwys.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://sgh.gotoacloud.top

[Q88] 行转列（条件聚合）
来源：http://upk.sjlbkw.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ewd.pycfn.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://zop.kuanghao11.cn

[Q89] 判断表是否存在
来源：http://atk.jinqigfzy.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://jih.jinqigufen.top

[Q90] 生成序号列
来源：http://obg.aizwys.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ovw.guannengcc.top

================================================================================
来源：http://ran.chenzaomai.com

R. Bash 专题
来源：http://kaa.tarul.cn

================================================================================
来源：http://fyk.tanke756.top

[R01] shebang 与严格模式
来源：http://eds.jinqigfzy.top

#!/usr/bin/env bash
来源：http://fvr.yj20258888.top

set -euo pipefail
来源：http://qps.dianchejie.cn

[R02] 变量赋值与使用
来源：http://nis.cdnleiting.top

name="Tom"; echo "$name"
来源：http://tup.cheryme.top

[R03] 只读变量
来源：http://uuf.epnwcf.com

readonly PI=3.14
来源：http://yxm.haohaochexian.top

[R04] 位置参数
来源：http://tfu.jqgufenzy.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://uro.smart0.xyz

[R05] 参数默认值
来源：http://xuy.sweek.top

name="${1:-default}"
来源：http://mnp.nanxinkj.top

[R06] 判断命令是否存在
来源：http://vpg.ydjk.org.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mjs.hesvh.cn

[R07] if 判断文件
来源：http://pgi.fktsv.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://rgt.xuetiantiany.cn

[R08] 数值比较
来源：http://ujx.jqgufenzy.top

if (( a > b )); then echo "a 更大"; fi
来源：http://oub.bjfxy.top

[R09] 字符串比较
来源：http://ryp.ywan-chungtsiang.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://vhw.sysykeji.top

[R10] 正则匹配
来源：http://nee.cqqwz.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://jaa.guowangkeji.top

[R11] case 多分支
来源：http://ahr.sufxvd.cn

case "$1" in
来源：http://jip.shangyingyoupin.top

start) echo "启动" ;;
来源：http://jfv.gotoacloud.top

stop)  echo "停止" ;;
来源：http://ikv.tarul.cn

*)     echo "未知命令" ;;
来源：http://jfl.nanxinkj.top

esac
来源：http://ipb.yfazqb.com

[R12] for 遍历文件
来源：http://ahl.nanxinkj.top

for f in *.txt; do echo "$f"; done
来源：http://blq.hysaishi.cn

[R13] for 计数循环
来源：http://quk.hfpthk.cn

for i in {1..10}; do echo "$i"; done
来源：http://lae.mhx1999.top

[R14] C 风格 for
来源：http://vvb.wangshuangyany.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://iwq.sufxvd.cn

[R15] while 逐行读文件
来源：http://aya.hammf.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://bse.ywan-chungtsiang.top

[R16] until 等待条件
来源：http://jim.vqdsnc.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://zdv.ivvv.top

[R17] 数组定义与取值
来源：http://kla.bbcook.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ezi.xinyue.icu

[R18] 遍历数组
来源：http://ifh.gzhubu.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://pxx.guowangkeji.top

[R19] 数组长度
来源：http://rsf.vqdsnc.cn

echo "${#arr[@]}"
来源：http://lsu.pengpengdd.cyou

[R20] 关联数组（字典）
来源：http://meq.zhongyouzk.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://fky.gotoacloud.top

[R21] 字符串长度
来源：http://exn.haohaochexian.top

echo "${#s}"
来源：http://hnm.birdmap.top

[R22] 截取子串
来源：http://nru.shuidangran.top

echo "${s:0:5}"
来源：http://asn.jyoumei.cn

[R23] 字符串替换
来源：http://skr.yj20258888.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://stx.jinghuilouyu.cn

[R24] 大小写转换
来源：http://hlz.ehwqpu.com

echo "${s^^}"; echo "${s,,}"
来源：http://klz.yvedp.cn

[R25] 去后缀 / 去前缀
来源：http://pgl.zdbjq.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://mbo.svipenyu.cn

[R26] 命令替换
来源：http://tii.cucudq.cn

now=$(date +%F); echo "$now"
来源：http://wml.aibaodan.cn

[R27] 算术展开
来源：http://ing.chenzaomai.com

echo $((1 + 2 * 3))
来源：http://meu.gzhubu.top

[R28] 浮点运算
来源：http://aem.snrcjt.cn

echo "scale=2; 10/3" | bc
来源：http://cws.smart0.xyz

[R29] 定义函数
来源：http://dgy.chenzaomai.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ayw.hysaishi.cn

[R30] 函数返回状态码
来源：http://sdf.52xcode.cn

f() { return 0; }; f || echo "失败了"
来源：http://kat.ydjk.org.cn

[R31] 局部变量
来源：http://nhd.ybcxt.top

f() { local x=1; echo "$x"; }
来源：http://gbf.andypj.xyz

[R32] 参数个数校验
来源：http://yyu.daxiang520.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://bsk.ppjwa.cn

[R33] 捕获错误并提示行号
来源：http://xcf.kuanghao11.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://nyn.iojbl.cn

[R34] 退出时清理
来源：http://its.fehbvm.com

trap 'rm -f "$tmp"' EXIT
来源：http://mfr.guowangkeji.top

[R35] 后台执行并等待
来源：http://ytw.chenlongwang.top

sleep 5 & pid=$!; wait "$pid"
来源：http://frv.yangfankeji.com

[R36] 并发执行多个任务
来源：http://ulr.aibaodan.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://dhi.hywenlv.cn

[R37] 把输出赋给变量
来源：http://kfp.shanyushiyangkeji.top

files=$(ls -1)
来源：http://itl.c1oappe.top

[R38] 管道串联
来源：http://ajc.xuanzx.com

cat a.txt | grep -i error | wc -l
来源：http://gck.yuxming.cn

[R39] 重定向标准输出与错误
来源：http://wog.shangyingyoupin.top

cmd > out.log 2>&1
来源：http://epv.andypj.xyz

[R40] 追加写日志
来源：http://wyq.cqqwz.cn

echo "log" >> out.log
来源：http://nyf.sjlbkw.cn

[R41] 丢弃输出
来源：http://ydq.iojbl.cn

cmd >/dev/null 2>&1
来源：http://hou.yueranfly.top

[R42] 输入重定向
来源：http://ymh.hesvh.cn

wc -l < a.txt
来源：http://oap.jqgfzy.top

[R43] 按名字查找文件
来源：http://rzl.yonumen.top

find . -name "*.log" -type f
来源：http://jsc.yueranfly.top

[R44] 按修改时间查找
来源：http://nxy.birdmap.top

find . -mtime -7 -type f
来源：http://dlg.haohaochexian.top

[R45] 批量删除
来源：http://gcf.hnxiangtu.top

find . -name "*.tmp" -delete
来源：http://uqg.9152youxi.cn

[R46] 递归替换文件内容
来源：http://qoj.yuanzhike.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://fdm.fanxiaobao.xyz

[R47] sed 单行替换
来源：http://jva.sweek.top

sed -i 's/foo/bar/g' a.txt
来源：http://aps.dashuyun.cn

[R48] awk 取指定列
来源：http://acq.fengsongda.top

awk '{print $1, $3}' a.txt
来源：http://oco.guannengcc.top

[R49] awk 带条件
来源：http://bap.xuetiantiany.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://bvg.andypj.xyz

[R50] awk 求和
来源：http://vhu.guannengcc.top

awk '{s += $2} END {print s}' a.txt
来源：http://cqq.daria6918.cn

[R51] 排序去重取前几
来源：http://itz.smart0.xyz

sort a.txt | uniq -c | sort -rn | head
来源：http://ify.sysykeji.top

[R52] 统计行数
来源：http://ace.shanyushiyangkeji.top

wc -l a.txt
来源：http://iow.cashguo.top

[R53] 查看文件头与实时尾
来源：http://obn.xylfe.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://vcf.guowangkeji.top

[R54] 比较两个文件
来源：http://mop.mhx1999.top

diff a.txt b.txt
来源：http://nru.hammf.cn

[R55] 压缩与解压
来源：http://ofy.yvedp.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ufg.kuanghao11.cn

[R56] 远程拷贝
来源：http://cdc.hnqzz.top

scp file user@host:/path/
来源：http://weu.cdnleiting.top

[R57] 远程执行命令
来源：http://wwy.jyoumei.cn

ssh user@host 'uptime'
来源：http://avp.ybcxt.top

[R58] 下载文件
来源：http://pdx.fehbvm.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://htc.vehdjk.com

[R59] 发 POST JSON
来源：http://mkx.hesvh.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://nre.meibo888.top

[R60] 只看 HTTP 状态码
来源：http://feb.tanke756.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wim.havefunace.top

[R61] 磁盘占用
来源：http://yjp.jinyuanbaomall.cn

df -h;  du -sh *
来源：http://usq.aibaodan.cn

[R62] 找最占空间的文件
来源：http://wrf.ivvv.top

du -ah . | sort -rh | head -10
来源：http://uzt.kuanghao11.cn

[R63] 内存与进程
来源：http://wql.52xcode.cn

free -h;  ps aux | grep nginx
来源：http://wlm.xylfe.cn

[R64] 结束进程
来源：http://poa.zycfv.cn

kill -9 $(pgrep -f app.py)
来源：http://ssc.ivvv.top

[R65] 查看端口占用
来源：http://awl.tarul.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://gag.yanxiufei.cn

[R66] 定时任务
来源：http://nfi.tianlin.xyz

crontab -e;  crontab -l
来源：http://slc.epnwcf.com

[R67] 生成随机十六进制串
来源：http://phz.ppjwa.cn

openssl rand -hex 16
来源：http://ulx.shzxlz.cn

[R68] 计算文件校验值
来源：http://hzr.bbcook.cn

sha256sum a.txt;  md5sum a.txt
来源：http://mlu.fzhhl.top

[R69] 生成随机密码
来源：http://lfd.yuanzhike.top

head -c 16 /dev/urandom | base64
来源：http://xff.hcnkem.com

[R70] 时间戳与互转
来源：http://hcg.shanyushiyangkeji.top

date +%s;  date -d @1700000000
来源：http://var.hongshengwenyu.top

[R71] 日期格式化
来源：http://ykt.dianchejie.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://rct.shangyingyoupin.top

[R72] 等待端口就绪
来源：http://eyf.jinghuilouyu.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://iod.fanxiaobao.xyz

[R73] 分割大日志
来源：http://ewu.tanke756.top


<!-- 参考信息 -->