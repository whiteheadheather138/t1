代发 wailian999

INSERT INTO users (name) VALUES ('C');
来源：http://ger.haohaochexian.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://nek.jiagoushi.top

[Q13] 忽略重复插入
来源：http://emf.jqgufenzy.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://nml.gaohongyu789.top

[Q14] 存在则更新（upsert）
来源：http://sno.cheryme.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://evb.chenjidiqi.icu

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://uuu.zhoulong.xyz

[Q15] 查询全部
来源：http://yck.yuxming.cn

SELECT * FROM users;
来源：http://upe.ybcxt.top

[Q16] 查询指定列
来源：http://ejs.dianchejie.cn

SELECT id, name FROM users;
来源：http://ygn.mhx1999.top

[Q17] 条件查询
来源：http://caq.haohaochexian.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://enu.shzxlz.cn

[Q18] 模糊匹配
来源：http://uhw.vqdsnc.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wnb.redwolf501.top

[Q19] 范围查询
来源：http://hhc.guowangkeji.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://gwq.aizwys.cn

[Q20] IN 列表
来源：http://uad.svipenyu.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://xzz.zhongyouzk.top

[Q21] 空值判断
来源：http://eif.aibaodan.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://pnv.jinyuanbaomall.cn

[Q22] 排序
来源：http://ses.xuetiantiany.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://dvc.jianghu66.top

[Q23] 分页
来源：http://diy.jqgfzy.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://fns.snrcjt.cn

[Q24] 去重
来源：http://bjv.hongshengwenyu.top

SELECT DISTINCT city FROM users;
来源：http://tzk.yj20258888.top

[Q25] 只取前 N 条
来源：http://jhz.fanxiaobao.xyz

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ywg.shanyushiyangtech.top

[Q26] 计数
来源：http://ikv.jqgufenzy.top

SELECT COUNT(*) FROM users;
来源：http://kyp.yj202588.top

[Q27] 条件计数
来源：http://cxl.jqgufenzy.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://rgq.meibo888.top

[Q28] 求和与平均
来源：http://zov.nanxinkj.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://tas.mhx1999.top

[Q29] 最大最小值
来源：http://ekt.sufxvd.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://rzs.aibaodan.cn

[Q30] 分组统计
来源：http://zkm.zdqjudy.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://prm.hesvh.cn

[Q31] 分组后过滤
来源：http://pyq.guannengcc.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://zxc.wangshuangyany.cn

[Q32] 分组拼接字符串
来源：http://xoz.shuidangran.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://fhb.hammf.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://dnu.havefunace.top

[Q33] 多列分组
来源：http://uji.hywenlv.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://opj.nanxuanxn.top

[Q34] 每组取第一条
来源：http://myz.jqgfzy.top

SELECT * FROM (
来源：http://alz.redwolf501.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://osi.guowangkeji.top

) t WHERE rn = 1;
来源：http://zsb.aibaodan.cn

[Q35] 内连接
来源：http://bps.birdmap.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://nlr.chenzaomai.com

[Q36] 左连接
来源：http://yrt.ppjwa.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wdp.tanke756.top

[Q37] 右连接
来源：http://tpd.jlsjyb.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://cna.tarul.cn

[Q38] 全外连接（PostgreSQL）
来源：http://yva.hesvh.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://xfz.zhoulong.xyz

[Q39] 自连接（查上下级）
来源：http://sxj.yangfankeji.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://gor.tarul.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://rxk.meibo888.top

[Q40] 交叉连接（笛卡尔积）
来源：http://uvh.jlsjyb.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ytp.hcnkem.com

[Q41] 多表连接
来源：http://lvo.hywenlv.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ccb.xziqi.cn

JOIN users u ON u.id = o.user_id
来源：http://ggg.daxiang520.top

JOIN products p ON p.id = o.product_id;
来源：http://quf.jyoumei.cn

[Q42] 连接条件附加过滤
来源：http://oqv.fengsongda.top

SELECT u.name, o.amount FROM users u
来源：http://sdf.zdqjudy.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://isx.ivvv.top

[Q43] 标量子查询
来源：http://bqx.jlsjyb.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mif.xziqi.cn

[Q44] IN 子查询
来源：http://itj.nanxuanxn.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://nta.havefunace.top

[Q45] EXISTS 判断存在
来源：http://dii.kuanghao11.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://aec.vqdsnc.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ynq.mhx1999.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://iny.ywan-chungtsiang.top

[Q47] 与平均值比较
来源：http://trh.shanyushiyangtech.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://aao.sufxvd.cn

[Q48] CTE 公用表表达式
来源：http://aot.pengpengdd.cyou

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://jnc.shanyushiyangkeji.top

SELECT * FROM t WHERE c > 5;
来源：http://ztz.shanyushiyangkeji.top

[Q49] 更新单行
来源：http://pkv.zhiwuduotai.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://xpr.ctjpmb.com

[Q50] 批量更新
来源：http://pov.fktsv.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://pgy.dashuyun.cn

[Q51] 用子查询更新
来源：http://vtr.yanxiufei.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://fph.shuidangran.top

[Q52] 删除指定行
来源：http://gpy.316326.xyz

DELETE FROM users WHERE id = 10;
来源：http://uuu.jiagoushi.top

[Q53] 按条件删除
来源：http://vly.chenzaomai.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ppq.dianchejie.cn

[Q54] 清空表
来源：http://qgp.pycfn.com

TRUNCATE TABLE logs;
来源：http://zub.cdnleiting.top

[Q55] 排名（并列占位）
来源：http://zhg.chenjidiqi.icu

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://yhb.wangshuangyany.cn

[Q56] 密集排名（并列不占位）
来源：http://fwe.jinqigfzy.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://lfr.guannengcc.top

[Q57] 行号
来源：http://tcc.zdqjudy.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://swu.ppjwa.cn

[Q58] 累计求和
来源：http://okn.jqgufenzy.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ktw.sweek.top

[Q59] 分组内累计
来源：http://nog.hnqzz.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://tvo.gotoacloud.top

[Q60] 取上一行 / 下一行
来源：http://ywq.sysykeji.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://yuq.hywenlv.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://xcu.havefunace.top

[Q61] 移动平均
来源：http://bjx.xuanzx.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://frp.sjlbkw.cn

[Q62] 分组占比
来源：http://nwr.shzxlz.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://pja.zhiwuduotai.top

[Q63] 开启事务
来源：http://rsc.sweek.top

START TRANSACTION;                -- 或 BEGIN
来源：http://ekj.yj20258.top

[Q64] 提交事务
来源：http://mcb.jinqigufen.top

COMMIT;
来源：http://ngg.hnxiangtu.top

[Q65] 回滚事务
来源：http://yro.tarul.cn

ROLLBACK;
来源：http://zag.hywenlv.cn

[Q66] 行锁查询
来源：http://eib.bjfxy.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://dfn.zhixingplan.top

[Q67] 设置隔离级别
来源：http://afy.gzhubu.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://nhg.gogol.net.cn

[Q68] 保存点
来源：http://fjq.yueranfly.top

SAVEPOINT sp1;
来源：http://vyl.epnwcf.com

ROLLBACK TO sp1;
来源：http://qhr.fehbvm.com

[Q69] 查看执行计划
来源：http://bsq.tian-w.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://nwy.cheryme.top

[Q70] 更新统计信息
来源：http://jky.yj20258888.top

ANALYZE TABLE users;
来源：http://nnv.zhongyouzk.top

[Q71] 查看建表语句
来源：http://tal.zycfv.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ucg.yvedp.cn

[Q72] 查看索引
来源：http://ttn.hfpthk.cn

SHOW INDEX FROM users;
来源：http://abi.fzhhl.top

[Q73] 查看表状态
来源：http://fqr.smart0.xyz

SHOW TABLE STATUS LIKE 'users';
来源：http://kqg.9152youxi.cn

[Q74] 强制使用索引
来源：http://jzs.bbcook.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mzb.zhaomingkeji.xyz

[Q75] 日期格式化
来源：http://dfg.feifeiyinyue.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://lep.gotoacloud.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ufb.cashguo.top

[Q76] 按天统计
来源：http://ozv.jinqigufen.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ifw.chenjidiqi.icu

[Q77] 时间加减
来源：http://ier.shanyushiyangkeji.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://nxr.gogol.net.cn

[Q78] 当前时间
来源：http://apx.zhaomingkeji.xyz

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://tzt.haohaochexian.top

[Q79] 字符串拼接
来源：http://zzn.jiagoushi.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://kyb.yj202588.top

[Q80] 字符串截取
来源：http://uhg.shzxlz.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://vgb.ywan-chungtsiang.top

[Q81] 字符串替换
来源：http://hbl.zhengqikj.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://fgc.hammf.cn

[Q82] 字符长度与字节长度
来源：http://llc.birdmap.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ypg.tanke756.top

[Q83] 大小写转换
来源：http://zbn.yfazqb.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ybx.zdbjq.cn

[Q84] 去除首尾空格
来源：http://ddo.birdmap.top

SELECT TRIM(name) FROM users;
来源：http://eup.haohaochexian.top

[Q85] 数值取整
来源：http://epq.cucudq.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mej.gaohongyu789.top

[Q86] 读取 JSON 字段
来源：http://dyo.fktsv.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://shk.andypj.xyz

[Q87] JSON 字段做条件
来源：http://hqi.xuetiantiany.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://jyp.ydzc1.top

[Q88] 行转列（条件聚合）
来源：http://fub.pycfn.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://dtc.sufxvd.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://rnv.yj202588.top

[Q89] 判断表是否存在
来源：http://jeq.zhoulong.xyz

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://dbb.bjfxy.top

[Q90] 生成序号列
来源：http://gnb.pengpengdd.cyou

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://nbh.sxryk.cn

================================================================================
来源：http://ixl.snrcjt.cn

R. Bash 专题
来源：http://hwy.quarkkingdee.top

================================================================================
来源：http://ojm.yj202588.top

[R01] shebang 与严格模式
来源：http://duo.dashuyun.cn

#!/usr/bin/env bash
来源：http://qlq.uphjek.com

set -euo pipefail
来源：http://aqy.xuanzx.com

[R02] 变量赋值与使用
来源：http://znv.ydzc1.top

name="Tom"; echo "$name"
来源：http://les.316326.xyz

[R03] 只读变量
来源：http://sqg.zdbjq.cn

readonly PI=3.14
来源：http://jzl.gaohongyu789.top

[R04] 位置参数
来源：http://xst.wangshuangyany.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://bnj.tian-w.cn

[R05] 参数默认值
来源：http://jec.cqqwz.cn

name="${1:-default}"
来源：http://oww.ybcxt.top

[R06] 判断命令是否存在
来源：http://hwa.nanxinkj.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://efj.jlsjyb.cn

[R07] if 判断文件
来源：http://xha.xinyue.icu

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://rvf.snrcjt.cn

[R08] 数值比较
来源：http://lre.shanyushiyangtech.top

if (( a > b )); then echo "a 更大"; fi
来源：http://zwu.zhoulong.xyz

[R09] 字符串比较
来源：http://bec.cheryme.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://xda.yangfankeji.com

[R10] 正则匹配
来源：http://idz.hcnkem.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://jaz.yj20258888.top

[R11] case 多分支
来源：http://gxw.cdnleiting.top

case "$1" in
来源：http://icu.0kj1m.cn

start) echo "启动" ;;
来源：http://gds.c1oappe.top

stop)  echo "停止" ;;
来源：http://brh.tanke756.top

*)     echo "未知命令" ;;
来源：http://rqk.nwbrower.top

esac
来源：http://xrl.shzxlz.cn

[R12] for 遍历文件
来源：http://nke.chenzaomai.com

for f in *.txt; do echo "$f"; done
来源：http://cht.vqdsnc.cn

[R13] for 计数循环
来源：http://stl.zycfv.cn

for i in {1..10}; do echo "$i"; done
来源：http://unw.cashguo.top

[R14] C 风格 for
来源：http://tgr.yj202588.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://eed.daxiang520.top

[R15] while 逐行读文件
来源：http://mxe.sxryk.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://xzl.chenjidiqi.icu

[R16] until 等待条件
来源：http://mvn.yj20258.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hgy.gotoacloud.top

[R17] 数组定义与取值
来源：http://raa.jyoumei.cn

arr=(a b c); echo "${arr[0]}"
来源：http://var.yvedp.cn

[R18] 遍历数组
来源：http://xoo.sxryk.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://xsz.yongpay.top

[R19] 数组长度
来源：http://zno.smart0.xyz

echo "${#arr[@]}"
来源：http://row.aizwys.cn

[R20] 关联数组（字典）
来源：http://osy.cheryme.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://rda.jyoumei.cn

[R21] 字符串长度
来源：http://jfe.xylfe.cn

echo "${#s}"
来源：http://fuj.yj202588.top

[R22] 截取子串
来源：http://nyd.zdbjq.cn

echo "${s:0:5}"
来源：http://kbj.tian-w.cn

[R23] 字符串替换
来源：http://cnu.vehdjk.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://oey.tarul.cn

[R24] 大小写转换
来源：http://bzh.feifeiyinyue.top

echo "${s^^}"; echo "${s,,}"
来源：http://mzo.pengpengdd.cyou

[R25] 去后缀 / 去前缀
来源：http://fat.wangdashe.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://trm.hywenlv.cn

[R26] 命令替换
来源：http://xea.52xcode.cn

now=$(date +%F); echo "$now"
来源：http://gen.jinghuilouyu.cn

[R27] 算术展开
来源：http://buz.shuidangran.top

echo $((1 + 2 * 3))
来源：http://nmz.chenlongwang.top

[R28] 浮点运算
来源：http://iwd.yj20258888.top

echo "scale=2; 10/3" | bc
来源：http://ltp.cheryme.top

[R29] 定义函数
来源：http://dnc.ehwqpu.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mkl.daxiang520.top

[R30] 函数返回状态码
来源：http://ccx.epnwcf.com

f() { return 0; }; f || echo "失败了"
来源：http://ylg.52xcode.cn

[R31] 局部变量
来源：http://tuj.nanxinkj.top

f() { local x=1; echo "$x"; }
来源：http://mvh.hcnkem.com

[R32] 参数个数校验
来源：http://fnv.dianchejie.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://gaz.hesvh.cn

[R33] 捕获错误并提示行号
来源：http://icy.quarkkingdee.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://aji.xingfuxueyuan.xyz

[R34] 退出时清理
来源：http://opl.zdbjq.cn

trap 'rm -f "$tmp"' EXIT
来源：http://lrq.jinyuanbaomall.cn

[R35] 后台执行并等待
来源：http://axm.ivvv.top

sleep 5 & pid=$!; wait "$pid"
来源：http://quo.sjlbkw.cn

[R36] 并发执行多个任务
来源：http://wvx.smart0.xyz

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://knd.birdmap.top

[R37] 把输出赋给变量
来源：http://ehd.mhx1999.top

files=$(ls -1)
来源：http://uek.ywan-chungtsiang.top

[R38] 管道串联
来源：http://dxm.shanyushiyangtech.top

cat a.txt | grep -i error | wc -l
来源：http://gms.cqqwz.cn

[R39] 重定向标准输出与错误
来源：http://fky.gaohongyu789.top

cmd > out.log 2>&1
来源：http://wdk.jinqigufen.top

[R40] 追加写日志
来源：http://xib.jianghu66.top

echo "log" >> out.log
来源：http://vlu.yanxiufei.cn

[R41] 丢弃输出
来源：http://mqe.haohaochexian.top

cmd >/dev/null 2>&1
来源：http://ben.fehbvm.com

[R42] 输入重定向
来源：http://qqo.ivvv.top

wc -l < a.txt
来源：http://kck.c1oappe.top

[R43] 按名字查找文件
来源：http://ygh.quarkkingdee.top

find . -name "*.log" -type f
来源：http://ytv.jinqigfzy.top

[R44] 按修改时间查找
来源：http://cmi.smart0.xyz

find . -mtime -7 -type f
来源：http://ijd.aizwys.cn

[R45] 批量删除
来源：http://vrz.havefunace.top

find . -name "*.tmp" -delete
来源：http://ptg.gotoacloud.top

[R46] 递归替换文件内容
来源：http://zod.chenlongwang.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://rnr.ybcxt.top

[R47] sed 单行替换
来源：http://kmn.fehbvm.com

sed -i 's/foo/bar/g' a.txt
来源：http://soe.yongpay.top

[R48] awk 取指定列
来源：http://wtu.jyoumei.cn

awk '{print $1, $3}' a.txt
来源：http://hxd.jinqigufen.top

[R49] awk 带条件
来源：http://syg.nanxuanxn.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://pyx.jiagoushi.top

[R50] awk 求和
来源：http://ugi.gotoacloud.top

awk '{s += $2} END {print s}' a.txt
来源：http://rah.sxryk.cn

[R51] 排序去重取前几
来源：http://zhp.chenlongwang.top

sort a.txt | uniq -c | sort -rn | head
来源：http://uub.xuanzx.com

[R52] 统计行数
来源：http://kpa.zhijiandao.cn

wc -l a.txt
来源：http://sml.zhongyouzk.top

[R53] 查看文件头与实时尾
来源：http://eut.feifeiyinyue.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wkg.hnxiangtu.top

[R54] 比较两个文件
来源：http://uqx.wangshuangyany.cn

diff a.txt b.txt
来源：http://qfl.tarul.cn

[R55] 压缩与解压
来源：http://cgq.c1oappe.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://uxe.sysykeji.top

[R56] 远程拷贝
来源：http://lwx.fzhhl.top

scp file user@host:/path/
来源：http://kmt.guannengcc.top

[R57] 远程执行命令
来源：http://cpd.redwolf501.top

ssh user@host 'uptime'
来源：http://ths.epnwcf.com

[R58] 下载文件
来源：http://nqm.tanke756.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hjp.yongpay.top

[R59] 发 POST JSON
来源：http://iea.yuanzhike.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://cis.cucudq.cn

[R60] 只看 HTTP 状态码
来源：http://sfm.yanxiufei.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://zeh.daxiang520.top

[R61] 磁盘占用
来源：http://plx.hesvh.cn


<!-- 参考信息 -->