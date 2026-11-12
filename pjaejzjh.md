代发 wailian999

INSERT INTO users (name) VALUES ('C');
来源：http://jio.xylfe.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://gjm.daria6918.cn

[Q13] 忽略重复插入
来源：http://qek.fengsongda.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://onq.meibo888.top

[Q14] 存在则更新（upsert）
来源：http://krg.hesvh.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ddp.cqqwz.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://rcl.xingfuxueyuan.xyz

[Q15] 查询全部
来源：http://dcn.cdnleiting.top

SELECT * FROM users;
来源：http://khs.9152youxi.cn

[Q16] 查询指定列
来源：http://qqr.pengpengdd.cyou

SELECT id, name FROM users;
来源：http://lmx.yuanzhike.top

[Q17] 条件查询
来源：http://rog.cashguo.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wxj.shanyushiyangkeji.top

[Q18] 模糊匹配
来源：http://bsx.cucudq.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://gmm.fehbvm.com

[Q19] 范围查询
来源：http://oxn.snrcjt.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ybf.pycfn.com

[Q20] IN 列表
来源：http://smg.nanxinkj.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://deo.andypj.xyz

[Q21] 空值判断
来源：http://fpa.gotoacloud.top

SELECT * FROM users WHERE email IS NULL;
来源：http://lwd.uphjek.com

[Q22] 排序
来源：http://unl.gogol.net.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://rgf.jinqigufen.top

[Q23] 分页
来源：http://ghp.tianlin.xyz

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ulf.vehdjk.com

[Q24] 去重
来源：http://crr.smart0.xyz

SELECT DISTINCT city FROM users;
来源：http://jwf.gotoacloud.top

[Q25] 只取前 N 条
来源：http://tnu.shangyingyoupin.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://tsb.gaohongyu789.top

[Q26] 计数
来源：http://cfm.tian-w.cn

SELECT COUNT(*) FROM users;
来源：http://ias.shangyingyoupin.top

[Q27] 条件计数
来源：http://kan.hongshengwenyu.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://arf.yfazqb.com

[Q28] 求和与平均
来源：http://mps.yueranfly.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://bpx.zdqjudy.top

[Q29] 最大最小值
来源：http://sij.ywan-chungtsiang.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://ckh.cucudq.cn

[Q30] 分组统计
来源：http://gra.gotoacloud.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://sqq.guannengcc.top

[Q31] 分组后过滤
来源：http://msz.iojbl.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://pcu.mhx1999.top

[Q32] 分组拼接字符串
来源：http://ykr.chenzaomai.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ram.xylfe.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://qox.yangfankeji.com

[Q33] 多列分组
来源：http://xbg.zhengqikj.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://grr.smart0.xyz

[Q34] 每组取第一条
来源：http://haq.ydjk.org.cn

SELECT * FROM (
来源：http://qfm.jinyuanbaomall.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ecy.jqgfzy.top

) t WHERE rn = 1;
来源：http://zkj.ctjpmb.com

[Q35] 内连接
来源：http://soy.yuxming.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mcf.bbcook.cn

[Q36] 左连接
来源：http://gdi.jinqigfzy.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://imf.chenlongwang.top

[Q37] 右连接
来源：http://qkb.xziqi.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://gse.xuanzx.com

[Q38] 全外连接（PostgreSQL）
来源：http://glq.xinyue.icu

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://kjc.chenzaomai.com

[Q39] 自连接（查上下级）
来源：http://wfu.smart0.xyz

SELECT e.name, m.name AS manager FROM employees e
来源：http://hqs.yuanzhike.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://tsl.wangshuangyany.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://dqv.yvedp.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hzl.shuidangran.top

[Q41] 多表连接
来源：http://blj.aibaodan.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://exp.tian-w.cn

JOIN users u ON u.id = o.user_id
来源：http://dou.zhaomingkeji.xyz

JOIN products p ON p.id = o.product_id;
来源：http://rbd.aizwys.cn

[Q42] 连接条件附加过滤
来源：http://ulz.yuxming.cn

SELECT u.name, o.amount FROM users u
来源：http://sdj.xinyue.icu

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mgn.nanxuanxn.top

[Q43] 标量子查询
来源：http://fhi.jinqigfzy.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://vmv.daria6918.cn

[Q44] IN 子查询
来源：http://imq.fktsv.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://fre.quarkkingdee.top

[Q45] EXISTS 判断存在
来源：http://vff.guannengcc.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://gxp.hesvh.cn

[Q46] NOT EXISTS 判断不存在
来源：http://dcd.yvedp.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://yrw.hnqzz.top

[Q47] 与平均值比较
来源：http://apv.aizwys.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ysp.shanyushiyangtech.top

[Q48] CTE 公用表表达式
来源：http://gfk.jinghuilouyu.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ovk.gogol.net.cn

SELECT * FROM t WHERE c > 5;
来源：http://eum.zhengqikj.top

[Q49] 更新单行
来源：http://ksl.dashuyun.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://abh.zhoulong.xyz

[Q50] 批量更新
来源：http://rkl.snrcjt.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ggq.zhixingplan.top

[Q51] 用子查询更新
来源：http://rev.guannengcc.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://tye.316326.xyz

[Q52] 删除指定行
来源：http://aak.ehwqpu.com

DELETE FROM users WHERE id = 10;
来源：http://van.hcnkem.com

[Q53] 按条件删除
来源：http://ids.iojbl.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://lty.yueranfly.top

[Q54] 清空表
来源：http://sgx.uphjek.com

TRUNCATE TABLE logs;
来源：http://ahm.gzhubu.top

[Q55] 排名（并列占位）
来源：http://nbj.9152youxi.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://kvt.smart0.xyz

[Q56] 密集排名（并列不占位）
来源：http://mpp.bbcook.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mvb.yj202588.top

[Q57] 行号
来源：http://fbu.fzhhl.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://his.redwolf501.top

[Q58] 累计求和
来源：http://btc.jinyuanbaomall.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ukl.guannengcc.top

[Q59] 分组内累计
来源：http://sgg.dianchejie.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://jpt.jinqigufen.top

[Q60] 取上一行 / 下一行
来源：http://bem.yj20258.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://pan.vqdsnc.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://zki.hywenlv.cn

[Q61] 移动平均
来源：http://bwv.aibaodan.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wvx.tian-w.cn

[Q62] 分组占比
来源：http://uin.svipenyu.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ziq.jqgfzy.top

[Q63] 开启事务
来源：http://xgt.yonumen.top

START TRANSACTION;                -- 或 BEGIN
来源：http://pit.hysaishi.cn

[Q64] 提交事务
来源：http://qqg.jyoumei.cn

COMMIT;
来源：http://urq.cashguo.top

[Q65] 回滚事务
来源：http://rxc.gotoacloud.top

ROLLBACK;
来源：http://yld.shanyushiyangtech.top

[Q66] 行锁查询
来源：http://mqo.9152youxi.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://arh.pengpengdd.cyou

[Q67] 设置隔离级别
来源：http://sje.ctjpmb.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://tzk.uphjek.com

[Q68] 保存点
来源：http://kpw.yvedp.cn

SAVEPOINT sp1;
来源：http://qod.mhx1999.top

ROLLBACK TO sp1;
来源：http://awc.nwbrower.top

[Q69] 查看执行计划
来源：http://kgc.cucudq.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://bpu.ydzc1.top

[Q70] 更新统计信息
来源：http://abx.yuanzhike.top

ANALYZE TABLE users;
来源：http://ier.pengpengdd.cyou

[Q71] 查看建表语句
来源：http://fvo.zhongyouzk.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://xll.ivvv.top

[Q72] 查看索引
来源：http://qsc.fktsv.cn

SHOW INDEX FROM users;
来源：http://piu.cheryme.top

[Q73] 查看表状态
来源：http://wkc.shangyingyoupin.top

SHOW TABLE STATUS LIKE 'users';
来源：http://kgv.quarkkingdee.top

[Q74] 强制使用索引
来源：http://asp.jiagoushi.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wpx.havefunace.top

[Q75] 日期格式化
来源：http://xfw.cdnleiting.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ari.jqgfzy.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ssv.kuanghao11.cn

[Q76] 按天统计
来源：http://nhm.yongpay.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ugw.zhiwuduotai.top

[Q77] 时间加减
来源：http://xdq.jiagoushi.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://fqo.hcnkem.com

[Q78] 当前时间
来源：http://idj.yongpay.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://vgm.gaohongyu789.top

[Q79] 字符串拼接
来源：http://dbw.aibaodan.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://kax.bbcook.cn

[Q80] 字符串截取
来源：http://cgl.vqdsnc.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://nnu.bjfxy.top

[Q81] 字符串替换
来源：http://dro.dianchejie.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://jmj.xinyue.icu

[Q82] 字符长度与字节长度
来源：http://kbc.bjfxy.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://cvw.316326.xyz

[Q83] 大小写转换
来源：http://owm.xziqi.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://yqm.cucudq.cn

[Q84] 去除首尾空格
来源：http://dsy.jinqigufen.top

SELECT TRIM(name) FROM users;
来源：http://mwh.jlsjyb.cn

[Q85] 数值取整
来源：http://qyf.ppjwa.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://gyd.tian-w.cn

[Q86] 读取 JSON 字段
来源：http://rfp.zhixingplan.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://xdb.tian-w.cn

[Q87] JSON 字段做条件
来源：http://xoz.zhaomingkeji.xyz

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://lof.svipenyu.cn

[Q88] 行转列（条件聚合）
来源：http://rmx.wangdashe.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://lbr.haohaochexian.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hki.gaohongyu789.top

[Q89] 判断表是否存在
来源：http://lgr.xziqi.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://buh.uphjek.com

[Q90] 生成序号列
来源：http://kny.sjlbkw.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://chc.xziqi.cn

================================================================================
来源：http://dzx.cashguo.top

R. Bash 专题
来源：http://oay.0kj1m.cn

================================================================================
来源：http://dqr.fktsv.cn

[R01] shebang 与严格模式
来源：http://bzg.zhengqikj.top

#!/usr/bin/env bash
来源：http://qrz.guannengcc.top

set -euo pipefail
来源：http://igk.shangyingyoupin.top

[R02] 变量赋值与使用
来源：http://xbx.chenjidiqi.icu

name="Tom"; echo "$name"
来源：http://xvv.tanke756.top

[R03] 只读变量
来源：http://riy.sxryk.cn

readonly PI=3.14
来源：http://vzu.chenlongwang.top

[R04] 位置参数
来源：http://ven.hnqzz.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mvl.zhaomingkeji.xyz

[R05] 参数默认值
来源：http://rrk.hnqzz.top

name="${1:-default}"
来源：http://ehy.zhoulong.xyz

[R06] 判断命令是否存在
来源：http://obv.yueranfly.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mrv.guannengcc.top

[R07] if 判断文件
来源：http://nda.zhengqikj.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://yiu.xinyue.icu

[R08] 数值比较
来源：http://apu.jinghuilouyu.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://jtn.vqdsnc.cn

[R09] 字符串比较
来源：http://yih.jiagoushi.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://yda.cdnleiting.top

[R10] 正则匹配
来源：http://erq.yvedp.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://xmq.gogol.net.cn

[R11] case 多分支
来源：http://ruv.jqgufenzy.top

case "$1" in
来源：http://meh.sxryk.cn

start) echo "启动" ;;
来源：http://pfx.gaohongyu789.top

stop)  echo "停止" ;;
来源：http://tth.yongpay.top

*)     echo "未知命令" ;;
来源：http://mzh.9152youxi.cn

esac
来源：http://wyb.jiagoushi.top

[R12] for 遍历文件
来源：http://zux.zhengqikj.top

for f in *.txt; do echo "$f"; done
来源：http://ozv.zhongyouzk.top

[R13] for 计数循环
来源：http://cce.hammf.cn

for i in {1..10}; do echo "$i"; done
来源：http://xfo.ydjk.org.cn

[R14] C 风格 for
来源：http://shp.ppjwa.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://dbo.chenjidiqi.icu

[R15] while 逐行读文件
来源：http://oqa.redwolf501.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://rzq.daria6918.cn

[R16] until 等待条件
来源：http://feo.tarul.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://fuj.epnwcf.com

[R17] 数组定义与取值
来源：http://bwa.cdnleiting.top

arr=(a b c); echo "${arr[0]}"
来源：http://zrr.yj20258.top

[R18] 遍历数组
来源：http://wrw.birdmap.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://zwn.tianlin.xyz

[R19] 数组长度
来源：http://fxs.zycfv.cn

echo "${#arr[@]}"
来源：http://rmd.jyoumei.cn

[R20] 关联数组（字典）
来源：http://oqj.jqgfzy.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://czx.vehdjk.com

[R21] 字符串长度
来源：http://dnn.shuidangran.top

echo "${#s}"
来源：http://fyt.sysykeji.top

[R22] 截取子串
来源：http://wlx.shzxlz.cn

echo "${s:0:5}"
来源：http://iwa.fktsv.cn

[R23] 字符串替换
来源：http://llm.yanxiufei.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://zfh.chenlongwang.top

[R24] 大小写转换
来源：http://xys.shanyushiyangtech.top

echo "${s^^}"; echo "${s,,}"
来源：http://byt.gzhubu.top

[R25] 去后缀 / 去前缀
来源：http://cqt.nanxinkj.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://vyo.fengsongda.top

[R26] 命令替换
来源：http://avw.quarkkingdee.top

now=$(date +%F); echo "$now"
来源：http://jra.epnwcf.com

[R27] 算术展开
来源：http://xzf.gaohongyu789.top

echo $((1 + 2 * 3))
来源：http://vcu.zdqjudy.top

[R28] 浮点运算
来源：http://oat.redwolf501.top

echo "scale=2; 10/3" | bc
来源：http://uyl.chenzaomai.com

[R29] 定义函数
来源：http://xdi.ivvv.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://krj.52xcode.cn

[R30] 函数返回状态码
来源：http://idc.zdqjudy.top

f() { return 0; }; f || echo "失败了"
来源：http://ekk.ehwqpu.com

[R31] 局部变量
来源：http://cia.cheryme.top

f() { local x=1; echo "$x"; }
来源：http://qbv.uphjek.com

[R32] 参数个数校验
来源：http://vzx.gaohongyu789.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://gqy.fzhhl.top

[R33] 捕获错误并提示行号
来源：http://rjy.316326.xyz

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://yuv.vehdjk.com

[R34] 退出时清理
来源：http://was.shangyingyoupin.top

trap 'rm -f "$tmp"' EXIT
来源：http://wfm.nanxinkj.top

[R35] 后台执行并等待
来源：http://dlx.chenzaomai.com

sleep 5 & pid=$!; wait "$pid"
来源：http://ugh.pycfn.com

[R36] 并发执行多个任务
来源：http://orf.vqdsnc.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://glo.ivvv.top

[R37] 把输出赋给变量
来源：http://fpn.dianchejie.cn

files=$(ls -1)
来源：http://csn.xylfe.cn

[R38] 管道串联
来源：http://uzz.fanxiaobao.xyz

cat a.txt | grep -i error | wc -l
来源：http://xok.dashuyun.cn

[R39] 重定向标准输出与错误
来源：http://wno.sysykeji.top

cmd > out.log 2>&1
来源：http://joi.vehdjk.com

[R40] 追加写日志
来源：http://bhh.meibo888.top

echo "log" >> out.log
来源：http://hbz.chenlongwang.top

[R41] 丢弃输出
来源：http://quz.ppjwa.cn

cmd >/dev/null 2>&1
来源：http://vod.sufxvd.cn

[R42] 输入重定向
来源：http://gyu.tarul.cn

wc -l < a.txt
来源：http://ywd.havefunace.top

[R43] 按名字查找文件
来源：http://zdz.ivvv.top

find . -name "*.log" -type f
来源：http://mej.chenzaomai.com

[R44] 按修改时间查找
来源：http://gbb.hysaishi.cn

find . -mtime -7 -type f
来源：http://jli.yfazqb.com

[R45] 批量删除
来源：http://flh.daria6918.cn

find . -name "*.tmp" -delete
来源：http://kvh.meibo888.top

[R46] 递归替换文件内容
来源：http://pqr.vqdsnc.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ruh.yangfankeji.com

[R47] sed 单行替换
来源：http://nnx.snrcjt.cn

sed -i 's/foo/bar/g' a.txt
来源：http://eqk.jinghuilouyu.cn

[R48] awk 取指定列
来源：http://oqa.zhijiandao.cn

awk '{print $1, $3}' a.txt
来源：http://gig.dianchejie.cn

[R49] awk 带条件
来源：http://kxt.xziqi.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ryw.aizwys.cn

[R50] awk 求和
来源：http://rqa.zhixingplan.top

awk '{s += $2} END {print s}' a.txt
来源：http://okj.xuetiantiany.cn

[R51] 排序去重取前几
来源：http://anf.gaohongyu789.top

sort a.txt | uniq -c | sort -rn | head
来源：http://tjg.ywan-chungtsiang.top

[R52] 统计行数
来源：http://xox.tian-w.cn

wc -l a.txt
来源：http://zzx.birdmap.top

[R53] 查看文件头与实时尾
来源：http://xqv.vqdsnc.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wim.fengsongda.top

[R54] 比较两个文件
来源：http://jjq.xinyue.icu

diff a.txt b.txt
来源：http://mmo.zhongyouzk.top

[R55] 压缩与解压
来源：http://ctx.shanyushiyangtech.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wid.9152youxi.cn

[R56] 远程拷贝
来源：http://qfz.daria6918.cn

scp file user@host:/path/
来源：http://wpv.ctjpmb.com

[R57] 远程执行命令
来源：http://jfr.tianlin.xyz

ssh user@host 'uptime'
来源：http://izu.tanke756.top

[R58] 下载文件
来源：http://dyi.cdnleiting.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://qfu.hnxiangtu.top

[R59] 发 POST JSON
来源：http://akf.yanxiufei.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://lok.yuxming.cn

[R60] 只看 HTTP 状态码
来源：http://hqj.9152youxi.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://sbv.aibaodan.cn

[R61] 磁盘占用
来源：http://dfc.zhiwuduotai.top


<!-- 参考信息 -->