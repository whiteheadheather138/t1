代发 wailian999

[Q14] 存在则更新（upsert）
来源：http://fcl.hywenlv.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://qpu.9152youxi.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ufx.9152youxi.cn

[Q15] 查询全部
来源：http://owu.dianchejie.cn

SELECT * FROM users;
来源：http://ntw.hywenlv.cn

[Q16] 查询指定列
来源：http://nfi.yonumen.top

SELECT id, name FROM users;
来源：http://txl.nanxuanxn.top

[Q17] 条件查询
来源：http://xkv.jinyuanbaomall.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://nbo.dashuyun.cn

[Q18] 模糊匹配
来源：http://mhe.cashguo.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://jfw.xingfuxueyuan.xyz

[Q19] 范围查询
来源：http://pzy.zhaomingkeji.xyz

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://sau.cashguo.top

[Q20] IN 列表
来源：http://iql.shuidangran.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://pco.pengpengdd.cyou

[Q21] 空值判断
来源：http://tdb.chenjidiqi.icu

SELECT * FROM users WHERE email IS NULL;
来源：http://nub.vehdjk.com

[Q22] 排序
来源：http://avu.chenjidiqi.icu

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://urp.gogol.net.cn

[Q23] 分页
来源：http://xfe.sysykeji.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ymp.cashguo.top

[Q24] 去重
来源：http://psn.shangyingyoupin.top

SELECT DISTINCT city FROM users;
来源：http://njp.nanxuanxn.top

[Q25] 只取前 N 条
来源：http://zka.316326.xyz

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://qhz.aizwys.cn

[Q26] 计数
来源：http://ugr.yangfankeji.com

SELECT COUNT(*) FROM users;
来源：http://pnz.ybcxt.top

[Q27] 条件计数
来源：http://kvb.c1oappe.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://eks.smart0.xyz

[Q28] 求和与平均
来源：http://hlh.yangfankeji.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://xvx.yvedp.cn

[Q29] 最大最小值
来源：http://fln.hammf.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ict.jinqigfzy.top

[Q30] 分组统计
来源：http://glq.cucudq.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://kvd.hcnkem.com

[Q31] 分组后过滤
来源：http://wsc.nwbrower.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ppg.tian-w.cn

[Q32] 分组拼接字符串
来源：http://pah.tianlin.xyz

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hxo.fzhhl.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://nbx.bjfxy.top

[Q33] 多列分组
来源：http://bbg.svipenyu.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hzc.wangshuangyany.cn

[Q34] 每组取第一条
来源：http://fhx.aibaodan.cn

SELECT * FROM (
来源：http://iht.xinyue.icu

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://gds.ywan-chungtsiang.top

) t WHERE rn = 1;
来源：http://vpn.nwbrower.top

[Q35] 内连接
来源：http://ynj.zhiwuduotai.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://kit.nwbrower.top

[Q36] 左连接
来源：http://dlq.yj202588.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://paz.jlsjyb.cn

[Q37] 右连接
来源：http://hep.yj20258888.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ffd.chenjidiqi.icu

[Q38] 全外连接（PostgreSQL）
来源：http://sqt.fengsongda.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://efo.gogol.net.cn

[Q39] 自连接（查上下级）
来源：http://ayy.hnxiangtu.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://mzu.ydzc1.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://jfv.vqdsnc.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://sld.cdnleiting.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://bop.gaohongyu789.top

[Q41] 多表连接
来源：http://msy.chenzaomai.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://niv.uphjek.com

JOIN users u ON u.id = o.user_id
来源：http://cdw.feifeiyinyue.top

JOIN products p ON p.id = o.product_id;
来源：http://yhh.cqqwz.cn

[Q42] 连接条件附加过滤
来源：http://ool.bbcook.cn

SELECT u.name, o.amount FROM users u
来源：http://wsq.gaohongyu789.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://tpc.sysykeji.top

[Q43] 标量子查询
来源：http://myp.hcnkem.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://jnj.aibaodan.cn

[Q44] IN 子查询
来源：http://bmu.9152youxi.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://phx.chenjidiqi.icu

[Q45] EXISTS 判断存在
来源：http://nmt.zycfv.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://nje.daria6918.cn

[Q46] NOT EXISTS 判断不存在
来源：http://bmf.dianchejie.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://tgp.yj202588.top

[Q47] 与平均值比较
来源：http://sfk.guowangkeji.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://exj.chenjidiqi.icu

[Q48] CTE 公用表表达式
来源：http://geq.shanyushiyangtech.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://gue.hcnkem.com

SELECT * FROM t WHERE c > 5;
来源：http://vvg.haohaochexian.top

[Q49] 更新单行
来源：http://eao.guannengcc.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://pkc.xinyue.icu

[Q50] 批量更新
来源：http://qzr.sxryk.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://lnn.ppjwa.cn

[Q51] 用子查询更新
来源：http://cmw.yanxiufei.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://aat.yj202588.top

[Q52] 删除指定行
来源：http://emq.chenjidiqi.icu

DELETE FROM users WHERE id = 10;
来源：http://mis.ydjk.org.cn

[Q53] 按条件删除
来源：http://seu.sxryk.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://lhk.shanyushiyangtech.top

[Q54] 清空表
来源：http://zfg.birdmap.top

TRUNCATE TABLE logs;
来源：http://jbt.birdmap.top

[Q55] 排名（并列占位）
来源：http://qvo.aibaodan.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://rsk.yanxiufei.cn

[Q56] 密集排名（并列不占位）
来源：http://thh.uphjek.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://qmr.jinyuanbaomall.cn

[Q57] 行号
来源：http://ims.tianlin.xyz

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://rkd.0kj1m.cn

[Q58] 累计求和
来源：http://nop.smart0.xyz

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://sey.sysykeji.top

[Q59] 分组内累计
来源：http://qqq.bbcook.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://brq.cqqwz.cn

[Q60] 取上一行 / 下一行
来源：http://cdq.tianlin.xyz

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://pqo.jinyuanbaomall.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://fsy.vehdjk.com

[Q61] 移动平均
来源：http://lsg.chenzaomai.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://vsl.9152youxi.cn

[Q62] 分组占比
来源：http://zmu.xylfe.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ujh.iojbl.cn

[Q63] 开启事务
来源：http://vwk.andypj.xyz

START TRANSACTION;                -- 或 BEGIN
来源：http://kbz.shangyingyoupin.top

[Q64] 提交事务
来源：http://tay.jqgfzy.top

COMMIT;
来源：http://sjs.yonumen.top

[Q65] 回滚事务
来源：http://apw.yonumen.top

ROLLBACK;
来源：http://bvu.zhoulong.xyz

[Q66] 行锁查询
来源：http://edt.hywenlv.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mpt.zhongyouzk.top

[Q67] 设置隔离级别
来源：http://dtz.hnqzz.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ldy.pengpengdd.cyou

[Q68] 保存点
来源：http://obg.jinghuilouyu.cn

SAVEPOINT sp1;
来源：http://hjv.aizwys.cn

ROLLBACK TO sp1;
来源：http://zam.smart0.xyz

[Q69] 查看执行计划
来源：http://fli.zhijiandao.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mqo.tanke756.top

[Q70] 更新统计信息
来源：http://esk.nwbrower.top

ANALYZE TABLE users;
来源：http://hoe.zdqjudy.top

[Q71] 查看建表语句
来源：http://aoe.jqgufenzy.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ozx.quarkkingdee.top

[Q72] 查看索引
来源：http://jft.yj20258.top

SHOW INDEX FROM users;
来源：http://vkv.gogol.net.cn

[Q73] 查看表状态
来源：http://upe.sxryk.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://phc.hesvh.cn

[Q74] 强制使用索引
来源：http://udp.jinqigfzy.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://pvo.fzhhl.top

[Q75] 日期格式化
来源：http://fio.jinyuanbaomall.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://elq.hnqzz.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mza.nanxuanxn.top

[Q76] 按天统计
来源：http://ife.fktsv.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://try.ehwqpu.com

[Q77] 时间加减
来源：http://eke.zycfv.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://gks.yuanzhike.top

[Q78] 当前时间
来源：http://zhi.xinyue.icu

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://csr.shzxlz.cn

[Q79] 字符串拼接
来源：http://zdw.shanyushiyangkeji.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://zbc.fktsv.cn

[Q80] 字符串截取
来源：http://amu.chenlongwang.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://uzs.havefunace.top

[Q81] 字符串替换
来源：http://zru.zycfv.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://gsn.hammf.cn

[Q82] 字符长度与字节长度
来源：http://dxi.9152youxi.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mbn.iojbl.cn

[Q83] 大小写转换
来源：http://fwb.cashguo.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://zqt.ehwqpu.com

[Q84] 去除首尾空格
来源：http://dmj.jyoumei.cn

SELECT TRIM(name) FROM users;
来源：http://nsp.xinyue.icu

[Q85] 数值取整
来源：http://gnm.gaohongyu789.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hvc.sjlbkw.cn

[Q86] 读取 JSON 字段
来源：http://xcq.hammf.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mqh.fzhhl.top

[Q87] JSON 字段做条件
来源：http://stn.haohaochexian.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://kci.jyoumei.cn

[Q88] 行转列（条件聚合）
来源：http://roi.ppjwa.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://xsx.jqgufenzy.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://dph.sjlbkw.cn

[Q89] 判断表是否存在
来源：http://rgp.wangshuangyany.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://iox.jqgufenzy.top

[Q90] 生成序号列
来源：http://gxo.xuetiantiany.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://yjx.hcnkem.com

================================================================================
来源：http://wld.jinghuilouyu.cn

R. Bash 专题
来源：http://fsm.zhengqikj.top

================================================================================
来源：http://ucn.pengpengdd.cyou

[R01] shebang 与严格模式
来源：http://rvv.jinqigufen.top

#!/usr/bin/env bash
来源：http://uww.hammf.cn

set -euo pipefail
来源：http://unt.smart0.xyz

[R02] 变量赋值与使用
来源：http://mgv.316326.xyz

name="Tom"; echo "$name"
来源：http://eyh.gaohongyu789.top

[R03] 只读变量
来源：http://wjl.hesvh.cn

readonly PI=3.14
来源：http://vfa.c1oappe.top

[R04] 位置参数
来源：http://nzp.shanyushiyangkeji.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://upx.chenlongwang.top

[R05] 参数默认值
来源：http://agx.shzxlz.cn

name="${1:-default}"
来源：http://dck.fzhhl.top

[R06] 判断命令是否存在
来源：http://xtc.ppjwa.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://lfi.gotoacloud.top

[R07] if 判断文件
来源：http://lwv.cqqwz.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ojx.jinyuanbaomall.cn

[R08] 数值比较
来源：http://xzt.yanxiufei.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ngk.chenjidiqi.icu

[R09] 字符串比较
来源：http://yfl.jqgfzy.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://thd.xziqi.cn

[R10] 正则匹配
来源：http://eyj.yj20258.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ixg.sweek.top

[R11] case 多分支
来源：http://uoa.bbcook.cn

case "$1" in
来源：http://lcl.fengsongda.top

start) echo "启动" ;;
来源：http://yxn.birdmap.top

stop)  echo "停止" ;;
来源：http://utt.chenlongwang.top

*)     echo "未知命令" ;;
来源：http://qbj.gzhubu.top

esac
来源：http://jdl.tianlin.xyz

[R12] for 遍历文件
来源：http://ghx.zhengqikj.top

for f in *.txt; do echo "$f"; done
来源：http://yda.smart0.xyz

[R13] for 计数循环
来源：http://pze.nanxuanxn.top

for i in {1..10}; do echo "$i"; done
来源：http://zxa.shuidangran.top

[R14] C 风格 for
来源：http://eah.xylfe.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mfs.xinyue.icu

[R15] while 逐行读文件
来源：http://ucl.ydjk.org.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hol.yuxming.cn

[R16] until 等待条件
来源：http://gcd.cashguo.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://jtw.nanxinkj.top

[R17] 数组定义与取值
来源：http://kgo.xinyue.icu

arr=(a b c); echo "${arr[0]}"
来源：http://kod.wangshuangyany.cn

[R18] 遍历数组
来源：http://xga.c1oappe.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://usf.xziqi.cn

[R19] 数组长度
来源：http://wth.tanke756.top

echo "${#arr[@]}"
来源：http://apj.jinyuanbaomall.cn

[R20] 关联数组（字典）
来源：http://hvd.cashguo.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://aqm.hongshengwenyu.top

[R21] 字符串长度
来源：http://omc.jinqigfzy.top

echo "${#s}"
来源：http://wft.zhoulong.xyz

[R22] 截取子串
来源：http://ybo.nwbrower.top

echo "${s:0:5}"
来源：http://yws.316326.xyz

[R23] 字符串替换
来源：http://rzv.gotoacloud.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://fgf.jianghu66.top

[R24] 大小写转换
来源：http://gvs.vqdsnc.cn

echo "${s^^}"; echo "${s,,}"
来源：http://wqf.sufxvd.cn

[R25] 去后缀 / 去前缀
来源：http://fwm.smart0.xyz

echo "${f%.txt}"; echo "${f#./}"
来源：http://xpl.ydzc1.top

[R26] 命令替换
来源：http://fil.tian-w.cn

now=$(date +%F); echo "$now"
来源：http://aho.zhaomingkeji.xyz

[R27] 算术展开
来源：http://gci.xingfuxueyuan.xyz

echo $((1 + 2 * 3))
来源：http://mer.uphjek.com

[R28] 浮点运算
来源：http://jlt.hfpthk.cn

echo "scale=2; 10/3" | bc
来源：http://axl.nwbrower.top

[R29] 定义函数
来源：http://mvd.guowangkeji.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ztu.jianghu66.top

[R30] 函数返回状态码
来源：http://bcn.0kj1m.cn

f() { return 0; }; f || echo "失败了"
来源：http://mbi.meibo888.top

[R31] 局部变量
来源：http://uyz.ivvv.top

f() { local x=1; echo "$x"; }
来源：http://xwc.yj20258888.top

[R32] 参数个数校验
来源：http://xdm.hcnkem.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://qpt.sjlbkw.cn

[R33] 捕获错误并提示行号
来源：http://hkh.yonumen.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://yag.yongpay.top

[R34] 退出时清理
来源：http://xfr.jinghuilouyu.cn

trap 'rm -f "$tmp"' EXIT
来源：http://xfz.9152youxi.cn

[R35] 后台执行并等待
来源：http://rzj.quarkkingdee.top

sleep 5 & pid=$!; wait "$pid"
来源：http://osg.vqdsnc.cn

[R36] 并发执行多个任务
来源：http://iuf.kuanghao11.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://zjh.zhengqikj.top

[R37] 把输出赋给变量
来源：http://qtz.fktsv.cn

files=$(ls -1)
来源：http://xqu.nwbrower.top

[R38] 管道串联
来源：http://ezz.chenzaomai.com

cat a.txt | grep -i error | wc -l
来源：http://xyl.sufxvd.cn

[R39] 重定向标准输出与错误
来源：http://dwp.fzhhl.top

cmd > out.log 2>&1
来源：http://fvs.shanyushiyangtech.top

[R40] 追加写日志
来源：http://svx.fanxiaobao.xyz

echo "log" >> out.log
来源：http://rvr.uphjek.com

[R41] 丢弃输出
来源：http://yhx.yuxming.cn

cmd >/dev/null 2>&1
来源：http://kcn.hnqzz.top

[R42] 输入重定向
来源：http://akg.yfazqb.com

wc -l < a.txt
来源：http://ltj.hfpthk.cn

[R43] 按名字查找文件
来源：http://ial.jinqigufen.top

find . -name "*.log" -type f
来源：http://tad.zhaomingkeji.xyz

[R44] 按修改时间查找
来源：http://nuz.yueranfly.top

find . -mtime -7 -type f
来源：http://fta.ydjk.org.cn

[R45] 批量删除
来源：http://hvm.aizwys.cn

find . -name "*.tmp" -delete
来源：http://rku.yj202588.top

[R46] 递归替换文件内容
来源：http://yau.yj202588.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ugk.redwolf501.top

[R47] sed 单行替换
来源：http://yld.zdqjudy.top

sed -i 's/foo/bar/g' a.txt
来源：http://khf.chenlongwang.top

[R48] awk 取指定列
来源：http://tmh.pycfn.com

awk '{print $1, $3}' a.txt
来源：http://tri.birdmap.top

[R49] awk 带条件
来源：http://fgw.yj202588.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://psz.vqdsnc.cn

[R50] awk 求和
来源：http://kay.yongpay.top

awk '{s += $2} END {print s}' a.txt
来源：http://oza.jinqigufen.top

[R51] 排序去重取前几
来源：http://rjy.daxiang520.top

sort a.txt | uniq -c | sort -rn | head
来源：http://qvn.gogol.net.cn

[R52] 统计行数
来源：http://rxg.52xcode.cn

wc -l a.txt
来源：http://pqc.yonumen.top

[R53] 查看文件头与实时尾
来源：http://ftj.yvedp.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://gxs.zycfv.cn

[R54] 比较两个文件
来源：http://brz.bbcook.cn

diff a.txt b.txt
来源：http://chp.haohaochexian.top

[R55] 压缩与解压
来源：http://ffk.gzhubu.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://lsg.hysaishi.cn

[R56] 远程拷贝
来源：http://zjc.cqqwz.cn

scp file user@host:/path/
来源：http://iek.shanyushiyangtech.top

[R57] 远程执行命令
来源：http://sej.ivvv.top

ssh user@host 'uptime'
来源：http://qlw.pycfn.com

[R58] 下载文件
来源：http://ogu.hongshengwenyu.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ygz.epnwcf.com

[R59] 发 POST JSON
来源：http://ihq.zdqjudy.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://lsz.dianchejie.cn

[R60] 只看 HTTP 状态码
来源：http://wbr.yuxming.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ylj.ctjpmb.com

[R61] 磁盘占用
来源：http://uus.sufxvd.cn

df -h;  du -sh *
来源：http://mdz.zhongyouzk.top

[R62] 找最占空间的文件
来源：http://vwd.jqgfzy.top

du -ah . | sort -rh | head -10
来源：http://xiq.cucudq.cn

[R63] 内存与进程
来源：http://tet.vehdjk.com


<!-- 参考信息 -->