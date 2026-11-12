代发 wailian999

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://rrr.chenzaomai.com

[Q24] 去重
来源：http://ijz.shanyushiyangkeji.top

SELECT DISTINCT city FROM users;
来源：http://dqu.sufxvd.cn

[Q25] 只取前 N 条
来源：http://knb.zhengqikj.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://rub.yueranfly.top

[Q26] 计数
来源：http://wzp.ybcxt.top

SELECT COUNT(*) FROM users;
来源：http://tnw.fktsv.cn

[Q27] 条件计数
来源：http://qzh.zhijiandao.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://irh.xinyue.icu

[Q28] 求和与平均
来源：http://ppr.smart0.xyz

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://vlb.fktsv.cn

[Q29] 最大最小值
来源：http://qcf.zhixingplan.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://ykl.yanxiufei.cn

[Q30] 分组统计
来源：http://tad.0kj1m.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://dhg.zdbjq.cn

[Q31] 分组后过滤
来源：http://mrr.nanxuanxn.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://kkd.yonumen.top

[Q32] 分组拼接字符串
来源：http://yfp.ydzc1.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://lkd.ydzc1.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://gph.hcnkem.com

[Q33] 多列分组
来源：http://lqj.gotoacloud.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hmd.xziqi.cn

[Q34] 每组取第一条
来源：http://phd.hnqzz.top

SELECT * FROM (
来源：http://qic.guowangkeji.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://xqs.zycfv.cn

) t WHERE rn = 1;
来源：http://uog.xuetiantiany.cn

[Q35] 内连接
来源：http://xjw.c1oappe.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://afi.sjlbkw.cn

[Q36] 左连接
来源：http://ybd.cheryme.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://yvk.yonumen.top

[Q37] 右连接
来源：http://wqg.yuxming.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hvv.hnqzz.top

[Q38] 全外连接（PostgreSQL）
来源：http://mtp.pengpengdd.cyou

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://jcx.bjfxy.top

[Q39] 自连接（查上下级）
来源：http://ika.zhixingplan.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://xoc.meibo888.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mzy.jinqigfzy.top

[Q40] 交叉连接（笛卡尔积）
来源：http://coe.bjfxy.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://edv.jyoumei.cn

[Q41] 多表连接
来源：http://zme.fktsv.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ojl.xylfe.cn

JOIN users u ON u.id = o.user_id
来源：http://fdh.sweek.top

JOIN products p ON p.id = o.product_id;
来源：http://uof.zycfv.cn

[Q42] 连接条件附加过滤
来源：http://aua.yj20258.top

SELECT u.name, o.amount FROM users u
来源：http://hcv.zycfv.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://now.hcnkem.com

[Q43] 标量子查询
来源：http://rhd.gotoacloud.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://seb.jinqigufen.top

[Q44] IN 子查询
来源：http://ruf.sysykeji.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://obh.xuanzx.com

[Q45] EXISTS 判断存在
来源：http://dke.hysaishi.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zpk.redwolf501.top

[Q46] NOT EXISTS 判断不存在
来源：http://jez.sufxvd.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hyy.nwbrower.top

[Q47] 与平均值比较
来源：http://gug.jinghuilouyu.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://qnk.aibaodan.cn

[Q48] CTE 公用表表达式
来源：http://ydq.chenzaomai.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://rkq.iojbl.cn

SELECT * FROM t WHERE c > 5;
来源：http://ngt.316326.xyz

[Q49] 更新单行
来源：http://unc.aibaodan.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://uzr.yj20258.top

[Q50] 批量更新
来源：http://vzd.jinyuanbaomall.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://iwt.sufxvd.cn

[Q51] 用子查询更新
来源：http://pgz.pycfn.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://fyq.zhiwuduotai.top

[Q52] 删除指定行
来源：http://cep.mhx1999.top

DELETE FROM users WHERE id = 10;
来源：http://dho.zhijiandao.cn

[Q53] 按条件删除
来源：http://xfi.jinyuanbaomall.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://atg.hfpthk.cn

[Q54] 清空表
来源：http://aqm.fzhhl.top

TRUNCATE TABLE logs;
来源：http://bix.bbcook.cn

[Q55] 排名（并列占位）
来源：http://dac.yj20258888.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://aro.sjlbkw.cn

[Q56] 密集排名（并列不占位）
来源：http://fqh.hesvh.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wwg.hywenlv.cn

[Q57] 行号
来源：http://rvc.cheryme.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hdc.hesvh.cn

[Q58] 累计求和
来源：http://axy.zhongyouzk.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://pcv.zhengqikj.top

[Q59] 分组内累计
来源：http://zdk.52xcode.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://akt.quarkkingdee.top

[Q60] 取上一行 / 下一行
来源：http://bkx.cheryme.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://sfz.fengsongda.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ral.cqqwz.cn

[Q61] 移动平均
来源：http://paw.jianghu66.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://jdk.shangyingyoupin.top

[Q62] 分组占比
来源：http://azs.fengsongda.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mli.zhoulong.xyz

[Q63] 开启事务
来源：http://blw.svipenyu.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://hfv.yj202588.top

[Q64] 提交事务
来源：http://qps.kuanghao11.cn

COMMIT;
来源：http://gcs.vehdjk.com

[Q65] 回滚事务
来源：http://dqo.0kj1m.cn

ROLLBACK;
来源：http://zbv.jianghu66.top

[Q66] 行锁查询
来源：http://uyu.fzhhl.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ddo.pycfn.com

[Q67] 设置隔离级别
来源：http://uvl.316326.xyz

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://fsm.pengpengdd.cyou

[Q68] 保存点
来源：http://vff.yuanzhike.top

SAVEPOINT sp1;
来源：http://qjw.pycfn.com

ROLLBACK TO sp1;
来源：http://hsl.cheryme.top

[Q69] 查看执行计划
来源：http://kzv.meibo888.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://aet.jlsjyb.cn

[Q70] 更新统计信息
来源：http://uvd.cucudq.cn

ANALYZE TABLE users;
来源：http://czh.tanke756.top

[Q71] 查看建表语句
来源：http://rjg.hywenlv.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://liq.hnqzz.top

[Q72] 查看索引
来源：http://tey.aizwys.cn

SHOW INDEX FROM users;
来源：http://kwu.yj20258.top

[Q73] 查看表状态
来源：http://mhg.yfazqb.com

SHOW TABLE STATUS LIKE 'users';
来源：http://lcl.shuidangran.top

[Q74] 强制使用索引
来源：http://isl.jinqigufen.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://lov.fzhhl.top

[Q75] 日期格式化
来源：http://lfc.wangdashe.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://rlr.ppjwa.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://veo.guowangkeji.top

[Q76] 按天统计
来源：http://hdx.redwolf501.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://iex.ehwqpu.com

[Q77] 时间加减
来源：http://enk.tanke756.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://amf.nanxuanxn.top

[Q78] 当前时间
来源：http://ovm.xinyue.icu

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://bzb.bbcook.cn

[Q79] 字符串拼接
来源：http://jiu.zhaomingkeji.xyz

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://flr.xziqi.cn

[Q80] 字符串截取
来源：http://nro.fktsv.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://vdx.yonumen.top

[Q81] 字符串替换
来源：http://xxp.pengpengdd.cyou

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mtm.hammf.cn

[Q82] 字符长度与字节长度
来源：http://mro.yonumen.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://nqx.sysykeji.top

[Q83] 大小写转换
来源：http://koz.pengpengdd.cyou

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://yzv.yongpay.top

[Q84] 去除首尾空格
来源：http://ova.uphjek.com

SELECT TRIM(name) FROM users;
来源：http://nko.hongshengwenyu.top

[Q85] 数值取整
来源：http://psd.fanxiaobao.xyz

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://fqg.wangshuangyany.cn

[Q86] 读取 JSON 字段
来源：http://mpn.cheryme.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://jmf.aizwys.cn

[Q87] JSON 字段做条件
来源：http://vok.yuxming.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ltp.hongshengwenyu.top

[Q88] 行转列（条件聚合）
来源：http://ibv.yj20258888.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://qwl.shanyushiyangtech.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ptc.fanxiaobao.xyz

[Q89] 判断表是否存在
来源：http://svh.cqqwz.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://xcn.cheryme.top

[Q90] 生成序号列
来源：http://etf.yj202588.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://iip.feifeiyinyue.top

================================================================================
来源：http://ibt.nanxinkj.top

R. Bash 专题
来源：http://wpy.vqdsnc.cn

================================================================================
来源：http://skz.jlsjyb.cn

[R01] shebang 与严格模式
来源：http://pui.zhijiandao.cn

#!/usr/bin/env bash
来源：http://kif.hysaishi.cn

set -euo pipefail
来源：http://ngo.jyoumei.cn

[R02] 变量赋值与使用
来源：http://qsu.ybcxt.top

name="Tom"; echo "$name"
来源：http://eeo.yanxiufei.cn

[R03] 只读变量
来源：http://smi.guannengcc.top

readonly PI=3.14
来源：http://oeo.nanxuanxn.top

[R04] 位置参数
来源：http://wdf.jianghu66.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mmi.tanke756.top

[R05] 参数默认值
来源：http://bxp.hesvh.cn

name="${1:-default}"
来源：http://ogw.gaohongyu789.top

[R06] 判断命令是否存在
来源：http://eyh.sjlbkw.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://lac.shanyushiyangkeji.top

[R07] if 判断文件
来源：http://tdi.yuxming.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://xab.ehwqpu.com

[R08] 数值比较
来源：http://tfd.316326.xyz

if (( a > b )); then echo "a 更大"; fi
来源：http://vok.xylfe.cn

[R09] 字符串比较
来源：http://cjh.gaohongyu789.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://rpx.yj20258.top

[R10] 正则匹配
来源：http://hao.gogol.net.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://tvc.fzhhl.top

[R11] case 多分支
来源：http://gms.vehdjk.com

case "$1" in
来源：http://ket.zhijiandao.cn

start) echo "启动" ;;
来源：http://lda.shanyushiyangkeji.top

stop)  echo "停止" ;;
来源：http://cva.zycfv.cn

*)     echo "未知命令" ;;
来源：http://sey.yueranfly.top

esac
来源：http://qwu.cucudq.cn

[R12] for 遍历文件
来源：http://lby.yfazqb.com

for f in *.txt; do echo "$f"; done
来源：http://suk.sweek.top

[R13] for 计数循环
来源：http://poq.jinqigfzy.top

for i in {1..10}; do echo "$i"; done
来源：http://std.hongshengwenyu.top

[R14] C 风格 for
来源：http://tcn.dianchejie.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://kkz.yanxiufei.cn

[R15] while 逐行读文件
来源：http://ixd.sufxvd.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://lxn.yueranfly.top

[R16] until 等待条件
来源：http://mwu.xingfuxueyuan.xyz

until [[ -f done.flag ]]; do sleep 1; done
来源：http://qjh.yvedp.cn

[R17] 数组定义与取值
来源：http://cnh.nanxinkj.top

arr=(a b c); echo "${arr[0]}"
来源：http://imv.iojbl.cn

[R18] 遍历数组
来源：http://acd.yanxiufei.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://oyx.hnxiangtu.top

[R19] 数组长度
来源：http://nra.yonumen.top

echo "${#arr[@]}"
来源：http://yri.sufxvd.cn

[R20] 关联数组（字典）
来源：http://kze.xuanzx.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://rxd.tianlin.xyz

[R21] 字符串长度
来源：http://flc.haohaochexian.top

echo "${#s}"
来源：http://bys.hywenlv.cn

[R22] 截取子串
来源：http://uiq.gotoacloud.top

echo "${s:0:5}"
来源：http://uvk.fanxiaobao.xyz

[R23] 字符串替换
来源：http://agr.bbcook.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://osi.daria6918.cn

[R24] 大小写转换
来源：http://ule.hnqzz.top

echo "${s^^}"; echo "${s,,}"
来源：http://oel.bjfxy.top

[R25] 去后缀 / 去前缀
来源：http://ctq.vehdjk.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://vnh.sysykeji.top

[R26] 命令替换
来源：http://nzt.ppjwa.cn

now=$(date +%F); echo "$now"
来源：http://tcw.tarul.cn

[R27] 算术展开
来源：http://yjm.hnxiangtu.top

echo $((1 + 2 * 3))
来源：http://izn.yonumen.top

[R28] 浮点运算
来源：http://brq.shangyingyoupin.top

echo "scale=2; 10/3" | bc
来源：http://fia.jqgufenzy.top

[R29] 定义函数
来源：http://uki.zhongyouzk.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://pvr.yongpay.top

[R30] 函数返回状态码
来源：http://ksx.meibo888.top

f() { return 0; }; f || echo "失败了"
来源：http://gxb.zhaomingkeji.xyz

[R31] 局部变量
来源：http://gnz.yongpay.top

f() { local x=1; echo "$x"; }
来源：http://zer.yongpay.top

[R32] 参数个数校验
来源：http://nxi.wangshuangyany.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://cna.ehwqpu.com

[R33] 捕获错误并提示行号
来源：http://sol.iojbl.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://geh.zhixingplan.top

[R34] 退出时清理
来源：http://orq.tianlin.xyz

trap 'rm -f "$tmp"' EXIT
来源：http://zki.quarkkingdee.top

[R35] 后台执行并等待
来源：http://dgz.feifeiyinyue.top

sleep 5 & pid=$!; wait "$pid"
来源：http://pka.xingfuxueyuan.xyz

[R36] 并发执行多个任务
来源：http://xio.zhengqikj.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://qlr.shanyushiyangkeji.top

[R37] 把输出赋给变量
来源：http://mug.sjlbkw.cn

files=$(ls -1)
来源：http://usk.hnxiangtu.top

[R38] 管道串联
来源：http://bey.bbcook.cn

cat a.txt | grep -i error | wc -l
来源：http://fvp.iojbl.cn

[R39] 重定向标准输出与错误
来源：http://kgc.daria6918.cn

cmd > out.log 2>&1
来源：http://gcw.xinyue.icu

[R40] 追加写日志
来源：http://ete.sjlbkw.cn

echo "log" >> out.log
来源：http://gul.zhoulong.xyz

[R41] 丢弃输出
来源：http://feb.sweek.top

cmd >/dev/null 2>&1
来源：http://zif.xinyue.icu

[R42] 输入重定向
来源：http://ovz.jinqigufen.top

wc -l < a.txt
来源：http://gqg.sweek.top

[R43] 按名字查找文件
来源：http://woy.0kj1m.cn

find . -name "*.log" -type f
来源：http://iqd.yanxiufei.cn

[R44] 按修改时间查找
来源：http://leh.shangyingyoupin.top

find . -mtime -7 -type f
来源：http://vau.xinyue.icu

[R45] 批量删除
来源：http://ydd.xuetiantiany.cn

find . -name "*.tmp" -delete
来源：http://knl.zhixingplan.top

[R46] 递归替换文件内容
来源：http://ijk.bjfxy.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wxj.hnqzz.top

[R47] sed 单行替换
来源：http://dil.cashguo.top

sed -i 's/foo/bar/g' a.txt
来源：http://euq.shangyingyoupin.top

[R48] awk 取指定列
来源：http://ugw.jinghuilouyu.cn

awk '{print $1, $3}' a.txt
来源：http://xya.ydjk.org.cn

[R49] awk 带条件
来源：http://xxv.sufxvd.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://gzm.tarul.cn

[R50] awk 求和
来源：http://gnd.daxiang520.top

awk '{s += $2} END {print s}' a.txt
来源：http://gmd.fzhhl.top

[R51] 排序去重取前几
来源：http://dpd.hongshengwenyu.top

sort a.txt | uniq -c | sort -rn | head
来源：http://wag.xuanzx.com

[R52] 统计行数
来源：http://wxi.cheryme.top

wc -l a.txt
来源：http://zwb.ybcxt.top

[R53] 查看文件头与实时尾
来源：http://ero.hnqzz.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ibg.gaohongyu789.top

[R54] 比较两个文件
来源：http://smf.chenlongwang.top

diff a.txt b.txt
来源：http://kjl.cheryme.top

[R55] 压缩与解压
来源：http://ztb.cucudq.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://tvf.quarkkingdee.top

[R56] 远程拷贝
来源：http://egd.cheryme.top

scp file user@host:/path/
来源：http://kwh.guowangkeji.top

[R57] 远程执行命令
来源：http://hqh.jyoumei.cn

ssh user@host 'uptime'
来源：http://sfy.xylfe.cn

[R58] 下载文件
来源：http://kfb.316326.xyz

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://gts.guowangkeji.top

[R59] 发 POST JSON
来源：http://fhu.yj20258888.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://fxg.ppjwa.cn

[R60] 只看 HTTP 状态码
来源：http://iet.zhijiandao.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://piz.zdbjq.cn

[R61] 磁盘占用
来源：http://npa.hammf.cn

df -h;  du -sh *
来源：http://ahj.svipenyu.cn

[R62] 找最占空间的文件
来源：http://xtm.nanxinkj.top

du -ah . | sort -rh | head -10
来源：http://dhr.sufxvd.cn

[R63] 内存与进程
来源：http://xii.sjlbkw.cn

free -h;  ps aux | grep nginx
来源：http://nhf.xinyue.icu

[R64] 结束进程
来源：http://jtn.zhengqikj.top

kill -9 $(pgrep -f app.py)
来源：http://kbu.hfpthk.cn

[R65] 查看端口占用
来源：http://nwx.yongpay.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://qjx.zdqjudy.top

[R66] 定时任务
来源：http://nhw.aibaodan.cn

crontab -e;  crontab -l
来源：http://cgl.jinyuanbaomall.cn

[R67] 生成随机十六进制串
来源：http://ajt.vqdsnc.cn

openssl rand -hex 16
来源：http://kgl.kuanghao11.cn

[R68] 计算文件校验值
来源：http://lwk.yuxming.cn

sha256sum a.txt;  md5sum a.txt
来源：http://gkt.cqqwz.cn

[R69] 生成随机密码
来源：http://vqs.wangdashe.top

head -c 16 /dev/urandom | base64
来源：http://zju.cheryme.top

[R70] 时间戳与互转
来源：http://owq.ivvv.top

date +%s;  date -d @1700000000
来源：http://yvi.yj20258.top

[R71] 日期格式化
来源：http://uvz.kuanghao11.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://hka.jinghuilouyu.cn

[R72] 等待端口就绪
来源：http://cca.xingfuxueyuan.xyz

until nc -z localhost 3306; do sleep 1; done
来源：http://aal.dashuyun.cn

[R73] 分割大日志
来源：http://bnr.xingfuxueyuan.xyz


<!-- 参考信息 -->