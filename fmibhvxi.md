代发 wailian999

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://xhv.gotoacloud.top

[Q11] 一次插入多行
来源：http://kio.xingfuxueyuan.xyz

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://bud.hywenlv.cn

[Q12] 插入后取自增 ID
来源：http://rfu.jyoumei.cn

INSERT INTO users (name) VALUES ('C');
来源：http://mlb.ivvv.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://cuh.daxiang520.top

[Q13] 忽略重复插入
来源：http://twe.xuanzx.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mqu.ehwqpu.com

[Q14] 存在则更新（upsert）
来源：http://agv.nanxinkj.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://trp.ppjwa.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://lxr.hcnkem.com

[Q15] 查询全部
来源：http://ebw.gzhubu.top

SELECT * FROM users;
来源：http://taa.chenjidiqi.icu

[Q16] 查询指定列
来源：http://rsb.tianlin.xyz

SELECT id, name FROM users;
来源：http://coa.daria6918.cn

[Q17] 条件查询
来源：http://xzr.nanxuanxn.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://nsl.ydzc1.top

[Q18] 模糊匹配
来源：http://csg.hnxiangtu.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hni.smart0.xyz

[Q19] 范围查询
来源：http://quu.jinqigfzy.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://xky.hesvh.cn

[Q20] IN 列表
来源：http://yop.ppjwa.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://qyp.hnqzz.top

[Q21] 空值判断
来源：http://yde.epnwcf.com

SELECT * FROM users WHERE email IS NULL;
来源：http://rpt.guowangkeji.top

[Q22] 排序
来源：http://aap.cqqwz.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://lnc.jyoumei.cn

[Q23] 分页
来源：http://yyd.yongpay.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://uam.ywan-chungtsiang.top

[Q24] 去重
来源：http://zav.aizwys.cn

SELECT DISTINCT city FROM users;
来源：http://wkd.aizwys.cn

[Q25] 只取前 N 条
来源：http://qzp.snrcjt.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wxt.redwolf501.top

[Q26] 计数
来源：http://wgl.pengpengdd.cyou

SELECT COUNT(*) FROM users;
来源：http://jap.cheryme.top

[Q27] 条件计数
来源：http://cho.zhijiandao.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://tbj.haohaochexian.top

[Q28] 求和与平均
来源：http://rwv.gzhubu.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://dfb.shanyushiyangtech.top

[Q29] 最大最小值
来源：http://abj.yueranfly.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://jxd.ppjwa.cn

[Q30] 分组统计
来源：http://mfv.uphjek.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://zir.yongpay.top

[Q31] 分组后过滤
来源：http://iic.chenzaomai.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://puk.jqgfzy.top

[Q32] 分组拼接字符串
来源：http://wtz.hongshengwenyu.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://qpe.aibaodan.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://akz.vqdsnc.cn

[Q33] 多列分组
来源：http://luj.cucudq.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ufv.redwolf501.top

[Q34] 每组取第一条
来源：http://hkp.redwolf501.top

SELECT * FROM (
来源：http://iwt.9152youxi.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mnm.zycfv.cn

) t WHERE rn = 1;
来源：http://njy.zhixingplan.top

[Q35] 内连接
来源：http://gji.jlsjyb.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://oby.zhongyouzk.top

[Q36] 左连接
来源：http://fat.ehwqpu.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://rqx.guannengcc.top

[Q37] 右连接
来源：http://hen.smart0.xyz

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wzo.c1oappe.top

[Q38] 全外连接（PostgreSQL）
来源：http://hjv.zycfv.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ygy.tianlin.xyz

[Q39] 自连接（查上下级）
来源：http://azx.nwbrower.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://teo.guowangkeji.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://oyw.gogol.net.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://abb.dianchejie.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://iyh.ppjwa.cn

[Q41] 多表连接
来源：http://jlc.hysaishi.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://qqv.jinqigfzy.top

JOIN users u ON u.id = o.user_id
来源：http://nnf.gaohongyu789.top

JOIN products p ON p.id = o.product_id;
来源：http://gpx.vehdjk.com

[Q42] 连接条件附加过滤
来源：http://ygn.bjfxy.top

SELECT u.name, o.amount FROM users u
来源：http://lva.sysykeji.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mrr.epnwcf.com

[Q43] 标量子查询
来源：http://vtl.yonumen.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://tcr.mhx1999.top

[Q44] IN 子查询
来源：http://ywt.hywenlv.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://cli.jinyuanbaomall.cn

[Q45] EXISTS 判断存在
来源：http://fvq.nanxinkj.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ukg.jinyuanbaomall.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ixl.shuidangran.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://awi.9152youxi.cn

[Q47] 与平均值比较
来源：http://jbb.zhongyouzk.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://aab.snrcjt.cn

[Q48] CTE 公用表表达式
来源：http://jqr.jqgfzy.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ane.zhongyouzk.top

SELECT * FROM t WHERE c > 5;
来源：http://owp.wangdashe.top

[Q49] 更新单行
来源：http://njz.bjfxy.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://jyx.yongpay.top

[Q50] 批量更新
来源：http://oia.mhx1999.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://iog.gzhubu.top

[Q51] 用子查询更新
来源：http://xly.bjfxy.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://piz.xuetiantiany.cn

[Q52] 删除指定行
来源：http://urx.andypj.xyz

DELETE FROM users WHERE id = 10;
来源：http://tqw.zhixingplan.top

[Q53] 按条件删除
来源：http://qav.snrcjt.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://jdh.9152youxi.cn

[Q54] 清空表
来源：http://ztb.zhongyouzk.top

TRUNCATE TABLE logs;
来源：http://lsd.fzhhl.top

[Q55] 排名（并列占位）
来源：http://wng.cheryme.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://rwe.shanyushiyangkeji.top

[Q56] 密集排名（并列不占位）
来源：http://thq.shangyingyoupin.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://pex.cucudq.cn

[Q57] 行号
来源：http://sod.zhaomingkeji.xyz

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://tvs.jinqigufen.top

[Q58] 累计求和
来源：http://uif.fengsongda.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://oyh.xuanzx.com

[Q59] 分组内累计
来源：http://jzu.nanxinkj.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://oqm.pycfn.com

[Q60] 取上一行 / 下一行
来源：http://gzh.jqgufenzy.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://otd.jyoumei.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mmq.chenlongwang.top

[Q61] 移动平均
来源：http://ech.hnqzz.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://zvt.tian-w.cn

[Q62] 分组占比
来源：http://gpb.fzhhl.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://nxr.guannengcc.top

[Q63] 开启事务
来源：http://azk.zhoulong.xyz

START TRANSACTION;                -- 或 BEGIN
来源：http://efh.quarkkingdee.top

[Q64] 提交事务
来源：http://ngq.epnwcf.com

COMMIT;
来源：http://xly.jinyuanbaomall.cn

[Q65] 回滚事务
来源：http://osg.316326.xyz

ROLLBACK;
来源：http://omi.yj20258.top

[Q66] 行锁查询
来源：http://iau.smart0.xyz

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://vmo.shanyushiyangkeji.top

[Q67] 设置隔离级别
来源：http://ggt.feifeiyinyue.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hky.yuxming.cn

[Q68] 保存点
来源：http://nba.zdqjudy.top

SAVEPOINT sp1;
来源：http://lht.svipenyu.cn

ROLLBACK TO sp1;
来源：http://fzh.chenzaomai.com

[Q69] 查看执行计划
来源：http://lju.shangyingyoupin.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://lda.yueranfly.top

[Q70] 更新统计信息
来源：http://cuw.yj20258.top

ANALYZE TABLE users;
来源：http://bnf.zhixingplan.top

[Q71] 查看建表语句
来源：http://lnj.xylfe.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://yea.kuanghao11.cn

[Q72] 查看索引
来源：http://syk.redwolf501.top

SHOW INDEX FROM users;
来源：http://muy.sxryk.cn

[Q73] 查看表状态
来源：http://tqm.smart0.xyz

SHOW TABLE STATUS LIKE 'users';
来源：http://jgs.hnxiangtu.top

[Q74] 强制使用索引
来源：http://utd.uphjek.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://nvg.wangshuangyany.cn

[Q75] 日期格式化
来源：http://yum.fanxiaobao.xyz

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://yct.svipenyu.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://tlc.daria6918.cn

[Q76] 按天统计
来源：http://uxe.yongpay.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://xog.0kj1m.cn

[Q77] 时间加减
来源：http://sjr.redwolf501.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ria.nwbrower.top

[Q78] 当前时间
来源：http://vpr.feifeiyinyue.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://zhk.chenjidiqi.icu

[Q79] 字符串拼接
来源：http://mqj.haohaochexian.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://prd.iojbl.cn

[Q80] 字符串截取
来源：http://kgs.yj202588.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://tln.ehwqpu.com

[Q81] 字符串替换
来源：http://qrf.svipenyu.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://irr.zhengqikj.top

[Q82] 字符长度与字节长度
来源：http://ipa.epnwcf.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://eet.wangdashe.top

[Q83] 大小写转换
来源：http://bjh.hywenlv.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://gyp.kuanghao11.cn

[Q84] 去除首尾空格
来源：http://kfq.birdmap.top

SELECT TRIM(name) FROM users;
来源：http://cxd.hnxiangtu.top

[Q85] 数值取整
来源：http://qsq.hywenlv.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://spv.jinghuilouyu.cn

[Q86] 读取 JSON 字段
来源：http://lkl.uphjek.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://pbg.xingfuxueyuan.xyz

[Q87] JSON 字段做条件
来源：http://qzh.svipenyu.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://rbe.hammf.cn

[Q88] 行转列（条件聚合）
来源：http://qdy.sweek.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://iqh.sufxvd.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://aug.ywan-chungtsiang.top

[Q89] 判断表是否存在
来源：http://wru.sufxvd.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://udu.ydzc1.top

[Q90] 生成序号列
来源：http://hpx.redwolf501.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://zpo.daria6918.cn

================================================================================
来源：http://gte.jiagoushi.top

R. Bash 专题
来源：http://ydf.xylfe.cn

================================================================================
来源：http://eqr.hcnkem.com

[R01] shebang 与严格模式
来源：http://umu.shzxlz.cn

#!/usr/bin/env bash
来源：http://uoj.shangyingyoupin.top

set -euo pipefail
来源：http://dcy.xziqi.cn

[R02] 变量赋值与使用
来源：http://ezj.cdnleiting.top

name="Tom"; echo "$name"
来源：http://fgy.ivvv.top

[R03] 只读变量
来源：http://tho.xinyue.icu

readonly PI=3.14
来源：http://tew.svipenyu.cn

[R04] 位置参数
来源：http://vxe.wangdashe.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://fpi.havefunace.top

[R05] 参数默认值
来源：http://hpl.iojbl.cn

name="${1:-default}"
来源：http://hsb.jyoumei.cn

[R06] 判断命令是否存在
来源：http://tdg.nanxinkj.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://noq.haohaochexian.top

[R07] if 判断文件
来源：http://ust.fktsv.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://xjb.nanxuanxn.top

[R08] 数值比较
来源：http://mjt.vehdjk.com

if (( a > b )); then echo "a 更大"; fi
来源：http://zsy.ppjwa.cn

[R09] 字符串比较
来源：http://kci.aibaodan.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://qdq.hywenlv.cn

[R10] 正则匹配
来源：http://rok.guannengcc.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://upg.kuanghao11.cn

[R11] case 多分支
来源：http://evt.0kj1m.cn

case "$1" in
来源：http://lta.andypj.xyz

start) echo "启动" ;;
来源：http://odr.bbcook.cn

stop)  echo "停止" ;;
来源：http://ojy.hcnkem.com

*)     echo "未知命令" ;;
来源：http://ful.ivvv.top

esac
来源：http://hux.zycfv.cn

[R12] for 遍历文件
来源：http://hlw.havefunace.top

for f in *.txt; do echo "$f"; done
来源：http://pkm.iojbl.cn

[R13] for 计数循环
来源：http://aww.jqgufenzy.top

for i in {1..10}; do echo "$i"; done
来源：http://xjo.xinyue.icu

[R14] C 风格 for
来源：http://ihf.quarkkingdee.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://tdx.vqdsnc.cn

[R15] while 逐行读文件
来源：http://nuz.shanyushiyangtech.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ptp.zhiwuduotai.top

[R16] until 等待条件
来源：http://qqn.shanyushiyangtech.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ukn.yonumen.top

[R17] 数组定义与取值
来源：http://dne.ydjk.org.cn

arr=(a b c); echo "${arr[0]}"
来源：http://fia.yonumen.top

[R18] 遍历数组
来源：http://bgt.jlsjyb.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://zlg.tianlin.xyz

[R19] 数组长度
来源：http://hhp.gzhubu.top

echo "${#arr[@]}"
来源：http://kmz.jlsjyb.cn

[R20] 关联数组（字典）
来源：http://dvf.sjlbkw.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mfx.dianchejie.cn

[R21] 字符串长度
来源：http://wpn.ivvv.top

echo "${#s}"
来源：http://krz.gogol.net.cn

[R22] 截取子串
来源：http://mas.tarul.cn

echo "${s:0:5}"
来源：http://qdc.jqgfzy.top

[R23] 字符串替换
来源：http://nbr.havefunace.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://qnp.iojbl.cn

[R24] 大小写转换
来源：http://hav.hywenlv.cn

echo "${s^^}"; echo "${s,,}"
来源：http://pio.cdnleiting.top

[R25] 去后缀 / 去前缀
来源：http://lgr.wangshuangyany.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://lkt.0kj1m.cn

[R26] 命令替换
来源：http://hkj.yj20258888.top

now=$(date +%F); echo "$now"
来源：http://nit.gzhubu.top

[R27] 算术展开
来源：http://dkn.zdbjq.cn

echo $((1 + 2 * 3))
来源：http://kep.hysaishi.cn

[R28] 浮点运算
来源：http://kob.yj20258.top

echo "scale=2; 10/3" | bc
来源：http://cnb.c1oappe.top

[R29] 定义函数
来源：http://kcc.hywenlv.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://qzg.cheryme.top

[R30] 函数返回状态码
来源：http://ion.nanxinkj.top

f() { return 0; }; f || echo "失败了"
来源：http://jxo.chenzaomai.com

[R31] 局部变量
来源：http://sca.zhengqikj.top

f() { local x=1; echo "$x"; }
来源：http://cdr.wangdashe.top

[R32] 参数个数校验
来源：http://mdh.ehwqpu.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ndv.jinghuilouyu.cn

[R33] 捕获错误并提示行号
来源：http://dvg.fzhhl.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://nkx.yanxiufei.cn

[R34] 退出时清理
来源：http://yyd.dashuyun.cn

trap 'rm -f "$tmp"' EXIT
来源：http://vzv.guowangkeji.top

[R35] 后台执行并等待
来源：http://bcz.hongshengwenyu.top

sleep 5 & pid=$!; wait "$pid"
来源：http://nhc.aizwys.cn

[R36] 并发执行多个任务
来源：http://fqn.cqqwz.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://nma.iojbl.cn

[R37] 把输出赋给变量
来源：http://djf.jinyuanbaomall.cn

files=$(ls -1)
来源：http://ycj.zdqjudy.top

[R38] 管道串联
来源：http://bwr.zdqjudy.top

cat a.txt | grep -i error | wc -l
来源：http://tam.yuxming.cn

[R39] 重定向标准输出与错误
来源：http://ees.zhengqikj.top

cmd > out.log 2>&1
来源：http://xxo.jinyuanbaomall.cn

[R40] 追加写日志
来源：http://kbe.ppjwa.cn

echo "log" >> out.log
来源：http://lks.0kj1m.cn

[R41] 丢弃输出
来源：http://tdv.yj20258888.top

cmd >/dev/null 2>&1
来源：http://znx.zhaomingkeji.xyz

[R42] 输入重定向
来源：http://bef.tianlin.xyz

wc -l < a.txt
来源：http://rhb.shanyushiyangkeji.top

[R43] 按名字查找文件
来源：http://bvi.yanxiufei.cn

find . -name "*.log" -type f
来源：http://bpt.guowangkeji.top

[R44] 按修改时间查找
来源：http://rga.yongpay.top

find . -mtime -7 -type f
来源：http://nqc.zhongyouzk.top

[R45] 批量删除
来源：http://nwv.zhengqikj.top

find . -name "*.tmp" -delete
来源：http://gxl.xylfe.cn

[R46] 递归替换文件内容
来源：http://trr.shanyushiyangtech.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://zou.yuanzhike.top

[R47] sed 单行替换
来源：http://kwv.gzhubu.top

sed -i 's/foo/bar/g' a.txt
来源：http://jbo.jqgfzy.top

[R48] awk 取指定列
来源：http://lix.jyoumei.cn

awk '{print $1, $3}' a.txt
来源：http://lhj.jqgfzy.top

[R49] awk 带条件
来源：http://ztn.kuanghao11.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://sgn.smart0.xyz

[R50] awk 求和
来源：http://hro.zhengqikj.top

awk '{s += $2} END {print s}' a.txt
来源：http://xka.fzhhl.top

[R51] 排序去重取前几
来源：http://eac.jyoumei.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://tlt.jinqigufen.top

[R52] 统计行数
来源：http://smr.nanxuanxn.top

wc -l a.txt
来源：http://dwk.redwolf501.top

[R53] 查看文件头与实时尾
来源：http://wrp.fengsongda.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://equ.316326.xyz

[R54] 比较两个文件
来源：http://gwu.snrcjt.cn

diff a.txt b.txt
来源：http://esg.0kj1m.cn

[R55] 压缩与解压
来源：http://dgz.zhoulong.xyz

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mdc.dianchejie.cn

[R56] 远程拷贝
来源：http://gxy.jinqigufen.top

scp file user@host:/path/
来源：http://bng.yonumen.top

[R57] 远程执行命令
来源：http://hcy.jlsjyb.cn

ssh user@host 'uptime'
来源：http://kzo.gogol.net.cn

[R58] 下载文件
来源：http://yvb.haohaochexian.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ztg.zhijiandao.cn

[R59] 发 POST JSON
来源：http://fpz.jinqigufen.top


<!-- 参考信息 -->