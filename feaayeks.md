代发 wailian999

[Q14] 存在则更新（upsert）
来源：http://vsm.jianghu66.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://zlv.nanxuanxn.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://qfc.cashguo.top

[Q15] 查询全部
来源：http://afq.tian-w.cn

SELECT * FROM users;
来源：http://cru.svipenyu.cn

[Q16] 查询指定列
来源：http://qbt.shuidangran.top

SELECT id, name FROM users;
来源：http://gwy.svipenyu.cn

[Q17] 条件查询
来源：http://fam.birdmap.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://erg.feifeiyinyue.top

[Q18] 模糊匹配
来源：http://zno.c1oappe.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://seq.gaohongyu789.top

[Q19] 范围查询
来源：http://rza.zhengqikj.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://myt.xuetiantiany.cn

[Q20] IN 列表
来源：http://hfl.yuxming.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ftt.9152youxi.cn

[Q21] 空值判断
来源：http://cvv.zhiwuduotai.top

SELECT * FROM users WHERE email IS NULL;
来源：http://xdk.yj20258888.top

[Q22] 排序
来源：http://tmg.wangshuangyany.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://osn.yj202588.top

[Q23] 分页
来源：http://mpa.redwolf501.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://app.fanxiaobao.xyz

[Q24] 去重
来源：http://ypw.aizwys.cn

SELECT DISTINCT city FROM users;
来源：http://ymx.quarkkingdee.top

[Q25] 只取前 N 条
来源：http://otv.ehwqpu.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://lqj.svipenyu.cn

[Q26] 计数
来源：http://usj.yj20258.top

SELECT COUNT(*) FROM users;
来源：http://fpt.ywan-chungtsiang.top

[Q27] 条件计数
来源：http://blm.jinqigfzy.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://nez.jianghu66.top

[Q28] 求和与平均
来源：http://jxb.tarul.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://afg.quarkkingdee.top

[Q29] 最大最小值
来源：http://ohp.hysaishi.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://xsn.birdmap.top

[Q30] 分组统计
来源：http://zxn.zhiwuduotai.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://fbi.svipenyu.cn

[Q31] 分组后过滤
来源：http://szs.guannengcc.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ejo.xziqi.cn

[Q32] 分组拼接字符串
来源：http://dgt.chenlongwang.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://kva.nanxuanxn.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ezb.gotoacloud.top

[Q33] 多列分组
来源：http://kpi.hammf.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://paw.yonumen.top

[Q34] 每组取第一条
来源：http://hkd.gzhubu.top

SELECT * FROM (
来源：http://vxk.c1oappe.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://qth.yvedp.cn

) t WHERE rn = 1;
来源：http://hea.bjfxy.top

[Q35] 内连接
来源：http://rvd.hcnkem.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://fgm.zhoulong.xyz

[Q36] 左连接
来源：http://ijb.ydzc1.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ilr.gzhubu.top

[Q37] 右连接
来源：http://eem.jqgfzy.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://nmr.dashuyun.cn

[Q38] 全外连接（PostgreSQL）
来源：http://dus.ivvv.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mdj.sysykeji.top

[Q39] 自连接（查上下级）
来源：http://cyi.epnwcf.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://qrk.gogol.net.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://xpg.zycfv.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://lja.ybcxt.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://zbd.redwolf501.top

[Q41] 多表连接
来源：http://lww.bbcook.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://pmv.jinqigufen.top

JOIN users u ON u.id = o.user_id
来源：http://ifk.fengsongda.top

JOIN products p ON p.id = o.product_id;
来源：http://xxi.jlsjyb.cn

[Q42] 连接条件附加过滤
来源：http://smr.ivvv.top

SELECT u.name, o.amount FROM users u
来源：http://aio.zhoulong.xyz

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://bbk.andypj.xyz

[Q43] 标量子查询
来源：http://nrz.nanxinkj.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://jxa.yongpay.top

[Q44] IN 子查询
来源：http://kfz.fengsongda.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://zsr.epnwcf.com

[Q45] EXISTS 判断存在
来源：http://zxr.bbcook.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jxv.yuxming.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ujr.zhiwuduotai.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ayp.ivvv.top

[Q47] 与平均值比较
来源：http://yjw.kuanghao11.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://eiy.svipenyu.cn

[Q48] CTE 公用表表达式
来源：http://mwv.daxiang520.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://kfd.vqdsnc.cn

SELECT * FROM t WHERE c > 5;
来源：http://zhj.jqgufenzy.top

[Q49] 更新单行
来源：http://fnz.yonumen.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://zlg.dashuyun.cn

[Q50] 批量更新
来源：http://ukw.dashuyun.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://flk.yanxiufei.cn

[Q51] 用子查询更新
来源：http://xrw.tarul.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mjc.xziqi.cn

[Q52] 删除指定行
来源：http://oht.9152youxi.cn

DELETE FROM users WHERE id = 10;
来源：http://puq.zhiwuduotai.top

[Q53] 按条件删除
来源：http://hpm.gotoacloud.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://kni.shangyingyoupin.top

[Q54] 清空表
来源：http://rnn.fengsongda.top

TRUNCATE TABLE logs;
来源：http://xos.tarul.cn

[Q55] 排名（并列占位）
来源：http://lmp.tanke756.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ewn.pengpengdd.cyou

[Q56] 密集排名（并列不占位）
来源：http://kku.shanyushiyangkeji.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://sgb.jyoumei.cn

[Q57] 行号
来源：http://chm.ybcxt.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mes.dashuyun.cn

[Q58] 累计求和
来源：http://spc.yj20258888.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://tiy.nanxinkj.top

[Q59] 分组内累计
来源：http://iqx.xinyue.icu

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://fqe.cashguo.top

[Q60] 取上一行 / 下一行
来源：http://hjv.chenlongwang.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ikz.cashguo.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://inr.ehwqpu.com

[Q61] 移动平均
来源：http://lvl.fktsv.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://gfq.redwolf501.top

[Q62] 分组占比
来源：http://fwn.hongshengwenyu.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ofm.yonumen.top

[Q63] 开启事务
来源：http://pfj.hesvh.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://kyf.c1oappe.top

[Q64] 提交事务
来源：http://txb.snrcjt.cn

COMMIT;
来源：http://xbd.hammf.cn

[Q65] 回滚事务
来源：http://lld.fengsongda.top

ROLLBACK;
来源：http://fmw.fengsongda.top

[Q66] 行锁查询
来源：http://lzc.bjfxy.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://rkq.tian-w.cn

[Q67] 设置隔离级别
来源：http://wpx.yangfankeji.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://brf.shangyingyoupin.top

[Q68] 保存点
来源：http://fpl.ywan-chungtsiang.top

SAVEPOINT sp1;
来源：http://xhn.hnqzz.top

ROLLBACK TO sp1;
来源：http://hhg.tanke756.top

[Q69] 查看执行计划
来源：http://kgz.hysaishi.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ths.iojbl.cn

[Q70] 更新统计信息
来源：http://fgf.snrcjt.cn

ANALYZE TABLE users;
来源：http://ect.gogol.net.cn

[Q71] 查看建表语句
来源：http://azb.yanxiufei.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://iei.jlsjyb.cn

[Q72] 查看索引
来源：http://szf.bjfxy.top

SHOW INDEX FROM users;
来源：http://nqi.yueranfly.top

[Q73] 查看表状态
来源：http://qyz.feifeiyinyue.top

SHOW TABLE STATUS LIKE 'users';
来源：http://hdg.jianghu66.top

[Q74] 强制使用索引
来源：http://syt.zycfv.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://kcw.daria6918.cn

[Q75] 日期格式化
来源：http://pmq.andypj.xyz

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://srg.shanyushiyangkeji.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ril.fehbvm.com

[Q76] 按天统计
来源：http://jcu.0kj1m.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://flf.zhijiandao.cn

[Q77] 时间加减
来源：http://yds.jlsjyb.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mhk.zdqjudy.top

[Q78] 当前时间
来源：http://owt.hesvh.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wvd.fanxiaobao.xyz

[Q79] 字符串拼接
来源：http://kaq.zhaomingkeji.xyz

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://iic.zycfv.cn

[Q80] 字符串截取
来源：http://tca.daxiang520.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://qut.bbcook.cn

[Q81] 字符串替换
来源：http://sfx.nanxinkj.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://gdc.chenjidiqi.icu

[Q82] 字符长度与字节长度
来源：http://yrw.xinyue.icu

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://faq.vehdjk.com

[Q83] 大小写转换
来源：http://amb.uphjek.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://iqj.pycfn.com

[Q84] 去除首尾空格
来源：http://dgj.sjlbkw.cn

SELECT TRIM(name) FROM users;
来源：http://awt.zycfv.cn

[Q85] 数值取整
来源：http://peg.yonumen.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://qmo.meibo888.top

[Q86] 读取 JSON 字段
来源：http://nfr.fehbvm.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://tef.shanyushiyangtech.top

[Q87] JSON 字段做条件
来源：http://uwy.wangdashe.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://idv.fengsongda.top

[Q88] 行转列（条件聚合）
来源：http://yzp.xinyue.icu

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://day.shzxlz.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://dcn.zhaomingkeji.xyz

[Q89] 判断表是否存在
来源：http://ojp.zdbjq.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://frt.hammf.cn

[Q90] 生成序号列
来源：http://vfd.ehwqpu.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://bqa.sufxvd.cn

================================================================================
来源：http://jll.birdmap.top

R. Bash 专题
来源：http://imm.fengsongda.top

================================================================================
来源：http://rmh.guannengcc.top

[R01] shebang 与严格模式
来源：http://pdg.aizwys.cn

#!/usr/bin/env bash
来源：http://qpo.jinqigufen.top

set -euo pipefail
来源：http://qsg.redwolf501.top

[R02] 变量赋值与使用
来源：http://dfi.xuanzx.com

name="Tom"; echo "$name"
来源：http://ybi.uphjek.com

[R03] 只读变量
来源：http://qbb.kuanghao11.cn

readonly PI=3.14
来源：http://sru.jinqigfzy.top

[R04] 位置参数
来源：http://ria.iojbl.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://bgf.jinqigufen.top

[R05] 参数默认值
来源：http://yay.tian-w.cn

name="${1:-default}"
来源：http://zrz.0kj1m.cn

[R06] 判断命令是否存在
来源：http://qdv.yj20258.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wea.nwbrower.top

[R07] if 判断文件
来源：http://eyy.jinghuilouyu.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://yle.redwolf501.top

[R08] 数值比较
来源：http://ktk.9152youxi.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://fcf.tian-w.cn

[R09] 字符串比较
来源：http://sku.redwolf501.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://jdq.hammf.cn

[R10] 正则匹配
来源：http://kxk.yj202588.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://jbj.xziqi.cn

[R11] case 多分支
来源：http://mbi.smart0.xyz

case "$1" in
来源：http://sqb.jiagoushi.top

start) echo "启动" ;;
来源：http://cuw.haohaochexian.top

stop)  echo "停止" ;;
来源：http://aqq.zdbjq.cn

*)     echo "未知命令" ;;
来源：http://vst.gotoacloud.top

esac
来源：http://qvl.tanke756.top

[R12] for 遍历文件
来源：http://bsn.chenlongwang.top

for f in *.txt; do echo "$f"; done
来源：http://eey.sysykeji.top

[R13] for 计数循环
来源：http://uwe.ybcxt.top

for i in {1..10}; do echo "$i"; done
来源：http://gkv.shanyushiyangtech.top

[R14] C 风格 for
来源：http://omy.daxiang520.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://nfw.c1oappe.top

[R15] while 逐行读文件
来源：http://xzw.316326.xyz

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://pwz.epnwcf.com

[R16] until 等待条件
来源：http://gda.zhoulong.xyz

until [[ -f done.flag ]]; do sleep 1; done
来源：http://abx.ydzc1.top

[R17] 数组定义与取值
来源：http://uiw.zhaomingkeji.xyz

arr=(a b c); echo "${arr[0]}"
来源：http://kcz.xuetiantiany.cn

[R18] 遍历数组
来源：http://und.sxryk.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://lyk.vqdsnc.cn

[R19] 数组长度
来源：http://iyz.dianchejie.cn

echo "${#arr[@]}"
来源：http://wqu.zhiwuduotai.top

[R20] 关联数组（字典）
来源：http://hje.cheryme.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://acg.yueranfly.top

[R21] 字符串长度
来源：http://gwu.zhaomingkeji.xyz

echo "${#s}"
来源：http://fju.aibaodan.cn

[R22] 截取子串
来源：http://zvj.xylfe.cn

echo "${s:0:5}"
来源：http://hpl.birdmap.top

[R23] 字符串替换
来源：http://jor.fzhhl.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://cpl.xuetiantiany.cn

[R24] 大小写转换
来源：http://hfw.zhongyouzk.top

echo "${s^^}"; echo "${s,,}"
来源：http://cvr.fzhhl.top

[R25] 去后缀 / 去前缀
来源：http://phy.mhx1999.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://cuu.svipenyu.cn

[R26] 命令替换
来源：http://zbh.shangyingyoupin.top

now=$(date +%F); echo "$now"
来源：http://sqx.andypj.xyz

[R27] 算术展开
来源：http://uwe.zhaomingkeji.xyz

echo $((1 + 2 * 3))
来源：http://zgg.feifeiyinyue.top

[R28] 浮点运算
来源：http://phr.fengsongda.top

echo "scale=2; 10/3" | bc
来源：http://oha.gogol.net.cn

[R29] 定义函数
来源：http://hfp.uphjek.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://pxd.hfpthk.cn

[R30] 函数返回状态码
来源：http://dmn.feifeiyinyue.top

f() { return 0; }; f || echo "失败了"
来源：http://sjj.jqgfzy.top

[R31] 局部变量
来源：http://ypt.havefunace.top

f() { local x=1; echo "$x"; }
来源：http://gbt.tian-w.cn

[R32] 参数个数校验
来源：http://euy.xingfuxueyuan.xyz

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://evu.meibo888.top

[R33] 捕获错误并提示行号
来源：http://tjl.yonumen.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://dwv.hysaishi.cn

[R34] 退出时清理
来源：http://vbt.jinyuanbaomall.cn

trap 'rm -f "$tmp"' EXIT
来源：http://kkf.tanke756.top

[R35] 后台执行并等待
来源：http://yuh.xylfe.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://skl.cdnleiting.top

[R36] 并发执行多个任务
来源：http://ygb.xziqi.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://iej.aizwys.cn

[R37] 把输出赋给变量
来源：http://luy.316326.xyz

files=$(ls -1)
来源：http://tro.shanyushiyangtech.top

[R38] 管道串联
来源：http://wqu.ywan-chungtsiang.top

cat a.txt | grep -i error | wc -l
来源：http://ani.fehbvm.com

[R39] 重定向标准输出与错误
来源：http://xvo.hammf.cn

cmd > out.log 2>&1
来源：http://ydr.feifeiyinyue.top

[R40] 追加写日志
来源：http://fkk.gzhubu.top

echo "log" >> out.log
来源：http://qvq.fanxiaobao.xyz

[R41] 丢弃输出
来源：http://ggb.cdnleiting.top

cmd >/dev/null 2>&1
来源：http://rcb.daxiang520.top

[R42] 输入重定向
来源：http://haf.shzxlz.cn

wc -l < a.txt
来源：http://voa.sweek.top

[R43] 按名字查找文件
来源：http://zwt.sufxvd.cn

find . -name "*.log" -type f
来源：http://jtv.ydjk.org.cn

[R44] 按修改时间查找
来源：http://yqt.ydjk.org.cn

find . -mtime -7 -type f
来源：http://hzn.0kj1m.cn

[R45] 批量删除
来源：http://swl.quarkkingdee.top

find . -name "*.tmp" -delete
来源：http://rgf.jinqigfzy.top

[R46] 递归替换文件内容
来源：http://ntk.andypj.xyz

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://abr.cucudq.cn

[R47] sed 单行替换
来源：http://dwo.jqgfzy.top

sed -i 's/foo/bar/g' a.txt
来源：http://sps.52xcode.cn

[R48] awk 取指定列
来源：http://zbs.vehdjk.com

awk '{print $1, $3}' a.txt
来源：http://gou.hnxiangtu.top

[R49] awk 带条件
来源：http://odt.guannengcc.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://zsk.vehdjk.com

[R50] awk 求和
来源：http://kyb.redwolf501.top

awk '{s += $2} END {print s}' a.txt
来源：http://ewg.aizwys.cn

[R51] 排序去重取前几
来源：http://sto.zhixingplan.top

sort a.txt | uniq -c | sort -rn | head
来源：http://scr.jinghuilouyu.cn

[R52] 统计行数
来源：http://sjg.yj20258888.top

wc -l a.txt
来源：http://bmd.jqgfzy.top

[R53] 查看文件头与实时尾
来源：http://gzn.chenlongwang.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://xmz.hesvh.cn

[R54] 比较两个文件
来源：http://vcs.aibaodan.cn

diff a.txt b.txt
来源：http://sac.chenlongwang.top

[R55] 压缩与解压
来源：http://snx.chenlongwang.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://zry.zhiwuduotai.top

[R56] 远程拷贝
来源：http://wdh.tarul.cn

scp file user@host:/path/
来源：http://ryv.smart0.xyz

[R57] 远程执行命令
来源：http://swx.sysykeji.top

ssh user@host 'uptime'
来源：http://www.jyoumei.cn

[R58] 下载文件
来源：http://rbu.ybcxt.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ivq.chenjidiqi.icu

[R59] 发 POST JSON
来源：http://ciz.yj202588.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://znu.yfazqb.com

[R60] 只看 HTTP 状态码
来源：http://tli.hysaishi.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://fqf.ppjwa.cn

[R61] 磁盘占用
来源：http://szw.yonumen.top

df -h;  du -sh *
来源：http://lsn.yongpay.top

[R62] 找最占空间的文件
来源：http://nzz.sweek.top

du -ah . | sort -rh | head -10
来源：http://xmg.fzhhl.top

[R63] 内存与进程
来源：http://fjb.daria6918.cn


<!-- 参考信息 -->