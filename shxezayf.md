代发 wailian999

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://lwj.yvedp.cn

[Q20] IN 列表
来源：http://ues.9152youxi.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://azv.chenlongwang.top

[Q21] 空值判断
来源：http://ngw.gaohongyu789.top

SELECT * FROM users WHERE email IS NULL;
来源：http://xod.cdnleiting.top

[Q22] 排序
来源：http://gvc.zhoulong.xyz

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://xfr.nanxinkj.top

[Q23] 分页
来源：http://ubz.nanxinkj.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://vrb.aizwys.cn

[Q24] 去重
来源：http://dxv.fktsv.cn

SELECT DISTINCT city FROM users;
来源：http://rzv.yj202588.top

[Q25] 只取前 N 条
来源：http://dja.sufxvd.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wng.nanxinkj.top

[Q26] 计数
来源：http://piz.andypj.xyz

SELECT COUNT(*) FROM users;
来源：http://mhc.zhengqikj.top

[Q27] 条件计数
来源：http://ncn.shangyingyoupin.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ygc.daxiang520.top

[Q28] 求和与平均
来源：http://wax.sysykeji.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://cxl.chenjidiqi.icu

[Q29] 最大最小值
来源：http://cok.52xcode.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://nwf.cdnleiting.top

[Q30] 分组统计
来源：http://yly.jianghu66.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://axs.gotoacloud.top

[Q31] 分组后过滤
来源：http://ioe.jlsjyb.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://tqe.wangdashe.top

[Q32] 分组拼接字符串
来源：http://hpk.uphjek.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://vqr.zdqjudy.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ouo.hnqzz.top

[Q33] 多列分组
来源：http://nxs.ywan-chungtsiang.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://abc.chenlongwang.top

[Q34] 每组取第一条
来源：http://yso.chenjidiqi.icu

SELECT * FROM (
来源：http://zpj.yueranfly.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ict.shuidangran.top

) t WHERE rn = 1;
来源：http://trg.tarul.cn

[Q35] 内连接
来源：http://kbm.hnxiangtu.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mcl.pycfn.com

[Q36] 左连接
来源：http://zup.aibaodan.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://xsk.feifeiyinyue.top

[Q37] 右连接
来源：http://rnd.daxiang520.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://rrw.aizwys.cn

[Q38] 全外连接（PostgreSQL）
来源：http://elj.meibo888.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://zbo.wangshuangyany.cn

[Q39] 自连接（查上下级）
来源：http://qok.zhaomingkeji.xyz

SELECT e.name, m.name AS manager FROM employees e
来源：http://ecy.hesvh.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mds.sjlbkw.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://sya.chenlongwang.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ixo.shangyingyoupin.top

[Q41] 多表连接
来源：http://uhi.dashuyun.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://xfr.cucudq.cn

JOIN users u ON u.id = o.user_id
来源：http://tgg.hnqzz.top

JOIN products p ON p.id = o.product_id;
来源：http://quk.c1oappe.top

[Q42] 连接条件附加过滤
来源：http://hqd.yangfankeji.com

SELECT u.name, o.amount FROM users u
来源：http://ojd.yj20258.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://riv.vqdsnc.cn

[Q43] 标量子查询
来源：http://lwm.jinghuilouyu.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ovu.jianghu66.top

[Q44] IN 子查询
来源：http://igq.tianlin.xyz

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://nom.feifeiyinyue.top

[Q45] EXISTS 判断存在
来源：http://wdz.fehbvm.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wmi.smart0.xyz

[Q46] NOT EXISTS 判断不存在
来源：http://ywx.zhongyouzk.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://miw.yuanzhike.top

[Q47] 与平均值比较
来源：http://txk.tian-w.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://gkq.feifeiyinyue.top

[Q48] CTE 公用表表达式
来源：http://dih.shuidangran.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://nqc.jinyuanbaomall.cn

SELECT * FROM t WHERE c > 5;
来源：http://myr.hammf.cn

[Q49] 更新单行
来源：http://dsm.ehwqpu.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://phl.ywan-chungtsiang.top

[Q50] 批量更新
来源：http://rjg.bjfxy.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://iqu.havefunace.top

[Q51] 用子查询更新
来源：http://gut.hysaishi.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://kmj.aizwys.cn

[Q52] 删除指定行
来源：http://pvu.yj202588.top

DELETE FROM users WHERE id = 10;
来源：http://cpc.ivvv.top

[Q53] 按条件删除
来源：http://uha.tian-w.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://oos.zdqjudy.top

[Q54] 清空表
来源：http://mfq.shanyushiyangtech.top

TRUNCATE TABLE logs;
来源：http://nbr.tarul.cn

[Q55] 排名（并列占位）
来源：http://wgv.yj202588.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://byp.dianchejie.cn

[Q56] 密集排名（并列不占位）
来源：http://asd.zhoulong.xyz

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://rkx.jinqigufen.top

[Q57] 行号
来源：http://ltx.svipenyu.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://erm.yuanzhike.top

[Q58] 累计求和
来源：http://aqd.c1oappe.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://chd.uphjek.com

[Q59] 分组内累计
来源：http://ohx.vqdsnc.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://zgt.c1oappe.top

[Q60] 取上一行 / 下一行
来源：http://ygu.kuanghao11.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ert.gaohongyu789.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://faj.ppjwa.cn

[Q61] 移动平均
来源：http://ofy.jqgufenzy.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://cie.0kj1m.cn

[Q62] 分组占比
来源：http://bpo.yonumen.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://qms.cqqwz.cn

[Q63] 开启事务
来源：http://dxl.hongshengwenyu.top

START TRANSACTION;                -- 或 BEGIN
来源：http://gsq.c1oappe.top

[Q64] 提交事务
来源：http://lvf.cqqwz.cn

COMMIT;
来源：http://qgj.shanyushiyangkeji.top

[Q65] 回滚事务
来源：http://ksu.iojbl.cn

ROLLBACK;
来源：http://ais.cheryme.top

[Q66] 行锁查询
来源：http://emj.jinqigufen.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://kzw.zhaomingkeji.xyz

[Q67] 设置隔离级别
来源：http://qwc.zdqjudy.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://akh.jyoumei.cn

[Q68] 保存点
来源：http://gua.zdbjq.cn

SAVEPOINT sp1;
来源：http://pkn.zhiwuduotai.top

ROLLBACK TO sp1;
来源：http://zsb.hcnkem.com

[Q69] 查看执行计划
来源：http://tld.nanxuanxn.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wbi.jiagoushi.top

[Q70] 更新统计信息
来源：http://ave.ybcxt.top

ANALYZE TABLE users;
来源：http://ilr.ywan-chungtsiang.top

[Q71] 查看建表语句
来源：http://axq.shanyushiyangkeji.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hzf.hongshengwenyu.top

[Q72] 查看索引
来源：http://uec.yonumen.top

SHOW INDEX FROM users;
来源：http://tey.cqqwz.cn

[Q73] 查看表状态
来源：http://knn.jyoumei.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://cfo.nanxuanxn.top

[Q74] 强制使用索引
来源：http://rep.cdnleiting.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://tpd.sxryk.cn

[Q75] 日期格式化
来源：http://yyq.kuanghao11.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://icr.chenjidiqi.icu

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://nfw.zycfv.cn

[Q76] 按天统计
来源：http://off.xingfuxueyuan.xyz

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ovp.jianghu66.top

[Q77] 时间加减
来源：http://qft.nanxuanxn.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://eox.0kj1m.cn

[Q78] 当前时间
来源：http://aod.shzxlz.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ivm.pycfn.com

[Q79] 字符串拼接
来源：http://pkd.0kj1m.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://qqp.ybcxt.top

[Q80] 字符串截取
来源：http://onu.zhijiandao.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://xqk.sjlbkw.cn

[Q81] 字符串替换
来源：http://wzl.zhixingplan.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://qdn.yvedp.cn

[Q82] 字符长度与字节长度
来源：http://wtr.sxryk.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://odx.xuetiantiany.cn

[Q83] 大小写转换
来源：http://kyx.redwolf501.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://qju.gotoacloud.top

[Q84] 去除首尾空格
来源：http://orf.zhongyouzk.top

SELECT TRIM(name) FROM users;
来源：http://dtv.zhoulong.xyz

[Q85] 数值取整
来源：http://vil.hesvh.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hts.yanxiufei.cn

[Q86] 读取 JSON 字段
来源：http://gxf.jqgfzy.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://bvc.ppjwa.cn

[Q87] JSON 字段做条件
来源：http://hiw.cashguo.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://jau.fengsongda.top

[Q88] 行转列（条件聚合）
来源：http://aky.jqgfzy.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://cbj.dianchejie.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hlz.bbcook.cn

[Q89] 判断表是否存在
来源：http://cho.jinyuanbaomall.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://bbv.guowangkeji.top

[Q90] 生成序号列
来源：http://koq.epnwcf.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://htd.xziqi.cn

================================================================================
来源：http://vaw.feifeiyinyue.top

R. Bash 专题
来源：http://dbq.ehwqpu.com

================================================================================
来源：http://uzn.sufxvd.cn

[R01] shebang 与严格模式
来源：http://prz.cheryme.top

#!/usr/bin/env bash
来源：http://edc.gotoacloud.top

set -euo pipefail
来源：http://ibn.havefunace.top

[R02] 变量赋值与使用
来源：http://tvf.ehwqpu.com

name="Tom"; echo "$name"
来源：http://non.hnqzz.top

[R03] 只读变量
来源：http://pgj.aizwys.cn

readonly PI=3.14
来源：http://klf.snrcjt.cn

[R04] 位置参数
来源：http://mgr.guannengcc.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://vkc.haohaochexian.top

[R05] 参数默认值
来源：http://lga.haohaochexian.top

name="${1:-default}"
来源：http://tzc.shzxlz.cn

[R06] 判断命令是否存在
来源：http://esm.hcnkem.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://xjv.kuanghao11.cn

[R07] if 判断文件
来源：http://xgs.daxiang520.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://gir.ywan-chungtsiang.top

[R08] 数值比较
来源：http://njy.mhx1999.top

if (( a > b )); then echo "a 更大"; fi
来源：http://zue.redwolf501.top

[R09] 字符串比较
来源：http://cvu.hywenlv.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hhf.shuidangran.top

[R10] 正则匹配
来源：http://ecp.zycfv.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ltl.hcnkem.com

[R11] case 多分支
来源：http://jsj.gogol.net.cn

case "$1" in
来源：http://vaj.cheryme.top

start) echo "启动" ;;
来源：http://dez.yj202588.top

stop)  echo "停止" ;;
来源：http://rjs.nanxuanxn.top

*)     echo "未知命令" ;;
来源：http://mfq.birdmap.top

esac
来源：http://hss.haohaochexian.top

[R12] for 遍历文件
来源：http://egy.redwolf501.top

for f in *.txt; do echo "$f"; done
来源：http://gvg.uphjek.com

[R13] for 计数循环
来源：http://irm.jlsjyb.cn

for i in {1..10}; do echo "$i"; done
来源：http://bta.ehwqpu.com

[R14] C 风格 for
来源：http://fhe.gaohongyu789.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://jal.jinghuilouyu.cn

[R15] while 逐行读文件
来源：http://yqn.jiagoushi.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://rwc.cdnleiting.top

[R16] until 等待条件
来源：http://isy.ybcxt.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://spb.feifeiyinyue.top

[R17] 数组定义与取值
来源：http://pee.haohaochexian.top

arr=(a b c); echo "${arr[0]}"
来源：http://uni.wangdashe.top

[R18] 遍历数组
来源：http://ikj.yanxiufei.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://dlm.zhixingplan.top

[R19] 数组长度
来源：http://vgx.tianlin.xyz

echo "${#arr[@]}"
来源：http://xnq.aizwys.cn

[R20] 关联数组（字典）
来源：http://yrp.guowangkeji.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://dpq.uphjek.com

[R21] 字符串长度
来源：http://fup.fengsongda.top

echo "${#s}"
来源：http://wpd.ppjwa.cn

[R22] 截取子串
来源：http://hzo.jianghu66.top

echo "${s:0:5}"
来源：http://olk.jlsjyb.cn

[R23] 字符串替换
来源：http://kqs.andypj.xyz

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://trk.52xcode.cn

[R24] 大小写转换
来源：http://opd.andypj.xyz

echo "${s^^}"; echo "${s,,}"
来源：http://nnh.redwolf501.top

[R25] 去后缀 / 去前缀
来源：http://fco.aizwys.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://wox.jinghuilouyu.cn

[R26] 命令替换
来源：http://plw.guannengcc.top

now=$(date +%F); echo "$now"
来源：http://mwv.vehdjk.com

[R27] 算术展开
来源：http://vww.yongpay.top

echo $((1 + 2 * 3))
来源：http://mjg.yangfankeji.com

[R28] 浮点运算
来源：http://ahu.tianlin.xyz

echo "scale=2; 10/3" | bc
来源：http://grf.jinqigfzy.top

[R29] 定义函数
来源：http://pqk.svipenyu.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://arx.vehdjk.com

[R30] 函数返回状态码
来源：http://aeo.hongshengwenyu.top

f() { return 0; }; f || echo "失败了"
来源：http://uwr.fzhhl.top

[R31] 局部变量
来源：http://xsy.cheryme.top

f() { local x=1; echo "$x"; }
来源：http://sby.shanyushiyangtech.top

[R32] 参数个数校验
来源：http://vnl.gotoacloud.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://yay.yuxming.cn

[R33] 捕获错误并提示行号
来源：http://eal.aibaodan.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://gue.zdqjudy.top

[R34] 退出时清理
来源：http://abm.ywan-chungtsiang.top

trap 'rm -f "$tmp"' EXIT
来源：http://hst.jqgufenzy.top

[R35] 后台执行并等待
来源：http://gru.sweek.top

sleep 5 & pid=$!; wait "$pid"
来源：http://jib.hysaishi.cn

[R36] 并发执行多个任务
来源：http://ijd.quarkkingdee.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ykd.svipenyu.cn

[R37] 把输出赋给变量
来源：http://tuu.hnqzz.top

files=$(ls -1)
来源：http://ycv.ywan-chungtsiang.top

[R38] 管道串联
来源：http://ggk.wangshuangyany.cn

cat a.txt | grep -i error | wc -l
来源：http://lsq.andypj.xyz

[R39] 重定向标准输出与错误
来源：http://kvt.meibo888.top

cmd > out.log 2>&1
来源：http://vun.quarkkingdee.top

[R40] 追加写日志
来源：http://gab.yangfankeji.com

echo "log" >> out.log
来源：http://ibl.zhiwuduotai.top

[R41] 丢弃输出
来源：http://uvw.chenjidiqi.icu

cmd >/dev/null 2>&1
来源：http://erh.9152youxi.cn

[R42] 输入重定向
来源：http://aqg.chenzaomai.com

wc -l < a.txt
来源：http://yfr.fehbvm.com

[R43] 按名字查找文件
来源：http://sis.ydzc1.top

find . -name "*.log" -type f
来源：http://etk.dashuyun.cn

[R44] 按修改时间查找
来源：http://kxr.zhaomingkeji.xyz

find . -mtime -7 -type f
来源：http://uvx.sufxvd.cn

[R45] 批量删除
来源：http://hht.jqgfzy.top

find . -name "*.tmp" -delete
来源：http://ieu.xziqi.cn

[R46] 递归替换文件内容
来源：http://stg.daxiang520.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://fur.zdbjq.cn

[R47] sed 单行替换
来源：http://ace.andypj.xyz

sed -i 's/foo/bar/g' a.txt
来源：http://vxn.pycfn.com

[R48] awk 取指定列
来源：http://hvg.bbcook.cn

awk '{print $1, $3}' a.txt
来源：http://xja.0kj1m.cn

[R49] awk 带条件
来源：http://ylj.cheryme.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ozo.fktsv.cn

[R50] awk 求和
来源：http://ppk.xuanzx.com

awk '{s += $2} END {print s}' a.txt
来源：http://zsi.hongshengwenyu.top

[R51] 排序去重取前几
来源：http://zoq.gogol.net.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://gga.haohaochexian.top

[R52] 统计行数
来源：http://eir.tianlin.xyz

wc -l a.txt
来源：http://vun.aibaodan.cn

[R53] 查看文件头与实时尾
来源：http://sfe.chenzaomai.com

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://qhn.hammf.cn

[R54] 比较两个文件
来源：http://owk.guowangkeji.top

diff a.txt b.txt
来源：http://grq.shanyushiyangtech.top

[R55] 压缩与解压
来源：http://atd.hywenlv.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://oqe.ydzc1.top

[R56] 远程拷贝
来源：http://nwj.tarul.cn

scp file user@host:/path/
来源：http://kjq.shanyushiyangtech.top

[R57] 远程执行命令
来源：http://oiq.jinghuilouyu.cn

ssh user@host 'uptime'
来源：http://khc.zhijiandao.cn

[R58] 下载文件
来源：http://uux.daria6918.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://fwy.yj20258.top

[R59] 发 POST JSON
来源：http://kxl.shuidangran.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ohm.cdnleiting.top

[R60] 只看 HTTP 状态码
来源：http://jcb.sweek.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://vok.hammf.cn

[R61] 磁盘占用
来源：http://pdz.ybcxt.top

df -h;  du -sh *
来源：http://osr.sxryk.cn

[R62] 找最占空间的文件
来源：http://hxl.yuanzhike.top

du -ah . | sort -rh | head -10
来源：http://cny.nanxuanxn.top

[R63] 内存与进程
来源：http://hwo.sysykeji.top

free -h;  ps aux | grep nginx
来源：http://hds.jinyuanbaomall.cn

[R64] 结束进程
来源：http://zwg.wangdashe.top

kill -9 $(pgrep -f app.py)
来源：http://zzc.sysykeji.top

[R65] 查看端口占用
来源：http://otk.bbcook.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wzc.c1oappe.top

[R66] 定时任务
来源：http://doh.svipenyu.cn

crontab -e;  crontab -l
来源：http://rlr.yonumen.top

[R67] 生成随机十六进制串
来源：http://iyf.guannengcc.top

openssl rand -hex 16
来源：http://jih.nanxinkj.top

[R68] 计算文件校验值
来源：http://fou.xuetiantiany.cn

sha256sum a.txt;  md5sum a.txt
来源：http://gcs.jinghuilouyu.cn

[R69] 生成随机密码
来源：http://egg.jqgufenzy.top


<!-- 参考信息 -->