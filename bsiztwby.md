代发 wailian999

SELECT * FROM users;
来源：http://qjt.nwbrower.top

[Q16] 查询指定列
来源：http://vuz.316326.xyz

SELECT id, name FROM users;
来源：http://ech.yuanzhike.top

[Q17] 条件查询
来源：http://suy.hysaishi.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://yyz.hongshengwenyu.top

[Q18] 模糊匹配
来源：http://ymf.sxryk.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://xne.wangshuangyany.cn

[Q19] 范围查询
来源：http://kpf.iojbl.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://liz.birdmap.top

[Q20] IN 列表
来源：http://trt.havefunace.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://vlk.hywenlv.cn

[Q21] 空值判断
来源：http://zbo.cashguo.top

SELECT * FROM users WHERE email IS NULL;
来源：http://ald.hesvh.cn

[Q22] 排序
来源：http://ahg.tian-w.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://syk.shanyushiyangtech.top

[Q23] 分页
来源：http://hfd.andypj.xyz

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://swr.shuidangran.top

[Q24] 去重
来源：http://vmf.mhx1999.top

SELECT DISTINCT city FROM users;
来源：http://lye.zhijiandao.cn

[Q25] 只取前 N 条
来源：http://gdv.ydjk.org.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://jms.jinghuilouyu.cn

[Q26] 计数
来源：http://yom.pengpengdd.cyou

SELECT COUNT(*) FROM users;
来源：http://cpz.zhongyouzk.top

[Q27] 条件计数
来源：http://cse.daxiang520.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://niv.yj20258.top

[Q28] 求和与平均
来源：http://rjm.gzhubu.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://rwp.haohaochexian.top

[Q29] 最大最小值
来源：http://bhx.epnwcf.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://rnu.jiagoushi.top

[Q30] 分组统计
来源：http://ijz.jqgfzy.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://gut.c1oappe.top

[Q31] 分组后过滤
来源：http://cch.xuanzx.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://egr.cucudq.cn

[Q32] 分组拼接字符串
来源：http://bgh.zhoulong.xyz

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://dbi.fanxiaobao.xyz

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wwk.zhiwuduotai.top

[Q33] 多列分组
来源：http://bzo.epnwcf.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://nic.andypj.xyz

[Q34] 每组取第一条
来源：http://wfn.jiagoushi.top

SELECT * FROM (
来源：http://xhf.zhaomingkeji.xyz

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://sbd.havefunace.top

) t WHERE rn = 1;
来源：http://sxt.sxryk.cn

[Q35] 内连接
来源：http://vrp.xuetiantiany.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mex.smart0.xyz

[Q36] 左连接
来源：http://afo.daria6918.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://jjw.c1oappe.top

[Q37] 右连接
来源：http://rio.cucudq.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://pyu.cqqwz.cn

[Q38] 全外连接（PostgreSQL）
来源：http://wzw.yonumen.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://qzi.yj20258888.top

[Q39] 自连接（查上下级）
来源：http://bhw.nwbrower.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://riy.c1oappe.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://fii.shanyushiyangtech.top

[Q40] 交叉连接（笛卡尔积）
来源：http://hiq.dashuyun.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://nrp.sufxvd.cn

[Q41] 多表连接
来源：http://ccq.zdbjq.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://iej.hfpthk.cn

JOIN users u ON u.id = o.user_id
来源：http://svb.yonumen.top

JOIN products p ON p.id = o.product_id;
来源：http://vgp.andypj.xyz

[Q42] 连接条件附加过滤
来源：http://tzb.ppjwa.cn

SELECT u.name, o.amount FROM users u
来源：http://vhg.jinqigufen.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ryw.tianlin.xyz

[Q43] 标量子查询
来源：http://amf.fktsv.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://qom.meibo888.top

[Q44] IN 子查询
来源：http://chv.yfazqb.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ebb.yuanzhike.top

[Q45] EXISTS 判断存在
来源：http://fpj.ybcxt.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ryv.tanke756.top

[Q46] NOT EXISTS 判断不存在
来源：http://uaj.redwolf501.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://cqt.shzxlz.cn

[Q47] 与平均值比较
来源：http://iwk.gzhubu.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://yod.fzhhl.top

[Q48] CTE 公用表表达式
来源：http://ehc.hesvh.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://plc.yonumen.top

SELECT * FROM t WHERE c > 5;
来源：http://qhd.jinyuanbaomall.cn

[Q49] 更新单行
来源：http://jbb.chenzaomai.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://vyd.yj20258888.top

[Q50] 批量更新
来源：http://ayo.shzxlz.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ixv.yfazqb.com

[Q51] 用子查询更新
来源：http://wuu.vqdsnc.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://oxt.ehwqpu.com

[Q52] 删除指定行
来源：http://ubq.vqdsnc.cn

DELETE FROM users WHERE id = 10;
来源：http://ynq.cdnleiting.top

[Q53] 按条件删除
来源：http://tnp.tanke756.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://eub.iojbl.cn

[Q54] 清空表
来源：http://usj.zdbjq.cn

TRUNCATE TABLE logs;
来源：http://qau.zhaomingkeji.xyz

[Q55] 排名（并列占位）
来源：http://mda.hfpthk.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ynq.gzhubu.top

[Q56] 密集排名（并列不占位）
来源：http://bdl.tanke756.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hfp.9152youxi.cn

[Q57] 行号
来源：http://nkw.havefunace.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://lkk.sjlbkw.cn

[Q58] 累计求和
来源：http://boe.jiagoushi.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mue.pengpengdd.cyou

[Q59] 分组内累计
来源：http://xwn.smart0.xyz

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://fvt.vehdjk.com

[Q60] 取上一行 / 下一行
来源：http://bxn.aibaodan.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://dez.chenzaomai.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://rco.hcnkem.com

[Q61] 移动平均
来源：http://ffj.pengpengdd.cyou

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ukg.nwbrower.top

[Q62] 分组占比
来源：http://mtm.jinghuilouyu.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://sfv.yanxiufei.cn

[Q63] 开启事务
来源：http://cwm.gzhubu.top

START TRANSACTION;                -- 或 BEGIN
来源：http://jxv.xziqi.cn

[Q64] 提交事务
来源：http://dyy.316326.xyz

COMMIT;
来源：http://qwr.zhixingplan.top

[Q65] 回滚事务
来源：http://ues.0kj1m.cn

ROLLBACK;
来源：http://hyr.sufxvd.cn

[Q66] 行锁查询
来源：http://rea.dashuyun.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://yqc.hysaishi.cn

[Q67] 设置隔离级别
来源：http://mxh.cheryme.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://gbp.tarul.cn

[Q68] 保存点
来源：http://eir.shanyushiyangkeji.top

SAVEPOINT sp1;
来源：http://ajx.gotoacloud.top

ROLLBACK TO sp1;
来源：http://qpl.shanyushiyangtech.top

[Q69] 查看执行计划
来源：http://mrz.yvedp.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://cjm.yanxiufei.cn

[Q70] 更新统计信息
来源：http://bgn.yueranfly.top

ANALYZE TABLE users;
来源：http://bwe.yonumen.top

[Q71] 查看建表语句
来源：http://ggk.hammf.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://nxi.xziqi.cn

[Q72] 查看索引
来源：http://afw.daria6918.cn

SHOW INDEX FROM users;
来源：http://bro.jianghu66.top

[Q73] 查看表状态
来源：http://dzt.jyoumei.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://das.xingfuxueyuan.xyz

[Q74] 强制使用索引
来源：http://bto.gzhubu.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wfv.redwolf501.top

[Q75] 日期格式化
来源：http://wvo.fehbvm.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://eyf.c1oappe.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://nhs.feifeiyinyue.top

[Q76] 按天统计
来源：http://rdm.gzhubu.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mbx.chenlongwang.top

[Q77] 时间加减
来源：http://wbi.yongpay.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://acr.birdmap.top

[Q78] 当前时间
来源：http://dxp.yj20258.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ygb.jqgufenzy.top

[Q79] 字符串拼接
来源：http://iyi.tarul.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://jer.c1oappe.top

[Q80] 字符串截取
来源：http://djo.ydjk.org.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://zix.ivvv.top

[Q81] 字符串替换
来源：http://lum.wangshuangyany.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://jdd.cashguo.top

[Q82] 字符长度与字节长度
来源：http://lkj.feifeiyinyue.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://swi.gotoacloud.top

[Q83] 大小写转换
来源：http://njf.jqgufenzy.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://oeq.tianlin.xyz

[Q84] 去除首尾空格
来源：http://ycs.zhengqikj.top

SELECT TRIM(name) FROM users;
来源：http://rcg.zdqjudy.top

[Q85] 数值取整
来源：http://kpe.hnqzz.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://tcj.shanyushiyangkeji.top

[Q86] 读取 JSON 字段
来源：http://eec.quarkkingdee.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://xzv.vqdsnc.cn

[Q87] JSON 字段做条件
来源：http://eoj.xylfe.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://vsi.jinqigufen.top

[Q88] 行转列（条件聚合）
来源：http://lct.zhijiandao.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ynt.hammf.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://awg.yj20258.top

[Q89] 判断表是否存在
来源：http://jyo.meibo888.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://rxg.ppjwa.cn

[Q90] 生成序号列
来源：http://ddi.shuidangran.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://taz.fanxiaobao.xyz

================================================================================
来源：http://arq.xuanzx.com

R. Bash 专题
来源：http://yoa.shanyushiyangkeji.top

================================================================================
来源：http://dit.svipenyu.cn

[R01] shebang 与严格模式
来源：http://ijv.sjlbkw.cn

#!/usr/bin/env bash
来源：http://auu.zdbjq.cn

set -euo pipefail
来源：http://xew.dianchejie.cn

[R02] 变量赋值与使用
来源：http://ggq.daxiang520.top

name="Tom"; echo "$name"
来源：http://yrk.yongpay.top

[R03] 只读变量
来源：http://jkk.shuidangran.top

readonly PI=3.14
来源：http://pcq.yuanzhike.top

[R04] 位置参数
来源：http://dkq.nanxinkj.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://nyl.nanxinkj.top

[R05] 参数默认值
来源：http://ppx.sufxvd.cn

name="${1:-default}"
来源：http://agv.bjfxy.top

[R06] 判断命令是否存在
来源：http://xng.shuidangran.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ukl.zhaomingkeji.xyz

[R07] if 判断文件
来源：http://mjw.gogol.net.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://jeb.andypj.xyz

[R08] 数值比较
来源：http://scv.yanxiufei.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://phf.cucudq.cn

[R09] 字符串比较
来源：http://gfe.jlsjyb.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://tyy.nanxinkj.top

[R10] 正则匹配
来源：http://qmz.yongpay.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://pez.jqgufenzy.top

[R11] case 多分支
来源：http://job.316326.xyz

case "$1" in
来源：http://fnw.sjlbkw.cn

start) echo "启动" ;;
来源：http://vpg.gaohongyu789.top

stop)  echo "停止" ;;
来源：http://smz.xuetiantiany.cn

*)     echo "未知命令" ;;
来源：http://ovo.wangshuangyany.cn

esac
来源：http://qxi.nwbrower.top

[R12] for 遍历文件
来源：http://uww.0kj1m.cn

for f in *.txt; do echo "$f"; done
来源：http://grw.sxryk.cn

[R13] for 计数循环
来源：http://uoa.yj20258.top

for i in {1..10}; do echo "$i"; done
来源：http://fcx.guannengcc.top

[R14] C 风格 for
来源：http://wzb.jianghu66.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://npu.gotoacloud.top

[R15] while 逐行读文件
来源：http://mrq.shzxlz.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://crm.shanyushiyangtech.top

[R16] until 等待条件
来源：http://vcy.zhiwuduotai.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://zuj.xziqi.cn

[R17] 数组定义与取值
来源：http://rbe.smart0.xyz

arr=(a b c); echo "${arr[0]}"
来源：http://sel.zhaomingkeji.xyz

[R18] 遍历数组
来源：http://ihl.jiagoushi.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://osu.sjlbkw.cn

[R19] 数组长度
来源：http://tys.zhongyouzk.top

echo "${#arr[@]}"
来源：http://pvv.jqgfzy.top

[R20] 关联数组（字典）
来源：http://nqj.yj20258.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://izi.shangyingyoupin.top

[R21] 字符串长度
来源：http://knw.shzxlz.cn

echo "${#s}"
来源：http://nfv.gotoacloud.top

[R22] 截取子串
来源：http://jpz.sweek.top

echo "${s:0:5}"
来源：http://tcq.yj202588.top

[R23] 字符串替换
来源：http://dui.zhoulong.xyz

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://uhi.snrcjt.cn

[R24] 大小写转换
来源：http://fta.ydjk.org.cn

echo "${s^^}"; echo "${s,,}"
来源：http://dbc.ydzc1.top

[R25] 去后缀 / 去前缀
来源：http://vmd.aizwys.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://lqw.dashuyun.cn

[R26] 命令替换
来源：http://biw.yj202588.top

now=$(date +%F); echo "$now"
来源：http://tln.xuetiantiany.cn

[R27] 算术展开
来源：http://nab.jianghu66.top

echo $((1 + 2 * 3))
来源：http://wnu.epnwcf.com

[R28] 浮点运算
来源：http://yuo.quarkkingdee.top

echo "scale=2; 10/3" | bc
来源：http://uwp.aibaodan.cn

[R29] 定义函数
来源：http://lss.ywan-chungtsiang.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ivt.c1oappe.top

[R30] 函数返回状态码
来源：http://uqj.shanyushiyangtech.top

f() { return 0; }; f || echo "失败了"
来源：http://wyu.sufxvd.cn

[R31] 局部变量
来源：http://axw.hesvh.cn

f() { local x=1; echo "$x"; }
来源：http://fwp.tarul.cn

[R32] 参数个数校验
来源：http://btf.chenzaomai.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://qvm.havefunace.top

[R33] 捕获错误并提示行号
来源：http://ovh.yongpay.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ogr.feifeiyinyue.top

[R34] 退出时清理
来源：http://ltb.sxryk.cn

trap 'rm -f "$tmp"' EXIT
来源：http://rcs.fzhhl.top

[R35] 后台执行并等待
来源：http://jgu.sxryk.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://oen.hesvh.cn

[R36] 并发执行多个任务
来源：http://ydq.vqdsnc.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://grj.jinyuanbaomall.cn

[R37] 把输出赋给变量
来源：http://ykk.c1oappe.top

files=$(ls -1)
来源：http://vnb.xingfuxueyuan.xyz

[R38] 管道串联
来源：http://uqd.yfazqb.com

cat a.txt | grep -i error | wc -l
来源：http://cje.xylfe.cn

[R39] 重定向标准输出与错误
来源：http://nna.yongpay.top

cmd > out.log 2>&1
来源：http://uhw.cdnleiting.top

[R40] 追加写日志
来源：http://hie.ehwqpu.com

echo "log" >> out.log
来源：http://cry.gogol.net.cn

[R41] 丢弃输出
来源：http://ezo.pycfn.com

cmd >/dev/null 2>&1
来源：http://isx.c1oappe.top

[R42] 输入重定向
来源：http://bbu.ehwqpu.com

wc -l < a.txt
来源：http://quc.gogol.net.cn

[R43] 按名字查找文件
来源：http://tfi.cashguo.top

find . -name "*.log" -type f
来源：http://yly.pycfn.com

[R44] 按修改时间查找
来源：http://pxu.daxiang520.top

find . -mtime -7 -type f
来源：http://sgl.cashguo.top

[R45] 批量删除
来源：http://igu.316326.xyz

find . -name "*.tmp" -delete
来源：http://cxu.haohaochexian.top

[R46] 递归替换文件内容
来源：http://jni.hywenlv.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hqd.daria6918.cn

[R47] sed 单行替换
来源：http://nkf.zhoulong.xyz

sed -i 's/foo/bar/g' a.txt
来源：http://tzi.cqqwz.cn

[R48] awk 取指定列
来源：http://kir.yanxiufei.cn

awk '{print $1, $3}' a.txt
来源：http://vff.nanxuanxn.top

[R49] awk 带条件
来源：http://ope.jinyuanbaomall.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wjl.yj20258.top

[R50] awk 求和
来源：http://vyi.0kj1m.cn

awk '{s += $2} END {print s}' a.txt
来源：http://nmb.zhaomingkeji.xyz

[R51] 排序去重取前几
来源：http://ted.quarkkingdee.top

sort a.txt | uniq -c | sort -rn | head
来源：http://zln.sysykeji.top

[R52] 统计行数
来源：http://nky.svipenyu.cn

wc -l a.txt
来源：http://qdf.shzxlz.cn

[R53] 查看文件头与实时尾
来源：http://yhr.jqgufenzy.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://jck.haohaochexian.top

[R54] 比较两个文件
来源：http://iqw.jlsjyb.cn

diff a.txt b.txt
来源：http://nnf.zhongyouzk.top

[R55] 压缩与解压
来源：http://oyw.gotoacloud.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://yzr.xuanzx.com

[R56] 远程拷贝
来源：http://gue.sufxvd.cn

scp file user@host:/path/
来源：http://wuh.pengpengdd.cyou

[R57] 远程执行命令
来源：http://nio.jyoumei.cn

ssh user@host 'uptime'
来源：http://crd.xuanzx.com

[R58] 下载文件
来源：http://ovc.yonumen.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ejm.pengpengdd.cyou

[R59] 发 POST JSON
来源：http://vst.gaohongyu789.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://kza.yj20258888.top

[R60] 只看 HTTP 状态码
来源：http://kei.wangdashe.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://dcj.iojbl.cn

[R61] 磁盘占用
来源：http://cjm.gotoacloud.top

df -h;  du -sh *
来源：http://hsg.guowangkeji.top

[R62] 找最占空间的文件
来源：http://rqm.gzhubu.top

du -ah . | sort -rh | head -10
来源：http://iiv.bjfxy.top

[R63] 内存与进程
来源：http://xwj.yfazqb.com

free -h;  ps aux | grep nginx
来源：http://afp.chenlongwang.top

[R64] 结束进程
来源：http://cxm.epnwcf.com

kill -9 $(pgrep -f app.py)
来源：http://eux.quarkkingdee.top

[R65] 查看端口占用
来源：http://chy.nanxuanxn.top


<!-- 参考信息 -->