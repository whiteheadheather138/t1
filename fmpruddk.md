代发 wailian999

INSERT INTO users (name) VALUES ('C');
来源：http://ehd.cqqwz.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://dka.snrcjt.cn

[Q13] 忽略重复插入
来源：http://uvk.yuxming.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hhe.jqgufenzy.top

[Q14] 存在则更新（upsert）
来源：http://top.zycfv.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://eul.aizwys.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://yru.ehwqpu.com

[Q15] 查询全部
来源：http://sls.hywenlv.cn

SELECT * FROM users;
来源：http://emx.chenzaomai.com

[Q16] 查询指定列
来源：http://uwe.quarkkingdee.top

SELECT id, name FROM users;
来源：http://fmg.yj202588.top

[Q17] 条件查询
来源：http://xxl.zhoulong.xyz

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://bdc.tarul.cn

[Q18] 模糊匹配
来源：http://dob.fktsv.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://nhx.jinyuanbaomall.cn

[Q19] 范围查询
来源：http://fvl.shuidangran.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://erh.sjlbkw.cn

[Q20] IN 列表
来源：http://lls.jinqigufen.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://fei.wangdashe.top

[Q21] 空值判断
来源：http://owg.yuanzhike.top

SELECT * FROM users WHERE email IS NULL;
来源：http://nbq.shuidangran.top

[Q22] 排序
来源：http://dfa.zhijiandao.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hhj.zhixingplan.top

[Q23] 分页
来源：http://chi.feifeiyinyue.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ddw.epnwcf.com

[Q24] 去重
来源：http://adm.dashuyun.cn

SELECT DISTINCT city FROM users;
来源：http://zmf.xylfe.cn

[Q25] 只取前 N 条
来源：http://vsw.jlsjyb.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://pil.bjfxy.top

[Q26] 计数
来源：http://ynn.hongshengwenyu.top

SELECT COUNT(*) FROM users;
来源：http://lkr.chenzaomai.com

[Q27] 条件计数
来源：http://ram.daxiang520.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://nuh.sufxvd.cn

[Q28] 求和与平均
来源：http://qhi.jqgufenzy.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://enj.zhixingplan.top

[Q29] 最大最小值
来源：http://vlc.jqgufenzy.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://bsl.yuanzhike.top

[Q30] 分组统计
来源：http://jyp.sufxvd.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ezo.quarkkingdee.top

[Q31] 分组后过滤
来源：http://faa.zhongyouzk.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://oxl.xuanzx.com

[Q32] 分组拼接字符串
来源：http://ben.mhx1999.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ark.zdbjq.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://rbq.cheryme.top

[Q33] 多列分组
来源：http://tuk.nanxinkj.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://yxi.sysykeji.top

[Q34] 每组取第一条
来源：http://qyd.9152youxi.cn

SELECT * FROM (
来源：http://ksd.9152youxi.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://oia.sxryk.cn

) t WHERE rn = 1;
来源：http://ekl.mhx1999.top

[Q35] 内连接
来源：http://nsf.andypj.xyz

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://rmy.cqqwz.cn

[Q36] 左连接
来源：http://tsh.hywenlv.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://lwz.jqgfzy.top

[Q37] 右连接
来源：http://zol.xuetiantiany.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://xgq.fengsongda.top

[Q38] 全外连接（PostgreSQL）
来源：http://wrg.sxryk.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://odx.dianchejie.cn

[Q39] 自连接（查上下级）
来源：http://cwt.316326.xyz

SELECT e.name, m.name AS manager FROM employees e
来源：http://yar.ywan-chungtsiang.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://enx.hnqzz.top

[Q40] 交叉连接（笛卡尔积）
来源：http://joy.hnxiangtu.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://afs.ybcxt.top

[Q41] 多表连接
来源：http://rhe.yj20258888.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://uav.redwolf501.top

JOIN users u ON u.id = o.user_id
来源：http://phj.yueranfly.top

JOIN products p ON p.id = o.product_id;
来源：http://ffv.guowangkeji.top

[Q42] 连接条件附加过滤
来源：http://hlc.sufxvd.cn

SELECT u.name, o.amount FROM users u
来源：http://rox.chenzaomai.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://nry.tianlin.xyz

[Q43] 标量子查询
来源：http://uka.hcnkem.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://fxr.andypj.xyz

[Q44] IN 子查询
来源：http://aky.cucudq.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://eyk.jqgufenzy.top

[Q45] EXISTS 判断存在
来源：http://eba.chenzaomai.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://trs.tian-w.cn

[Q46] NOT EXISTS 判断不存在
来源：http://eix.guowangkeji.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xny.zhixingplan.top

[Q47] 与平均值比较
来源：http://viv.feifeiyinyue.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://zha.vehdjk.com

[Q48] CTE 公用表表达式
来源：http://rmz.ehwqpu.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://vui.sysykeji.top

SELECT * FROM t WHERE c > 5;
来源：http://dvq.chenjidiqi.icu

[Q49] 更新单行
来源：http://bbh.pycfn.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://xdj.jinqigufen.top

[Q50] 批量更新
来源：http://okn.hcnkem.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://nlo.zhiwuduotai.top

[Q51] 用子查询更新
来源：http://how.fehbvm.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ohv.aizwys.cn

[Q52] 删除指定行
来源：http://wnr.gzhubu.top

DELETE FROM users WHERE id = 10;
来源：http://rhq.xinyue.icu

[Q53] 按条件删除
来源：http://aau.wangshuangyany.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mvv.yuanzhike.top

[Q54] 清空表
来源：http://pml.pycfn.com

TRUNCATE TABLE logs;
来源：http://sok.jinghuilouyu.cn

[Q55] 排名（并列占位）
来源：http://buo.guannengcc.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://qmo.hfpthk.cn

[Q56] 密集排名（并列不占位）
来源：http://hgy.yj20258888.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://qio.hammf.cn

[Q57] 行号
来源：http://byt.dashuyun.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://vju.feifeiyinyue.top

[Q58] 累计求和
来源：http://wad.52xcode.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://aqm.aibaodan.cn

[Q59] 分组内累计
来源：http://vaa.kuanghao11.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wwk.vehdjk.com

[Q60] 取上一行 / 下一行
来源：http://urd.quarkkingdee.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://dop.zhijiandao.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://nlr.jinghuilouyu.cn

[Q61] 移动平均
来源：http://tka.zhoulong.xyz

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://eyi.xylfe.cn

[Q62] 分组占比
来源：http://zls.hywenlv.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://uhf.bjfxy.top

[Q63] 开启事务
来源：http://hgh.cucudq.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://vfs.iojbl.cn

[Q64] 提交事务
来源：http://vod.tarul.cn

COMMIT;
来源：http://wbc.chenlongwang.top

[Q65] 回滚事务
来源：http://fys.ivvv.top

ROLLBACK;
来源：http://fen.wangdashe.top

[Q66] 行锁查询
来源：http://lbr.snrcjt.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ayg.ybcxt.top

[Q67] 设置隔离级别
来源：http://utd.hywenlv.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://jtb.redwolf501.top

[Q68] 保存点
来源：http://tft.sxryk.cn

SAVEPOINT sp1;
来源：http://gnl.yuanzhike.top

ROLLBACK TO sp1;
来源：http://pyn.havefunace.top

[Q69] 查看执行计划
来源：http://lsz.sysykeji.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ljf.tanke756.top

[Q70] 更新统计信息
来源：http://wka.jiagoushi.top

ANALYZE TABLE users;
来源：http://vzf.sxryk.cn

[Q71] 查看建表语句
来源：http://jkg.hammf.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://nod.yvedp.cn

[Q72] 查看索引
来源：http://xex.tianlin.xyz

SHOW INDEX FROM users;
来源：http://iyh.shanyushiyangkeji.top

[Q73] 查看表状态
来源：http://off.sufxvd.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://sbb.xuetiantiany.cn

[Q74] 强制使用索引
来源：http://bfe.zhengqikj.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://xac.jinyuanbaomall.cn

[Q75] 日期格式化
来源：http://txb.jiagoushi.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://fdw.bjfxy.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://zbo.sxryk.cn

[Q76] 按天统计
来源：http://oow.c1oappe.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://zzg.wangshuangyany.cn

[Q77] 时间加减
来源：http://rwz.epnwcf.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wts.9152youxi.cn

[Q78] 当前时间
来源：http://cvh.shuidangran.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://urb.zhijiandao.cn

[Q79] 字符串拼接
来源：http://uuo.yongpay.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hlw.ivvv.top

[Q80] 字符串截取
来源：http://hbh.tian-w.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mfq.dashuyun.cn

[Q81] 字符串替换
来源：http://duo.yj202588.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://qmm.kuanghao11.cn

[Q82] 字符长度与字节长度
来源：http://nus.xuanzx.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://imx.bjfxy.top

[Q83] 大小写转换
来源：http://yad.tian-w.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ylw.hcnkem.com

[Q84] 去除首尾空格
来源：http://shv.yfazqb.com

SELECT TRIM(name) FROM users;
来源：http://jjo.gogol.net.cn

[Q85] 数值取整
来源：http://dzy.aizwys.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ptx.zycfv.cn

[Q86] 读取 JSON 字段
来源：http://ejx.zycfv.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://elc.nwbrower.top

[Q87] JSON 字段做条件
来源：http://vpl.sxryk.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://tzg.hammf.cn

[Q88] 行转列（条件聚合）
来源：http://zja.xingfuxueyuan.xyz

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://lee.ydzc1.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mcx.yonumen.top

[Q89] 判断表是否存在
来源：http://ofg.chenjidiqi.icu

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://pzm.hammf.cn

[Q90] 生成序号列
来源：http://jii.fktsv.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://cvf.jqgufenzy.top

================================================================================
来源：http://wvw.mhx1999.top

R. Bash 专题
来源：http://pom.dashuyun.cn

================================================================================
来源：http://ihe.chenjidiqi.icu

[R01] shebang 与严格模式
来源：http://sgs.zdqjudy.top

#!/usr/bin/env bash
来源：http://eal.jyoumei.cn

set -euo pipefail
来源：http://scf.sxryk.cn

[R02] 变量赋值与使用
来源：http://stb.chenlongwang.top

name="Tom"; echo "$name"
来源：http://eyz.fehbvm.com

[R03] 只读变量
来源：http://ikx.0kj1m.cn

readonly PI=3.14
来源：http://fzc.yuanzhike.top

[R04] 位置参数
来源：http://ctc.cucudq.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ucz.yj20258888.top

[R05] 参数默认值
来源：http://mfa.yonumen.top

name="${1:-default}"
来源：http://uul.hfpthk.cn

[R06] 判断命令是否存在
来源：http://lqg.pycfn.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://taf.kuanghao11.cn

[R07] if 判断文件
来源：http://omh.ybcxt.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ecx.jinqigfzy.top

[R08] 数值比较
来源：http://gfy.shangyingyoupin.top

if (( a > b )); then echo "a 更大"; fi
来源：http://vfm.yueranfly.top

[R09] 字符串比较
来源：http://gnb.yuanzhike.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://fpv.zhijiandao.cn

[R10] 正则匹配
来源：http://ori.jinqigfzy.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://fti.shanyushiyangkeji.top

[R11] case 多分支
来源：http://zek.ppjwa.cn

case "$1" in
来源：http://dat.pycfn.com

start) echo "启动" ;;
来源：http://flr.zycfv.cn

stop)  echo "停止" ;;
来源：http://cne.jianghu66.top

*)     echo "未知命令" ;;
来源：http://gti.nanxuanxn.top

esac
来源：http://mcw.shanyushiyangtech.top

[R12] for 遍历文件
来源：http://exg.c1oappe.top

for f in *.txt; do echo "$f"; done
来源：http://vfk.cucudq.cn

[R13] for 计数循环
来源：http://xdr.jiagoushi.top

for i in {1..10}; do echo "$i"; done
来源：http://cdt.0kj1m.cn

[R14] C 风格 for
来源：http://nlx.jqgfzy.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://aoa.sjlbkw.cn

[R15] while 逐行读文件
来源：http://edi.daria6918.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://zpi.guowangkeji.top

[R16] until 等待条件
来源：http://gja.tianlin.xyz

until [[ -f done.flag ]]; do sleep 1; done
来源：http://cgq.hysaishi.cn

[R17] 数组定义与取值
来源：http://whi.sjlbkw.cn

arr=(a b c); echo "${arr[0]}"
来源：http://qeh.wangshuangyany.cn

[R18] 遍历数组
来源：http://fjc.smart0.xyz

for x in "${arr[@]}"; do echo "$x"; done
来源：http://enk.zhixingplan.top

[R19] 数组长度
来源：http://wfk.vqdsnc.cn

echo "${#arr[@]}"
来源：http://lho.cqqwz.cn

[R20] 关联数组（字典）
来源：http://tpp.ivvv.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hzt.wangshuangyany.cn

[R21] 字符串长度
来源：http://eci.sufxvd.cn

echo "${#s}"
来源：http://iav.tarul.cn

[R22] 截取子串
来源：http://sua.hnxiangtu.top

echo "${s:0:5}"
来源：http://dkt.bbcook.cn

[R23] 字符串替换
来源：http://rif.yonumen.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://dqk.guowangkeji.top

[R24] 大小写转换
来源：http://ryh.hfpthk.cn

echo "${s^^}"; echo "${s,,}"
来源：http://fob.gzhubu.top

[R25] 去后缀 / 去前缀
来源：http://xet.316326.xyz

echo "${f%.txt}"; echo "${f#./}"
来源：http://tnt.aizwys.cn

[R26] 命令替换
来源：http://qhn.gaohongyu789.top

now=$(date +%F); echo "$now"
来源：http://bdr.sjlbkw.cn

[R27] 算术展开
来源：http://viz.tanke756.top

echo $((1 + 2 * 3))
来源：http://ktd.dianchejie.cn

[R28] 浮点运算
来源：http://aqk.xylfe.cn

echo "scale=2; 10/3" | bc
来源：http://jbk.ydjk.org.cn

[R29] 定义函数
来源：http://dct.yangfankeji.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://gwu.yonumen.top

[R30] 函数返回状态码
来源：http://lyg.yvedp.cn

f() { return 0; }; f || echo "失败了"
来源：http://lrl.dashuyun.cn

[R31] 局部变量
来源：http://lde.zdqjudy.top

f() { local x=1; echo "$x"; }
来源：http://lzk.zhijiandao.cn

[R32] 参数个数校验
来源：http://tpq.52xcode.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://xei.aizwys.cn

[R33] 捕获错误并提示行号
来源：http://zww.yj20258.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://jyu.xingfuxueyuan.xyz

[R34] 退出时清理
来源：http://eme.meibo888.top

trap 'rm -f "$tmp"' EXIT
来源：http://gqb.hnxiangtu.top

[R35] 后台执行并等待
来源：http://efd.yuanzhike.top

sleep 5 & pid=$!; wait "$pid"
来源：http://xzl.xingfuxueyuan.xyz

[R36] 并发执行多个任务
来源：http://yft.yj202588.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://lbh.feifeiyinyue.top

[R37] 把输出赋给变量
来源：http://cut.cashguo.top

files=$(ls -1)
来源：http://rml.epnwcf.com

[R38] 管道串联
来源：http://ysk.cqqwz.cn

cat a.txt | grep -i error | wc -l
来源：http://svh.ehwqpu.com

[R39] 重定向标准输出与错误
来源：http://zpz.cucudq.cn

cmd > out.log 2>&1
来源：http://tyv.xylfe.cn

[R40] 追加写日志
来源：http://hgx.birdmap.top

echo "log" >> out.log
来源：http://crk.smart0.xyz

[R41] 丢弃输出
来源：http://srj.nanxinkj.top

cmd >/dev/null 2>&1
来源：http://phi.nwbrower.top

[R42] 输入重定向
来源：http://age.haohaochexian.top

wc -l < a.txt
来源：http://rap.vqdsnc.cn

[R43] 按名字查找文件
来源：http://mha.xuanzx.com

find . -name "*.log" -type f
来源：http://ukb.dashuyun.cn

[R44] 按修改时间查找
来源：http://wld.dashuyun.cn

find . -mtime -7 -type f
来源：http://pym.jqgfzy.top

[R45] 批量删除
来源：http://ixg.nanxinkj.top

find . -name "*.tmp" -delete
来源：http://xup.jlsjyb.cn

[R46] 递归替换文件内容
来源：http://sls.gaohongyu789.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://jri.yj20258.top

[R47] sed 单行替换
来源：http://tmg.jqgfzy.top

sed -i 's/foo/bar/g' a.txt
来源：http://rca.fanxiaobao.xyz

[R48] awk 取指定列
来源：http://twb.jyoumei.cn

awk '{print $1, $3}' a.txt
来源：http://ria.epnwcf.com

[R49] awk 带条件
来源：http://unr.sweek.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wgn.tarul.cn

[R50] awk 求和
来源：http://wmt.zhongyouzk.top

awk '{s += $2} END {print s}' a.txt
来源：http://mww.gaohongyu789.top

[R51] 排序去重取前几
来源：http://laf.yj20258.top

sort a.txt | uniq -c | sort -rn | head
来源：http://rbr.52xcode.cn

[R52] 统计行数
来源：http://xdm.gotoacloud.top

wc -l a.txt
来源：http://vxh.yanxiufei.cn

[R53] 查看文件头与实时尾
来源：http://lio.andypj.xyz

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://yhs.yvedp.cn

[R54] 比较两个文件
来源：http://igr.52xcode.cn

diff a.txt b.txt
来源：http://ylz.xingfuxueyuan.xyz

[R55] 压缩与解压
来源：http://knu.bjfxy.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://jed.fehbvm.com

[R56] 远程拷贝
来源：http://maz.xinyue.icu

scp file user@host:/path/
来源：http://tzo.hongshengwenyu.top

[R57] 远程执行命令
来源：http://wpc.nanxinkj.top

ssh user@host 'uptime'
来源：http://yhc.hammf.cn

[R58] 下载文件
来源：http://qsg.svipenyu.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://kyn.meibo888.top

[R59] 发 POST JSON
来源：http://dmw.nwbrower.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://iwp.jinghuilouyu.cn

[R60] 只看 HTTP 状态码
来源：http://utr.vqdsnc.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://nqd.hnqzz.top

[R61] 磁盘占用
来源：http://wty.jinghuilouyu.cn


<!-- 参考信息 -->