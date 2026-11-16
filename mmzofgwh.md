代发 wailian999

SELECT * FROM users;
来源：http://lpq.gogol.net.cn

[Q16] 查询指定列
来源：http://onc.9152youxi.cn

SELECT id, name FROM users;
来源：http://mcl.ehwqpu.com

[Q17] 条件查询
来源：http://jxu.wangdashe.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://tmy.ydzc1.top

[Q18] 模糊匹配
来源：http://ndj.xuanzx.com

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ynl.fzhhl.top

[Q19] 范围查询
来源：http://qqh.daria6918.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://kwl.ehwqpu.com

[Q20] IN 列表
来源：http://tgh.yonumen.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hhj.jiagoushi.top

[Q21] 空值判断
来源：http://wwl.hcnkem.com

SELECT * FROM users WHERE email IS NULL;
来源：http://ykx.wangdashe.top

[Q22] 排序
来源：http://lrg.uphjek.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ktc.yonumen.top

[Q23] 分页
来源：http://djs.ivvv.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://kxs.bbcook.cn

[Q24] 去重
来源：http://yml.vqdsnc.cn

SELECT DISTINCT city FROM users;
来源：http://oxh.yj202588.top

[Q25] 只取前 N 条
来源：http://haw.ctjpmb.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://tue.ybcxt.top

[Q26] 计数
来源：http://mla.bbcook.cn

SELECT COUNT(*) FROM users;
来源：http://huk.fzhhl.top

[Q27] 条件计数
来源：http://ntx.c1oappe.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://efx.zhoulong.xyz

[Q28] 求和与平均
来源：http://yag.ehwqpu.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://bpk.jianghu66.top

[Q29] 最大最小值
来源：http://jdg.nwbrower.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://gwc.smart0.xyz

[Q30] 分组统计
来源：http://gcb.jinqigfzy.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wms.yanxiufei.cn

[Q31] 分组后过滤
来源：http://xtg.9152youxi.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://uje.guannengcc.top

[Q32] 分组拼接字符串
来源：http://tmj.dashuyun.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://gws.zhaomingkeji.xyz

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://aqt.zdqjudy.top

[Q33] 多列分组
来源：http://pws.cdnleiting.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://elt.vqdsnc.cn

[Q34] 每组取第一条
来源：http://pbr.guowangkeji.top

SELECT * FROM (
来源：http://zrf.guowangkeji.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hyr.hnqzz.top

) t WHERE rn = 1;
来源：http://des.fehbvm.com

[Q35] 内连接
来源：http://hei.sysykeji.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://uri.fktsv.cn

[Q36] 左连接
来源：http://xea.pengpengdd.cyou

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mhv.fzhhl.top

[Q37] 右连接
来源：http://apd.jiagoushi.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://otd.shanyushiyangkeji.top

[Q38] 全外连接（PostgreSQL）
来源：http://cep.zhoulong.xyz

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://spl.pengpengdd.cyou

[Q39] 自连接（查上下级）
来源：http://ixi.jiagoushi.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://fhu.guannengcc.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mzw.sxryk.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://rye.yangfankeji.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://noo.c1oappe.top

[Q41] 多表连接
来源：http://lyz.zhengqikj.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://bpm.shanyushiyangtech.top

JOIN users u ON u.id = o.user_id
来源：http://pwp.quarkkingdee.top

JOIN products p ON p.id = o.product_id;
来源：http://rqi.iojbl.cn

[Q42] 连接条件附加过滤
来源：http://uca.sysykeji.top

SELECT u.name, o.amount FROM users u
来源：http://mmy.jianghu66.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://kdt.jyoumei.cn

[Q43] 标量子查询
来源：http://ggd.sweek.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ntt.gotoacloud.top

[Q44] IN 子查询
来源：http://prf.pycfn.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://rpn.jinyuanbaomall.cn

[Q45] EXISTS 判断存在
来源：http://prg.epnwcf.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://oqa.yongpay.top

[Q46] NOT EXISTS 判断不存在
来源：http://xbc.yj202588.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ggk.epnwcf.com

[Q47] 与平均值比较
来源：http://acu.fzhhl.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://gsj.yanxiufei.cn

[Q48] CTE 公用表表达式
来源：http://qez.shzxlz.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://txl.quarkkingdee.top

SELECT * FROM t WHERE c > 5;
来源：http://jvn.sweek.top

[Q49] 更新单行
来源：http://hhf.gotoacloud.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://vnv.316326.xyz

[Q50] 批量更新
来源：http://wqw.wangshuangyany.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://epn.gogol.net.cn

[Q51] 用子查询更新
来源：http://aly.jinghuilouyu.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://fqs.ehwqpu.com

[Q52] 删除指定行
来源：http://rki.ivvv.top

DELETE FROM users WHERE id = 10;
来源：http://xan.sysykeji.top

[Q53] 按条件删除
来源：http://hrn.uphjek.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://qqo.zdqjudy.top

[Q54] 清空表
来源：http://hkc.aizwys.cn

TRUNCATE TABLE logs;
来源：http://sez.cqqwz.cn

[Q55] 排名（并列占位）
来源：http://rxa.fehbvm.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://qec.jiagoushi.top

[Q56] 密集排名（并列不占位）
来源：http://mpw.hywenlv.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://oin.jinqigufen.top

[Q57] 行号
来源：http://obp.yangfankeji.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://dcq.andypj.xyz

[Q58] 累计求和
来源：http://apb.yonumen.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hbv.hammf.cn

[Q59] 分组内累计
来源：http://ioo.chenzaomai.com

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://zgo.sweek.top

[Q60] 取上一行 / 下一行
来源：http://ill.xziqi.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://sjl.ydjk.org.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://cae.jqgufenzy.top

[Q61] 移动平均
来源：http://jmx.hnxiangtu.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://pei.svipenyu.cn

[Q62] 分组占比
来源：http://syl.nanxinkj.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://yog.epnwcf.com

[Q63] 开启事务
来源：http://ccn.dianchejie.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://tog.nanxinkj.top

[Q64] 提交事务
来源：http://ygs.jyoumei.cn

COMMIT;
来源：http://ksv.wangshuangyany.cn

[Q65] 回滚事务
来源：http://cyb.birdmap.top

ROLLBACK;
来源：http://opa.aizwys.cn

[Q66] 行锁查询
来源：http://bps.aibaodan.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://sfz.xziqi.cn

[Q67] 设置隔离级别
来源：http://qcb.haohaochexian.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://anq.cucudq.cn

[Q68] 保存点
来源：http://djp.gzhubu.top

SAVEPOINT sp1;
来源：http://ovv.meibo888.top

ROLLBACK TO sp1;
来源：http://ooe.svipenyu.cn

[Q69] 查看执行计划
来源：http://yvb.gzhubu.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://nje.bbcook.cn

[Q70] 更新统计信息
来源：http://jvh.jqgufenzy.top

ANALYZE TABLE users;
来源：http://tfy.snrcjt.cn

[Q71] 查看建表语句
来源：http://krn.chenlongwang.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://dam.hysaishi.cn

[Q72] 查看索引
来源：http://niy.dianchejie.cn

SHOW INDEX FROM users;
来源：http://lbf.jinqigufen.top

[Q73] 查看表状态
来源：http://eiv.zycfv.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://qos.ehwqpu.com

[Q74] 强制使用索引
来源：http://oli.yfazqb.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ang.yj20258888.top

[Q75] 日期格式化
来源：http://afb.zhengqikj.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://xpi.cucudq.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://zdf.ivvv.top

[Q76] 按天统计
来源：http://awb.hesvh.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://olc.jyoumei.cn

[Q77] 时间加减
来源：http://qxp.jinghuilouyu.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://cxx.jiagoushi.top

[Q78] 当前时间
来源：http://fsg.tianlin.xyz

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://pet.vehdjk.com

[Q79] 字符串拼接
来源：http://bid.iojbl.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ngb.birdmap.top

[Q80] 字符串截取
来源：http://tmb.cucudq.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://bpg.sxryk.cn

[Q81] 字符串替换
来源：http://fyx.wangshuangyany.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://qbd.yongpay.top

[Q82] 字符长度与字节长度
来源：http://zyk.yj202588.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ysh.zycfv.cn

[Q83] 大小写转换
来源：http://ool.yfazqb.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wds.fktsv.cn

[Q84] 去除首尾空格
来源：http://xeb.xziqi.cn

SELECT TRIM(name) FROM users;
来源：http://yhw.wangdashe.top

[Q85] 数值取整
来源：http://ons.svipenyu.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://lej.vehdjk.com

[Q86] 读取 JSON 字段
来源：http://pve.zhixingplan.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mcr.ywan-chungtsiang.top

[Q87] JSON 字段做条件
来源：http://lzh.yvedp.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://fzm.gaohongyu789.top

[Q88] 行转列（条件聚合）
来源：http://uxs.yj20258.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://plt.sysykeji.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ydq.yuxming.cn

[Q89] 判断表是否存在
来源：http://cjm.hfpthk.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://jny.0kj1m.cn

[Q90] 生成序号列
来源：http://ris.cheryme.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://elw.yuxming.cn

================================================================================
来源：http://gym.guowangkeji.top

R. Bash 专题
来源：http://aam.ydjk.org.cn

================================================================================
来源：http://myh.nanxinkj.top

[R01] shebang 与严格模式
来源：http://mbj.bbcook.cn

#!/usr/bin/env bash
来源：http://qes.xingfuxueyuan.xyz

set -euo pipefail
来源：http://isz.hywenlv.cn

[R02] 变量赋值与使用
来源：http://dwl.xingfuxueyuan.xyz

name="Tom"; echo "$name"
来源：http://tsx.feifeiyinyue.top

[R03] 只读变量
来源：http://uhu.tanke756.top

readonly PI=3.14
来源：http://edj.zhongyouzk.top

[R04] 位置参数
来源：http://rhm.9152youxi.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://chi.fzhhl.top

[R05] 参数默认值
来源：http://stj.jinqigufen.top

name="${1:-default}"
来源：http://xcb.yanxiufei.cn

[R06] 判断命令是否存在
来源：http://vti.zhiwuduotai.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ilb.sufxvd.cn

[R07] if 判断文件
来源：http://nwk.xinyue.icu

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://qwa.tianlin.xyz

[R08] 数值比较
来源：http://stj.vehdjk.com

if (( a > b )); then echo "a 更大"; fi
来源：http://pob.jyoumei.cn

[R09] 字符串比较
来源：http://uzg.ydjk.org.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://obw.hywenlv.cn

[R10] 正则匹配
来源：http://bbp.cdnleiting.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://bdc.daxiang520.top

[R11] case 多分支
来源：http://rio.sjlbkw.cn

case "$1" in
来源：http://sqf.ppjwa.cn

start) echo "启动" ;;
来源：http://qam.jinghuilouyu.cn

stop)  echo "停止" ;;
来源：http://tdo.jyoumei.cn

*)     echo "未知命令" ;;
来源：http://njk.cheryme.top

esac
来源：http://chl.jianghu66.top

[R12] for 遍历文件
来源：http://fmy.fktsv.cn

for f in *.txt; do echo "$f"; done
来源：http://afr.jiagoushi.top

[R13] for 计数循环
来源：http://pit.haohaochexian.top

for i in {1..10}; do echo "$i"; done
来源：http://oob.guowangkeji.top

[R14] C 风格 for
来源：http://lgp.xziqi.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://njj.zhongyouzk.top

[R15] while 逐行读文件
来源：http://jqd.yuxming.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://fgq.ywan-chungtsiang.top

[R16] until 等待条件
来源：http://swd.xinyue.icu

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mpk.andypj.xyz

[R17] 数组定义与取值
来源：http://jsv.xingfuxueyuan.xyz

arr=(a b c); echo "${arr[0]}"
来源：http://ybm.zdqjudy.top

[R18] 遍历数组
来源：http://wxg.cqqwz.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://unc.uphjek.com

[R19] 数组长度
来源：http://sec.jiagoushi.top

echo "${#arr[@]}"
来源：http://tpz.zhixingplan.top

[R20] 关联数组（字典）
来源：http://hos.xuanzx.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://tkw.ctjpmb.com

[R21] 字符串长度
来源：http://vvm.ydjk.org.cn

echo "${#s}"
来源：http://fwj.dashuyun.cn

[R22] 截取子串
来源：http://cqn.tianlin.xyz

echo "${s:0:5}"
来源：http://doj.cqqwz.cn

[R23] 字符串替换
来源：http://epm.ywan-chungtsiang.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://myf.zhengqikj.top

[R24] 大小写转换
来源：http://zqs.cucudq.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ncg.pengpengdd.cyou

[R25] 去后缀 / 去前缀
来源：http://sqx.dianchejie.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://nef.jinqigfzy.top

[R26] 命令替换
来源：http://jyc.yueranfly.top

now=$(date +%F); echo "$now"
来源：http://mcp.yfazqb.com

[R27] 算术展开
来源：http://ztr.xuetiantiany.cn

echo $((1 + 2 * 3))
来源：http://zwv.jyoumei.cn

[R28] 浮点运算
来源：http://vlx.jinqigfzy.top

echo "scale=2; 10/3" | bc
来源：http://uqh.yongpay.top

[R29] 定义函数
来源：http://lwc.cqqwz.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://sha.guowangkeji.top

[R30] 函数返回状态码
来源：http://nmu.daria6918.cn

f() { return 0; }; f || echo "失败了"
来源：http://bhb.shanyushiyangkeji.top

[R31] 局部变量
来源：http://fmj.jqgfzy.top

f() { local x=1; echo "$x"; }
来源：http://zdf.fanxiaobao.xyz

[R32] 参数个数校验
来源：http://vba.c1oappe.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://xoz.ybcxt.top

[R33] 捕获错误并提示行号
来源：http://qpa.xziqi.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://jhp.yueranfly.top

[R34] 退出时清理
来源：http://uwc.sufxvd.cn

trap 'rm -f "$tmp"' EXIT
来源：http://niv.nanxuanxn.top

[R35] 后台执行并等待
来源：http://coh.hammf.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://lnl.xinyue.icu

[R36] 并发执行多个任务
来源：http://wfg.nanxinkj.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://rdb.jinghuilouyu.cn

[R37] 把输出赋给变量
来源：http://ppe.ppjwa.cn

files=$(ls -1)
来源：http://ndj.yj20258.top

[R38] 管道串联
来源：http://xzo.zycfv.cn

cat a.txt | grep -i error | wc -l
来源：http://maw.shanyushiyangtech.top

[R39] 重定向标准输出与错误
来源：http://iit.gogol.net.cn

cmd > out.log 2>&1
来源：http://oav.shanyushiyangkeji.top

[R40] 追加写日志
来源：http://nop.hysaishi.cn

echo "log" >> out.log
来源：http://yvg.ydzc1.top

[R41] 丢弃输出
来源：http://vrn.birdmap.top

cmd >/dev/null 2>&1
来源：http://zwq.guowangkeji.top

[R42] 输入重定向
来源：http://unv.ybcxt.top

wc -l < a.txt
来源：http://uxp.cheryme.top

[R43] 按名字查找文件
来源：http://als.snrcjt.cn

find . -name "*.log" -type f
来源：http://kzj.hnxiangtu.top

[R44] 按修改时间查找
来源：http://njs.hfpthk.cn

find . -mtime -7 -type f
来源：http://iws.fanxiaobao.xyz

[R45] 批量删除
来源：http://xkq.yanxiufei.cn

find . -name "*.tmp" -delete
来源：http://qbn.xziqi.cn

[R46] 递归替换文件内容
来源：http://bug.9152youxi.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://dzi.sxryk.cn

[R47] sed 单行替换
来源：http://iaa.cashguo.top

sed -i 's/foo/bar/g' a.txt
来源：http://gbx.vehdjk.com

[R48] awk 取指定列
来源：http://uls.pycfn.com

awk '{print $1, $3}' a.txt
来源：http://ghv.quarkkingdee.top

[R49] awk 带条件
来源：http://iyt.hnqzz.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://acf.svipenyu.cn

[R50] awk 求和
来源：http://hpd.yj20258.top

awk '{s += $2} END {print s}' a.txt
来源：http://lrx.fktsv.cn

[R51] 排序去重取前几
来源：http://aky.xziqi.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://aze.jinyuanbaomall.cn

[R52] 统计行数
来源：http://ppg.yfazqb.com

wc -l a.txt
来源：http://div.quarkkingdee.top

[R53] 查看文件头与实时尾
来源：http://jtf.quarkkingdee.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://chp.zhengqikj.top

[R54] 比较两个文件
来源：http://phk.nanxinkj.top

diff a.txt b.txt
来源：http://ijl.hesvh.cn

[R55] 压缩与解压
来源：http://pff.jinqigfzy.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://jlm.tanke756.top

[R56] 远程拷贝
来源：http://ahs.guowangkeji.top

scp file user@host:/path/
来源：http://ezl.shanyushiyangtech.top

[R57] 远程执行命令
来源：http://jch.yuxming.cn

ssh user@host 'uptime'
来源：http://lso.xuanzx.com

[R58] 下载文件
来源：http://btz.316326.xyz

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://bgj.ppjwa.cn

[R59] 发 POST JSON
来源：http://cka.havefunace.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ezi.fzhhl.top

[R60] 只看 HTTP 状态码
来源：http://tco.aizwys.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://cpq.quarkkingdee.top

[R61] 磁盘占用
来源：http://cdf.yj20258888.top

df -h;  du -sh *
来源：http://krg.daxiang520.top

[R62] 找最占空间的文件
来源：http://rhz.52xcode.cn

du -ah . | sort -rh | head -10
来源：http://gii.tanke756.top

[R63] 内存与进程
来源：http://xvc.sufxvd.cn

free -h;  ps aux | grep nginx
来源：http://zam.jyoumei.cn

[R64] 结束进程
来源：http://lkj.aibaodan.cn

kill -9 $(pgrep -f app.py)
来源：http://xjm.jqgufenzy.top

[R65] 查看端口占用
来源：http://pnq.sysykeji.top


<!-- 参考信息 -->