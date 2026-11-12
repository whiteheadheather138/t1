代发 wailian999

[Q14] 存在则更新（upsert）
来源：http://ddi.daxiang520.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://oqu.yvedp.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://jme.yj20258888.top

[Q15] 查询全部
来源：http://mlb.sweek.top

SELECT * FROM users;
来源：http://bda.zdbjq.cn

[Q16] 查询指定列
来源：http://iut.dianchejie.cn

SELECT id, name FROM users;
来源：http://eku.ydjk.org.cn

[Q17] 条件查询
来源：http://rsj.yfazqb.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://twz.nanxinkj.top

[Q18] 模糊匹配
来源：http://wzj.yuanzhike.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://cqt.gaohongyu789.top

[Q19] 范围查询
来源：http://ssk.svipenyu.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://qed.fanxiaobao.xyz

[Q20] IN 列表
来源：http://omx.cucudq.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://jde.jinqigufen.top

[Q21] 空值判断
来源：http://pnp.tian-w.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://wmw.smart0.xyz

[Q22] 排序
来源：http://ojc.sysykeji.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://goo.nanxinkj.top

[Q23] 分页
来源：http://pun.xylfe.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://uqn.shanyushiyangkeji.top

[Q24] 去重
来源：http://ost.sufxvd.cn

SELECT DISTINCT city FROM users;
来源：http://win.yanxiufei.cn

[Q25] 只取前 N 条
来源：http://vaj.yj20258.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hny.nanxuanxn.top

[Q26] 计数
来源：http://odt.wangdashe.top

SELECT COUNT(*) FROM users;
来源：http://czl.guowangkeji.top

[Q27] 条件计数
来源：http://pbl.xuanzx.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://byv.jyoumei.cn

[Q28] 求和与平均
来源：http://zzn.vqdsnc.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wka.feifeiyinyue.top

[Q29] 最大最小值
来源：http://ufn.dianchejie.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://fxv.zhixingplan.top

[Q30] 分组统计
来源：http://tnc.dashuyun.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://yow.yj202588.top

[Q31] 分组后过滤
来源：http://zkd.shangyingyoupin.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://xco.hongshengwenyu.top

[Q32] 分组拼接字符串
来源：http://ppj.aizwys.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://itf.sufxvd.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hfy.chenzaomai.com

[Q33] 多列分组
来源：http://yka.c1oappe.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://jnk.gotoacloud.top

[Q34] 每组取第一条
来源：http://mcm.cucudq.cn

SELECT * FROM (
来源：http://iyp.chenzaomai.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wte.ivvv.top

) t WHERE rn = 1;
来源：http://awj.sjlbkw.cn

[Q35] 内连接
来源：http://zrm.wangshuangyany.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://gmy.iojbl.cn

[Q36] 左连接
来源：http://opw.xziqi.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ndv.yj20258.top

[Q37] 右连接
来源：http://nsf.jinghuilouyu.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://klx.9152youxi.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ods.nanxuanxn.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ike.yvedp.cn

[Q39] 自连接（查上下级）
来源：http://gvx.cashguo.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://wex.jyoumei.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://syc.0kj1m.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://kqb.hcnkem.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://yie.jyoumei.cn

[Q41] 多表连接
来源：http://uud.redwolf501.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://dao.quarkkingdee.top

JOIN users u ON u.id = o.user_id
来源：http://eyv.yongpay.top

JOIN products p ON p.id = o.product_id;
来源：http://btv.andypj.xyz

[Q42] 连接条件附加过滤
来源：http://rti.nwbrower.top

SELECT u.name, o.amount FROM users u
来源：http://zcu.0kj1m.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ngq.ctjpmb.com

[Q43] 标量子查询
来源：http://man.daxiang520.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://xce.pengpengdd.cyou

[Q44] IN 子查询
来源：http://six.daxiang520.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://uyk.sjlbkw.cn

[Q45] EXISTS 判断存在
来源：http://vgx.dianchejie.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://tpp.hysaishi.cn

[Q46] NOT EXISTS 判断不存在
来源：http://vaq.xingfuxueyuan.xyz

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bwm.9152youxi.cn

[Q47] 与平均值比较
来源：http://rbm.cdnleiting.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://nzt.meibo888.top

[Q48] CTE 公用表表达式
来源：http://fsz.yanxiufei.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://zbb.jinqigufen.top

SELECT * FROM t WHERE c > 5;
来源：http://gpa.tianlin.xyz

[Q49] 更新单行
来源：http://kfd.jinyuanbaomall.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://xby.meibo888.top

[Q50] 批量更新
来源：http://opy.nwbrower.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://vsp.ywan-chungtsiang.top

[Q51] 用子查询更新
来源：http://vxo.hfpthk.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://oei.chenzaomai.com

[Q52] 删除指定行
来源：http://kid.zhaomingkeji.xyz

DELETE FROM users WHERE id = 10;
来源：http://qpf.zycfv.cn

[Q53] 按条件删除
来源：http://xtp.shangyingyoupin.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://myp.jianghu66.top

[Q54] 清空表
来源：http://ebx.jinyuanbaomall.cn

TRUNCATE TABLE logs;
来源：http://bej.xziqi.cn

[Q55] 排名（并列占位）
来源：http://dyp.9152youxi.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://smw.zdbjq.cn

[Q56] 密集排名（并列不占位）
来源：http://syt.jinqigfzy.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://sou.hywenlv.cn

[Q57] 行号
来源：http://qys.ehwqpu.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://vaj.meibo888.top

[Q58] 累计求和
来源：http://mmi.ywan-chungtsiang.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mac.sysykeji.top

[Q59] 分组内累计
来源：http://qkl.vqdsnc.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://gyh.chenlongwang.top

[Q60] 取上一行 / 下一行
来源：http://yed.0kj1m.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://lxz.chenjidiqi.icu

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ugd.fehbvm.com

[Q61] 移动平均
来源：http://elj.ywan-chungtsiang.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://aav.shanyushiyangkeji.top

[Q62] 分组占比
来源：http://ztj.cqqwz.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ybx.yvedp.cn

[Q63] 开启事务
来源：http://bha.yuxming.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://vkg.jinyuanbaomall.cn

[Q64] 提交事务
来源：http://qtg.aibaodan.cn

COMMIT;
来源：http://dcn.vqdsnc.cn

[Q65] 回滚事务
来源：http://rrv.gotoacloud.top

ROLLBACK;
来源：http://mda.meibo888.top

[Q66] 行锁查询
来源：http://yez.aibaodan.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://sxx.hammf.cn

[Q67] 设置隔离级别
来源：http://itg.hfpthk.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://xne.zdqjudy.top

[Q68] 保存点
来源：http://fbn.dashuyun.cn

SAVEPOINT sp1;
来源：http://kho.shuidangran.top

ROLLBACK TO sp1;
来源：http://fhd.cqqwz.cn

[Q69] 查看执行计划
来源：http://fre.ydzc1.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://dwq.daria6918.cn

[Q70] 更新统计信息
来源：http://gwd.dianchejie.cn

ANALYZE TABLE users;
来源：http://nxb.ydjk.org.cn

[Q71] 查看建表语句
来源：http://jza.ydjk.org.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mcg.epnwcf.com

[Q72] 查看索引
来源：http://gmj.zhaomingkeji.xyz

SHOW INDEX FROM users;
来源：http://dqu.yangfankeji.com

[Q73] 查看表状态
来源：http://tyw.gaohongyu789.top

SHOW TABLE STATUS LIKE 'users';
来源：http://hzr.zhaomingkeji.xyz

[Q74] 强制使用索引
来源：http://sku.tanke756.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://xwc.nanxuanxn.top

[Q75] 日期格式化
来源：http://chk.yangfankeji.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hjx.316326.xyz

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ths.nwbrower.top

[Q76] 按天统计
来源：http://cwi.chenlongwang.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://nwb.meibo888.top

[Q77] 时间加减
来源：http://fwg.yonumen.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hwk.fehbvm.com

[Q78] 当前时间
来源：http://xkc.uphjek.com

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://qgp.fanxiaobao.xyz

[Q79] 字符串拼接
来源：http://jqo.hongshengwenyu.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://luk.jqgufenzy.top

[Q80] 字符串截取
来源：http://wod.chenlongwang.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://bgi.yuanzhike.top

[Q81] 字符串替换
来源：http://hjw.nwbrower.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://xfr.xuanzx.com

[Q82] 字符长度与字节长度
来源：http://bda.jlsjyb.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://dmm.zhijiandao.cn

[Q83] 大小写转换
来源：http://gzw.dashuyun.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://qen.zhengqikj.top

[Q84] 去除首尾空格
来源：http://jmq.zhixingplan.top

SELECT TRIM(name) FROM users;
来源：http://zuz.daxiang520.top

[Q85] 数值取整
来源：http://zwj.guannengcc.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://gcl.zhaomingkeji.xyz

[Q86] 读取 JSON 字段
来源：http://hvj.cucudq.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://tww.uphjek.com

[Q87] JSON 字段做条件
来源：http://wxr.yonumen.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://vog.snrcjt.cn

[Q88] 行转列（条件聚合）
来源：http://pjk.gogol.net.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wep.tanke756.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://lkg.yangfankeji.com

[Q89] 判断表是否存在
来源：http://knq.xuanzx.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://zig.birdmap.top

[Q90] 生成序号列
来源：http://rdv.ppjwa.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://nkc.sxryk.cn

================================================================================
来源：http://uud.ivvv.top

R. Bash 专题
来源：http://wwz.yj202588.top

================================================================================
来源：http://bty.xylfe.cn

[R01] shebang 与严格模式
来源：http://qgy.xziqi.cn

#!/usr/bin/env bash
来源：http://eek.bbcook.cn

set -euo pipefail
来源：http://knu.zhoulong.xyz

[R02] 变量赋值与使用
来源：http://sgq.yanxiufei.cn

name="Tom"; echo "$name"
来源：http://wjb.gotoacloud.top

[R03] 只读变量
来源：http://lfy.bbcook.cn

readonly PI=3.14
来源：http://jfy.hcnkem.com

[R04] 位置参数
来源：http://wta.jqgfzy.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://cpa.tarul.cn

[R05] 参数默认值
来源：http://brq.chenjidiqi.icu

name="${1:-default}"
来源：http://xbu.cheryme.top

[R06] 判断命令是否存在
来源：http://ipd.fktsv.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://uaw.shzxlz.cn

[R07] if 判断文件
来源：http://ezy.yj20258.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://vwc.jiagoushi.top

[R08] 数值比较
来源：http://kza.jinyuanbaomall.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://sbb.bjfxy.top

[R09] 字符串比较
来源：http://qgs.ydzc1.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://sbt.gzhubu.top

[R10] 正则匹配
来源：http://zcf.cheryme.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://gxb.zdqjudy.top

[R11] case 多分支
来源：http://yts.zhiwuduotai.top

case "$1" in
来源：http://lnr.9152youxi.cn

start) echo "启动" ;;
来源：http://dbd.ydjk.org.cn

stop)  echo "停止" ;;
来源：http://xmf.316326.xyz

*)     echo "未知命令" ;;
来源：http://cch.daria6918.cn

esac
来源：http://isd.aizwys.cn

[R12] for 遍历文件
来源：http://qrd.ivvv.top

for f in *.txt; do echo "$f"; done
来源：http://uut.gogol.net.cn

[R13] for 计数循环
来源：http://ugg.kuanghao11.cn

for i in {1..10}; do echo "$i"; done
来源：http://upy.guannengcc.top

[R14] C 风格 for
来源：http://fql.jqgfzy.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://lmv.sysykeji.top

[R15] while 逐行读文件
来源：http://fmi.nwbrower.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://tou.guowangkeji.top

[R16] until 等待条件
来源：http://tuh.0kj1m.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://dbd.ydzc1.top

[R17] 数组定义与取值
来源：http://wul.iojbl.cn

arr=(a b c); echo "${arr[0]}"
来源：http://aan.jianghu66.top

[R18] 遍历数组
来源：http://cdm.zhiwuduotai.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://yoq.daxiang520.top

[R19] 数组长度
来源：http://pef.shuidangran.top

echo "${#arr[@]}"
来源：http://wdo.feifeiyinyue.top

[R20] 关联数组（字典）
来源：http://adc.iojbl.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://maz.zhengqikj.top

[R21] 字符串长度
来源：http://rfk.iojbl.cn

echo "${#s}"
来源：http://yvw.xinyue.icu

[R22] 截取子串
来源：http://ebt.jinqigufen.top

echo "${s:0:5}"
来源：http://ozs.zdbjq.cn

[R23] 字符串替换
来源：http://zhi.wangdashe.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://dym.ydjk.org.cn

[R24] 大小写转换
来源：http://jgt.sjlbkw.cn

echo "${s^^}"; echo "${s,,}"
来源：http://lrb.yueranfly.top

[R25] 去后缀 / 去前缀
来源：http://vpr.shanyushiyangtech.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://fou.cdnleiting.top

[R26] 命令替换
来源：http://uer.snrcjt.cn

now=$(date +%F); echo "$now"
来源：http://bvs.yongpay.top

[R27] 算术展开
来源：http://mmb.gaohongyu789.top

echo $((1 + 2 * 3))
来源：http://kte.cucudq.cn

[R28] 浮点运算
来源：http://udk.meibo888.top

echo "scale=2; 10/3" | bc
来源：http://hzc.wangshuangyany.cn

[R29] 定义函数
来源：http://iqs.zhiwuduotai.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://qhf.zhaomingkeji.xyz

[R30] 函数返回状态码
来源：http://dah.kuanghao11.cn

f() { return 0; }; f || echo "失败了"
来源：http://jqy.zhaomingkeji.xyz

[R31] 局部变量
来源：http://tba.nanxuanxn.top

f() { local x=1; echo "$x"; }
来源：http://jwf.ywan-chungtsiang.top

[R32] 参数个数校验
来源：http://eyj.bbcook.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ihu.ctjpmb.com

[R33] 捕获错误并提示行号
来源：http://kkq.yvedp.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ttb.hysaishi.cn

[R34] 退出时清理
来源：http://xws.xylfe.cn

trap 'rm -f "$tmp"' EXIT
来源：http://sik.yongpay.top

[R35] 后台执行并等待
来源：http://ydf.jiagoushi.top

sleep 5 & pid=$!; wait "$pid"
来源：http://lio.ydjk.org.cn

[R36] 并发执行多个任务
来源：http://dzk.kuanghao11.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://kkr.daxiang520.top

[R37] 把输出赋给变量
来源：http://pgr.vehdjk.com

files=$(ls -1)
来源：http://smj.vqdsnc.cn

[R38] 管道串联
来源：http://nze.wangdashe.top

cat a.txt | grep -i error | wc -l
来源：http://czp.jianghu66.top

[R39] 重定向标准输出与错误
来源：http://gdo.jyoumei.cn

cmd > out.log 2>&1
来源：http://nxl.mhx1999.top

[R40] 追加写日志
来源：http://eie.zhengqikj.top

echo "log" >> out.log
来源：http://soq.yuanzhike.top

[R41] 丢弃输出
来源：http://cce.yanxiufei.cn

cmd >/dev/null 2>&1
来源：http://fvd.hammf.cn

[R42] 输入重定向
来源：http://tzw.pengpengdd.cyou

wc -l < a.txt
来源：http://nic.ehwqpu.com

[R43] 按名字查找文件
来源：http://mnr.vqdsnc.cn

find . -name "*.log" -type f
来源：http://krj.cucudq.cn

[R44] 按修改时间查找
来源：http://iub.9152youxi.cn

find . -mtime -7 -type f
来源：http://wsb.ybcxt.top

[R45] 批量删除
来源：http://ngg.sweek.top

find . -name "*.tmp" -delete
来源：http://lnq.tianlin.xyz

[R46] 递归替换文件内容
来源：http://ylf.daxiang520.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hqb.fanxiaobao.xyz

[R47] sed 单行替换
来源：http://whc.jyoumei.cn

sed -i 's/foo/bar/g' a.txt
来源：http://epz.hysaishi.cn

[R48] awk 取指定列
来源：http://xod.ctjpmb.com

awk '{print $1, $3}' a.txt
来源：http://ltg.zhaomingkeji.xyz

[R49] awk 带条件
来源：http://ovy.fengsongda.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ntg.smart0.xyz

[R50] awk 求和
来源：http://yml.smart0.xyz

awk '{s += $2} END {print s}' a.txt
来源：http://tjy.cqqwz.cn

[R51] 排序去重取前几
来源：http://ktu.yj20258888.top

sort a.txt | uniq -c | sort -rn | head
来源：http://kyd.nanxuanxn.top

[R52] 统计行数
来源：http://nto.cheryme.top

wc -l a.txt
来源：http://xnk.birdmap.top

[R53] 查看文件头与实时尾
来源：http://mkz.cdnleiting.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mxm.chenjidiqi.icu

[R54] 比较两个文件
来源：http://kok.jyoumei.cn

diff a.txt b.txt
来源：http://soj.fzhhl.top

[R55] 压缩与解压
来源：http://vop.ctjpmb.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://omw.daxiang520.top

[R56] 远程拷贝
来源：http://zbn.gzhubu.top

scp file user@host:/path/
来源：http://rrz.xuetiantiany.cn

[R57] 远程执行命令
来源：http://fxj.feifeiyinyue.top

ssh user@host 'uptime'
来源：http://uwu.gotoacloud.top

[R58] 下载文件
来源：http://czc.52xcode.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hfs.sweek.top

[R59] 发 POST JSON
来源：http://ikt.pengpengdd.cyou

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://qro.yj202588.top

[R60] 只看 HTTP 状态码
来源：http://pxc.fengsongda.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://pjk.zhijiandao.cn

[R61] 磁盘占用
来源：http://biz.jinyuanbaomall.cn

df -h;  du -sh *
来源：http://cnw.ehwqpu.com

[R62] 找最占空间的文件
来源：http://tir.hcnkem.com

du -ah . | sort -rh | head -10
来源：http://emz.hnxiangtu.top

[R63] 内存与进程
来源：http://fge.yvedp.cn


<!-- 参考信息 -->