代发 wailian999

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://uha.xinyue.icu

[Q26] 计数
来源：http://ihk.ybcxt.top

SELECT COUNT(*) FROM users;
来源：http://mle.tanke756.top

[Q27] 条件计数
来源：http://gtx.fehbvm.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://uyr.havefunace.top

[Q28] 求和与平均
来源：http://pvz.guannengcc.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://rft.ydzc1.top

[Q29] 最大最小值
来源：http://vpa.nwbrower.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://ozn.jianghu66.top

[Q30] 分组统计
来源：http://ngr.xuanzx.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://tgn.zdbjq.cn

[Q31] 分组后过滤
来源：http://smu.aizwys.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://vrj.zdqjudy.top

[Q32] 分组拼接字符串
来源：http://ujy.xinyue.icu

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://gbh.cdnleiting.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://rar.andypj.xyz

[Q33] 多列分组
来源：http://jae.jqgfzy.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://voq.aizwys.cn

[Q34] 每组取第一条
来源：http://uxa.chenlongwang.top

SELECT * FROM (
来源：http://bad.dianchejie.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://bxj.cashguo.top

) t WHERE rn = 1;
来源：http://ycq.hnxiangtu.top

[Q35] 内连接
来源：http://hkn.cheryme.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ono.zhongyouzk.top

[Q36] 左连接
来源：http://vis.hongshengwenyu.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wdf.fanxiaobao.xyz

[Q37] 右连接
来源：http://zhp.chenlongwang.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://yqn.zycfv.cn

[Q38] 全外连接（PostgreSQL）
来源：http://oqo.cqqwz.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://cwf.aizwys.cn

[Q39] 自连接（查上下级）
来源：http://crl.zhongyouzk.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://kvq.0kj1m.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://quv.sweek.top

[Q40] 交叉连接（笛卡尔积）
来源：http://xzb.jqgfzy.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://pln.yueranfly.top

[Q41] 多表连接
来源：http://sod.jinghuilouyu.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://kga.yangfankeji.com

JOIN users u ON u.id = o.user_id
来源：http://rgh.dianchejie.cn

JOIN products p ON p.id = o.product_id;
来源：http://tlj.jinghuilouyu.cn

[Q42] 连接条件附加过滤
来源：http://dea.xuetiantiany.cn

SELECT u.name, o.amount FROM users u
来源：http://dxa.xuanzx.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ige.cheryme.top

[Q43] 标量子查询
来源：http://ihc.xingfuxueyuan.xyz

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://its.zhijiandao.cn

[Q44] IN 子查询
来源：http://nfs.jinyuanbaomall.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://rbt.fanxiaobao.xyz

[Q45] EXISTS 判断存在
来源：http://ynv.uphjek.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://exg.vqdsnc.cn

[Q46] NOT EXISTS 判断不存在
来源：http://dhx.yuxming.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://yds.sweek.top

[Q47] 与平均值比较
来源：http://lps.nanxuanxn.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ssb.kuanghao11.cn

[Q48] CTE 公用表表达式
来源：http://ith.xingfuxueyuan.xyz

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mol.xinyue.icu

SELECT * FROM t WHERE c > 5;
来源：http://dpe.wangdashe.top

[Q49] 更新单行
来源：http://iol.dianchejie.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://sde.yuanzhike.top

[Q50] 批量更新
来源：http://ivy.hnxiangtu.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://oeq.haohaochexian.top

[Q51] 用子查询更新
来源：http://cuh.jlsjyb.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://nuv.shanyushiyangkeji.top

[Q52] 删除指定行
来源：http://uwy.yvedp.cn

DELETE FROM users WHERE id = 10;
来源：http://apb.52xcode.cn

[Q53] 按条件删除
来源：http://jel.yongpay.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://acz.fehbvm.com

[Q54] 清空表
来源：http://voq.tarul.cn

TRUNCATE TABLE logs;
来源：http://xym.xuanzx.com

[Q55] 排名（并列占位）
来源：http://luh.sxryk.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://oyo.chenlongwang.top

[Q56] 密集排名（并列不占位）
来源：http://heo.hongshengwenyu.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://vff.jiagoushi.top

[Q57] 行号
来源：http://avd.zycfv.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://aiu.aizwys.cn

[Q58] 累计求和
来源：http://xos.cdnleiting.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://jkr.feifeiyinyue.top

[Q59] 分组内累计
来源：http://tzl.yj20258.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://jwb.zhaomingkeji.xyz

[Q60] 取上一行 / 下一行
来源：http://kvg.cashguo.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://rlp.fehbvm.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ite.epnwcf.com

[Q61] 移动平均
来源：http://fsv.fzhhl.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://joq.sysykeji.top

[Q62] 分组占比
来源：http://hig.daxiang520.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://fix.yj20258888.top

[Q63] 开启事务
来源：http://sff.jyoumei.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://qfm.feifeiyinyue.top

[Q64] 提交事务
来源：http://xdd.cashguo.top

COMMIT;
来源：http://wuc.zhixingplan.top

[Q65] 回滚事务
来源：http://tno.shzxlz.cn

ROLLBACK;
来源：http://xiq.tianlin.xyz

[Q66] 行锁查询
来源：http://zsg.9152youxi.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://uog.jianghu66.top

[Q67] 设置隔离级别
来源：http://ttf.316326.xyz

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://xhe.cheryme.top

[Q68] 保存点
来源：http://jtf.yuanzhike.top

SAVEPOINT sp1;
来源：http://vdw.gzhubu.top

ROLLBACK TO sp1;
来源：http://hrm.xylfe.cn

[Q69] 查看执行计划
来源：http://ksc.aizwys.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://zng.0kj1m.cn

[Q70] 更新统计信息
来源：http://dxf.daria6918.cn

ANALYZE TABLE users;
来源：http://kbd.tanke756.top

[Q71] 查看建表语句
来源：http://bha.vqdsnc.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wao.gzhubu.top

[Q72] 查看索引
来源：http://bxt.wangdashe.top

SHOW INDEX FROM users;
来源：http://klm.nanxinkj.top

[Q73] 查看表状态
来源：http://cez.sysykeji.top

SHOW TABLE STATUS LIKE 'users';
来源：http://yvh.yj20258888.top

[Q74] 强制使用索引
来源：http://tvo.yanxiufei.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://zvf.xuetiantiany.cn

[Q75] 日期格式化
来源：http://gbr.sxryk.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ylq.chenlongwang.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://fmw.redwolf501.top

[Q76] 按天统计
来源：http://nve.tarul.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://otv.ywan-chungtsiang.top

[Q77] 时间加减
来源：http://juu.fehbvm.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://gsh.0kj1m.cn

[Q78] 当前时间
来源：http://ufu.jqgfzy.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://uhq.yfazqb.com

[Q79] 字符串拼接
来源：http://dtl.redwolf501.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://pdp.cashguo.top

[Q80] 字符串截取
来源：http://tjh.sysykeji.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://kbd.jinqigfzy.top

[Q81] 字符串替换
来源：http://qxo.yj20258888.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://gcf.zhiwuduotai.top

[Q82] 字符长度与字节长度
来源：http://dti.jqgfzy.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://cqo.cheryme.top

[Q83] 大小写转换
来源：http://hwc.zhixingplan.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blx.jinghuilouyu.cn

[Q84] 去除首尾空格
来源：http://iyi.zhiwuduotai.top

SELECT TRIM(name) FROM users;
来源：http://xtj.guowangkeji.top

[Q85] 数值取整
来源：http://gsl.guowangkeji.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://fnx.gotoacloud.top

[Q86] 读取 JSON 字段
来源：http://hbu.aizwys.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://vus.cucudq.cn

[Q87] JSON 字段做条件
来源：http://yea.meibo888.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://lyx.jinyuanbaomall.cn

[Q88] 行转列（条件聚合）
来源：http://llq.yfazqb.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://zqg.gotoacloud.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mvn.zhengqikj.top

[Q89] 判断表是否存在
来源：http://rib.yueranfly.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://psg.vehdjk.com

[Q90] 生成序号列
来源：http://uml.sweek.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://zly.xinyue.icu

================================================================================
来源：http://gnd.chenzaomai.com

R. Bash 专题
来源：http://phh.gogol.net.cn

================================================================================
来源：http://dci.zhongyouzk.top

[R01] shebang 与严格模式
来源：http://gkv.daria6918.cn

#!/usr/bin/env bash
来源：http://hsz.redwolf501.top

set -euo pipefail
来源：http://kct.smart0.xyz

[R02] 变量赋值与使用
来源：http://uqs.yj20258888.top

name="Tom"; echo "$name"
来源：http://jyf.jqgfzy.top

[R03] 只读变量
来源：http://err.smart0.xyz

readonly PI=3.14
来源：http://yux.yongpay.top

[R04] 位置参数
来源：http://wtz.zdqjudy.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://iwf.yonumen.top

[R05] 参数默认值
来源：http://xql.fzhhl.top

name="${1:-default}"
来源：http://iyx.quarkkingdee.top

[R06] 判断命令是否存在
来源：http://jjk.yanxiufei.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://fam.jinqigfzy.top

[R07] if 判断文件
来源：http://ons.cheryme.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://vrn.aizwys.cn

[R08] 数值比较
来源：http://szy.zhijiandao.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://kur.shzxlz.cn

[R09] 字符串比较
来源：http://nol.pycfn.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://pma.xuanzx.com

[R10] 正则匹配
来源：http://puc.daria6918.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wmh.yuanzhike.top

[R11] case 多分支
来源：http://rjh.pengpengdd.cyou

case "$1" in
来源：http://vzi.sweek.top

start) echo "启动" ;;
来源：http://fsv.quarkkingdee.top

stop)  echo "停止" ;;
来源：http://nwy.ywan-chungtsiang.top

*)     echo "未知命令" ;;
来源：http://mme.c1oappe.top

esac
来源：http://qul.zhiwuduotai.top

[R12] for 遍历文件
来源：http://klk.gaohongyu789.top

for f in *.txt; do echo "$f"; done
来源：http://rqu.tianlin.xyz

[R13] for 计数循环
来源：http://umn.hywenlv.cn

for i in {1..10}; do echo "$i"; done
来源：http://ydg.jinyuanbaomall.cn

[R14] C 风格 for
来源：http://kcf.xziqi.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://yyf.chenzaomai.com

[R15] while 逐行读文件
来源：http://rko.yonumen.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://kgw.wangshuangyany.cn

[R16] until 等待条件
来源：http://itl.pycfn.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://eec.zhengqikj.top

[R17] 数组定义与取值
来源：http://pac.svipenyu.cn

arr=(a b c); echo "${arr[0]}"
来源：http://znd.smart0.xyz

[R18] 遍历数组
来源：http://kqt.tanke756.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://tue.guannengcc.top

[R19] 数组长度
来源：http://qws.jiagoushi.top

echo "${#arr[@]}"
来源：http://yei.havefunace.top

[R20] 关联数组（字典）
来源：http://dbz.9152youxi.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://jky.chenlongwang.top

[R21] 字符串长度
来源：http://vzn.shzxlz.cn

echo "${#s}"
来源：http://uwf.pengpengdd.cyou

[R22] 截取子串
来源：http://ymh.shuidangran.top

echo "${s:0:5}"
来源：http://jtv.jinqigfzy.top

[R23] 字符串替换
来源：http://sor.gogol.net.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ezt.jlsjyb.cn

[R24] 大小写转换
来源：http://ouo.fzhhl.top

echo "${s^^}"; echo "${s,,}"
来源：http://qik.meibo888.top

[R25] 去后缀 / 去前缀
来源：http://swo.yangfankeji.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://izy.shanyushiyangtech.top

[R26] 命令替换
来源：http://qnd.jinqigufen.top

now=$(date +%F); echo "$now"
来源：http://duh.guannengcc.top

[R27] 算术展开
来源：http://azi.nanxinkj.top

echo $((1 + 2 * 3))
来源：http://vwh.0kj1m.cn

[R28] 浮点运算
来源：http://isd.fehbvm.com

echo "scale=2; 10/3" | bc
来源：http://mpq.jlsjyb.cn

[R29] 定义函数
来源：http://epu.feifeiyinyue.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://elj.jqgfzy.top

[R30] 函数返回状态码
来源：http://lbs.nwbrower.top

f() { return 0; }; f || echo "失败了"
来源：http://iuj.sysykeji.top

[R31] 局部变量
来源：http://eyl.shzxlz.cn

f() { local x=1; echo "$x"; }
来源：http://opa.chenjidiqi.icu

[R32] 参数个数校验
来源：http://nrg.hcnkem.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://lhj.aizwys.cn

[R33] 捕获错误并提示行号
来源：http://qxj.uphjek.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://aed.jqgfzy.top

[R34] 退出时清理
来源：http://hir.gzhubu.top

trap 'rm -f "$tmp"' EXIT
来源：http://hrz.snrcjt.cn

[R35] 后台执行并等待
来源：http://zso.hysaishi.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://gwc.xuetiantiany.cn

[R36] 并发执行多个任务
来源：http://ypj.mhx1999.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://rag.andypj.xyz

[R37] 把输出赋给变量
来源：http://tyo.chenlongwang.top

files=$(ls -1)
来源：http://orf.wangdashe.top

[R38] 管道串联
来源：http://nra.yj20258.top

cat a.txt | grep -i error | wc -l
来源：http://wsn.andypj.xyz

[R39] 重定向标准输出与错误
来源：http://jve.shzxlz.cn

cmd > out.log 2>&1
来源：http://eqm.chenlongwang.top

[R40] 追加写日志
来源：http://lzw.quarkkingdee.top

echo "log" >> out.log
来源：http://fju.fengsongda.top

[R41] 丢弃输出
来源：http://ixe.zhengqikj.top

cmd >/dev/null 2>&1
来源：http://waq.redwolf501.top

[R42] 输入重定向
来源：http://vnx.smart0.xyz

wc -l < a.txt
来源：http://szq.havefunace.top

[R43] 按名字查找文件
来源：http://thb.hesvh.cn

find . -name "*.log" -type f
来源：http://fus.zhongyouzk.top

[R44] 按修改时间查找
来源：http://jta.guannengcc.top

find . -mtime -7 -type f
来源：http://ued.uphjek.com

[R45] 批量删除
来源：http://aqn.aizwys.cn

find . -name "*.tmp" -delete
来源：http://zlj.shangyingyoupin.top

[R46] 递归替换文件内容
来源：http://oqu.quarkkingdee.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://kic.316326.xyz

[R47] sed 单行替换
来源：http://ppo.uphjek.com

sed -i 's/foo/bar/g' a.txt
来源：http://kaq.xziqi.cn

[R48] awk 取指定列
来源：http://see.bjfxy.top

awk '{print $1, $3}' a.txt
来源：http://tlu.xuanzx.com

[R49] awk 带条件
来源：http://bjj.hnqzz.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://vys.uphjek.com

[R50] awk 求和
来源：http://fmx.zhengqikj.top

awk '{s += $2} END {print s}' a.txt
来源：http://ueq.zhiwuduotai.top

[R51] 排序去重取前几
来源：http://hqu.yfazqb.com

sort a.txt | uniq -c | sort -rn | head
来源：http://lbb.jinqigufen.top

[R52] 统计行数
来源：http://dds.tian-w.cn

wc -l a.txt
来源：http://yno.smart0.xyz

[R53] 查看文件头与实时尾
来源：http://qyl.yuanzhike.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://agh.yangfankeji.com

[R54] 比较两个文件
来源：http://pbb.yongpay.top

diff a.txt b.txt
来源：http://trl.tarul.cn

[R55] 压缩与解压
来源：http://zfi.daxiang520.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://cij.cucudq.cn

[R56] 远程拷贝
来源：http://zha.dianchejie.cn

scp file user@host:/path/
来源：http://dnc.sjlbkw.cn

[R57] 远程执行命令
来源：http://evf.xuanzx.com

ssh user@host 'uptime'
来源：http://onr.ppjwa.cn

[R58] 下载文件
来源：http://cos.gaohongyu789.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://rpg.hywenlv.cn

[R59] 发 POST JSON
来源：http://ipo.316326.xyz

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ivy.jinghuilouyu.cn

[R60] 只看 HTTP 状态码
来源：http://kee.fzhhl.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hje.svipenyu.cn

[R61] 磁盘占用
来源：http://bze.yongpay.top

df -h;  du -sh *
来源：http://qql.ybcxt.top

[R62] 找最占空间的文件
来源：http://awp.epnwcf.com

du -ah . | sort -rh | head -10
来源：http://ten.hfpthk.cn

[R63] 内存与进程
来源：http://ccb.redwolf501.top

free -h;  ps aux | grep nginx
来源：http://smn.xuanzx.com

[R64] 结束进程
来源：http://gbx.cheryme.top

kill -9 $(pgrep -f app.py)
来源：http://rwq.jinqigufen.top

[R65] 查看端口占用
来源：http://mbi.yj20258.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://eck.vqdsnc.cn

[R66] 定时任务
来源：http://rvg.ehwqpu.com

crontab -e;  crontab -l
来源：http://wss.hammf.cn

[R67] 生成随机十六进制串
来源：http://dpz.pengpengdd.cyou

openssl rand -hex 16
来源：http://bkq.sysykeji.top

[R68] 计算文件校验值
来源：http://qkp.yj20258.top

sha256sum a.txt;  md5sum a.txt
来源：http://drr.yj202588.top

[R69] 生成随机密码
来源：http://lsq.zhengqikj.top

head -c 16 /dev/urandom | base64
来源：http://wtf.shzxlz.cn

[R70] 时间戳与互转
来源：http://nko.cucudq.cn

date +%s;  date -d @1700000000
来源：http://qey.xuetiantiany.cn

[R71] 日期格式化
来源：http://zuk.feifeiyinyue.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://hso.epnwcf.com

[R72] 等待端口就绪
来源：http://ztr.haohaochexian.top

until nc -z localhost 3306; do sleep 1; done
来源：http://zdx.nwbrower.top

[R73] 分割大日志
来源：http://gyd.gotoacloud.top

split -l 1000 big.log part_
来源：http://jxm.xziqi.cn

[R74] 批量重命名
来源：http://jbu.jqgufenzy.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://tln.sysykeji.top

[R75] 导出环境变量
来源：http://gpj.chenjidiqi.icu


<!-- 参考信息 -->