代发 wailian999

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ngt.fehbvm.com

[Q18] 模糊匹配
来源：http://swa.vqdsnc.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://rlo.zdqjudy.top

[Q19] 范围查询
来源：http://dte.kuanghao11.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://qty.aizwys.cn

[Q20] IN 列表
来源：http://sxx.fengsongda.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mbm.shanyushiyangkeji.top

[Q21] 空值判断
来源：http://awg.gotoacloud.top

SELECT * FROM users WHERE email IS NULL;
来源：http://blz.mhx1999.top

[Q22] 排序
来源：http://ozr.snrcjt.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://knd.chenzaomai.com

[Q23] 分页
来源：http://tqy.bbcook.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://brv.jiagoushi.top

[Q24] 去重
来源：http://pxd.aizwys.cn

SELECT DISTINCT city FROM users;
来源：http://tvy.xylfe.cn

[Q25] 只取前 N 条
来源：http://adw.jinqigfzy.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://phc.meibo888.top

[Q26] 计数
来源：http://hge.shuidangran.top

SELECT COUNT(*) FROM users;
来源：http://msg.shangyingyoupin.top

[Q27] 条件计数
来源：http://ldr.shangyingyoupin.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://orz.jqgfzy.top

[Q28] 求和与平均
来源：http://xzo.zhengqikj.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wja.uphjek.com

[Q29] 最大最小值
来源：http://avn.vqdsnc.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://gjw.tian-w.cn

[Q30] 分组统计
来源：http://xfi.redwolf501.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://yrx.yj20258888.top

[Q31] 分组后过滤
来源：http://wbv.tianlin.xyz

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://arm.xylfe.cn

[Q32] 分组拼接字符串
来源：http://gkd.zhongyouzk.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://qqc.yangfankeji.com

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://tni.tarul.cn

[Q33] 多列分组
来源：http://blm.yj202588.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ffk.wangshuangyany.cn

[Q34] 每组取第一条
来源：http://yep.yueranfly.top

SELECT * FROM (
来源：http://vqp.shanyushiyangtech.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://fod.andypj.xyz

) t WHERE rn = 1;
来源：http://duc.hnqzz.top

[Q35] 内连接
来源：http://ojb.gaohongyu789.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://bsj.aibaodan.cn

[Q36] 左连接
来源：http://iub.zhaomingkeji.xyz

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hqs.jyoumei.cn

[Q37] 右连接
来源：http://qfh.yuxming.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://gkv.svipenyu.cn

[Q38] 全外连接（PostgreSQL）
来源：http://kma.yongpay.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://teh.zhoulong.xyz

[Q39] 自连接（查上下级）
来源：http://zpm.chenlongwang.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://dnl.guannengcc.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://rex.yj20258888.top

[Q40] 交叉连接（笛卡尔积）
来源：http://ofv.svipenyu.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://tci.jinyuanbaomall.cn

[Q41] 多表连接
来源：http://lso.feifeiyinyue.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://sdo.jqgufenzy.top

JOIN users u ON u.id = o.user_id
来源：http://uky.jinqigfzy.top

JOIN products p ON p.id = o.product_id;
来源：http://ykz.yuanzhike.top

[Q42] 连接条件附加过滤
来源：http://pvc.zdbjq.cn

SELECT u.name, o.amount FROM users u
来源：http://wyn.zhoulong.xyz

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://lch.zhaomingkeji.xyz

[Q43] 标量子查询
来源：http://lon.nwbrower.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://uam.hesvh.cn

[Q44] IN 子查询
来源：http://rzu.uphjek.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ypm.9152youxi.cn

[Q45] EXISTS 判断存在
来源：http://jsj.0kj1m.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kqb.sxryk.cn

[Q46] NOT EXISTS 判断不存在
来源：http://lgp.haohaochexian.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wjr.xinyue.icu

[Q47] 与平均值比较
来源：http://ugo.xziqi.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://eue.xuanzx.com

[Q48] CTE 公用表表达式
来源：http://qve.hnqzz.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://doh.yueranfly.top

SELECT * FROM t WHERE c > 5;
来源：http://mcr.ywan-chungtsiang.top

[Q49] 更新单行
来源：http://sqk.tian-w.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://znx.shangyingyoupin.top

[Q50] 批量更新
来源：http://bxn.yvedp.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://kdr.gotoacloud.top

[Q51] 用子查询更新
来源：http://nni.hcnkem.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://fky.zhaomingkeji.xyz

[Q52] 删除指定行
来源：http://hzu.chenzaomai.com

DELETE FROM users WHERE id = 10;
来源：http://vez.tianlin.xyz

[Q53] 按条件删除
来源：http://byw.xylfe.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://xpt.hnxiangtu.top

[Q54] 清空表
来源：http://nar.hfpthk.cn

TRUNCATE TABLE logs;
来源：http://vue.0kj1m.cn

[Q55] 排名（并列占位）
来源：http://eed.guannengcc.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://lmp.ydzc1.top

[Q56] 密集排名（并列不占位）
来源：http://fum.svipenyu.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://dgq.ehwqpu.com

[Q57] 行号
来源：http://ryx.316326.xyz

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://eqg.hesvh.cn

[Q58] 累计求和
来源：http://eyx.ybcxt.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://jbl.feifeiyinyue.top

[Q59] 分组内累计
来源：http://ckw.aizwys.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://auk.zhijiandao.cn

[Q60] 取上一行 / 下一行
来源：http://sib.meibo888.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://nhq.chenlongwang.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://tyv.ctjpmb.com

[Q61] 移动平均
来源：http://aao.yuxming.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://eii.chenzaomai.com

[Q62] 分组占比
来源：http://adc.cucudq.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://emp.hysaishi.cn

[Q63] 开启事务
来源：http://yzf.xinyue.icu

START TRANSACTION;                -- 或 BEGIN
来源：http://kqv.wangdashe.top

[Q64] 提交事务
来源：http://tlb.bjfxy.top

COMMIT;
来源：http://mpr.meibo888.top

[Q65] 回滚事务
来源：http://phi.shanyushiyangtech.top

ROLLBACK;
来源：http://mbu.xylfe.cn

[Q66] 行锁查询
来源：http://pcs.zycfv.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://cjb.xuanzx.com

[Q67] 设置隔离级别
来源：http://txw.epnwcf.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://okg.wangdashe.top

[Q68] 保存点
来源：http://itp.sweek.top

SAVEPOINT sp1;
来源：http://xpr.zhaomingkeji.xyz

ROLLBACK TO sp1;
来源：http://bpb.fehbvm.com

[Q69] 查看执行计划
来源：http://lbk.yueranfly.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mev.zhiwuduotai.top

[Q70] 更新统计信息
来源：http://mnr.epnwcf.com

ANALYZE TABLE users;
来源：http://jyi.svipenyu.cn

[Q71] 查看建表语句
来源：http://oaq.yj20258888.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://jsi.haohaochexian.top

[Q72] 查看索引
来源：http://ggu.shzxlz.cn

SHOW INDEX FROM users;
来源：http://pbm.iojbl.cn

[Q73] 查看表状态
来源：http://izm.hnqzz.top

SHOW TABLE STATUS LIKE 'users';
来源：http://vqn.bjfxy.top

[Q74] 强制使用索引
来源：http://nbz.kuanghao11.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://zep.aibaodan.cn

[Q75] 日期格式化
来源：http://eqe.0kj1m.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://lra.sysykeji.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://atx.bjfxy.top

[Q76] 按天统计
来源：http://wev.tianlin.xyz

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ecb.chenzaomai.com

[Q77] 时间加减
来源：http://huj.zhoulong.xyz

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ffy.hammf.cn

[Q78] 当前时间
来源：http://hbv.quarkkingdee.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://kla.ivvv.top

[Q79] 字符串拼接
来源：http://ksk.haohaochexian.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://fdp.jqgufenzy.top

[Q80] 字符串截取
来源：http://gut.ehwqpu.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hjc.cheryme.top

[Q81] 字符串替换
来源：http://ptx.yj20258.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://adj.epnwcf.com

[Q82] 字符长度与字节长度
来源：http://wbg.xinyue.icu

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ksm.xziqi.cn

[Q83] 大小写转换
来源：http://kcb.shuidangran.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ejk.daria6918.cn

[Q84] 去除首尾空格
来源：http://wlp.fengsongda.top

SELECT TRIM(name) FROM users;
来源：http://dds.feifeiyinyue.top

[Q85] 数值取整
来源：http://yef.hywenlv.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://zvw.zdbjq.cn

[Q86] 读取 JSON 字段
来源：http://bta.fehbvm.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ewq.jqgfzy.top

[Q87] JSON 字段做条件
来源：http://jit.cucudq.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://gvp.jqgufenzy.top

[Q88] 行转列（条件聚合）
来源：http://cyt.zhijiandao.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ayk.zhongyouzk.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://jjc.jianghu66.top

[Q89] 判断表是否存在
来源：http://iqe.uphjek.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hsa.redwolf501.top

[Q90] 生成序号列
来源：http://svx.tianlin.xyz

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://bdn.cheryme.top

================================================================================
来源：http://wrx.yanxiufei.cn

R. Bash 专题
来源：http://iwq.zhengqikj.top

================================================================================
来源：http://ixq.gzhubu.top

[R01] shebang 与严格模式
来源：http://bbq.cheryme.top

#!/usr/bin/env bash
来源：http://bov.jinghuilouyu.cn

set -euo pipefail
来源：http://eeu.zhongyouzk.top

[R02] 变量赋值与使用
来源：http://jym.yanxiufei.cn

name="Tom"; echo "$name"
来源：http://fxt.dashuyun.cn

[R03] 只读变量
来源：http://ghg.nanxinkj.top

readonly PI=3.14
来源：http://fko.zhongyouzk.top

[R04] 位置参数
来源：http://hdp.zhongyouzk.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://xvv.bbcook.cn

[R05] 参数默认值
来源：http://cor.andypj.xyz

name="${1:-default}"
来源：http://thj.smart0.xyz

[R06] 判断命令是否存在
来源：http://kea.sufxvd.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://dvo.redwolf501.top

[R07] if 判断文件
来源：http://ngp.jyoumei.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://lkl.hongshengwenyu.top

[R08] 数值比较
来源：http://xen.shangyingyoupin.top

if (( a > b )); then echo "a 更大"; fi
来源：http://nmd.chenjidiqi.icu

[R09] 字符串比较
来源：http://chx.hcnkem.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mub.cdnleiting.top

[R10] 正则匹配
来源：http://mkn.mhx1999.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://dik.9152youxi.cn

[R11] case 多分支
来源：http://dio.sxryk.cn

case "$1" in
来源：http://qqj.gotoacloud.top

start) echo "启动" ;;
来源：http://oiy.epnwcf.com

stop)  echo "停止" ;;
来源：http://yuw.zycfv.cn

*)     echo "未知命令" ;;
来源：http://vke.andypj.xyz

esac
来源：http://kvi.guannengcc.top

[R12] for 遍历文件
来源：http://ial.daxiang520.top

for f in *.txt; do echo "$f"; done
来源：http://hpb.xuetiantiany.cn

[R13] for 计数循环
来源：http://skc.yj20258888.top

for i in {1..10}; do echo "$i"; done
来源：http://wsa.jlsjyb.cn

[R14] C 风格 for
来源：http://ote.yonumen.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://aei.zhoulong.xyz

[R15] while 逐行读文件
来源：http://ktf.fzhhl.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://zxi.cashguo.top

[R16] until 等待条件
来源：http://fsn.vqdsnc.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://kvx.jinghuilouyu.cn

[R17] 数组定义与取值
来源：http://nxq.xziqi.cn

arr=(a b c); echo "${arr[0]}"
来源：http://hsc.zhixingplan.top

[R18] 遍历数组
来源：http://upu.52xcode.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mvr.jinyuanbaomall.cn

[R19] 数组长度
来源：http://wog.c1oappe.top

echo "${#arr[@]}"
来源：http://hwy.jqgfzy.top

[R20] 关联数组（字典）
来源：http://buw.birdmap.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://lfe.epnwcf.com

[R21] 字符串长度
来源：http://rxt.hcnkem.com

echo "${#s}"
来源：http://qgz.smart0.xyz

[R22] 截取子串
来源：http://ynr.tianlin.xyz

echo "${s:0:5}"
来源：http://nnx.meibo888.top

[R23] 字符串替换
来源：http://zba.gotoacloud.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://pnn.316326.xyz

[R24] 大小写转换
来源：http://lzr.sjlbkw.cn

echo "${s^^}"; echo "${s,,}"
来源：http://rrh.jyoumei.cn

[R25] 去后缀 / 去前缀
来源：http://qdj.yj20258.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://zqx.xuetiantiany.cn

[R26] 命令替换
来源：http://vpa.redwolf501.top

now=$(date +%F); echo "$now"
来源：http://bpo.meibo888.top

[R27] 算术展开
来源：http://ipz.redwolf501.top

echo $((1 + 2 * 3))
来源：http://sql.cheryme.top

[R28] 浮点运算
来源：http://wbm.zhaomingkeji.xyz

echo "scale=2; 10/3" | bc
来源：http://xqd.jinqigufen.top

[R29] 定义函数
来源：http://mty.redwolf501.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://gtr.hywenlv.cn

[R30] 函数返回状态码
来源：http://ped.vehdjk.com

f() { return 0; }; f || echo "失败了"
来源：http://fbz.tian-w.cn

[R31] 局部变量
来源：http://lhx.mhx1999.top

f() { local x=1; echo "$x"; }
来源：http://qgu.sufxvd.cn

[R32] 参数个数校验
来源：http://gff.yanxiufei.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://pfu.sweek.top

[R33] 捕获错误并提示行号
来源：http://wrx.chenlongwang.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ued.zhoulong.xyz

[R34] 退出时清理
来源：http://iue.tanke756.top

trap 'rm -f "$tmp"' EXIT
来源：http://wjc.cashguo.top

[R35] 后台执行并等待
来源：http://nqh.bbcook.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ugh.zhoulong.xyz

[R36] 并发执行多个任务
来源：http://rbj.shzxlz.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://cfu.bbcook.cn

[R37] 把输出赋给变量
来源：http://gjy.bjfxy.top

files=$(ls -1)
来源：http://cad.havefunace.top

[R38] 管道串联
来源：http://mxl.nwbrower.top

cat a.txt | grep -i error | wc -l
来源：http://dxs.yangfankeji.com

[R39] 重定向标准输出与错误
来源：http://uro.hcnkem.com

cmd > out.log 2>&1
来源：http://ezm.redwolf501.top

[R40] 追加写日志
来源：http://lkf.aizwys.cn

echo "log" >> out.log
来源：http://euf.wangshuangyany.cn

[R41] 丢弃输出
来源：http://wlx.uphjek.com

cmd >/dev/null 2>&1
来源：http://amj.haohaochexian.top

[R42] 输入重定向
来源：http://rxl.chenlongwang.top

wc -l < a.txt
来源：http://pcf.hywenlv.cn

[R43] 按名字查找文件
来源：http://wlx.zhoulong.xyz

find . -name "*.log" -type f
来源：http://fns.dashuyun.cn

[R44] 按修改时间查找
来源：http://bql.zhaomingkeji.xyz

find . -mtime -7 -type f
来源：http://dtn.jianghu66.top

[R45] 批量删除
来源：http://hyb.iojbl.cn

find . -name "*.tmp" -delete
来源：http://vsj.cheryme.top

[R46] 递归替换文件内容
来源：http://fuk.ywan-chungtsiang.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://odf.nanxinkj.top

[R47] sed 单行替换
来源：http://zaw.gaohongyu789.top

sed -i 's/foo/bar/g' a.txt
来源：http://jxv.tianlin.xyz

[R48] awk 取指定列
来源：http://aug.c1oappe.top

awk '{print $1, $3}' a.txt
来源：http://puo.cucudq.cn

[R49] awk 带条件
来源：http://lku.jyoumei.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://pdy.jinghuilouyu.cn

[R50] awk 求和
来源：http://jxj.chenzaomai.com

awk '{s += $2} END {print s}' a.txt
来源：http://adl.hammf.cn

[R51] 排序去重取前几
来源：http://cqo.hammf.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://rrx.quarkkingdee.top

[R52] 统计行数
来源：http://pzw.fengsongda.top

wc -l a.txt
来源：http://dcx.jiagoushi.top

[R53] 查看文件头与实时尾
来源：http://myr.0kj1m.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://pkp.cucudq.cn

[R54] 比较两个文件
来源：http://tkm.hongshengwenyu.top

diff a.txt b.txt
来源：http://xgx.tian-w.cn

[R55] 压缩与解压
来源：http://pgx.guowangkeji.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://klr.quarkkingdee.top

[R56] 远程拷贝
来源：http://vax.pengpengdd.cyou

scp file user@host:/path/
来源：http://moy.guowangkeji.top

[R57] 远程执行命令
来源：http://afh.jinghuilouyu.cn

ssh user@host 'uptime'
来源：http://act.fengsongda.top

[R58] 下载文件
来源：http://yln.ppjwa.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://xls.jiagoushi.top

[R59] 发 POST JSON
来源：http://fip.316326.xyz

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://fhw.fanxiaobao.xyz

[R60] 只看 HTTP 状态码
来源：http://otj.ywan-chungtsiang.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://aoy.cucudq.cn

[R61] 磁盘占用
来源：http://bid.yangfankeji.com

df -h;  du -sh *
来源：http://mzy.fehbvm.com

[R62] 找最占空间的文件
来源：http://qhk.gotoacloud.top

du -ah . | sort -rh | head -10
来源：http://eys.vqdsnc.cn

[R63] 内存与进程
来源：http://nsf.smart0.xyz

free -h;  ps aux | grep nginx
来源：http://wir.9152youxi.cn

[R64] 结束进程
来源：http://znr.jiagoushi.top

kill -9 $(pgrep -f app.py)
来源：http://ore.yj20258.top

[R65] 查看端口占用
来源：http://axl.tian-w.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wle.jqgfzy.top

[R66] 定时任务
来源：http://mzj.sysykeji.top

crontab -e;  crontab -l
来源：http://lmn.hesvh.cn

[R67] 生成随机十六进制串
来源：http://ima.52xcode.cn


<!-- 参考信息 -->