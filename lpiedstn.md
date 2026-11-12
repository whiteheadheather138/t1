代发 wailian999

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://kib.hesvh.cn

[Q24] 去重
来源：http://vmj.tarul.cn

SELECT DISTINCT city FROM users;
来源：http://iko.smart0.xyz

[Q25] 只取前 N 条
来源：http://kew.xuanzx.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://szy.aizwys.cn

[Q26] 计数
来源：http://gtx.yj202588.top

SELECT COUNT(*) FROM users;
来源：http://glg.fktsv.cn

[Q27] 条件计数
来源：http://slv.hnqzz.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://iem.feifeiyinyue.top

[Q28] 求和与平均
来源：http://tfk.redwolf501.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ozo.yuxming.cn

[Q29] 最大最小值
来源：http://wrw.birdmap.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://oap.hcnkem.com

[Q30] 分组统计
来源：http://col.jyoumei.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://pbi.xuetiantiany.cn

[Q31] 分组后过滤
来源：http://dbb.hammf.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://oop.iojbl.cn

[Q32] 分组拼接字符串
来源：http://xuz.pengpengdd.cyou

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://bwz.0kj1m.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ywk.andypj.xyz

[Q33] 多列分组
来源：http://dgp.dianchejie.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://iyf.yanxiufei.cn

[Q34] 每组取第一条
来源：http://jli.xylfe.cn

SELECT * FROM (
来源：http://rbn.tarul.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://szo.sxryk.cn

) t WHERE rn = 1;
来源：http://rqa.xylfe.cn

[Q35] 内连接
来源：http://wwj.cucudq.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://qir.fehbvm.com

[Q36] 左连接
来源：http://pge.fktsv.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://tmu.svipenyu.cn

[Q37] 右连接
来源：http://bzc.guowangkeji.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://fqg.birdmap.top

[Q38] 全外连接（PostgreSQL）
来源：http://wxx.sufxvd.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wli.ppjwa.cn

[Q39] 自连接（查上下级）
来源：http://qar.gzhubu.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://alh.meibo888.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://kgp.gzhubu.top

[Q40] 交叉连接（笛卡尔积）
来源：http://bam.zhoulong.xyz

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hgp.cucudq.cn

[Q41] 多表连接
来源：http://nfz.fengsongda.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://hxu.shanyushiyangtech.top

JOIN users u ON u.id = o.user_id
来源：http://sgw.zhongyouzk.top

JOIN products p ON p.id = o.product_id;
来源：http://sju.jlsjyb.cn

[Q42] 连接条件附加过滤
来源：http://byk.aibaodan.cn

SELECT u.name, o.amount FROM users u
来源：http://vbc.haohaochexian.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://gto.0kj1m.cn

[Q43] 标量子查询
来源：http://htq.sjlbkw.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://nbn.zhiwuduotai.top

[Q44] IN 子查询
来源：http://nei.ydjk.org.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ilg.fengsongda.top

[Q45] EXISTS 判断存在
来源：http://jub.yfazqb.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://cei.fanxiaobao.xyz

[Q46] NOT EXISTS 判断不存在
来源：http://tyc.quarkkingdee.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zzq.zhoulong.xyz

[Q47] 与平均值比较
来源：http://azy.zycfv.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://znz.ybcxt.top

[Q48] CTE 公用表表达式
来源：http://myq.jqgufenzy.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://iqx.sxryk.cn

SELECT * FROM t WHERE c > 5;
来源：http://mht.shuidangran.top

[Q49] 更新单行
来源：http://klw.hammf.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ifu.zycfv.cn

[Q50] 批量更新
来源：http://lib.haohaochexian.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://kjc.xuanzx.com

[Q51] 用子查询更新
来源：http://efw.meibo888.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://anj.epnwcf.com

[Q52] 删除指定行
来源：http://avq.shanyushiyangtech.top

DELETE FROM users WHERE id = 10;
来源：http://euj.yj20258.top

[Q53] 按条件删除
来源：http://qbv.cucudq.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ejy.xinyue.icu

[Q54] 清空表
来源：http://dmf.sweek.top

TRUNCATE TABLE logs;
来源：http://tdq.yangfankeji.com

[Q55] 排名（并列占位）
来源：http://znn.sweek.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://crs.zhijiandao.cn

[Q56] 密集排名（并列不占位）
来源：http://baz.gotoacloud.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://bto.zhongyouzk.top

[Q57] 行号
来源：http://laz.ctjpmb.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wqt.tian-w.cn

[Q58] 累计求和
来源：http://zeu.9152youxi.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://pxo.yvedp.cn

[Q59] 分组内累计
来源：http://egs.aizwys.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ilw.guowangkeji.top

[Q60] 取上一行 / 下一行
来源：http://fje.cqqwz.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://uur.hesvh.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://tsu.pengpengdd.cyou

[Q61] 移动平均
来源：http://yfg.zhijiandao.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://sve.daxiang520.top

[Q62] 分组占比
来源：http://wjv.hesvh.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://uyn.mhx1999.top

[Q63] 开启事务
来源：http://uuz.smart0.xyz

START TRANSACTION;                -- 或 BEGIN
来源：http://oiu.jinyuanbaomall.cn

[Q64] 提交事务
来源：http://rlg.sufxvd.cn

COMMIT;
来源：http://fpw.fzhhl.top

[Q65] 回滚事务
来源：http://gfc.sweek.top

ROLLBACK;
来源：http://fiv.chenlongwang.top

[Q66] 行锁查询
来源：http://knt.fengsongda.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://jmq.tian-w.cn

[Q67] 设置隔离级别
来源：http://tar.zycfv.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://pxg.hysaishi.cn

[Q68] 保存点
来源：http://ubv.snrcjt.cn

SAVEPOINT sp1;
来源：http://rzn.jlsjyb.cn

ROLLBACK TO sp1;
来源：http://rhs.jinghuilouyu.cn

[Q69] 查看执行计划
来源：http://ukl.cashguo.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://svs.c1oappe.top

[Q70] 更新统计信息
来源：http://vdb.yuanzhike.top

ANALYZE TABLE users;
来源：http://hzc.zhoulong.xyz

[Q71] 查看建表语句
来源：http://pqi.xuanzx.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://kdu.guannengcc.top

[Q72] 查看索引
来源：http://jum.smart0.xyz

SHOW INDEX FROM users;
来源：http://jhw.epnwcf.com

[Q73] 查看表状态
来源：http://fbm.yj20258.top

SHOW TABLE STATUS LIKE 'users';
来源：http://rns.fengsongda.top

[Q74] 强制使用索引
来源：http://vaw.nanxuanxn.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ber.fengsongda.top

[Q75] 日期格式化
来源：http://blq.zhongyouzk.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://fdo.0kj1m.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://esw.zhaomingkeji.xyz

[Q76] 按天统计
来源：http://fgs.hysaishi.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://xvy.wangshuangyany.cn

[Q77] 时间加减
来源：http://xui.ydzc1.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://rcs.andypj.xyz

[Q78] 当前时间
来源：http://sni.vqdsnc.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://kha.chenjidiqi.icu

[Q79] 字符串拼接
来源：http://prc.birdmap.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://xsa.jinghuilouyu.cn

[Q80] 字符串截取
来源：http://liu.pengpengdd.cyou

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://pua.zhengqikj.top

[Q81] 字符串替换
来源：http://hvt.sxryk.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://avp.smart0.xyz

[Q82] 字符长度与字节长度
来源：http://ell.quarkkingdee.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://gkg.jinqigufen.top

[Q83] 大小写转换
来源：http://fpj.yanxiufei.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://cym.hongshengwenyu.top

[Q84] 去除首尾空格
来源：http://mgv.xylfe.cn

SELECT TRIM(name) FROM users;
来源：http://jir.haohaochexian.top

[Q85] 数值取整
来源：http://bzn.fzhhl.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ftj.ywan-chungtsiang.top

[Q86] 读取 JSON 字段
来源：http://pfl.yuanzhike.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://msg.chenjidiqi.icu

[Q87] JSON 字段做条件
来源：http://vzb.nwbrower.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://poh.nwbrower.top

[Q88] 行转列（条件聚合）
来源：http://tlu.nanxinkj.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://iaj.uphjek.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://jnf.hnqzz.top

[Q89] 判断表是否存在
来源：http://kyf.0kj1m.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wve.xinyue.icu

[Q90] 生成序号列
来源：http://czx.quarkkingdee.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://oxy.yj20258.top

================================================================================
来源：http://kzv.fzhhl.top

R. Bash 专题
来源：http://hvs.guannengcc.top

================================================================================
来源：http://njk.chenlongwang.top

[R01] shebang 与严格模式
来源：http://xjb.snrcjt.cn

#!/usr/bin/env bash
来源：http://wnf.hammf.cn

set -euo pipefail
来源：http://lxt.hfpthk.cn

[R02] 变量赋值与使用
来源：http://sfn.jqgufenzy.top

name="Tom"; echo "$name"
来源：http://mas.uphjek.com

[R03] 只读变量
来源：http://zqw.jinghuilouyu.cn

readonly PI=3.14
来源：http://xrc.sweek.top

[R04] 位置参数
来源：http://xlr.fehbvm.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://uxu.nanxuanxn.top

[R05] 参数默认值
来源：http://ahf.ybcxt.top

name="${1:-default}"
来源：http://met.wangdashe.top

[R06] 判断命令是否存在
来源：http://ifq.fzhhl.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://gxq.iojbl.cn

[R07] if 判断文件
来源：http://tac.shanyushiyangtech.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://rwd.xuanzx.com

[R08] 数值比较
来源：http://ugk.birdmap.top

if (( a > b )); then echo "a 更大"; fi
来源：http://dgk.zhijiandao.cn

[R09] 字符串比较
来源：http://uee.shangyingyoupin.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://rtl.epnwcf.com

[R10] 正则匹配
来源：http://uad.chenzaomai.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://nbg.uphjek.com

[R11] case 多分支
来源：http://qvc.zhijiandao.cn

case "$1" in
来源：http://kpm.zhoulong.xyz

start) echo "启动" ;;
来源：http://hdw.ehwqpu.com

stop)  echo "停止" ;;
来源：http://yhf.52xcode.cn

*)     echo "未知命令" ;;
来源：http://yvf.gotoacloud.top

esac
来源：http://lum.yj202588.top

[R12] for 遍历文件
来源：http://kjo.sxryk.cn

for f in *.txt; do echo "$f"; done
来源：http://joi.mhx1999.top

[R13] for 计数循环
来源：http://vkr.bbcook.cn

for i in {1..10}; do echo "$i"; done
来源：http://erx.zhoulong.xyz

[R14] C 风格 for
来源：http://hwk.dianchejie.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ijl.hesvh.cn

[R15] while 逐行读文件
来源：http://qnb.pycfn.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://say.jqgufenzy.top

[R16] until 等待条件
来源：http://poc.yfazqb.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hvv.gaohongyu789.top

[R17] 数组定义与取值
来源：http://zyt.gaohongyu789.top

arr=(a b c); echo "${arr[0]}"
来源：http://ybt.gogol.net.cn

[R18] 遍历数组
来源：http://xnz.mhx1999.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://azz.smart0.xyz

[R19] 数组长度
来源：http://vaz.haohaochexian.top

echo "${#arr[@]}"
来源：http://kiw.yj20258.top

[R20] 关联数组（字典）
来源：http://wko.bjfxy.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://kgs.feifeiyinyue.top

[R21] 字符串长度
来源：http://rqf.andypj.xyz

echo "${#s}"
来源：http://dqi.aizwys.cn

[R22] 截取子串
来源：http://kqd.epnwcf.com

echo "${s:0:5}"
来源：http://cdz.shzxlz.cn

[R23] 字符串替换
来源：http://rnf.316326.xyz

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://qoj.chenlongwang.top

[R24] 大小写转换
来源：http://qrn.vehdjk.com

echo "${s^^}"; echo "${s,,}"
来源：http://smf.jinqigfzy.top

[R25] 去后缀 / 去前缀
来源：http://pbt.ehwqpu.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://zgu.sxryk.cn

[R26] 命令替换
来源：http://xum.tianlin.xyz

now=$(date +%F); echo "$now"
来源：http://att.fktsv.cn

[R27] 算术展开
来源：http://lsv.nwbrower.top

echo $((1 + 2 * 3))
来源：http://bru.zhijiandao.cn

[R28] 浮点运算
来源：http://rsq.cqqwz.cn

echo "scale=2; 10/3" | bc
来源：http://liv.ywan-chungtsiang.top

[R29] 定义函数
来源：http://acu.yj202588.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://fga.sufxvd.cn

[R30] 函数返回状态码
来源：http://maa.zhixingplan.top

f() { return 0; }; f || echo "失败了"
来源：http://qlr.ybcxt.top

[R31] 局部变量
来源：http://ggw.zhijiandao.cn

f() { local x=1; echo "$x"; }
来源：http://iej.fktsv.cn

[R32] 参数个数校验
来源：http://kbo.jiagoushi.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://heq.aizwys.cn

[R33] 捕获错误并提示行号
来源：http://hbs.chenjidiqi.icu

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://lfi.fehbvm.com

[R34] 退出时清理
来源：http://zty.ppjwa.cn

trap 'rm -f "$tmp"' EXIT
来源：http://njp.ehwqpu.com

[R35] 后台执行并等待
来源：http://bpj.jinghuilouyu.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://mnx.jqgufenzy.top

[R36] 并发执行多个任务
来源：http://ikx.gogol.net.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://elg.yangfankeji.com

[R37] 把输出赋给变量
来源：http://aws.shangyingyoupin.top

files=$(ls -1)
来源：http://coy.nwbrower.top

[R38] 管道串联
来源：http://rbs.zhixingplan.top

cat a.txt | grep -i error | wc -l
来源：http://ebs.xylfe.cn

[R39] 重定向标准输出与错误
来源：http://zbe.yfazqb.com

cmd > out.log 2>&1
来源：http://wtq.xylfe.cn

[R40] 追加写日志
来源：http://sya.yonumen.top

echo "log" >> out.log
来源：http://mvm.sysykeji.top

[R41] 丢弃输出
来源：http://auq.fktsv.cn

cmd >/dev/null 2>&1
来源：http://tyd.pycfn.com

[R42] 输入重定向
来源：http://ptq.tarul.cn

wc -l < a.txt
来源：http://onp.bjfxy.top

[R43] 按名字查找文件
来源：http://thm.aizwys.cn

find . -name "*.log" -type f
来源：http://guq.svipenyu.cn

[R44] 按修改时间查找
来源：http://wdg.fktsv.cn

find . -mtime -7 -type f
来源：http://szw.yj202588.top

[R45] 批量删除
来源：http://kkv.tarul.cn

find . -name "*.tmp" -delete
来源：http://cyc.zhengqikj.top

[R46] 递归替换文件内容
来源：http://wgr.yj20258.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://fdw.xingfuxueyuan.xyz

[R47] sed 单行替换
来源：http://gqj.yongpay.top

sed -i 's/foo/bar/g' a.txt
来源：http://eyf.jqgfzy.top

[R48] awk 取指定列
来源：http://yew.bjfxy.top

awk '{print $1, $3}' a.txt
来源：http://izx.andypj.xyz

[R49] awk 带条件
来源：http://bjt.haohaochexian.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://rkw.jianghu66.top

[R50] awk 求和
来源：http://wiv.ctjpmb.com

awk '{s += $2} END {print s}' a.txt
来源：http://gwz.jinqigfzy.top

[R51] 排序去重取前几
来源：http://umf.chenzaomai.com

sort a.txt | uniq -c | sort -rn | head
来源：http://ghr.yj202588.top

[R52] 统计行数
来源：http://zqe.iojbl.cn

wc -l a.txt
来源：http://hap.shzxlz.cn

[R53] 查看文件头与实时尾
来源：http://wlw.gzhubu.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://uzp.nwbrower.top

[R54] 比较两个文件
来源：http://xlp.fzhhl.top

diff a.txt b.txt
来源：http://ruu.cashguo.top

[R55] 压缩与解压
来源：http://ocq.pycfn.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://oqe.ywan-chungtsiang.top

[R56] 远程拷贝
来源：http://sqw.yonumen.top

scp file user@host:/path/
来源：http://alz.jqgufenzy.top

[R57] 远程执行命令
来源：http://iyl.bbcook.cn

ssh user@host 'uptime'
来源：http://taa.zhiwuduotai.top

[R58] 下载文件
来源：http://dsj.yueranfly.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ssa.xuanzx.com

[R59] 发 POST JSON
来源：http://qiq.ivvv.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://inn.smart0.xyz

[R60] 只看 HTTP 状态码
来源：http://vfy.0kj1m.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://xph.0kj1m.cn

[R61] 磁盘占用
来源：http://aii.ctjpmb.com

df -h;  du -sh *
来源：http://dkg.uphjek.com

[R62] 找最占空间的文件
来源：http://bvn.aibaodan.cn

du -ah . | sort -rh | head -10
来源：http://kcd.tanke756.top

[R63] 内存与进程
来源：http://rvw.nanxinkj.top

free -h;  ps aux | grep nginx
来源：http://sxx.daxiang520.top

[R64] 结束进程
来源：http://duq.tanke756.top

kill -9 $(pgrep -f app.py)
来源：http://hxi.zhiwuduotai.top

[R65] 查看端口占用
来源：http://jyp.jqgufenzy.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://tvi.vehdjk.com

[R66] 定时任务
来源：http://jhb.hammf.cn

crontab -e;  crontab -l
来源：http://gsk.havefunace.top

[R67] 生成随机十六进制串
来源：http://fri.guannengcc.top

openssl rand -hex 16
来源：http://lbg.gotoacloud.top

[R68] 计算文件校验值
来源：http://lsq.hcnkem.com

sha256sum a.txt;  md5sum a.txt
来源：http://whp.hesvh.cn

[R69] 生成随机密码
来源：http://uvh.jinqigfzy.top

head -c 16 /dev/urandom | base64
来源：http://jdw.yongpay.top

[R70] 时间戳与互转
来源：http://mkr.sjlbkw.cn

date +%s;  date -d @1700000000
来源：http://rod.wangdashe.top

[R71] 日期格式化
来源：http://bmb.sxryk.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ngw.cdnleiting.top

[R72] 等待端口就绪
来源：http://geu.nanxuanxn.top

until nc -z localhost 3306; do sleep 1; done
来源：http://vly.cucudq.cn

[R73] 分割大日志
来源：http://nbj.xuetiantiany.cn


<!-- 参考信息 -->