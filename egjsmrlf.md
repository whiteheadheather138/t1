代发 wailian999

SELECT * FROM users WHERE email IS NULL;
来源：http://ysf.c1oappe.top

[Q22] 排序
来源：http://zju.52xcode.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hql.zycfv.cn

[Q23] 分页
来源：http://lgo.fehbvm.com

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://nij.snrcjt.cn

[Q24] 去重
来源：http://xkb.hywenlv.cn

SELECT DISTINCT city FROM users;
来源：http://sch.meibo888.top

[Q25] 只取前 N 条
来源：http://ijs.fanxiaobao.xyz

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://pwh.zdqjudy.top

[Q26] 计数
来源：http://wpe.wangdashe.top

SELECT COUNT(*) FROM users;
来源：http://fny.pycfn.com

[Q27] 条件计数
来源：http://fld.yongpay.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://vrs.pengpengdd.cyou

[Q28] 求和与平均
来源：http://wwg.chenjidiqi.icu

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://spg.sjlbkw.cn

[Q29] 最大最小值
来源：http://btu.9152youxi.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://zzw.bjfxy.top

[Q30] 分组统计
来源：http://hew.mhx1999.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ykg.zdqjudy.top

[Q31] 分组后过滤
来源：http://vaq.jyoumei.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://kmf.xingfuxueyuan.xyz

[Q32] 分组拼接字符串
来源：http://alw.hnqzz.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ujk.guowangkeji.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mpe.yangfankeji.com

[Q33] 多列分组
来源：http://erh.jinyuanbaomall.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://xdz.yj20258.top

[Q34] 每组取第一条
来源：http://sjr.hongshengwenyu.top

SELECT * FROM (
来源：http://sso.guannengcc.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://nez.jlsjyb.cn

) t WHERE rn = 1;
来源：http://qtk.nanxuanxn.top

[Q35] 内连接
来源：http://fql.gaohongyu789.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://lhc.9152youxi.cn

[Q36] 左连接
来源：http://bnb.tanke756.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://kje.cucudq.cn

[Q37] 右连接
来源：http://jhg.aizwys.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://bdj.ydjk.org.cn

[Q38] 全外连接（PostgreSQL）
来源：http://cpe.tianlin.xyz

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://gkx.ivvv.top

[Q39] 自连接（查上下级）
来源：http://jcp.tianlin.xyz

SELECT e.name, m.name AS manager FROM employees e
来源：http://hmw.gaohongyu789.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://pwd.jinqigufen.top

[Q40] 交叉连接（笛卡尔积）
来源：http://kfa.yuanzhike.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hlr.jinghuilouyu.cn

[Q41] 多表连接
来源：http://ufj.gaohongyu789.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://lxa.yuanzhike.top

JOIN users u ON u.id = o.user_id
来源：http://llc.bjfxy.top

JOIN products p ON p.id = o.product_id;
来源：http://pwn.guowangkeji.top

[Q42] 连接条件附加过滤
来源：http://tlq.cqqwz.cn

SELECT u.name, o.amount FROM users u
来源：http://bih.jinqigufen.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://xwi.jyoumei.cn

[Q43] 标量子查询
来源：http://jhv.tanke756.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://brh.sysykeji.top

[Q44] IN 子查询
来源：http://lls.kuanghao11.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wkm.zdqjudy.top

[Q45] EXISTS 判断存在
来源：http://psv.chenlongwang.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://acd.yuanzhike.top

[Q46] NOT EXISTS 判断不存在
来源：http://hch.gogol.net.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://pyz.zhijiandao.cn

[Q47] 与平均值比较
来源：http://urr.hnxiangtu.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://tgc.chenlongwang.top

[Q48] CTE 公用表表达式
来源：http://xby.tarul.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://nuf.ydjk.org.cn

SELECT * FROM t WHERE c > 5;
来源：http://ytf.cashguo.top

[Q49] 更新单行
来源：http://vfo.chenlongwang.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://czm.kuanghao11.cn

[Q50] 批量更新
来源：http://hud.guowangkeji.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://lfo.smart0.xyz

[Q51] 用子查询更新
来源：http://kpi.hongshengwenyu.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://bdo.ivvv.top

[Q52] 删除指定行
来源：http://gvk.chenlongwang.top

DELETE FROM users WHERE id = 10;
来源：http://wjp.tian-w.cn

[Q53] 按条件删除
来源：http://zwu.jinghuilouyu.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ubd.xingfuxueyuan.xyz

[Q54] 清空表
来源：http://bnw.andypj.xyz

TRUNCATE TABLE logs;
来源：http://swh.xinyue.icu

[Q55] 排名（并列占位）
来源：http://jmu.jiagoushi.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://kbr.chenlongwang.top

[Q56] 密集排名（并列不占位）
来源：http://zxv.guannengcc.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://pyf.sysykeji.top

[Q57] 行号
来源：http://uxk.dashuyun.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blo.yj202588.top

[Q58] 累计求和
来源：http://tpl.haohaochexian.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://xgp.yueranfly.top

[Q59] 分组内累计
来源：http://fjl.nwbrower.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://gsm.yueranfly.top

[Q60] 取上一行 / 下一行
来源：http://bll.gogol.net.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ivv.ivvv.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://xij.0kj1m.cn

[Q61] 移动平均
来源：http://ays.sweek.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ydr.zdbjq.cn

[Q62] 分组占比
来源：http://xot.tianlin.xyz

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://vhk.hfpthk.cn

[Q63] 开启事务
来源：http://acf.quarkkingdee.top

START TRANSACTION;                -- 或 BEGIN
来源：http://smj.bbcook.cn

[Q64] 提交事务
来源：http://mxf.ywan-chungtsiang.top

COMMIT;
来源：http://qfo.chenjidiqi.icu

[Q65] 回滚事务
来源：http://tgl.zycfv.cn

ROLLBACK;
来源：http://jvk.dashuyun.cn

[Q66] 行锁查询
来源：http://qqq.shuidangran.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://xis.jlsjyb.cn

[Q67] 设置隔离级别
来源：http://hmo.smart0.xyz

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://cek.xuetiantiany.cn

[Q68] 保存点
来源：http://oqm.vqdsnc.cn

SAVEPOINT sp1;
来源：http://uqt.hywenlv.cn

ROLLBACK TO sp1;
来源：http://dzg.tanke756.top

[Q69] 查看执行计划
来源：http://jbp.mhx1999.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://qsw.bjfxy.top

[Q70] 更新统计信息
来源：http://gqe.xuanzx.com

ANALYZE TABLE users;
来源：http://jsa.bbcook.cn

[Q71] 查看建表语句
来源：http://fqq.hysaishi.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://cjr.hongshengwenyu.top

[Q72] 查看索引
来源：http://mkz.316326.xyz

SHOW INDEX FROM users;
来源：http://wtv.wangdashe.top

[Q73] 查看表状态
来源：http://cah.feifeiyinyue.top

SHOW TABLE STATUS LIKE 'users';
来源：http://zxp.jlsjyb.cn

[Q74] 强制使用索引
来源：http://the.nanxinkj.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mdi.birdmap.top

[Q75] 日期格式化
来源：http://ala.ppjwa.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://xak.tanke756.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://dcn.xingfuxueyuan.xyz

[Q76] 按天统计
来源：http://srt.xziqi.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://dlx.vqdsnc.cn

[Q77] 时间加减
来源：http://ofq.dianchejie.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://zyw.chenlongwang.top

[Q78] 当前时间
来源：http://fxv.zycfv.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ukq.birdmap.top

[Q79] 字符串拼接
来源：http://mov.jiagoushi.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://imi.ppjwa.cn

[Q80] 字符串截取
来源：http://yfx.ywan-chungtsiang.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ciy.hywenlv.cn

[Q81] 字符串替换
来源：http://qel.yuanzhike.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://thx.fktsv.cn

[Q82] 字符长度与字节长度
来源：http://ysn.redwolf501.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://qpk.jinyuanbaomall.cn

[Q83] 大小写转换
来源：http://ikl.snrcjt.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://eyi.nanxuanxn.top

[Q84] 去除首尾空格
来源：http://yiy.yongpay.top

SELECT TRIM(name) FROM users;
来源：http://iml.zhoulong.xyz

[Q85] 数值取整
来源：http://rzy.jinyuanbaomall.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ovp.tian-w.cn

[Q86] 读取 JSON 字段
来源：http://zxa.xingfuxueyuan.xyz

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://jxd.kuanghao11.cn

[Q87] JSON 字段做条件
来源：http://ztr.yonumen.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://vxv.quarkkingdee.top

[Q88] 行转列（条件聚合）
来源：http://bqy.zhengqikj.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://eia.cucudq.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://isl.guowangkeji.top

[Q89] 判断表是否存在
来源：http://ceo.haohaochexian.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mcd.ybcxt.top

[Q90] 生成序号列
来源：http://dwv.xuanzx.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://bzz.chenzaomai.com

================================================================================
来源：http://wya.jinghuilouyu.cn

R. Bash 专题
来源：http://qqh.zhongyouzk.top

================================================================================
来源：http://ftv.mhx1999.top

[R01] shebang 与严格模式
来源：http://ukh.smart0.xyz

#!/usr/bin/env bash
来源：http://gcp.zhoulong.xyz

set -euo pipefail
来源：http://smr.daxiang520.top

[R02] 变量赋值与使用
来源：http://aae.jqgufenzy.top

name="Tom"; echo "$name"
来源：http://ufy.zhoulong.xyz

[R03] 只读变量
来源：http://xun.vqdsnc.cn

readonly PI=3.14
来源：http://oxi.yvedp.cn

[R04] 位置参数
来源：http://qdt.fanxiaobao.xyz

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://qli.zhaomingkeji.xyz

[R05] 参数默认值
来源：http://fwg.zhaomingkeji.xyz

name="${1:-default}"
来源：http://spr.chenjidiqi.icu

[R06] 判断命令是否存在
来源：http://qml.gotoacloud.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://tjm.chenjidiqi.icu

[R07] if 判断文件
来源：http://mib.ppjwa.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://veh.yj20258.top

[R08] 数值比较
来源：http://xiv.nanxinkj.top

if (( a > b )); then echo "a 更大"; fi
来源：http://sti.yangfankeji.com

[R09] 字符串比较
来源：http://eau.ydzc1.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mnd.smart0.xyz

[R10] 正则匹配
来源：http://yhz.xuetiantiany.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://htn.dianchejie.cn

[R11] case 多分支
来源：http://feq.cucudq.cn

case "$1" in
来源：http://cki.smart0.xyz

start) echo "启动" ;;
来源：http://ohp.pengpengdd.cyou

stop)  echo "停止" ;;
来源：http://dtl.52xcode.cn

*)     echo "未知命令" ;;
来源：http://qqb.hnxiangtu.top

esac
来源：http://bht.yangfankeji.com

[R12] for 遍历文件
来源：http://cat.ehwqpu.com

for f in *.txt; do echo "$f"; done
来源：http://wfs.0kj1m.cn

[R13] for 计数循环
来源：http://kvn.aibaodan.cn

for i in {1..10}; do echo "$i"; done
来源：http://ljq.hfpthk.cn

[R14] C 风格 for
来源：http://viw.cashguo.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://aoy.dashuyun.cn

[R15] while 逐行读文件
来源：http://jre.yueranfly.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://cqv.gogol.net.cn

[R16] until 等待条件
来源：http://lkl.vqdsnc.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mgk.dianchejie.cn

[R17] 数组定义与取值
来源：http://alp.jqgfzy.top

arr=(a b c); echo "${arr[0]}"
来源：http://xgz.vehdjk.com

[R18] 遍历数组
来源：http://grb.bjfxy.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wej.cucudq.cn

[R19] 数组长度
来源：http://wia.shuidangran.top

echo "${#arr[@]}"
来源：http://vfq.fktsv.cn

[R20] 关联数组（字典）
来源：http://dzp.bbcook.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://yhj.bbcook.cn

[R21] 字符串长度
来源：http://oga.52xcode.cn

echo "${#s}"
来源：http://ioo.vehdjk.com

[R22] 截取子串
来源：http://cih.quarkkingdee.top

echo "${s:0:5}"
来源：http://mnu.iojbl.cn

[R23] 字符串替换
来源：http://lre.vqdsnc.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://eem.quarkkingdee.top

[R24] 大小写转换
来源：http://lgs.zycfv.cn

echo "${s^^}"; echo "${s,,}"
来源：http://niu.jiagoushi.top

[R25] 去后缀 / 去前缀
来源：http://xdv.yueranfly.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://sup.fktsv.cn

[R26] 命令替换
来源：http://vsq.guannengcc.top

now=$(date +%F); echo "$now"
来源：http://aav.jinqigufen.top

[R27] 算术展开
来源：http://yns.yvedp.cn

echo $((1 + 2 * 3))
来源：http://jei.hnxiangtu.top

[R28] 浮点运算
来源：http://lac.vehdjk.com

echo "scale=2; 10/3" | bc
来源：http://rzs.zycfv.cn

[R29] 定义函数
来源：http://dvt.svipenyu.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ijz.zhongyouzk.top

[R30] 函数返回状态码
来源：http://sdm.jinqigfzy.top

f() { return 0; }; f || echo "失败了"
来源：http://hod.shangyingyoupin.top

[R31] 局部变量
来源：http://gsa.tian-w.cn

f() { local x=1; echo "$x"; }
来源：http://aee.chenjidiqi.icu

[R32] 参数个数校验
来源：http://enh.vqdsnc.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://zki.hfpthk.cn

[R33] 捕获错误并提示行号
来源：http://nlx.vqdsnc.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://bvd.xuanzx.com

[R34] 退出时清理
来源：http://pdb.shuidangran.top

trap 'rm -f "$tmp"' EXIT
来源：http://wlo.ivvv.top

[R35] 后台执行并等待
来源：http://uov.shanyushiyangkeji.top

sleep 5 & pid=$!; wait "$pid"
来源：http://oll.iojbl.cn

[R36] 并发执行多个任务
来源：http://ukz.snrcjt.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://thi.shangyingyoupin.top

[R37] 把输出赋给变量
来源：http://qnp.shanyushiyangkeji.top

files=$(ls -1)
来源：http://sag.sxryk.cn

[R38] 管道串联
来源：http://mfw.hammf.cn

cat a.txt | grep -i error | wc -l
来源：http://ssf.316326.xyz

[R39] 重定向标准输出与错误
来源：http://xbl.cdnleiting.top

cmd > out.log 2>&1
来源：http://nij.kuanghao11.cn

[R40] 追加写日志
来源：http://gtj.yongpay.top

echo "log" >> out.log
来源：http://byn.havefunace.top

[R41] 丢弃输出
来源：http://mue.ydjk.org.cn

cmd >/dev/null 2>&1
来源：http://nki.ybcxt.top

[R42] 输入重定向
来源：http://hjw.316326.xyz

wc -l < a.txt
来源：http://ooh.cheryme.top

[R43] 按名字查找文件
来源：http://duk.hnqzz.top

find . -name "*.log" -type f
来源：http://gjw.xingfuxueyuan.xyz

[R44] 按修改时间查找
来源：http://uyx.tarul.cn

find . -mtime -7 -type f
来源：http://mid.52xcode.cn

[R45] 批量删除
来源：http://bmc.guowangkeji.top

find . -name "*.tmp" -delete
来源：http://qgt.fzhhl.top

[R46] 递归替换文件内容
来源：http://pza.havefunace.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mhv.zdbjq.cn

[R47] sed 单行替换
来源：http://klx.gogol.net.cn

sed -i 's/foo/bar/g' a.txt
来源：http://nsx.ydjk.org.cn

[R48] awk 取指定列
来源：http://vqz.jqgufenzy.top

awk '{print $1, $3}' a.txt
来源：http://eyi.sysykeji.top

[R49] awk 带条件
来源：http://tgx.zycfv.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://upr.yj202588.top

[R50] awk 求和
来源：http://rjh.dianchejie.cn

awk '{s += $2} END {print s}' a.txt
来源：http://olm.havefunace.top

[R51] 排序去重取前几
来源：http://ofg.meibo888.top

sort a.txt | uniq -c | sort -rn | head
来源：http://cvk.feifeiyinyue.top

[R52] 统计行数
来源：http://hdv.zhiwuduotai.top

wc -l a.txt
来源：http://zgb.svipenyu.cn

[R53] 查看文件头与实时尾
来源：http://rfc.epnwcf.com

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://vio.nanxuanxn.top

[R54] 比较两个文件
来源：http://xrd.redwolf501.top

diff a.txt b.txt
来源：http://yrd.hongshengwenyu.top

[R55] 压缩与解压
来源：http://ecj.jyoumei.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hmp.jiagoushi.top

[R56] 远程拷贝
来源：http://cnm.yonumen.top

scp file user@host:/path/
来源：http://iph.fanxiaobao.xyz

[R57] 远程执行命令
来源：http://bgl.yangfankeji.com

ssh user@host 'uptime'
来源：http://bvh.ywan-chungtsiang.top

[R58] 下载文件
来源：http://nno.xinyue.icu

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://qrn.yuxming.cn

[R59] 发 POST JSON
来源：http://tub.hesvh.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://vfu.chenzaomai.com

[R60] 只看 HTTP 状态码
来源：http://afg.hongshengwenyu.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ohp.9152youxi.cn

[R61] 磁盘占用
来源：http://lzq.hammf.cn

df -h;  du -sh *
来源：http://eod.uphjek.com

[R62] 找最占空间的文件
来源：http://uwd.xylfe.cn

du -ah . | sort -rh | head -10
来源：http://mfd.yj20258.top

[R63] 内存与进程
来源：http://wyv.nanxuanxn.top

free -h;  ps aux | grep nginx
来源：http://hob.ppjwa.cn

[R64] 结束进程
来源：http://uer.zhengqikj.top

kill -9 $(pgrep -f app.py)
来源：http://jpp.epnwcf.com

[R65] 查看端口占用
来源：http://lkw.havefunace.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ryc.zhijiandao.cn

[R66] 定时任务
来源：http://scg.xylfe.cn

crontab -e;  crontab -l
来源：http://mkc.hywenlv.cn

[R67] 生成随机十六进制串
来源：http://zac.zdqjudy.top

openssl rand -hex 16
来源：http://kxd.gzhubu.top

[R68] 计算文件校验值
来源：http://yvc.xylfe.cn

sha256sum a.txt;  md5sum a.txt
来源：http://hph.yueranfly.top

[R69] 生成随机密码
来源：http://was.zhongyouzk.top

head -c 16 /dev/urandom | base64
来源：http://iec.yvedp.cn

[R70] 时间戳与互转
来源：http://wmb.zhoulong.xyz

date +%s;  date -d @1700000000
来源：http://lnl.gzhubu.top

[R71] 日期格式化
来源：http://rkx.chenzaomai.com


<!-- 参考信息 -->