代发 wailian999

INSERT INTO users (name) VALUES ('C');
来源：http://fxv.nanxuanxn.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://vqt.tanke756.top

[Q13] 忽略重复插入
来源：http://vvx.ywan-chungtsiang.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://kdj.316326.xyz

[Q14] 存在则更新（upsert）
来源：http://soy.guannengcc.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://tdv.xinyue.icu

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hkw.yvedp.cn

[Q15] 查询全部
来源：http://vgr.zhongyouzk.top

SELECT * FROM users;
来源：http://pzf.jyoumei.cn

[Q16] 查询指定列
来源：http://qme.shanyushiyangtech.top

SELECT id, name FROM users;
来源：http://ajp.aibaodan.cn

[Q17] 条件查询
来源：http://unc.hcnkem.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://moz.jinyuanbaomall.cn

[Q18] 模糊匹配
来源：http://fjt.jinqigufen.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mqf.hywenlv.cn

[Q19] 范围查询
来源：http://qsa.kuanghao11.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://aup.zhiwuduotai.top

[Q20] IN 列表
来源：http://zxf.yvedp.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://waf.ehwqpu.com

[Q21] 空值判断
来源：http://fan.bjfxy.top

SELECT * FROM users WHERE email IS NULL;
来源：http://mor.9152youxi.cn

[Q22] 排序
来源：http://fpi.9152youxi.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://osh.sufxvd.cn

[Q23] 分页
来源：http://pxs.bjfxy.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://qwr.jianghu66.top

[Q24] 去重
来源：http://kxh.xingfuxueyuan.xyz

SELECT DISTINCT city FROM users;
来源：http://zkq.tarul.cn

[Q25] 只取前 N 条
来源：http://kzu.ivvv.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://jyc.ybcxt.top

[Q26] 计数
来源：http://twk.jinqigufen.top

SELECT COUNT(*) FROM users;
来源：http://kty.bjfxy.top

[Q27] 条件计数
来源：http://exg.9152youxi.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://bzr.zycfv.cn

[Q28] 求和与平均
来源：http://dmd.snrcjt.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://jwg.chenlongwang.top

[Q29] 最大最小值
来源：http://itr.xziqi.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://cpo.xingfuxueyuan.xyz

[Q30] 分组统计
来源：http://uec.yanxiufei.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://dlh.xinyue.icu

[Q31] 分组后过滤
来源：http://ejo.ydzc1.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://pzr.daria6918.cn

[Q32] 分组拼接字符串
来源：http://kij.yvedp.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://woc.zycfv.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://qma.xziqi.cn

[Q33] 多列分组
来源：http://hfh.tian-w.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://xmq.ehwqpu.com

[Q34] 每组取第一条
来源：http://ame.ctjpmb.com

SELECT * FROM (
来源：http://ahk.cdnleiting.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://iec.ybcxt.top

) t WHERE rn = 1;
来源：http://zmk.nanxinkj.top

[Q35] 内连接
来源：http://nut.fktsv.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ueb.zhixingplan.top

[Q36] 左连接
来源：http://qsi.yueranfly.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://vfr.xinyue.icu

[Q37] 右连接
来源：http://xkk.shanyushiyangtech.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hpf.yanxiufei.cn

[Q38] 全外连接（PostgreSQL）
来源：http://vjk.dianchejie.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://flp.snrcjt.cn

[Q39] 自连接（查上下级）
来源：http://xyf.yuxming.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://bdr.sufxvd.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://dcg.jinqigfzy.top

[Q40] 交叉连接（笛卡尔积）
来源：http://ebb.zhiwuduotai.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hwq.meibo888.top

[Q41] 多表连接
来源：http://wwu.shanyushiyangkeji.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://pjg.yangfankeji.com

JOIN users u ON u.id = o.user_id
来源：http://cui.xziqi.cn

JOIN products p ON p.id = o.product_id;
来源：http://oew.jinqigufen.top

[Q42] 连接条件附加过滤
来源：http://hcv.tarul.cn

SELECT u.name, o.amount FROM users u
来源：http://uzk.redwolf501.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://yxv.hesvh.cn

[Q43] 标量子查询
来源：http://cvl.52xcode.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://knw.yangfankeji.com

[Q44] IN 子查询
来源：http://cdl.jinqigfzy.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://azj.ivvv.top

[Q45] EXISTS 判断存在
来源：http://iow.birdmap.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://uqt.tarul.cn

[Q46] NOT EXISTS 判断不存在
来源：http://xtb.xingfuxueyuan.xyz

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bxc.aibaodan.cn

[Q47] 与平均值比较
来源：http://ytn.shzxlz.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://caz.zhixingplan.top

[Q48] CTE 公用表表达式
来源：http://hmp.dianchejie.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ppz.tian-w.cn

SELECT * FROM t WHERE c > 5;
来源：http://jiz.pengpengdd.cyou

[Q49] 更新单行
来源：http://myl.uphjek.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://eic.cucudq.cn

[Q50] 批量更新
来源：http://yer.bbcook.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mpc.jianghu66.top

[Q51] 用子查询更新
来源：http://orv.daxiang520.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://krh.shzxlz.cn

[Q52] 删除指定行
来源：http://gfc.zhiwuduotai.top

DELETE FROM users WHERE id = 10;
来源：http://jkc.snrcjt.cn

[Q53] 按条件删除
来源：http://fna.daxiang520.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://fem.zycfv.cn

[Q54] 清空表
来源：http://evq.0kj1m.cn

TRUNCATE TABLE logs;
来源：http://yqg.aizwys.cn

[Q55] 排名（并列占位）
来源：http://cgu.haohaochexian.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://oea.nanxuanxn.top

[Q56] 密集排名（并列不占位）
来源：http://srt.xingfuxueyuan.xyz

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://qox.hysaishi.cn

[Q57] 行号
来源：http://kqa.sysykeji.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://qjg.zhijiandao.cn

[Q58] 累计求和
来源：http://xng.shzxlz.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://cou.9152youxi.cn

[Q59] 分组内累计
来源：http://gzl.jiagoushi.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://bcd.daria6918.cn

[Q60] 取上一行 / 下一行
来源：http://iih.zhiwuduotai.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://cty.xinyue.icu

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://fju.uphjek.com

[Q61] 移动平均
来源：http://amc.zdbjq.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://avv.xziqi.cn

[Q62] 分组占比
来源：http://eyj.jinyuanbaomall.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://vuz.havefunace.top

[Q63] 开启事务
来源：http://zpf.jinghuilouyu.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://wdj.shanyushiyangtech.top

[Q64] 提交事务
来源：http://qql.bbcook.cn

COMMIT;
来源：http://xka.chenzaomai.com

[Q65] 回滚事务
来源：http://ldw.dashuyun.cn

ROLLBACK;
来源：http://rrc.xuetiantiany.cn

[Q66] 行锁查询
来源：http://kcy.dashuyun.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://jma.feifeiyinyue.top

[Q67] 设置隔离级别
来源：http://axr.jlsjyb.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://atl.nwbrower.top

[Q68] 保存点
来源：http://vfp.yuxming.cn

SAVEPOINT sp1;
来源：http://kiu.jianghu66.top

ROLLBACK TO sp1;
来源：http://ddl.tarul.cn

[Q69] 查看执行计划
来源：http://fun.zycfv.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://moo.sxryk.cn

[Q70] 更新统计信息
来源：http://wcv.jqgfzy.top

ANALYZE TABLE users;
来源：http://afp.mhx1999.top

[Q71] 查看建表语句
来源：http://dzx.zhaomingkeji.xyz

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hbf.ehwqpu.com

[Q72] 查看索引
来源：http://rec.jinyuanbaomall.cn

SHOW INDEX FROM users;
来源：http://hng.gzhubu.top

[Q73] 查看表状态
来源：http://wko.316326.xyz

SHOW TABLE STATUS LIKE 'users';
来源：http://smq.aizwys.cn

[Q74] 强制使用索引
来源：http://ofg.uphjek.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://qay.ybcxt.top

[Q75] 日期格式化
来源：http://dmy.ywan-chungtsiang.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://gii.xziqi.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mig.zycfv.cn

[Q76] 按天统计
来源：http://fkb.sjlbkw.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wtg.hysaishi.cn

[Q77] 时间加减
来源：http://flq.havefunace.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://lzr.aibaodan.cn

[Q78] 当前时间
来源：http://kbz.c1oappe.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://vaw.ywan-chungtsiang.top

[Q79] 字符串拼接
来源：http://uok.xingfuxueyuan.xyz

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://aiq.smart0.xyz

[Q80] 字符串截取
来源：http://vou.hongshengwenyu.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://fye.fzhhl.top

[Q81] 字符串替换
来源：http://jgu.quarkkingdee.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://gzp.nanxuanxn.top

[Q82] 字符长度与字节长度
来源：http://nby.hammf.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://nhd.zhongyouzk.top

[Q83] 大小写转换
来源：http://owz.xinyue.icu

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mvu.chenzaomai.com

[Q84] 去除首尾空格
来源：http://zjg.pycfn.com

SELECT TRIM(name) FROM users;
来源：http://ypj.9152youxi.cn

[Q85] 数值取整
来源：http://adm.cqqwz.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://gnd.jyoumei.cn

[Q86] 读取 JSON 字段
来源：http://ckr.cdnleiting.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://slb.sufxvd.cn

[Q87] JSON 字段做条件
来源：http://mkq.fzhhl.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://tja.sweek.top

[Q88] 行转列（条件聚合）
来源：http://tyh.xinyue.icu

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://huw.aibaodan.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://dop.yueranfly.top

[Q89] 判断表是否存在
来源：http://keu.dianchejie.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://vjm.aibaodan.cn

[Q90] 生成序号列
来源：http://zgw.sufxvd.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://fkq.jinghuilouyu.cn

================================================================================
来源：http://iqj.dashuyun.cn

R. Bash 专题
来源：http://fic.yj20258888.top

================================================================================
来源：http://cwx.zdqjudy.top

[R01] shebang 与严格模式
来源：http://chi.jiagoushi.top

#!/usr/bin/env bash
来源：http://cfz.aizwys.cn

set -euo pipefail
来源：http://ojz.iojbl.cn

[R02] 变量赋值与使用
来源：http://gog.zhiwuduotai.top

name="Tom"; echo "$name"
来源：http://rou.shangyingyoupin.top

[R03] 只读变量
来源：http://xxy.yfazqb.com

readonly PI=3.14
来源：http://dee.yj20258888.top

[R04] 位置参数
来源：http://kde.guannengcc.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://xtt.havefunace.top

[R05] 参数默认值
来源：http://lnp.hongshengwenyu.top

name="${1:-default}"
来源：http://heu.316326.xyz

[R06] 判断命令是否存在
来源：http://gyw.daria6918.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ufw.havefunace.top

[R07] if 判断文件
来源：http://pym.hywenlv.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://tgg.ydjk.org.cn

[R08] 数值比较
来源：http://pex.andypj.xyz

if (( a > b )); then echo "a 更大"; fi
来源：http://geb.uphjek.com

[R09] 字符串比较
来源：http://aar.snrcjt.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://uay.haohaochexian.top

[R10] 正则匹配
来源：http://wem.pengpengdd.cyou

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://rai.9152youxi.cn

[R11] case 多分支
来源：http://ejh.tanke756.top

case "$1" in
来源：http://tve.yvedp.cn

start) echo "启动" ;;
来源：http://bgb.cashguo.top

stop)  echo "停止" ;;
来源：http://ctm.shanyushiyangkeji.top

*)     echo "未知命令" ;;
来源：http://yot.sxryk.cn

esac
来源：http://wlh.jqgfzy.top

[R12] for 遍历文件
来源：http://xyx.vqdsnc.cn

for f in *.txt; do echo "$f"; done
来源：http://ttb.iojbl.cn

[R13] for 计数循环
来源：http://xtp.yonumen.top

for i in {1..10}; do echo "$i"; done
来源：http://hly.shanyushiyangkeji.top

[R14] C 风格 for
来源：http://auy.nanxuanxn.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://qwz.jinghuilouyu.cn

[R15] while 逐行读文件
来源：http://nod.sjlbkw.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://jtu.shanyushiyangtech.top

[R16] until 等待条件
来源：http://cqz.yanxiufei.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://uqz.tanke756.top

[R17] 数组定义与取值
来源：http://yrx.tarul.cn

arr=(a b c); echo "${arr[0]}"
来源：http://syx.sjlbkw.cn

[R18] 遍历数组
来源：http://fvt.tanke756.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://kdv.hnqzz.top

[R19] 数组长度
来源：http://zpm.chenjidiqi.icu

echo "${#arr[@]}"
来源：http://bbm.sjlbkw.cn

[R20] 关联数组（字典）
来源：http://nsa.cucudq.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://kna.ydzc1.top

[R21] 字符串长度
来源：http://yus.zhaomingkeji.xyz

echo "${#s}"
来源：http://wgt.xylfe.cn

[R22] 截取子串
来源：http://rnq.yangfankeji.com

echo "${s:0:5}"
来源：http://syx.vehdjk.com

[R23] 字符串替换
来源：http://fln.cheryme.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://kpw.316326.xyz

[R24] 大小写转换
来源：http://jqi.vehdjk.com

echo "${s^^}"; echo "${s,,}"
来源：http://mzd.aizwys.cn

[R25] 去后缀 / 去前缀
来源：http://cxu.316326.xyz

echo "${f%.txt}"; echo "${f#./}"
来源：http://gjv.zycfv.cn

[R26] 命令替换
来源：http://ano.cucudq.cn

now=$(date +%F); echo "$now"
来源：http://vrc.xuetiantiany.cn

[R27] 算术展开
来源：http://atl.chenzaomai.com

echo $((1 + 2 * 3))
来源：http://udp.jinqigfzy.top

[R28] 浮点运算
来源：http://iie.0kj1m.cn

echo "scale=2; 10/3" | bc
来源：http://npr.svipenyu.cn

[R29] 定义函数
来源：http://aaz.cucudq.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mib.xziqi.cn

[R30] 函数返回状态码
来源：http://zqc.sxryk.cn

f() { return 0; }; f || echo "失败了"
来源：http://jvd.yj20258.top

[R31] 局部变量
来源：http://dot.jinghuilouyu.cn

f() { local x=1; echo "$x"; }
来源：http://dxf.jlsjyb.cn

[R32] 参数个数校验
来源：http://zqa.yuxming.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://upw.316326.xyz

[R33] 捕获错误并提示行号
来源：http://eze.pycfn.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://lyx.hcnkem.com

[R34] 退出时清理
来源：http://cks.tarul.cn

trap 'rm -f "$tmp"' EXIT
来源：http://jtd.meibo888.top

[R35] 后台执行并等待
来源：http://smp.jqgfzy.top

sleep 5 & pid=$!; wait "$pid"
来源：http://rrl.yongpay.top

[R36] 并发执行多个任务
来源：http://isc.pycfn.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hia.tanke756.top

[R37] 把输出赋给变量
来源：http://cdc.tianlin.xyz

files=$(ls -1)
来源：http://qxq.jqgufenzy.top

[R38] 管道串联
来源：http://kiz.ybcxt.top

cat a.txt | grep -i error | wc -l
来源：http://pgl.tianlin.xyz

[R39] 重定向标准输出与错误
来源：http://buh.ybcxt.top

cmd > out.log 2>&1
来源：http://iwx.jianghu66.top

[R40] 追加写日志
来源：http://vgs.sxryk.cn

echo "log" >> out.log
来源：http://zrl.fktsv.cn

[R41] 丢弃输出
来源：http://nbj.bbcook.cn

cmd >/dev/null 2>&1
来源：http://itm.xinyue.icu

[R42] 输入重定向
来源：http://chp.sufxvd.cn

wc -l < a.txt
来源：http://bdv.zhixingplan.top

[R43] 按名字查找文件
来源：http://wzq.xuanzx.com

find . -name "*.log" -type f
来源：http://dbu.xylfe.cn

[R44] 按修改时间查找
来源：http://yra.ybcxt.top

find . -mtime -7 -type f
来源：http://nlx.feifeiyinyue.top

[R45] 批量删除
来源：http://yvc.xingfuxueyuan.xyz

find . -name "*.tmp" -delete
来源：http://zfl.cheryme.top

[R46] 递归替换文件内容
来源：http://ymy.hfpthk.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://yco.ydjk.org.cn

[R47] sed 单行替换
来源：http://ppl.tianlin.xyz

sed -i 's/foo/bar/g' a.txt
来源：http://ezr.fanxiaobao.xyz

[R48] awk 取指定列
来源：http://dxg.ybcxt.top

awk '{print $1, $3}' a.txt
来源：http://opg.fengsongda.top

[R49] awk 带条件
来源：http://lih.wangdashe.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://oap.ybcxt.top

[R50] awk 求和
来源：http://wfc.shanyushiyangkeji.top

awk '{s += $2} END {print s}' a.txt
来源：http://zmc.jinghuilouyu.cn

[R51] 排序去重取前几
来源：http://fvy.0kj1m.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://spj.chenlongwang.top

[R52] 统计行数
来源：http://wnc.jiagoushi.top

wc -l a.txt
来源：http://sim.vqdsnc.cn

[R53] 查看文件头与实时尾
来源：http://vka.hnqzz.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://aqa.shanyushiyangtech.top

[R54] 比较两个文件
来源：http://irb.gogol.net.cn

diff a.txt b.txt
来源：http://esj.bjfxy.top

[R55] 压缩与解压
来源：http://lww.ppjwa.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ees.hammf.cn

[R56] 远程拷贝
来源：http://doi.wangshuangyany.cn

scp file user@host:/path/
来源：http://eyk.hysaishi.cn

[R57] 远程执行命令
来源：http://jyk.zycfv.cn

ssh user@host 'uptime'
来源：http://vlz.gzhubu.top

[R58] 下载文件
来源：http://kcd.ydzc1.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://twl.tanke756.top

[R59] 发 POST JSON
来源：http://sfr.tian-w.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ewx.chenzaomai.com

[R60] 只看 HTTP 状态码
来源：http://hmm.xingfuxueyuan.xyz

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://yps.zhongyouzk.top

[R61] 磁盘占用
来源：http://rjo.gotoacloud.top


<!-- 参考信息 -->