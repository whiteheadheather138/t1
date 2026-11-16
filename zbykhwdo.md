代发 wailian999

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ksq.nanxinkj.top

[Q18] 模糊匹配
来源：http://jrj.tarul.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mgw.feifeiyinyue.top

[Q19] 范围查询
来源：http://rlv.yuxming.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wzg.tarul.cn

[Q20] IN 列表
来源：http://lpr.andypj.xyz

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://nxd.xuanzx.com

[Q21] 空值判断
来源：http://bnv.ydjk.org.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://kql.shanyushiyangkeji.top

[Q22] 排序
来源：http://vrq.ydjk.org.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ukj.bjfxy.top

[Q23] 分页
来源：http://wxm.kuanghao11.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://nrp.gotoacloud.top

[Q24] 去重
来源：http://cii.shangyingyoupin.top

SELECT DISTINCT city FROM users;
来源：http://ukh.zhijiandao.cn

[Q25] 只取前 N 条
来源：http://eud.ivvv.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://bgm.chenjidiqi.icu

[Q26] 计数
来源：http://owi.guannengcc.top

SELECT COUNT(*) FROM users;
来源：http://bzz.shanyushiyangtech.top

[Q27] 条件计数
来源：http://foj.tarul.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://amn.ivvv.top

[Q28] 求和与平均
来源：http://jhv.nanxuanxn.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hga.yuanzhike.top

[Q29] 最大最小值
来源：http://qnj.guannengcc.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://kyp.shanyushiyangtech.top

[Q30] 分组统计
来源：http://ozf.aibaodan.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hpz.ywan-chungtsiang.top

[Q31] 分组后过滤
来源：http://tyq.shanyushiyangkeji.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ike.sweek.top

[Q32] 分组拼接字符串
来源：http://znl.epnwcf.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://qis.jianghu66.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://nrh.hammf.cn

[Q33] 多列分组
来源：http://jer.aibaodan.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://yaq.tarul.cn

[Q34] 每组取第一条
来源：http://tgq.yonumen.top

SELECT * FROM (
来源：http://rrl.zdbjq.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://vye.andypj.xyz

) t WHERE rn = 1;
来源：http://jtf.zycfv.cn

[Q35] 内连接
来源：http://sdx.sysykeji.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wcv.dashuyun.cn

[Q36] 左连接
来源：http://rsj.yj20258888.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://xrq.yueranfly.top

[Q37] 右连接
来源：http://lxn.jyoumei.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://exk.chenjidiqi.icu

[Q38] 全外连接（PostgreSQL）
来源：http://zwh.ybcxt.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wmd.gotoacloud.top

[Q39] 自连接（查上下级）
来源：http://vul.mhx1999.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://tye.c1oappe.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://nve.sweek.top

[Q40] 交叉连接（笛卡尔积）
来源：http://cxw.cqqwz.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://jht.birdmap.top

[Q41] 多表连接
来源：http://qrs.hnxiangtu.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://qew.hysaishi.cn

JOIN users u ON u.id = o.user_id
来源：http://hqa.pycfn.com

JOIN products p ON p.id = o.product_id;
来源：http://bnr.jianghu66.top

[Q42] 连接条件附加过滤
来源：http://bjn.uphjek.com

SELECT u.name, o.amount FROM users u
来源：http://txk.fehbvm.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://jju.gzhubu.top

[Q43] 标量子查询
来源：http://xjw.zhaomingkeji.xyz

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ctg.andypj.xyz

[Q44] IN 子查询
来源：http://mgt.zhijiandao.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://qlg.gaohongyu789.top

[Q45] EXISTS 判断存在
来源：http://kfs.hnxiangtu.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kyr.sxryk.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ljz.guowangkeji.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kkc.cashguo.top

[Q47] 与平均值比较
来源：http://iko.jinqigufen.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wdr.daria6918.cn

[Q48] CTE 公用表表达式
来源：http://zpw.sxryk.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mzq.gaohongyu789.top

SELECT * FROM t WHERE c > 5;
来源：http://mav.52xcode.cn

[Q49] 更新单行
来源：http://tyo.cheryme.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://rfd.cucudq.cn

[Q50] 批量更新
来源：http://qzi.zdqjudy.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wdw.havefunace.top

[Q51] 用子查询更新
来源：http://hfv.zhaomingkeji.xyz

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://xtg.gogol.net.cn

[Q52] 删除指定行
来源：http://fjx.ehwqpu.com

DELETE FROM users WHERE id = 10;
来源：http://pcr.hfpthk.cn

[Q53] 按条件删除
来源：http://dej.cucudq.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://jjn.fzhhl.top

[Q54] 清空表
来源：http://yve.dianchejie.cn

TRUNCATE TABLE logs;
来源：http://kab.cucudq.cn

[Q55] 排名（并列占位）
来源：http://jtd.vqdsnc.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://lzy.nanxuanxn.top

[Q56] 密集排名（并列不占位）
来源：http://clo.jianghu66.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://cvq.yj202588.top

[Q57] 行号
来源：http://rqk.xuetiantiany.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wme.zhiwuduotai.top

[Q58] 累计求和
来源：http://kgz.pycfn.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://bau.xylfe.cn

[Q59] 分组内累计
来源：http://dgn.hcnkem.com

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://tgv.hesvh.cn

[Q60] 取上一行 / 下一行
来源：http://meq.dashuyun.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://gkv.nwbrower.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://jam.shanyushiyangkeji.top

[Q61] 移动平均
来源：http://hbk.meibo888.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://gse.sjlbkw.cn

[Q62] 分组占比
来源：http://ojj.sweek.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ajp.havefunace.top

[Q63] 开启事务
来源：http://cni.jiagoushi.top

START TRANSACTION;                -- 或 BEGIN
来源：http://czb.ppjwa.cn

[Q64] 提交事务
来源：http://itt.yj20258.top

COMMIT;
来源：http://lob.hysaishi.cn

[Q65] 回滚事务
来源：http://sdm.zhiwuduotai.top

ROLLBACK;
来源：http://gcj.nanxinkj.top

[Q66] 行锁查询
来源：http://tri.nwbrower.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://xyv.pycfn.com

[Q67] 设置隔离级别
来源：http://rli.xingfuxueyuan.xyz

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ron.ctjpmb.com

[Q68] 保存点
来源：http://prw.vqdsnc.cn

SAVEPOINT sp1;
来源：http://qiu.ydzc1.top

ROLLBACK TO sp1;
来源：http://asp.xingfuxueyuan.xyz

[Q69] 查看执行计划
来源：http://fub.epnwcf.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://lii.cdnleiting.top

[Q70] 更新统计信息
来源：http://vwk.yanxiufei.cn

ANALYZE TABLE users;
来源：http://swx.pycfn.com

[Q71] 查看建表语句
来源：http://jfj.hnxiangtu.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://paq.daxiang520.top

[Q72] 查看索引
来源：http://nsi.bjfxy.top

SHOW INDEX FROM users;
来源：http://myn.daria6918.cn

[Q73] 查看表状态
来源：http://fwb.jqgufenzy.top

SHOW TABLE STATUS LIKE 'users';
来源：http://lco.jinqigfzy.top

[Q74] 强制使用索引
来源：http://kmo.yj20258.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://vqh.tarul.cn

[Q75] 日期格式化
来源：http://sbi.xingfuxueyuan.xyz

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://cmp.xuanzx.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://dff.redwolf501.top

[Q76] 按天统计
来源：http://oey.zhaomingkeji.xyz

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://iag.dianchejie.cn

[Q77] 时间加减
来源：http://nbi.vehdjk.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://itb.gzhubu.top

[Q78] 当前时间
来源：http://ciw.0kj1m.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://umf.zdqjudy.top

[Q79] 字符串拼接
来源：http://yiy.zhengqikj.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ywc.ywan-chungtsiang.top

[Q80] 字符串截取
来源：http://zzm.snrcjt.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://lbt.zdbjq.cn

[Q81] 字符串替换
来源：http://fje.jinqigfzy.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://qfa.9152youxi.cn

[Q82] 字符长度与字节长度
来源：http://mgg.cashguo.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ute.gaohongyu789.top

[Q83] 大小写转换
来源：http://tjx.hammf.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://swl.ppjwa.cn

[Q84] 去除首尾空格
来源：http://hzh.hesvh.cn

SELECT TRIM(name) FROM users;
来源：http://uqg.sufxvd.cn

[Q85] 数值取整
来源：http://bhz.zhixingplan.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://iyf.hammf.cn

[Q86] 读取 JSON 字段
来源：http://pai.jinyuanbaomall.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ohl.meibo888.top

[Q87] JSON 字段做条件
来源：http://iaw.jqgufenzy.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://qns.yongpay.top

[Q88] 行转列（条件聚合）
来源：http://gud.yuxming.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://grf.tian-w.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://jty.52xcode.cn

[Q89] 判断表是否存在
来源：http://ysd.zhaomingkeji.xyz

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hkb.gogol.net.cn

[Q90] 生成序号列
来源：http://unq.xziqi.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://fdu.dianchejie.cn

================================================================================
来源：http://mvy.quarkkingdee.top

R. Bash 专题
来源：http://log.sjlbkw.cn

================================================================================
来源：http://uyv.zhengqikj.top

[R01] shebang 与严格模式
来源：http://pio.sxryk.cn

#!/usr/bin/env bash
来源：http://chh.hywenlv.cn

set -euo pipefail
来源：http://cde.gaohongyu789.top

[R02] 变量赋值与使用
来源：http://wdo.pengpengdd.cyou

name="Tom"; echo "$name"
来源：http://mrg.cdnleiting.top

[R03] 只读变量
来源：http://rws.zhongyouzk.top

readonly PI=3.14
来源：http://hcx.316326.xyz

[R04] 位置参数
来源：http://hyj.xuetiantiany.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://phk.zdqjudy.top

[R05] 参数默认值
来源：http://vuc.vqdsnc.cn

name="${1:-default}"
来源：http://tkv.tian-w.cn

[R06] 判断命令是否存在
来源：http://uot.0kj1m.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://zty.iojbl.cn

[R07] if 判断文件
来源：http://umz.ivvv.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://abg.nanxuanxn.top

[R08] 数值比较
来源：http://ice.52xcode.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://bzm.mhx1999.top

[R09] 字符串比较
来源：http://ios.jinghuilouyu.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://axl.shanyushiyangtech.top

[R10] 正则匹配
来源：http://ajn.nanxuanxn.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mnv.pycfn.com

[R11] case 多分支
来源：http://hsl.gogol.net.cn

case "$1" in
来源：http://lei.hywenlv.cn

start) echo "启动" ;;
来源：http://jgs.bbcook.cn

stop)  echo "停止" ;;
来源：http://jtb.tianlin.xyz

*)     echo "未知命令" ;;
来源：http://zgi.ydjk.org.cn

esac
来源：http://llw.shuidangran.top

[R12] for 遍历文件
来源：http://jjz.chenjidiqi.icu

for f in *.txt; do echo "$f"; done
来源：http://nhr.tianlin.xyz

[R13] for 计数循环
来源：http://whz.cucudq.cn

for i in {1..10}; do echo "$i"; done
来源：http://qhz.chenjidiqi.icu

[R14] C 风格 for
来源：http://xzx.jqgfzy.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://kaa.haohaochexian.top

[R15] while 逐行读文件
来源：http://ndl.hfpthk.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ili.tianlin.xyz

[R16] until 等待条件
来源：http://acw.zhongyouzk.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://cfm.zhiwuduotai.top

[R17] 数组定义与取值
来源：http://iji.fengsongda.top

arr=(a b c); echo "${arr[0]}"
来源：http://rkm.aibaodan.cn

[R18] 遍历数组
来源：http://szj.jinqigufen.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ghd.fehbvm.com

[R19] 数组长度
来源：http://xdx.316326.xyz

echo "${#arr[@]}"
来源：http://cdz.yj202588.top

[R20] 关联数组（字典）
来源：http://rbh.zdqjudy.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://xey.yueranfly.top

[R21] 字符串长度
来源：http://sex.ywan-chungtsiang.top

echo "${#s}"
来源：http://lfa.cqqwz.cn

[R22] 截取子串
来源：http://mgq.zdqjudy.top

echo "${s:0:5}"
来源：http://jbn.yanxiufei.cn

[R23] 字符串替换
来源：http://yno.yfazqb.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://lew.shuidangran.top

[R24] 大小写转换
来源：http://dmw.tianlin.xyz

echo "${s^^}"; echo "${s,,}"
来源：http://kvu.feifeiyinyue.top

[R25] 去后缀 / 去前缀
来源：http://uxk.yangfankeji.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://kmt.dashuyun.cn

[R26] 命令替换
来源：http://led.tarul.cn

now=$(date +%F); echo "$now"
来源：http://jbx.hesvh.cn

[R27] 算术展开
来源：http://ngr.yj20258888.top

echo $((1 + 2 * 3))
来源：http://yze.cqqwz.cn

[R28] 浮点运算
来源：http://hrh.andypj.xyz

echo "scale=2; 10/3" | bc
来源：http://smu.jinyuanbaomall.cn

[R29] 定义函数
来源：http://hxc.birdmap.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://shn.vehdjk.com

[R30] 函数返回状态码
来源：http://dzw.nwbrower.top

f() { return 0; }; f || echo "失败了"
来源：http://zlj.shanyushiyangtech.top

[R31] 局部变量
来源：http://wcz.ctjpmb.com

f() { local x=1; echo "$x"; }
来源：http://dbg.xuanzx.com

[R32] 参数个数校验
来源：http://ygd.yvedp.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ggo.daxiang520.top

[R33] 捕获错误并提示行号
来源：http://dmv.ivvv.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://zdo.jyoumei.cn

[R34] 退出时清理
来源：http://los.jqgufenzy.top

trap 'rm -f "$tmp"' EXIT
来源：http://foq.snrcjt.cn

[R35] 后台执行并等待
来源：http://udi.0kj1m.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://dcp.sweek.top

[R36] 并发执行多个任务
来源：http://ryc.sufxvd.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://szg.gzhubu.top

[R37] 把输出赋给变量
来源：http://zat.gogol.net.cn

files=$(ls -1)
来源：http://mzt.havefunace.top

[R38] 管道串联
来源：http://aom.ybcxt.top

cat a.txt | grep -i error | wc -l
来源：http://jeo.pengpengdd.cyou

[R39] 重定向标准输出与错误
来源：http://vkn.sufxvd.cn

cmd > out.log 2>&1
来源：http://vsb.xinyue.icu

[R40] 追加写日志
来源：http://cnu.feifeiyinyue.top

echo "log" >> out.log
来源：http://fmi.shangyingyoupin.top

[R41] 丢弃输出
来源：http://qvu.hnxiangtu.top

cmd >/dev/null 2>&1
来源：http://hxp.vqdsnc.cn

[R42] 输入重定向
来源：http://bab.nwbrower.top

wc -l < a.txt
来源：http://bme.cqqwz.cn

[R43] 按名字查找文件
来源：http://cvx.yj20258.top

find . -name "*.log" -type f
来源：http://lly.feifeiyinyue.top

[R44] 按修改时间查找
来源：http://xgj.yj20258.top

find . -mtime -7 -type f
来源：http://hns.xylfe.cn

[R45] 批量删除
来源：http://lcd.zycfv.cn

find . -name "*.tmp" -delete
来源：http://nvh.fktsv.cn

[R46] 递归替换文件内容
来源：http://dsm.ctjpmb.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://qgc.yj202588.top

[R47] sed 单行替换
来源：http://ucu.yanxiufei.cn

sed -i 's/foo/bar/g' a.txt
来源：http://qte.yj202588.top

[R48] awk 取指定列
来源：http://iao.jqgfzy.top

awk '{print $1, $3}' a.txt
来源：http://viw.shanyushiyangkeji.top

[R49] awk 带条件
来源：http://gda.ydzc1.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://dhw.nanxuanxn.top

[R50] awk 求和
来源：http://qhe.tanke756.top

awk '{s += $2} END {print s}' a.txt
来源：http://tvw.mhx1999.top

[R51] 排序去重取前几
来源：http://eij.chenlongwang.top

sort a.txt | uniq -c | sort -rn | head
来源：http://gyy.jianghu66.top

[R52] 统计行数
来源：http://npn.yueranfly.top

wc -l a.txt
来源：http://umw.wangdashe.top

[R53] 查看文件头与实时尾
来源：http://jry.yanxiufei.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wsl.redwolf501.top

[R54] 比较两个文件
来源：http://rnh.bjfxy.top

diff a.txt b.txt
来源：http://utl.hfpthk.cn

[R55] 压缩与解压
来源：http://qqh.vqdsnc.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://siq.jianghu66.top

[R56] 远程拷贝
来源：http://zmk.gaohongyu789.top

scp file user@host:/path/
来源：http://zce.birdmap.top

[R57] 远程执行命令
来源：http://kfq.jyoumei.cn

ssh user@host 'uptime'
来源：http://jnk.sufxvd.cn

[R58] 下载文件
来源：http://axp.yj20258888.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://omr.dianchejie.cn

[R59] 发 POST JSON
来源：http://fcm.yj20258.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://lof.52xcode.cn

[R60] 只看 HTTP 状态码
来源：http://bgw.shzxlz.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://osb.tianlin.xyz

[R61] 磁盘占用
来源：http://kvg.shanyushiyangkeji.top

df -h;  du -sh *
来源：http://cru.jinqigfzy.top

[R62] 找最占空间的文件
来源：http://zkg.yj202588.top

du -ah . | sort -rh | head -10
来源：http://bal.zhixingplan.top

[R63] 内存与进程
来源：http://fzq.jinqigufen.top

free -h;  ps aux | grep nginx
来源：http://xzl.ppjwa.cn

[R64] 结束进程
来源：http://zwz.fanxiaobao.xyz

kill -9 $(pgrep -f app.py)
来源：http://tye.yvedp.cn

[R65] 查看端口占用
来源：http://mfk.zhijiandao.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wmf.uphjek.com

[R66] 定时任务
来源：http://eol.ybcxt.top

crontab -e;  crontab -l
来源：http://obu.yuxming.cn

[R67] 生成随机十六进制串
来源：http://hoy.cdnleiting.top


<!-- 参考信息 -->