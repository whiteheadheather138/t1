代发 wailian999

INSERT INTO users (name) VALUES ('C');
来源：http://tge.sjlbkw.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://trt.jinghuilouyu.cn

[Q13] 忽略重复插入
来源：http://efu.fktsv.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://sap.cqqwz.cn

[Q14] 存在则更新（upsert）
来源：http://xbc.aizwys.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://dis.cdnleiting.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wmi.hysaishi.cn

[Q15] 查询全部
来源：http://uvx.xingfuxueyuan.xyz

SELECT * FROM users;
来源：http://ujj.0kj1m.cn

[Q16] 查询指定列
来源：http://odu.xingfuxueyuan.xyz

SELECT id, name FROM users;
来源：http://mtp.xuetiantiany.cn

[Q17] 条件查询
来源：http://zls.zhiwuduotai.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://vai.xingfuxueyuan.xyz

[Q18] 模糊匹配
来源：http://ffm.xinyue.icu

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hwn.yongpay.top

[Q19] 范围查询
来源：http://don.sweek.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://dlv.fanxiaobao.xyz

[Q20] IN 列表
来源：http://vbb.cdnleiting.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://smg.uphjek.com

[Q21] 空值判断
来源：http://dwb.hnxiangtu.top

SELECT * FROM users WHERE email IS NULL;
来源：http://kvr.aibaodan.cn

[Q22] 排序
来源：http://xjx.zhoulong.xyz

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://qxy.wangshuangyany.cn

[Q23] 分页
来源：http://pdg.nanxinkj.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://qzg.daria6918.cn

[Q24] 去重
来源：http://egy.jiagoushi.top

SELECT DISTINCT city FROM users;
来源：http://fys.shzxlz.cn

[Q25] 只取前 N 条
来源：http://dhf.hywenlv.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://qon.tianlin.xyz

[Q26] 计数
来源：http://jxh.shangyingyoupin.top

SELECT COUNT(*) FROM users;
来源：http://zkm.tarul.cn

[Q27] 条件计数
来源：http://zeg.iojbl.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://bux.feifeiyinyue.top

[Q28] 求和与平均
来源：http://kgo.hfpthk.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ubq.haohaochexian.top

[Q29] 最大最小值
来源：http://eoz.jinghuilouyu.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://gin.yongpay.top

[Q30] 分组统计
来源：http://tnt.haohaochexian.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://jmu.zdqjudy.top

[Q31] 分组后过滤
来源：http://qfb.ctjpmb.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://pyo.feifeiyinyue.top

[Q32] 分组拼接字符串
来源：http://mcd.jinqigufen.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://zrz.svipenyu.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hji.zhoulong.xyz

[Q33] 多列分组
来源：http://eit.jqgufenzy.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://but.pengpengdd.cyou

[Q34] 每组取第一条
来源：http://vlk.guowangkeji.top

SELECT * FROM (
来源：http://bii.sufxvd.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://xac.jqgufenzy.top

) t WHERE rn = 1;
来源：http://gpv.zycfv.cn

[Q35] 内连接
来源：http://fxx.hcnkem.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://asp.52xcode.cn

[Q36] 左连接
来源：http://mnz.vehdjk.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hnn.jinqigufen.top

[Q37] 右连接
来源：http://ykv.aizwys.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://dml.ivvv.top

[Q38] 全外连接（PostgreSQL）
来源：http://qgv.gotoacloud.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://gvf.xziqi.cn

[Q39] 自连接（查上下级）
来源：http://iae.gaohongyu789.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://miv.tanke756.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baj.quarkkingdee.top

[Q40] 交叉连接（笛卡尔积）
来源：http://mnt.dianchejie.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://qey.nanxuanxn.top

[Q41] 多表连接
来源：http://bep.kuanghao11.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://urr.redwolf501.top

JOIN users u ON u.id = o.user_id
来源：http://kfr.xylfe.cn

JOIN products p ON p.id = o.product_id;
来源：http://bid.gotoacloud.top

[Q42] 连接条件附加过滤
来源：http://vqo.zhaomingkeji.xyz

SELECT u.name, o.amount FROM users u
来源：http://vjs.haohaochexian.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://nuh.cqqwz.cn

[Q43] 标量子查询
来源：http://idn.yvedp.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ayo.hongshengwenyu.top

[Q44] IN 子查询
来源：http://ivr.bjfxy.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://tul.cdnleiting.top

[Q45] EXISTS 判断存在
来源：http://kwi.chenlongwang.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://tye.yanxiufei.cn

[Q46] NOT EXISTS 判断不存在
来源：http://lkd.cqqwz.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://sdw.jinqigufen.top

[Q47] 与平均值比较
来源：http://wfv.jlsjyb.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://qey.wangshuangyany.cn

[Q48] CTE 公用表表达式
来源：http://did.svipenyu.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://utp.vehdjk.com

SELECT * FROM t WHERE c > 5;
来源：http://qua.sysykeji.top

[Q49] 更新单行
来源：http://tev.nanxinkj.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hiq.pycfn.com

[Q50] 批量更新
来源：http://dzm.yueranfly.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hox.shangyingyoupin.top

[Q51] 用子查询更新
来源：http://rwd.chenjidiqi.icu

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://eny.jinyuanbaomall.cn

[Q52] 删除指定行
来源：http://snt.zhongyouzk.top

DELETE FROM users WHERE id = 10;
来源：http://geu.zdbjq.cn

[Q53] 按条件删除
来源：http://hrs.wangshuangyany.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://dua.mhx1999.top

[Q54] 清空表
来源：http://iev.hcnkem.com

TRUNCATE TABLE logs;
来源：http://wxy.xingfuxueyuan.xyz

[Q55] 排名（并列占位）
来源：http://fyf.yuanzhike.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ssw.dianchejie.cn

[Q56] 密集排名（并列不占位）
来源：http://fhz.snrcjt.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://inv.hfpthk.cn

[Q57] 行号
来源：http://ant.dashuyun.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://fsb.ydjk.org.cn

[Q58] 累计求和
来源：http://ucp.svipenyu.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://sul.tianlin.xyz

[Q59] 分组内累计
来源：http://dbd.tian-w.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ffm.fengsongda.top

[Q60] 取上一行 / 下一行
来源：http://vyw.jiagoushi.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://syh.yuxming.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://njq.sweek.top

[Q61] 移动平均
来源：http://hvc.hysaishi.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://yfg.feifeiyinyue.top

[Q62] 分组占比
来源：http://ynr.yanxiufei.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://guk.dianchejie.cn

[Q63] 开启事务
来源：http://ofp.hnqzz.top

START TRANSACTION;                -- 或 BEGIN
来源：http://khw.epnwcf.com

[Q64] 提交事务
来源：http://tvl.mhx1999.top

COMMIT;
来源：http://kyn.mhx1999.top

[Q65] 回滚事务
来源：http://yqb.meibo888.top

ROLLBACK;
来源：http://oai.hywenlv.cn

[Q66] 行锁查询
来源：http://fut.nanxuanxn.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hqw.yangfankeji.com

[Q67] 设置隔离级别
来源：http://gzz.shangyingyoupin.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://pdi.fehbvm.com

[Q68] 保存点
来源：http://qge.gzhubu.top

SAVEPOINT sp1;
来源：http://dlp.ctjpmb.com

ROLLBACK TO sp1;
来源：http://skh.andypj.xyz

[Q69] 查看执行计划
来源：http://goj.tarul.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ewb.uphjek.com

[Q70] 更新统计信息
来源：http://ubo.vehdjk.com

ANALYZE TABLE users;
来源：http://rnu.ydzc1.top

[Q71] 查看建表语句
来源：http://htb.yanxiufei.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://glu.cashguo.top

[Q72] 查看索引
来源：http://afu.yj20258888.top

SHOW INDEX FROM users;
来源：http://reo.xinyue.icu

[Q73] 查看表状态
来源：http://jfc.smart0.xyz

SHOW TABLE STATUS LIKE 'users';
来源：http://mmh.zhiwuduotai.top

[Q74] 强制使用索引
来源：http://jck.birdmap.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://kyl.hywenlv.cn

[Q75] 日期格式化
来源：http://uks.fehbvm.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://zxw.jianghu66.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://aog.9152youxi.cn

[Q76] 按天统计
来源：http://mku.hongshengwenyu.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://yav.cheryme.top

[Q77] 时间加减
来源：http://bqc.chenzaomai.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://pyk.aibaodan.cn

[Q78] 当前时间
来源：http://yti.hywenlv.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://qto.jqgufenzy.top

[Q79] 字符串拼接
来源：http://mtq.yj20258888.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://zmj.yuxming.cn

[Q80] 字符串截取
来源：http://aqi.dashuyun.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hwi.cucudq.cn

[Q81] 字符串替换
来源：http://ats.shuidangran.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://zbq.shzxlz.cn

[Q82] 字符长度与字节长度
来源：http://dmv.tanke756.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://aqj.shanyushiyangkeji.top

[Q83] 大小写转换
来源：http://pcm.cheryme.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://smb.mhx1999.top

[Q84] 去除首尾空格
来源：http://rbk.jlsjyb.cn

SELECT TRIM(name) FROM users;
来源：http://aef.jqgfzy.top

[Q85] 数值取整
来源：http://ltz.havefunace.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://pmp.cdnleiting.top

[Q86] 读取 JSON 字段
来源：http://fqt.ctjpmb.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ezw.daxiang520.top

[Q87] JSON 字段做条件
来源：http://rhc.hesvh.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ani.xuetiantiany.cn

[Q88] 行转列（条件聚合）
来源：http://kfh.tanke756.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://sxd.shanyushiyangkeji.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://toi.bjfxy.top

[Q89] 判断表是否存在
来源：http://dfr.dashuyun.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://lmc.pengpengdd.cyou

[Q90] 生成序号列
来源：http://srq.zhengqikj.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://aef.jianghu66.top

================================================================================
来源：http://qpv.cheryme.top

R. Bash 专题
来源：http://cwu.tianlin.xyz

================================================================================
来源：http://blo.jinghuilouyu.cn

[R01] shebang 与严格模式
来源：http://xtc.pycfn.com

#!/usr/bin/env bash
来源：http://fnf.ydjk.org.cn

set -euo pipefail
来源：http://vbp.ivvv.top

[R02] 变量赋值与使用
来源：http://hki.daria6918.cn

name="Tom"; echo "$name"
来源：http://fom.zhixingplan.top

[R03] 只读变量
来源：http://ftc.zhongyouzk.top

readonly PI=3.14
来源：http://qhc.hysaishi.cn

[R04] 位置参数
来源：http://atp.tanke756.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://lxu.hesvh.cn

[R05] 参数默认值
来源：http://gbl.mhx1999.top

name="${1:-default}"
来源：http://jom.xylfe.cn

[R06] 判断命令是否存在
来源：http://mwq.daria6918.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ztq.gogol.net.cn

[R07] if 判断文件
来源：http://kxu.0kj1m.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://xgb.guannengcc.top

[R08] 数值比较
来源：http://bqk.yonumen.top

if (( a > b )); then echo "a 更大"; fi
来源：http://mcy.wangdashe.top

[R09] 字符串比较
来源：http://nnt.fanxiaobao.xyz

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://xyn.tanke756.top

[R10] 正则匹配
来源：http://bpz.ydjk.org.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://aqz.tian-w.cn

[R11] case 多分支
来源：http://oyk.yvedp.cn

case "$1" in
来源：http://rue.hcnkem.com

start) echo "启动" ;;
来源：http://fcv.yongpay.top

stop)  echo "停止" ;;
来源：http://dqc.9152youxi.cn

*)     echo "未知命令" ;;
来源：http://irl.jiagoushi.top

esac
来源：http://bmw.andypj.xyz

[R12] for 遍历文件
来源：http://lpz.cqqwz.cn

for f in *.txt; do echo "$f"; done
来源：http://vtd.feifeiyinyue.top

[R13] for 计数循环
来源：http://afw.fehbvm.com

for i in {1..10}; do echo "$i"; done
来源：http://ems.xziqi.cn

[R14] C 风格 for
来源：http://bqz.guannengcc.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://aso.zhaomingkeji.xyz

[R15] while 逐行读文件
来源：http://bfg.jiagoushi.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ccd.ppjwa.cn

[R16] until 等待条件
来源：http://esw.hnxiangtu.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://etm.fehbvm.com

[R17] 数组定义与取值
来源：http://rad.wangdashe.top

arr=(a b c); echo "${arr[0]}"
来源：http://jyi.gzhubu.top

[R18] 遍历数组
来源：http://vyf.xingfuxueyuan.xyz

for x in "${arr[@]}"; do echo "$x"; done
来源：http://qoa.daria6918.cn

[R19] 数组长度
来源：http://ita.zhoulong.xyz

echo "${#arr[@]}"
来源：http://jpq.xziqi.cn

[R20] 关联数组（字典）
来源：http://lmp.guowangkeji.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://kem.chenzaomai.com

[R21] 字符串长度
来源：http://fbz.bbcook.cn

echo "${#s}"
来源：http://sbj.yj20258.top

[R22] 截取子串
来源：http://ygq.shanyushiyangkeji.top

echo "${s:0:5}"
来源：http://hdk.zhijiandao.cn

[R23] 字符串替换
来源：http://pjm.jinqigufen.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://qfr.sweek.top

[R24] 大小写转换
来源：http://els.chenzaomai.com

echo "${s^^}"; echo "${s,,}"
来源：http://srf.aizwys.cn

[R25] 去后缀 / 去前缀
来源：http://nwa.daxiang520.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://oxj.c1oappe.top

[R26] 命令替换
来源：http://anr.hongshengwenyu.top

now=$(date +%F); echo "$now"
来源：http://xyr.sufxvd.cn

[R27] 算术展开
来源：http://ysp.zhaomingkeji.xyz

echo $((1 + 2 * 3))
来源：http://eoe.zhixingplan.top

[R28] 浮点运算
来源：http://psm.fanxiaobao.xyz

echo "scale=2; 10/3" | bc
来源：http://vnl.nanxuanxn.top

[R29] 定义函数
来源：http://fbz.hcnkem.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mio.hnqzz.top

[R30] 函数返回状态码
来源：http://efi.mhx1999.top

f() { return 0; }; f || echo "失败了"
来源：http://esg.vqdsnc.cn

[R31] 局部变量
来源：http://oua.yangfankeji.com

f() { local x=1; echo "$x"; }
来源：http://olp.ehwqpu.com

[R32] 参数个数校验
来源：http://zve.yuanzhike.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://uae.jiagoushi.top

[R33] 捕获错误并提示行号
来源：http://fgv.chenjidiqi.icu

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://src.daria6918.cn

[R34] 退出时清理
来源：http://gkv.cdnleiting.top

trap 'rm -f "$tmp"' EXIT
来源：http://wes.wangshuangyany.cn

[R35] 后台执行并等待
来源：http://cdt.redwolf501.top

sleep 5 & pid=$!; wait "$pid"
来源：http://nil.sxryk.cn

[R36] 并发执行多个任务
来源：http://uvn.birdmap.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://kwf.hcnkem.com

[R37] 把输出赋给变量
来源：http://gyt.zhongyouzk.top

files=$(ls -1)
来源：http://tea.hnxiangtu.top

[R38] 管道串联
来源：http://yhq.zhiwuduotai.top

cat a.txt | grep -i error | wc -l
来源：http://var.fzhhl.top

[R39] 重定向标准输出与错误
来源：http://ejo.yuxming.cn

cmd > out.log 2>&1
来源：http://htx.daria6918.cn

[R40] 追加写日志
来源：http://xpf.yj20258888.top

echo "log" >> out.log
来源：http://jjz.chenzaomai.com

[R41] 丢弃输出
来源：http://iok.nwbrower.top

cmd >/dev/null 2>&1
来源：http://ffd.uphjek.com

[R42] 输入重定向
来源：http://rql.gzhubu.top

wc -l < a.txt
来源：http://jtp.nanxuanxn.top

[R43] 按名字查找文件
来源：http://kel.havefunace.top

find . -name "*.log" -type f
来源：http://rfc.yj202588.top

[R44] 按修改时间查找
来源：http://gag.jyoumei.cn

find . -mtime -7 -type f
来源：http://ekt.gogol.net.cn

[R45] 批量删除
来源：http://ytx.ivvv.top

find . -name "*.tmp" -delete
来源：http://mpp.daxiang520.top

[R46] 递归替换文件内容
来源：http://mpq.fehbvm.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://lxy.redwolf501.top

[R47] sed 单行替换
来源：http://zig.yanxiufei.cn

sed -i 's/foo/bar/g' a.txt
来源：http://cpy.jinqigfzy.top

[R48] awk 取指定列
来源：http://iye.316326.xyz

awk '{print $1, $3}' a.txt
来源：http://knr.tianlin.xyz

[R49] awk 带条件
来源：http://jjn.cucudq.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://jky.tanke756.top

[R50] awk 求和
来源：http://wns.wangdashe.top

awk '{s += $2} END {print s}' a.txt
来源：http://uvj.zycfv.cn

[R51] 排序去重取前几
来源：http://dqz.chenzaomai.com

sort a.txt | uniq -c | sort -rn | head
来源：http://yaa.yj20258888.top

[R52] 统计行数
来源：http://uox.ehwqpu.com

wc -l a.txt
来源：http://yrz.dianchejie.cn

[R53] 查看文件头与实时尾
来源：http://nya.snrcjt.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://gjw.cashguo.top

[R54] 比较两个文件
来源：http://eft.zycfv.cn

diff a.txt b.txt
来源：http://pxl.jiagoushi.top

[R55] 压缩与解压
来源：http://ays.kuanghao11.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://fpe.shanyushiyangkeji.top

[R56] 远程拷贝
来源：http://pqk.cdnleiting.top

scp file user@host:/path/
来源：http://rrk.gaohongyu789.top

[R57] 远程执行命令
来源：http://nnm.jinqigufen.top

ssh user@host 'uptime'
来源：http://cnx.kuanghao11.cn

[R58] 下载文件
来源：http://guc.0kj1m.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hhz.chenlongwang.top

[R59] 发 POST JSON
来源：http://ahk.hcnkem.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://vcu.sweek.top

[R60] 只看 HTTP 状态码
来源：http://bwl.hfpthk.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wtd.daria6918.cn

[R61] 磁盘占用
来源：http://gfq.yanxiufei.cn


<!-- 参考信息 -->