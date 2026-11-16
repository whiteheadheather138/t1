代发 wailian999

SELECT * FROM users WHERE email IS NULL;
来源：http://ypp.hcnkem.com

[Q22] 排序
来源：http://pot.dashuyun.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://qlp.tanke756.top

[Q23] 分页
来源：http://pqf.epnwcf.com

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://uuy.pycfn.com

[Q24] 去重
来源：http://wto.fzhhl.top

SELECT DISTINCT city FROM users;
来源：http://ahz.epnwcf.com

[Q25] 只取前 N 条
来源：http://xfz.quarkkingdee.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://tny.ybcxt.top

[Q26] 计数
来源：http://ctl.jinghuilouyu.cn

SELECT COUNT(*) FROM users;
来源：http://jvq.jinqigufen.top

[Q27] 条件计数
来源：http://xtw.xingfuxueyuan.xyz

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://aat.kuanghao11.cn

[Q28] 求和与平均
来源：http://jbx.meibo888.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://lrm.feifeiyinyue.top

[Q29] 最大最小值
来源：http://yzx.jqgfzy.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://olx.chenjidiqi.icu

[Q30] 分组统计
来源：http://yrm.yangfankeji.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://kbs.shanyushiyangtech.top

[Q31] 分组后过滤
来源：http://vpk.ivvv.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ikn.gaohongyu789.top

[Q32] 分组拼接字符串
来源：http://vxh.sufxvd.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://min.nanxuanxn.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://vds.zhongyouzk.top

[Q33] 多列分组
来源：http://xrq.yonumen.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://cpd.ydzc1.top

[Q34] 每组取第一条
来源：http://bma.jinqigufen.top

SELECT * FROM (
来源：http://kxr.ywan-chungtsiang.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ztp.ywan-chungtsiang.top

) t WHERE rn = 1;
来源：http://pza.yangfankeji.com

[Q35] 内连接
来源：http://pjz.zhoulong.xyz

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ktb.zhiwuduotai.top

[Q36] 左连接
来源：http://yxs.wangdashe.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://bdi.zhaomingkeji.xyz

[Q37] 右连接
来源：http://mpx.kuanghao11.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://nla.ehwqpu.com

[Q38] 全外连接（PostgreSQL）
来源：http://xcj.tanke756.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://sii.9152youxi.cn

[Q39] 自连接（查上下级）
来源：http://oiy.zhengqikj.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://fkb.pengpengdd.cyou

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://uyn.chenzaomai.com

[Q40] 交叉连接（笛卡尔积）
来源：http://ddp.sweek.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://boh.gogol.net.cn

[Q41] 多表连接
来源：http://zon.tianlin.xyz

SELECT o.id, u.name, p.title FROM orders o
来源：http://uxl.fktsv.cn

JOIN users u ON u.id = o.user_id
来源：http://gyk.hnqzz.top

JOIN products p ON p.id = o.product_id;
来源：http://cuv.52xcode.cn

[Q42] 连接条件附加过滤
来源：http://kst.aibaodan.cn

SELECT u.name, o.amount FROM users u
来源：http://vji.haohaochexian.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://pwx.guannengcc.top

[Q43] 标量子查询
来源：http://fci.zhixingplan.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://xat.fzhhl.top

[Q44] IN 子查询
来源：http://peb.quarkkingdee.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://fpk.jqgfzy.top

[Q45] EXISTS 判断存在
来源：http://rpo.yvedp.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://goe.vqdsnc.cn

[Q46] NOT EXISTS 判断不存在
来源：http://uqi.yuanzhike.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://lau.yj20258888.top

[Q47] 与平均值比较
来源：http://ipq.hongshengwenyu.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://xjd.jlsjyb.cn

[Q48] CTE 公用表表达式
来源：http://jvc.jqgufenzy.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ueq.xinyue.icu

SELECT * FROM t WHERE c > 5;
来源：http://ykm.hysaishi.cn

[Q49] 更新单行
来源：http://qfw.svipenyu.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://dhq.xziqi.cn

[Q50] 批量更新
来源：http://wfj.jianghu66.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://rht.gogol.net.cn

[Q51] 用子查询更新
来源：http://klf.c1oappe.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://aya.sjlbkw.cn

[Q52] 删除指定行
来源：http://hax.snrcjt.cn

DELETE FROM users WHERE id = 10;
来源：http://ldk.ydzc1.top

[Q53] 按条件删除
来源：http://mag.fanxiaobao.xyz

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://avt.havefunace.top

[Q54] 清空表
来源：http://xht.cucudq.cn

TRUNCATE TABLE logs;
来源：http://lnc.chenlongwang.top

[Q55] 排名（并列占位）
来源：http://pvt.gotoacloud.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://jcu.gotoacloud.top

[Q56] 密集排名（并列不占位）
来源：http://rqi.yj202588.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://xfy.tianlin.xyz

[Q57] 行号
来源：http://gnc.kuanghao11.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://qzq.sysykeji.top

[Q58] 累计求和
来源：http://jsz.c1oappe.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://xqr.jinqigfzy.top

[Q59] 分组内累计
来源：http://rdd.cqqwz.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://qpn.jiagoushi.top

[Q60] 取上一行 / 下一行
来源：http://jap.yfazqb.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://nve.fengsongda.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://nuz.tian-w.cn

[Q61] 移动平均
来源：http://jmt.xinyue.icu

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ldb.ivvv.top

[Q62] 分组占比
来源：http://bxg.jianghu66.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://dvw.fzhhl.top

[Q63] 开启事务
来源：http://ncv.jianghu66.top

START TRANSACTION;                -- 或 BEGIN
来源：http://dyu.gotoacloud.top

[Q64] 提交事务
来源：http://boj.ybcxt.top

COMMIT;
来源：http://moa.yj20258.top

[Q65] 回滚事务
来源：http://fel.haohaochexian.top

ROLLBACK;
来源：http://wvu.zhijiandao.cn

[Q66] 行锁查询
来源：http://dyp.quarkkingdee.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://qjm.tarul.cn

[Q67] 设置隔离级别
来源：http://hvz.zhengqikj.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ytz.feifeiyinyue.top

[Q68] 保存点
来源：http://mwj.bbcook.cn

SAVEPOINT sp1;
来源：http://yro.jinqigfzy.top

ROLLBACK TO sp1;
来源：http://slg.bbcook.cn

[Q69] 查看执行计划
来源：http://sne.tanke756.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://jjv.daxiang520.top

[Q70] 更新统计信息
来源：http://mvd.jyoumei.cn

ANALYZE TABLE users;
来源：http://erm.aizwys.cn

[Q71] 查看建表语句
来源：http://hyp.jyoumei.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://tws.cucudq.cn

[Q72] 查看索引
来源：http://pcv.bbcook.cn

SHOW INDEX FROM users;
来源：http://zis.zhijiandao.cn

[Q73] 查看表状态
来源：http://ryq.sweek.top

SHOW TABLE STATUS LIKE 'users';
来源：http://tzi.xuanzx.com

[Q74] 强制使用索引
来源：http://aea.hnxiangtu.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://tuj.vqdsnc.cn

[Q75] 日期格式化
来源：http://cxk.tanke756.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://gpp.ywan-chungtsiang.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://xaj.nanxinkj.top

[Q76] 按天统计
来源：http://lwa.zycfv.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ijj.yangfankeji.com

[Q77] 时间加减
来源：http://rti.kuanghao11.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://vwl.smart0.xyz

[Q78] 当前时间
来源：http://pmv.zhixingplan.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://rpk.ydjk.org.cn

[Q79] 字符串拼接
来源：http://dvw.chenjidiqi.icu

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://zyd.shzxlz.cn

[Q80] 字符串截取
来源：http://opn.cashguo.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blf.wangshuangyany.cn

[Q81] 字符串替换
来源：http://ehs.bbcook.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://tyw.fengsongda.top

[Q82] 字符长度与字节长度
来源：http://fhf.jinghuilouyu.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wpf.ppjwa.cn

[Q83] 大小写转换
来源：http://ryv.daria6918.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://zey.tarul.cn

[Q84] 去除首尾空格
来源：http://oig.hesvh.cn

SELECT TRIM(name) FROM users;
来源：http://xte.snrcjt.cn

[Q85] 数值取整
来源：http://ybg.ywan-chungtsiang.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://iwi.gzhubu.top

[Q86] 读取 JSON 字段
来源：http://vwq.jqgfzy.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://fez.yangfankeji.com

[Q87] JSON 字段做条件
来源：http://sgg.ppjwa.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://erc.zhongyouzk.top

[Q88] 行转列（条件聚合）
来源：http://xgy.zycfv.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://xin.snrcjt.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://vkc.gotoacloud.top

[Q89] 判断表是否存在
来源：http://kha.zhixingplan.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://zmq.shangyingyoupin.top

[Q90] 生成序号列
来源：http://bci.ywan-chungtsiang.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://gsz.jinqigfzy.top

================================================================================
来源：http://ixe.chenjidiqi.icu

R. Bash 专题
来源：http://yrw.nanxuanxn.top

================================================================================
来源：http://npn.zdqjudy.top

[R01] shebang 与严格模式
来源：http://uys.pengpengdd.cyou

#!/usr/bin/env bash
来源：http://klu.xylfe.cn

set -euo pipefail
来源：http://jax.epnwcf.com

[R02] 变量赋值与使用
来源：http://emv.ehwqpu.com

name="Tom"; echo "$name"
来源：http://kuz.zhongyouzk.top

[R03] 只读变量
来源：http://umd.hesvh.cn

readonly PI=3.14
来源：http://dsp.jinqigufen.top

[R04] 位置参数
来源：http://wfp.havefunace.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://grx.havefunace.top

[R05] 参数默认值
来源：http://uai.hcnkem.com

name="${1:-default}"
来源：http://baw.ydjk.org.cn

[R06] 判断命令是否存在
来源：http://xsm.zhixingplan.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://esb.tarul.cn

[R07] if 判断文件
来源：http://bdv.tarul.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://qje.fanxiaobao.xyz

[R08] 数值比较
来源：http://ujp.fzhhl.top

if (( a > b )); then echo "a 更大"; fi
来源：http://csx.ctjpmb.com

[R09] 字符串比较
来源：http://gww.zycfv.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://vjn.sjlbkw.cn

[R10] 正则匹配
来源：http://wvj.9152youxi.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://gzl.andypj.xyz

[R11] case 多分支
来源：http://cvw.zhaomingkeji.xyz

case "$1" in
来源：http://esk.xingfuxueyuan.xyz

start) echo "启动" ;;
来源：http://kor.xingfuxueyuan.xyz

stop)  echo "停止" ;;
来源：http://fsd.wangdashe.top

*)     echo "未知命令" ;;
来源：http://kgp.ehwqpu.com

esac
来源：http://tbs.yuanzhike.top

[R12] for 遍历文件
来源：http://vpq.guannengcc.top

for f in *.txt; do echo "$f"; done
来源：http://bcp.svipenyu.cn

[R13] for 计数循环
来源：http://tto.daxiang520.top

for i in {1..10}; do echo "$i"; done
来源：http://ngs.aibaodan.cn

[R14] C 风格 for
来源：http://upp.fehbvm.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://sgu.zhengqikj.top

[R15] while 逐行读文件
来源：http://vba.cqqwz.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://olo.yanxiufei.cn

[R16] until 等待条件
来源：http://jpo.jianghu66.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://bgc.shuidangran.top

[R17] 数组定义与取值
来源：http://iyc.shanyushiyangtech.top

arr=(a b c); echo "${arr[0]}"
来源：http://akg.mhx1999.top

[R18] 遍历数组
来源：http://cux.cqqwz.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wmh.chenzaomai.com

[R19] 数组长度
来源：http://dqn.bjfxy.top

echo "${#arr[@]}"
来源：http://buv.snrcjt.cn

[R20] 关联数组（字典）
来源：http://mya.bjfxy.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://aak.dianchejie.cn

[R21] 字符串长度
来源：http://hds.tanke756.top

echo "${#s}"
来源：http://asd.vqdsnc.cn

[R22] 截取子串
来源：http://ekn.aizwys.cn

echo "${s:0:5}"
来源：http://dfg.xinyue.icu

[R23] 字符串替换
来源：http://lbu.pengpengdd.cyou

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://azd.andypj.xyz

[R24] 大小写转换
来源：http://qcy.cucudq.cn

echo "${s^^}"; echo "${s,,}"
来源：http://aro.yongpay.top

[R25] 去后缀 / 去前缀
来源：http://nao.ehwqpu.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://hjl.yfazqb.com

[R26] 命令替换
来源：http://llf.ivvv.top

now=$(date +%F); echo "$now"
来源：http://cgz.cdnleiting.top

[R27] 算术展开
来源：http://kbk.c1oappe.top

echo $((1 + 2 * 3))
来源：http://wzz.yj202588.top

[R28] 浮点运算
来源：http://jij.redwolf501.top

echo "scale=2; 10/3" | bc
来源：http://iqa.ybcxt.top

[R29] 定义函数
来源：http://szk.iojbl.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://coi.guannengcc.top

[R30] 函数返回状态码
来源：http://ghs.jinghuilouyu.cn

f() { return 0; }; f || echo "失败了"
来源：http://vdb.sweek.top

[R31] 局部变量
来源：http://ghz.vehdjk.com

f() { local x=1; echo "$x"; }
来源：http://kfb.jinghuilouyu.cn

[R32] 参数个数校验
来源：http://kvm.gzhubu.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wti.meibo888.top

[R33] 捕获错误并提示行号
来源：http://buu.shzxlz.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://aqu.yj202588.top

[R34] 退出时清理
来源：http://jhd.redwolf501.top

trap 'rm -f "$tmp"' EXIT
来源：http://yob.hcnkem.com

[R35] 后台执行并等待
来源：http://ukn.cdnleiting.top

sleep 5 & pid=$!; wait "$pid"
来源：http://xnq.mhx1999.top

[R36] 并发执行多个任务
来源：http://bks.cqqwz.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mto.fanxiaobao.xyz

[R37] 把输出赋给变量
来源：http://jru.aibaodan.cn

files=$(ls -1)
来源：http://nug.0kj1m.cn

[R38] 管道串联
来源：http://vbn.xingfuxueyuan.xyz

cat a.txt | grep -i error | wc -l
来源：http://knl.cdnleiting.top

[R39] 重定向标准输出与错误
来源：http://zrd.kuanghao11.cn

cmd > out.log 2>&1
来源：http://trg.kuanghao11.cn

[R40] 追加写日志
来源：http://ita.haohaochexian.top

echo "log" >> out.log
来源：http://lmh.ydzc1.top

[R41] 丢弃输出
来源：http://sza.fehbvm.com

cmd >/dev/null 2>&1
来源：http://gzw.vehdjk.com

[R42] 输入重定向
来源：http://vhl.mhx1999.top

wc -l < a.txt
来源：http://any.daxiang520.top

[R43] 按名字查找文件
来源：http://ota.haohaochexian.top

find . -name "*.log" -type f
来源：http://pgw.yj202588.top

[R44] 按修改时间查找
来源：http://oqf.chenlongwang.top

find . -mtime -7 -type f
来源：http://tal.hesvh.cn

[R45] 批量删除
来源：http://gzl.nanxinkj.top

find . -name "*.tmp" -delete
来源：http://agb.ybcxt.top

[R46] 递归替换文件内容
来源：http://erj.cdnleiting.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://vbd.bjfxy.top

[R47] sed 单行替换
来源：http://upi.shuidangran.top

sed -i 's/foo/bar/g' a.txt
来源：http://qju.yj20258.top

[R48] awk 取指定列
来源：http://tmh.chenlongwang.top

awk '{print $1, $3}' a.txt
来源：http://gmb.zhengqikj.top

[R49] awk 带条件
来源：http://jpk.nanxinkj.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://cwp.sysykeji.top

[R50] awk 求和
来源：http://vzr.yanxiufei.cn

awk '{s += $2} END {print s}' a.txt
来源：http://bhi.hongshengwenyu.top

[R51] 排序去重取前几
来源：http://nmn.pycfn.com

sort a.txt | uniq -c | sort -rn | head
来源：http://eqz.fzhhl.top

[R52] 统计行数
来源：http://oug.smart0.xyz

wc -l a.txt
来源：http://mrw.yj202588.top

[R53] 查看文件头与实时尾
来源：http://gjm.yanxiufei.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://xge.yfazqb.com

[R54] 比较两个文件
来源：http://wmg.yvedp.cn

diff a.txt b.txt
来源：http://yjk.jqgfzy.top

[R55] 压缩与解压
来源：http://eqp.xuanzx.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wfm.daxiang520.top

[R56] 远程拷贝
来源：http://ner.aibaodan.cn

scp file user@host:/path/
来源：http://iem.hcnkem.com

[R57] 远程执行命令
来源：http://lmc.jqgfzy.top

ssh user@host 'uptime'
来源：http://mxg.dashuyun.cn

[R58] 下载文件
来源：http://pdf.dashuyun.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://clk.hnxiangtu.top

[R59] 发 POST JSON
来源：http://zcx.yuxming.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://urw.yj202588.top

[R60] 只看 HTTP 状态码
来源：http://gsa.jiagoushi.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ixw.yuxming.cn

[R61] 磁盘占用
来源：http://rnq.pengpengdd.cyou

df -h;  du -sh *
来源：http://xmd.zdqjudy.top

[R62] 找最占空间的文件
来源：http://tpe.shzxlz.cn

du -ah . | sort -rh | head -10
来源：http://frt.zdqjudy.top

[R63] 内存与进程
来源：http://tdt.yj20258888.top

free -h;  ps aux | grep nginx
来源：http://tgi.cashguo.top

[R64] 结束进程
来源：http://hbu.mhx1999.top

kill -9 $(pgrep -f app.py)
来源：http://tsx.chenlongwang.top

[R65] 查看端口占用
来源：http://sjf.yj202588.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://qmu.yj202588.top

[R66] 定时任务
来源：http://ner.cucudq.cn

crontab -e;  crontab -l
来源：http://our.cucudq.cn

[R67] 生成随机十六进制串
来源：http://pdx.kuanghao11.cn

openssl rand -hex 16
来源：http://xbw.ybcxt.top

[R68] 计算文件校验值
来源：http://tet.c1oappe.top

sha256sum a.txt;  md5sum a.txt
来源：http://kaj.shangyingyoupin.top

[R69] 生成随机密码
来源：http://qvf.zhijiandao.cn

head -c 16 /dev/urandom | base64
来源：http://pxr.jlsjyb.cn

[R70] 时间戳与互转
来源：http://nqy.ydzc1.top

date +%s;  date -d @1700000000
来源：http://jpd.fktsv.cn

[R71] 日期格式化
来源：http://qsj.havefunace.top


<!-- 参考信息 -->