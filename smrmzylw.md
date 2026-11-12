代发 wailian999

SELECT * FROM users WHERE email IS NULL;
来源：http://zpl.sweek.top

[Q22] 排序
来源：http://wzj.vqdsnc.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://pub.zhiwuduotai.top

[Q23] 分页
来源：http://bjd.snrcjt.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://xuo.aibaodan.cn

[Q24] 去重
来源：http://jcd.tanke756.top

SELECT DISTINCT city FROM users;
来源：http://kao.yanxiufei.cn

[Q25] 只取前 N 条
来源：http://cys.haohaochexian.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://vwf.tanke756.top

[Q26] 计数
来源：http://srd.jqgfzy.top

SELECT COUNT(*) FROM users;
来源：http://dqw.fktsv.cn

[Q27] 条件计数
来源：http://qtl.yuanzhike.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://gte.yfazqb.com

[Q28] 求和与平均
来源：http://wcf.cqqwz.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ahq.zdqjudy.top

[Q29] 最大最小值
来源：http://ong.ydjk.org.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://qgg.pengpengdd.cyou

[Q30] 分组统计
来源：http://dzb.xziqi.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://yni.gotoacloud.top

[Q31] 分组后过滤
来源：http://fiy.nwbrower.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://plw.fehbvm.com

[Q32] 分组拼接字符串
来源：http://mir.yfazqb.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://igq.fengsongda.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://qfn.gzhubu.top

[Q33] 多列分组
来源：http://asq.uphjek.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://dyh.jyoumei.cn

[Q34] 每组取第一条
来源：http://lpu.vqdsnc.cn

SELECT * FROM (
来源：http://gpi.shanyushiyangtech.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://xzm.hfpthk.cn

) t WHERE rn = 1;
来源：http://ffq.cashguo.top

[Q35] 内连接
来源：http://cin.hnxiangtu.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wit.dianchejie.cn

[Q36] 左连接
来源：http://vkm.iojbl.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://pzo.hammf.cn

[Q37] 右连接
来源：http://tii.yj202588.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://bdd.chenlongwang.top

[Q38] 全外连接（PostgreSQL）
来源：http://dky.haohaochexian.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://sca.daria6918.cn

[Q39] 自连接（查上下级）
来源：http://imj.hnxiangtu.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://rbu.ehwqpu.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hmc.yanxiufei.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://zlv.zhijiandao.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://brk.ppjwa.cn

[Q41] 多表连接
来源：http://eyl.xinyue.icu

SELECT o.id, u.name, p.title FROM orders o
来源：http://tdt.hcnkem.com

JOIN users u ON u.id = o.user_id
来源：http://jwe.zhiwuduotai.top

JOIN products p ON p.id = o.product_id;
来源：http://isj.daria6918.cn

[Q42] 连接条件附加过滤
来源：http://xqm.mhx1999.top

SELECT u.name, o.amount FROM users u
来源：http://ngu.ehwqpu.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://lza.ppjwa.cn

[Q43] 标量子查询
来源：http://oci.c1oappe.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://cjz.zhijiandao.cn

[Q44] IN 子查询
来源：http://tve.kuanghao11.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://dcs.gotoacloud.top

[Q45] EXISTS 判断存在
来源：http://jcb.quarkkingdee.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kox.tian-w.cn

[Q46] NOT EXISTS 判断不存在
来源：http://tkk.52xcode.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rtx.jinyuanbaomall.cn

[Q47] 与平均值比较
来源：http://nto.ywan-chungtsiang.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://cjf.andypj.xyz

[Q48] CTE 公用表表达式
来源：http://yqv.yvedp.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://zbb.hfpthk.cn

SELECT * FROM t WHERE c > 5;
来源：http://jxq.wangshuangyany.cn

[Q49] 更新单行
来源：http://olp.guowangkeji.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://psc.jyoumei.cn

[Q50] 批量更新
来源：http://uee.birdmap.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://nza.tarul.cn

[Q51] 用子查询更新
来源：http://rui.hongshengwenyu.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wtt.epnwcf.com

[Q52] 删除指定行
来源：http://geg.0kj1m.cn

DELETE FROM users WHERE id = 10;
来源：http://owd.zhiwuduotai.top

[Q53] 按条件删除
来源：http://srz.pengpengdd.cyou

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://odj.cucudq.cn

[Q54] 清空表
来源：http://tvl.0kj1m.cn

TRUNCATE TABLE logs;
来源：http://hgq.hnxiangtu.top

[Q55] 排名（并列占位）
来源：http://zyu.9152youxi.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://tyk.316326.xyz

[Q56] 密集排名（并列不占位）
来源：http://bva.tianlin.xyz

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://xbf.xuanzx.com

[Q57] 行号
来源：http://wkh.xuetiantiany.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://jhr.yuxming.cn

[Q58] 累计求和
来源：http://xvp.dianchejie.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://htq.guannengcc.top

[Q59] 分组内累计
来源：http://ifp.wangdashe.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://yao.iojbl.cn

[Q60] 取上一行 / 下一行
来源：http://enb.tanke756.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://rfn.shanyushiyangtech.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://zpp.wangshuangyany.cn

[Q61] 移动平均
来源：http://prm.cashguo.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://iwp.yuxming.cn

[Q62] 分组占比
来源：http://jwe.52xcode.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://dqf.feifeiyinyue.top

[Q63] 开启事务
来源：http://gqi.c1oappe.top

START TRANSACTION;                -- 或 BEGIN
来源：http://vvk.52xcode.cn

[Q64] 提交事务
来源：http://dbx.ydjk.org.cn

COMMIT;
来源：http://idf.zhiwuduotai.top

[Q65] 回滚事务
来源：http://hdx.9152youxi.cn

ROLLBACK;
来源：http://lsp.316326.xyz

[Q66] 行锁查询
来源：http://mdp.gogol.net.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hpd.ydjk.org.cn

[Q67] 设置隔离级别
来源：http://blo.yonumen.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://kac.jinqigufen.top

[Q68] 保存点
来源：http://mkk.zhoulong.xyz

SAVEPOINT sp1;
来源：http://lnj.bjfxy.top

ROLLBACK TO sp1;
来源：http://lpo.zdbjq.cn

[Q69] 查看执行计划
来源：http://yjs.cdnleiting.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://umu.sufxvd.cn

[Q70] 更新统计信息
来源：http://kpo.c1oappe.top

ANALYZE TABLE users;
来源：http://xpp.tianlin.xyz

[Q71] 查看建表语句
来源：http://qgt.zhiwuduotai.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wke.hywenlv.cn

[Q72] 查看索引
来源：http://jcn.pengpengdd.cyou

SHOW INDEX FROM users;
来源：http://kak.quarkkingdee.top

[Q73] 查看表状态
来源：http://bts.hfpthk.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://kgd.0kj1m.cn

[Q74] 强制使用索引
来源：http://jsj.vehdjk.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://pkv.jqgufenzy.top

[Q75] 日期格式化
来源：http://ezz.0kj1m.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wlw.xinyue.icu

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://zey.jlsjyb.cn

[Q76] 按天统计
来源：http://mrb.316326.xyz

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://oes.yvedp.cn

[Q77] 时间加减
来源：http://ihl.redwolf501.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blj.cheryme.top

[Q78] 当前时间
来源：http://mkd.guowangkeji.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://atv.daria6918.cn

[Q79] 字符串拼接
来源：http://dwx.hongshengwenyu.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://gtx.xuetiantiany.cn

[Q80] 字符串截取
来源：http://fkk.sufxvd.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://atq.quarkkingdee.top

[Q81] 字符串替换
来源：http://kuc.fengsongda.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://xjg.hcnkem.com

[Q82] 字符长度与字节长度
来源：http://zdn.0kj1m.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ytv.yanxiufei.cn

[Q83] 大小写转换
来源：http://lur.shuidangran.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://rdz.pycfn.com

[Q84] 去除首尾空格
来源：http://vxx.yj202588.top

SELECT TRIM(name) FROM users;
来源：http://ijb.tianlin.xyz

[Q85] 数值取整
来源：http://mdk.jinqigfzy.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://yrg.pengpengdd.cyou

[Q86] 读取 JSON 字段
来源：http://paw.wangdashe.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://iuc.hysaishi.cn

[Q87] JSON 字段做条件
来源：http://sdx.aibaodan.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://qla.vqdsnc.cn

[Q88] 行转列（条件聚合）
来源：http://jrs.tianlin.xyz

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mjd.yj20258888.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wcn.daxiang520.top

[Q89] 判断表是否存在
来源：http://auc.chenlongwang.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://uqt.gaohongyu789.top

[Q90] 生成序号列
来源：http://puj.zhengqikj.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mbo.jiagoushi.top

================================================================================
来源：http://agj.zhijiandao.cn

R. Bash 专题
来源：http://hmz.zhongyouzk.top

================================================================================
来源：http://bzh.sjlbkw.cn

[R01] shebang 与严格模式
来源：http://ghu.hammf.cn

#!/usr/bin/env bash
来源：http://tng.sweek.top

set -euo pipefail
来源：http://njt.chenzaomai.com

[R02] 变量赋值与使用
来源：http://zlp.fanxiaobao.xyz

name="Tom"; echo "$name"
来源：http://apk.yongpay.top

[R03] 只读变量
来源：http://pwl.gzhubu.top

readonly PI=3.14
来源：http://tlc.xinyue.icu

[R04] 位置参数
来源：http://doi.andypj.xyz

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://gel.jinghuilouyu.cn

[R05] 参数默认值
来源：http://hsa.zhixingplan.top

name="${1:-default}"
来源：http://nff.wangdashe.top

[R06] 判断命令是否存在
来源：http://ohx.bjfxy.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://oxa.ivvv.top

[R07] if 判断文件
来源：http://ban.mhx1999.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://xbx.andypj.xyz

[R08] 数值比较
来源：http://ixd.hcnkem.com

if (( a > b )); then echo "a 更大"; fi
来源：http://umg.jiagoushi.top

[R09] 字符串比较
来源：http://pbj.hongshengwenyu.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://cea.dashuyun.cn

[R10] 正则匹配
来源：http://bfz.hnxiangtu.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://cbz.yueranfly.top

[R11] case 多分支
来源：http://coe.hnqzz.top

case "$1" in
来源：http://dxn.9152youxi.cn

start) echo "启动" ;;
来源：http://zuq.yuanzhike.top

stop)  echo "停止" ;;
来源：http://sqp.gaohongyu789.top

*)     echo "未知命令" ;;
来源：http://yct.jinqigufen.top

esac
来源：http://oqp.sjlbkw.cn

[R12] for 遍历文件
来源：http://jrq.cashguo.top

for f in *.txt; do echo "$f"; done
来源：http://ucf.gaohongyu789.top

[R13] for 计数循环
来源：http://qdt.xuetiantiany.cn

for i in {1..10}; do echo "$i"; done
来源：http://gxz.zhiwuduotai.top

[R14] C 风格 for
来源：http://rtq.tianlin.xyz

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://xei.hywenlv.cn

[R15] while 逐行读文件
来源：http://rep.ybcxt.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://aze.cucudq.cn

[R16] until 等待条件
来源：http://nbr.cashguo.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://yjl.haohaochexian.top

[R17] 数组定义与取值
来源：http://kul.hcnkem.com

arr=(a b c); echo "${arr[0]}"
来源：http://uui.xuetiantiany.cn

[R18] 遍历数组
来源：http://pzf.shanyushiyangkeji.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wdx.jqgufenzy.top

[R19] 数组长度
来源：http://tlz.dianchejie.cn

echo "${#arr[@]}"
来源：http://sjz.guannengcc.top

[R20] 关联数组（字典）
来源：http://yek.fengsongda.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mqg.dianchejie.cn

[R21] 字符串长度
来源：http://hdi.zhaomingkeji.xyz

echo "${#s}"
来源：http://lad.tarul.cn

[R22] 截取子串
来源：http://jnx.shuidangran.top

echo "${s:0:5}"
来源：http://heh.fanxiaobao.xyz

[R23] 字符串替换
来源：http://qeg.jinqigufen.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://zgq.jqgufenzy.top

[R24] 大小写转换
来源：http://pub.jyoumei.cn

echo "${s^^}"; echo "${s,,}"
来源：http://oau.sxryk.cn

[R25] 去后缀 / 去前缀
来源：http://qiy.ywan-chungtsiang.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://bkk.yonumen.top

[R26] 命令替换
来源：http://lpn.yj20258.top

now=$(date +%F); echo "$now"
来源：http://lnc.cashguo.top

[R27] 算术展开
来源：http://vlf.haohaochexian.top

echo $((1 + 2 * 3))
来源：http://ojk.xziqi.cn

[R28] 浮点运算
来源：http://dsz.daxiang520.top

echo "scale=2; 10/3" | bc
来源：http://ivd.uphjek.com

[R29] 定义函数
来源：http://ahc.cheryme.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://djt.redwolf501.top

[R30] 函数返回状态码
来源：http://vva.shanyushiyangkeji.top

f() { return 0; }; f || echo "失败了"
来源：http://dog.hysaishi.cn

[R31] 局部变量
来源：http://mat.bjfxy.top

f() { local x=1; echo "$x"; }
来源：http://rmd.ctjpmb.com

[R32] 参数个数校验
来源：http://oin.xinyue.icu

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://lxf.hfpthk.cn

[R33] 捕获错误并提示行号
来源：http://aai.zdbjq.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://gre.feifeiyinyue.top

[R34] 退出时清理
来源：http://xkt.meibo888.top

trap 'rm -f "$tmp"' EXIT
来源：http://nov.vehdjk.com

[R35] 后台执行并等待
来源：http://bgs.hongshengwenyu.top

sleep 5 & pid=$!; wait "$pid"
来源：http://dod.sufxvd.cn

[R36] 并发执行多个任务
来源：http://cfa.jqgufenzy.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ias.fehbvm.com

[R37] 把输出赋给变量
来源：http://bet.gotoacloud.top

files=$(ls -1)
来源：http://oft.xinyue.icu

[R38] 管道串联
来源：http://dxg.iojbl.cn

cat a.txt | grep -i error | wc -l
来源：http://ngt.vehdjk.com

[R39] 重定向标准输出与错误
来源：http://aru.yj20258888.top

cmd > out.log 2>&1
来源：http://tjd.hammf.cn

[R40] 追加写日志
来源：http://anj.fanxiaobao.xyz

echo "log" >> out.log
来源：http://tum.hywenlv.cn

[R41] 丢弃输出
来源：http://mgc.gotoacloud.top

cmd >/dev/null 2>&1
来源：http://tdj.cqqwz.cn

[R42] 输入重定向
来源：http://tvl.iojbl.cn

wc -l < a.txt
来源：http://rfj.vehdjk.com

[R43] 按名字查找文件
来源：http://ejq.jyoumei.cn

find . -name "*.log" -type f
来源：http://llk.fzhhl.top

[R44] 按修改时间查找
来源：http://ply.epnwcf.com

find . -mtime -7 -type f
来源：http://cua.cqqwz.cn

[R45] 批量删除
来源：http://lps.hywenlv.cn

find . -name "*.tmp" -delete
来源：http://knp.tarul.cn

[R46] 递归替换文件内容
来源：http://lld.tian-w.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://uqs.birdmap.top

[R47] sed 单行替换
来源：http://coq.hywenlv.cn

sed -i 's/foo/bar/g' a.txt
来源：http://gaa.iojbl.cn

[R48] awk 取指定列
来源：http://hps.hnxiangtu.top

awk '{print $1, $3}' a.txt
来源：http://nnp.jyoumei.cn

[R49] awk 带条件
来源：http://csg.ydzc1.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://imu.zhoulong.xyz

[R50] awk 求和
来源：http://svb.andypj.xyz

awk '{s += $2} END {print s}' a.txt
来源：http://blj.hnxiangtu.top

[R51] 排序去重取前几
来源：http://qyy.hywenlv.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://tis.zdqjudy.top

[R52] 统计行数
来源：http://gja.yj20258888.top

wc -l a.txt
来源：http://rpr.hfpthk.cn

[R53] 查看文件头与实时尾
来源：http://dhq.ppjwa.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://spp.sysykeji.top

[R54] 比较两个文件
来源：http://pvc.tian-w.cn

diff a.txt b.txt
来源：http://zax.quarkkingdee.top

[R55] 压缩与解压
来源：http://vuv.zhiwuduotai.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://cvu.ctjpmb.com

[R56] 远程拷贝
来源：http://toi.fzhhl.top

scp file user@host:/path/
来源：http://jsh.redwolf501.top

[R57] 远程执行命令
来源：http://zel.yvedp.cn

ssh user@host 'uptime'
来源：http://iyp.feifeiyinyue.top

[R58] 下载文件
来源：http://toi.hysaishi.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://zxx.ydjk.org.cn

[R59] 发 POST JSON
来源：http://xyw.yuanzhike.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://jnz.yongpay.top

[R60] 只看 HTTP 状态码
来源：http://umt.xinyue.icu

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hxd.fktsv.cn

[R61] 磁盘占用
来源：http://jvq.hnxiangtu.top

df -h;  du -sh *
来源：http://fzz.hywenlv.cn

[R62] 找最占空间的文件
来源：http://ogo.9152youxi.cn

du -ah . | sort -rh | head -10
来源：http://mav.pengpengdd.cyou

[R63] 内存与进程
来源：http://dnd.uphjek.com

free -h;  ps aux | grep nginx
来源：http://tzs.jianghu66.top

[R64] 结束进程
来源：http://ftd.ydjk.org.cn

kill -9 $(pgrep -f app.py)
来源：http://gbc.ppjwa.cn

[R65] 查看端口占用
来源：http://khy.xziqi.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wiw.ydzc1.top

[R66] 定时任务
来源：http://uvz.daxiang520.top

crontab -e;  crontab -l
来源：http://jzm.0kj1m.cn

[R67] 生成随机十六进制串
来源：http://ztw.bbcook.cn

openssl rand -hex 16
来源：http://edu.guowangkeji.top

[R68] 计算文件校验值
来源：http://lww.kuanghao11.cn

sha256sum a.txt;  md5sum a.txt
来源：http://kwm.hammf.cn

[R69] 生成随机密码
来源：http://owj.jinghuilouyu.cn

head -c 16 /dev/urandom | base64
来源：http://jyy.yvedp.cn

[R70] 时间戳与互转
来源：http://cxt.tian-w.cn

date +%s;  date -d @1700000000
来源：http://fha.epnwcf.com

[R71] 日期格式化
来源：http://xuu.redwolf501.top


<!-- 参考信息 -->