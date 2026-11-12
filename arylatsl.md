代发 wailian999

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://yuv.chenlongwang.top

[Q20] IN 列表
来源：http://ifj.dashuyun.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hot.uphjek.com

[Q21] 空值判断
来源：http://zan.zhijiandao.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://byq.chenzaomai.com

[Q22] 排序
来源：http://fyw.sufxvd.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://gse.xinyue.icu

[Q23] 分页
来源：http://lhw.xingfuxueyuan.xyz

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://uds.sxryk.cn

[Q24] 去重
来源：http://ffd.jqgfzy.top

SELECT DISTINCT city FROM users;
来源：http://oun.tanke756.top

[Q25] 只取前 N 条
来源：http://yoe.hammf.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://npm.gzhubu.top

[Q26] 计数
来源：http://eou.birdmap.top

SELECT COUNT(*) FROM users;
来源：http://vmn.epnwcf.com

[Q27] 条件计数
来源：http://yfs.fengsongda.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://xlk.zhoulong.xyz

[Q28] 求和与平均
来源：http://vuu.havefunace.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://pag.sweek.top

[Q29] 最大最小值
来源：http://cxh.xinyue.icu

SELECT MAX(age), MIN(age) FROM users;
来源：http://ikh.jinyuanbaomall.cn

[Q30] 分组统计
来源：http://ill.jinghuilouyu.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mbo.ehwqpu.com

[Q31] 分组后过滤
来源：http://fqc.ywan-chungtsiang.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://vjl.ivvv.top

[Q32] 分组拼接字符串
来源：http://ciz.yanxiufei.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://new.tianlin.xyz

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://njy.epnwcf.com

[Q33] 多列分组
来源：http://nku.sysykeji.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://gdp.hnxiangtu.top

[Q34] 每组取第一条
来源：http://wsd.dianchejie.cn

SELECT * FROM (
来源：http://hag.jiagoushi.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hgn.zhoulong.xyz

) t WHERE rn = 1;
来源：http://ngc.meibo888.top

[Q35] 内连接
来源：http://dle.ydzc1.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ily.shuidangran.top

[Q36] 左连接
来源：http://cqf.tanke756.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://fbe.jinqigfzy.top

[Q37] 右连接
来源：http://cdr.fzhhl.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://gdn.svipenyu.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ezt.svipenyu.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://unb.andypj.xyz

[Q39] 自连接（查上下级）
来源：http://xmq.zhaomingkeji.xyz

SELECT e.name, m.name AS manager FROM employees e
来源：http://gqn.mhx1999.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://xty.vehdjk.com

[Q40] 交叉连接（笛卡尔积）
来源：http://ahj.cashguo.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://uib.jyoumei.cn

[Q41] 多表连接
来源：http://pwi.daxiang520.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://asx.tianlin.xyz

JOIN users u ON u.id = o.user_id
来源：http://hyp.hnxiangtu.top

JOIN products p ON p.id = o.product_id;
来源：http://pap.gzhubu.top

[Q42] 连接条件附加过滤
来源：http://eie.dashuyun.cn

SELECT u.name, o.amount FROM users u
来源：http://tbo.birdmap.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://fpv.zhongyouzk.top

[Q43] 标量子查询
来源：http://mnj.gzhubu.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ifu.jqgufenzy.top

[Q44] IN 子查询
来源：http://xfb.ybcxt.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hev.havefunace.top

[Q45] EXISTS 判断存在
来源：http://zkf.hammf.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://yov.shzxlz.cn

[Q46] NOT EXISTS 判断不存在
来源：http://mps.uphjek.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://aqu.0kj1m.cn

[Q47] 与平均值比较
来源：http://pro.gotoacloud.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://uvn.chenlongwang.top

[Q48] CTE 公用表表达式
来源：http://kkh.xziqi.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://vav.0kj1m.cn

SELECT * FROM t WHERE c > 5;
来源：http://rhg.tianlin.xyz

[Q49] 更新单行
来源：http://aad.yueranfly.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ohj.zhixingplan.top

[Q50] 批量更新
来源：http://zou.cashguo.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://bdr.shanyushiyangtech.top

[Q51] 用子查询更新
来源：http://tjs.jinyuanbaomall.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://pmw.wangshuangyany.cn

[Q52] 删除指定行
来源：http://ftz.jinghuilouyu.cn

DELETE FROM users WHERE id = 10;
来源：http://nwq.yonumen.top

[Q53] 按条件删除
来源：http://azp.chenzaomai.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://vqw.zhijiandao.cn

[Q54] 清空表
来源：http://mwd.hnxiangtu.top

TRUNCATE TABLE logs;
来源：http://mec.nwbrower.top

[Q55] 排名（并列占位）
来源：http://sby.yj20258888.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://dmc.pycfn.com

[Q56] 密集排名（并列不占位）
来源：http://gnp.feifeiyinyue.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://acv.yj20258888.top

[Q57] 行号
来源：http://jlb.zhoulong.xyz

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://uuc.hysaishi.cn

[Q58] 累计求和
来源：http://srn.pengpengdd.cyou

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://oas.guannengcc.top

[Q59] 分组内累计
来源：http://lpk.tanke756.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://gxo.hammf.cn

[Q60] 取上一行 / 下一行
来源：http://xla.zhixingplan.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://szo.vqdsnc.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://kxu.xuetiantiany.cn

[Q61] 移动平均
来源：http://qij.nanxuanxn.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hkr.jqgufenzy.top

[Q62] 分组占比
来源：http://uzh.hesvh.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://tfg.yj20258888.top

[Q63] 开启事务
来源：http://hsn.feifeiyinyue.top

START TRANSACTION;                -- 或 BEGIN
来源：http://sgk.bjfxy.top

[Q64] 提交事务
来源：http://nbc.chenjidiqi.icu

COMMIT;
来源：http://cwt.nanxinkj.top

[Q65] 回滚事务
来源：http://gnk.fanxiaobao.xyz

ROLLBACK;
来源：http://jpb.yongpay.top

[Q66] 行锁查询
来源：http://tlc.shanyushiyangkeji.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://nhe.hongshengwenyu.top

[Q67] 设置隔离级别
来源：http://sjh.yj20258888.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://xtl.hysaishi.cn

[Q68] 保存点
来源：http://nnt.feifeiyinyue.top

SAVEPOINT sp1;
来源：http://ozq.ivvv.top

ROLLBACK TO sp1;
来源：http://sas.bbcook.cn

[Q69] 查看执行计划
来源：http://qgk.uphjek.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ovi.zhoulong.xyz

[Q70] 更新统计信息
来源：http://nsf.epnwcf.com

ANALYZE TABLE users;
来源：http://ens.xziqi.cn

[Q71] 查看建表语句
来源：http://mfn.sufxvd.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://kgz.wangdashe.top

[Q72] 查看索引
来源：http://jee.chenjidiqi.icu

SHOW INDEX FROM users;
来源：http://vhe.chenlongwang.top

[Q73] 查看表状态
来源：http://fyh.cdnleiting.top

SHOW TABLE STATUS LIKE 'users';
来源：http://clv.guannengcc.top

[Q74] 强制使用索引
来源：http://lam.jinyuanbaomall.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://eah.wangshuangyany.cn

[Q75] 日期格式化
来源：http://nem.hnxiangtu.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://uai.cdnleiting.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://dny.guannengcc.top

[Q76] 按天统计
来源：http://uqs.zhiwuduotai.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://qbc.zhixingplan.top

[Q77] 时间加减
来源：http://lqi.uphjek.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://djw.316326.xyz

[Q78] 当前时间
来源：http://ofp.xziqi.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ejk.vehdjk.com

[Q79] 字符串拼接
来源：http://xrk.haohaochexian.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://per.tian-w.cn

[Q80] 字符串截取
来源：http://pbq.yfazqb.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://cbe.yvedp.cn

[Q81] 字符串替换
来源：http://mtj.redwolf501.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://iuo.zycfv.cn

[Q82] 字符长度与字节长度
来源：http://mzq.xziqi.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://acp.ybcxt.top

[Q83] 大小写转换
来源：http://nqc.tian-w.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://crk.xingfuxueyuan.xyz

[Q84] 去除首尾空格
来源：http://xbs.nwbrower.top

SELECT TRIM(name) FROM users;
来源：http://acl.yj20258888.top

[Q85] 数值取整
来源：http://ect.yj202588.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://lzi.wangdashe.top

[Q86] 读取 JSON 字段
来源：http://yze.sjlbkw.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ntw.tianlin.xyz

[Q87] JSON 字段做条件
来源：http://ook.zhongyouzk.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://thg.zhixingplan.top

[Q88] 行转列（条件聚合）
来源：http://ncb.daxiang520.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://rst.gotoacloud.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://olx.shanyushiyangkeji.top

[Q89] 判断表是否存在
来源：http://oif.cashguo.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hat.epnwcf.com

[Q90] 生成序号列
来源：http://ayn.zhoulong.xyz

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://bth.jqgfzy.top

================================================================================
来源：http://dov.redwolf501.top

R. Bash 专题
来源：http://jqe.xziqi.cn

================================================================================
来源：http://qsu.feifeiyinyue.top

[R01] shebang 与严格模式
来源：http://ump.yvedp.cn

#!/usr/bin/env bash
来源：http://yqg.cdnleiting.top

set -euo pipefail
来源：http://jth.hammf.cn

[R02] 变量赋值与使用
来源：http://xbx.meibo888.top

name="Tom"; echo "$name"
来源：http://gwp.epnwcf.com

[R03] 只读变量
来源：http://tnf.fehbvm.com

readonly PI=3.14
来源：http://hnc.cheryme.top

[R04] 位置参数
来源：http://kir.ydzc1.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wja.bbcook.cn

[R05] 参数默认值
来源：http://dsd.jinghuilouyu.cn

name="${1:-default}"
来源：http://mge.havefunace.top

[R06] 判断命令是否存在
来源：http://ymv.fanxiaobao.xyz

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://dbd.shanyushiyangkeji.top

[R07] if 判断文件
来源：http://ybe.zhongyouzk.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ioa.chenzaomai.com

[R08] 数值比较
来源：http://wxg.smart0.xyz

if (( a > b )); then echo "a 更大"; fi
来源：http://vsh.birdmap.top

[R09] 字符串比较
来源：http://qey.tian-w.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://pdl.xziqi.cn

[R10] 正则匹配
来源：http://loo.tarul.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hcy.zhoulong.xyz

[R11] case 多分支
来源：http://dih.snrcjt.cn

case "$1" in
来源：http://naj.0kj1m.cn

start) echo "启动" ;;
来源：http://qfy.guannengcc.top

stop)  echo "停止" ;;
来源：http://lgs.svipenyu.cn

*)     echo "未知命令" ;;
来源：http://ltc.dianchejie.cn

esac
来源：http://jgq.vehdjk.com

[R12] for 遍历文件
来源：http://fec.uphjek.com

for f in *.txt; do echo "$f"; done
来源：http://zij.xuetiantiany.cn

[R13] for 计数循环
来源：http://lyr.jqgufenzy.top

for i in {1..10}; do echo "$i"; done
来源：http://rsd.nwbrower.top

[R14] C 风格 for
来源：http://duw.jlsjyb.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://qbp.yj20258888.top

[R15] while 逐行读文件
来源：http://esg.xuanzx.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ihf.cashguo.top

[R16] until 等待条件
来源：http://fxi.yanxiufei.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://aim.pycfn.com

[R17] 数组定义与取值
来源：http://wad.aibaodan.cn

arr=(a b c); echo "${arr[0]}"
来源：http://vly.zhiwuduotai.top

[R18] 遍历数组
来源：http://knc.shzxlz.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wmz.fehbvm.com

[R19] 数组长度
来源：http://xya.ivvv.top

echo "${#arr[@]}"
来源：http://fgq.yj20258.top

[R20] 关联数组（字典）
来源：http://woq.vehdjk.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://pla.xuanzx.com

[R21] 字符串长度
来源：http://fmr.xuetiantiany.cn

echo "${#s}"
来源：http://qbk.svipenyu.cn

[R22] 截取子串
来源：http://reo.pengpengdd.cyou

echo "${s:0:5}"
来源：http://ogy.jinyuanbaomall.cn

[R23] 字符串替换
来源：http://ogv.redwolf501.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://fdt.yanxiufei.cn

[R24] 大小写转换
来源：http://mli.zhijiandao.cn

echo "${s^^}"; echo "${s,,}"
来源：http://qry.zdqjudy.top

[R25] 去后缀 / 去前缀
来源：http://loy.fzhhl.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://hfd.yj202588.top

[R26] 命令替换
来源：http://abs.vqdsnc.cn

now=$(date +%F); echo "$now"
来源：http://lhc.guannengcc.top

[R27] 算术展开
来源：http://tsk.yj20258888.top

echo $((1 + 2 * 3))
来源：http://gkh.hammf.cn

[R28] 浮点运算
来源：http://drp.0kj1m.cn

echo "scale=2; 10/3" | bc
来源：http://fyy.shzxlz.cn

[R29] 定义函数
来源：http://sbj.haohaochexian.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://gtd.ywan-chungtsiang.top

[R30] 函数返回状态码
来源：http://ncp.bjfxy.top

f() { return 0; }; f || echo "失败了"
来源：http://jww.hnqzz.top

[R31] 局部变量
来源：http://jig.haohaochexian.top

f() { local x=1; echo "$x"; }
来源：http://uju.yangfankeji.com

[R32] 参数个数校验
来源：http://cjv.xuanzx.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wdh.zhijiandao.cn

[R33] 捕获错误并提示行号
来源：http://zqn.tianlin.xyz

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ltv.gzhubu.top

[R34] 退出时清理
来源：http://uvj.tian-w.cn

trap 'rm -f "$tmp"' EXIT
来源：http://eum.gzhubu.top

[R35] 后台执行并等待
来源：http://ctb.tian-w.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://lcb.xinyue.icu

[R36] 并发执行多个任务
来源：http://aln.nanxuanxn.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://acc.shanyushiyangtech.top

[R37] 把输出赋给变量
来源：http://tts.yuxming.cn

files=$(ls -1)
来源：http://uhn.hnxiangtu.top

[R38] 管道串联
来源：http://fjt.hnqzz.top

cat a.txt | grep -i error | wc -l
来源：http://wyr.daxiang520.top

[R39] 重定向标准输出与错误
来源：http://qkv.birdmap.top

cmd > out.log 2>&1
来源：http://msh.9152youxi.cn

[R40] 追加写日志
来源：http://ltw.ehwqpu.com

echo "log" >> out.log
来源：http://vyj.jianghu66.top

[R41] 丢弃输出
来源：http://oob.shuidangran.top

cmd >/dev/null 2>&1
来源：http://uuu.gaohongyu789.top

[R42] 输入重定向
来源：http://hng.gzhubu.top

wc -l < a.txt
来源：http://ifq.hfpthk.cn

[R43] 按名字查找文件
来源：http://qko.sjlbkw.cn

find . -name "*.log" -type f
来源：http://wdh.yvedp.cn

[R44] 按修改时间查找
来源：http://xks.ybcxt.top

find . -mtime -7 -type f
来源：http://dqr.ybcxt.top

[R45] 批量删除
来源：http://byg.ehwqpu.com

find . -name "*.tmp" -delete
来源：http://lyf.tian-w.cn

[R46] 递归替换文件内容
来源：http://ulz.quarkkingdee.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://pql.ybcxt.top

[R47] sed 单行替换
来源：http://vuo.fktsv.cn

sed -i 's/foo/bar/g' a.txt
来源：http://civ.fanxiaobao.xyz

[R48] awk 取指定列
来源：http://kce.hammf.cn

awk '{print $1, $3}' a.txt
来源：http://sgq.gogol.net.cn

[R49] awk 带条件
来源：http://icx.yangfankeji.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://rss.fengsongda.top

[R50] awk 求和
来源：http://sii.yuxming.cn

awk '{s += $2} END {print s}' a.txt
来源：http://clo.yj20258888.top

[R51] 排序去重取前几
来源：http://xrx.dashuyun.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://qwa.xziqi.cn

[R52] 统计行数
来源：http://hpy.fktsv.cn

wc -l a.txt
来源：http://gwp.hcnkem.com

[R53] 查看文件头与实时尾
来源：http://bfa.jqgufenzy.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://bst.jqgufenzy.top

[R54] 比较两个文件
来源：http://wfr.kuanghao11.cn

diff a.txt b.txt
来源：http://gnl.chenjidiqi.icu

[R55] 压缩与解压
来源：http://ecp.zhengqikj.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hjh.quarkkingdee.top

[R56] 远程拷贝
来源：http://xax.zhaomingkeji.xyz

scp file user@host:/path/
来源：http://mwz.9152youxi.cn

[R57] 远程执行命令
来源：http://cuz.jinghuilouyu.cn

ssh user@host 'uptime'
来源：http://cgj.hnqzz.top

[R58] 下载文件
来源：http://myd.ppjwa.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://gwl.hnqzz.top

[R59] 发 POST JSON
来源：http://xax.hammf.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mdu.snrcjt.cn

[R60] 只看 HTTP 状态码
来源：http://ylw.nwbrower.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ncv.chenlongwang.top

[R61] 磁盘占用
来源：http://jjl.daxiang520.top

df -h;  du -sh *
来源：http://jmb.fzhhl.top

[R62] 找最占空间的文件
来源：http://zsq.nanxuanxn.top

du -ah . | sort -rh | head -10
来源：http://zlb.gogol.net.cn

[R63] 内存与进程
来源：http://lxr.andypj.xyz

free -h;  ps aux | grep nginx
来源：http://cdr.shanyushiyangtech.top

[R64] 结束进程
来源：http://oyj.jinqigfzy.top

kill -9 $(pgrep -f app.py)
来源：http://zhv.pycfn.com

[R65] 查看端口占用
来源：http://qnr.snrcjt.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://rqd.nanxuanxn.top

[R66] 定时任务
来源：http://sbf.yangfankeji.com

crontab -e;  crontab -l
来源：http://exn.yangfankeji.com

[R67] 生成随机十六进制串
来源：http://vud.hcnkem.com

openssl rand -hex 16
来源：http://vel.zhengqikj.top

[R68] 计算文件校验值
来源：http://peo.yuxming.cn

sha256sum a.txt;  md5sum a.txt
来源：http://hpv.chenzaomai.com

[R69] 生成随机密码
来源：http://zzb.hysaishi.cn


<!-- 参考信息 -->