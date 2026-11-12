代发 wailian999

CREATE INDEX idx_users_email ON users(email);
来源：http://ejx.gzhubu.top

[Q09] 创建唯一索引
来源：http://vus.tian-w.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://tgc.hongshengwenyu.top

[Q10] 插入单行
来源：http://wgs.ydjk.org.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://xiw.chenzaomai.com

[Q11] 一次插入多行
来源：http://hni.jyoumei.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://syi.zycfv.cn

[Q12] 插入后取自增 ID
来源：http://wmy.daxiang520.top

INSERT INTO users (name) VALUES ('C');
来源：http://hil.gotoacloud.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://zxg.mhx1999.top

[Q13] 忽略重复插入
来源：http://ecb.jiagoushi.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://lrl.shangyingyoupin.top

[Q14] 存在则更新（upsert）
来源：http://twt.yanxiufei.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://fzc.xylfe.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://pft.cashguo.top

[Q15] 查询全部
来源：http://lqo.zhoulong.xyz

SELECT * FROM users;
来源：http://mcg.sxryk.cn

[Q16] 查询指定列
来源：http://jus.hcnkem.com

SELECT id, name FROM users;
来源：http://smp.daria6918.cn

[Q17] 条件查询
来源：http://vjp.jqgfzy.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://qwa.xingfuxueyuan.xyz

[Q18] 模糊匹配
来源：http://gca.dashuyun.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://bju.havefunace.top

[Q19] 范围查询
来源：http://abh.hnxiangtu.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://xxj.jlsjyb.cn

[Q20] IN 列表
来源：http://xoz.cheryme.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://itb.fzhhl.top

[Q21] 空值判断
来源：http://nei.jianghu66.top

SELECT * FROM users WHERE email IS NULL;
来源：http://atm.dianchejie.cn

[Q22] 排序
来源：http://jlt.shuidangran.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://sng.redwolf501.top

[Q23] 分页
来源：http://mxr.gzhubu.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://fal.epnwcf.com

[Q24] 去重
来源：http://rtj.guowangkeji.top

SELECT DISTINCT city FROM users;
来源：http://mxo.havefunace.top

[Q25] 只取前 N 条
来源：http://hda.yuxming.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://egs.ydjk.org.cn

[Q26] 计数
来源：http://kat.jianghu66.top

SELECT COUNT(*) FROM users;
来源：http://bdz.hcnkem.com

[Q27] 条件计数
来源：http://rry.xylfe.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://qfu.xinyue.icu

[Q28] 求和与平均
来源：http://gkg.vqdsnc.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://eka.ppjwa.cn

[Q29] 最大最小值
来源：http://qxa.fehbvm.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://xjr.gaohongyu789.top

[Q30] 分组统计
来源：http://olf.yongpay.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://qnq.bjfxy.top

[Q31] 分组后过滤
来源：http://zkl.vqdsnc.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://zql.zdbjq.cn

[Q32] 分组拼接字符串
来源：http://wqf.yanxiufei.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mda.jinyuanbaomall.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://cqt.zycfv.cn

[Q33] 多列分组
来源：http://kot.ctjpmb.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://kbt.birdmap.top

[Q34] 每组取第一条
来源：http://xuw.sxryk.cn

SELECT * FROM (
来源：http://xxu.jinyuanbaomall.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://rvq.0kj1m.cn

) t WHERE rn = 1;
来源：http://yno.chenjidiqi.icu

[Q35] 内连接
来源：http://qrc.cashguo.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ahu.sufxvd.cn

[Q36] 左连接
来源：http://xdl.hnqzz.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ogm.epnwcf.com

[Q37] 右连接
来源：http://wif.jinqigufen.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://qmz.meibo888.top

[Q38] 全外连接（PostgreSQL）
来源：http://jag.wangdashe.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://kkc.cdnleiting.top

[Q39] 自连接（查上下级）
来源：http://cfl.cashguo.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://mke.jinghuilouyu.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://vzz.daxiang520.top

[Q40] 交叉连接（笛卡尔积）
来源：http://isd.jinqigfzy.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ryq.fktsv.cn

[Q41] 多表连接
来源：http://ngb.shangyingyoupin.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://xex.uphjek.com

JOIN users u ON u.id = o.user_id
来源：http://uag.vehdjk.com

JOIN products p ON p.id = o.product_id;
来源：http://kfy.yvedp.cn

[Q42] 连接条件附加过滤
来源：http://vkz.xuanzx.com

SELECT u.name, o.amount FROM users u
来源：http://err.xuetiantiany.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://sot.svipenyu.cn

[Q43] 标量子查询
来源：http://ohl.zdbjq.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hfn.yj20258888.top

[Q44] IN 子查询
来源：http://pjo.9152youxi.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://nib.fzhhl.top

[Q45] EXISTS 判断存在
来源：http://whl.cucudq.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ldl.fengsongda.top

[Q46] NOT EXISTS 判断不存在
来源：http://xps.dianchejie.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ztz.haohaochexian.top

[Q47] 与平均值比较
来源：http://uag.sjlbkw.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://knl.jqgfzy.top

[Q48] CTE 公用表表达式
来源：http://wpi.9152youxi.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://dxv.yueranfly.top

SELECT * FROM t WHERE c > 5;
来源：http://lys.hfpthk.cn

[Q49] 更新单行
来源：http://dae.tarul.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://lhf.sjlbkw.cn

[Q50] 批量更新
来源：http://lpa.dianchejie.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://nyr.52xcode.cn

[Q51] 用子查询更新
来源：http://ggw.zycfv.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://owx.yj20258888.top

[Q52] 删除指定行
来源：http://qlo.aibaodan.cn

DELETE FROM users WHERE id = 10;
来源：http://qlo.cheryme.top

[Q53] 按条件删除
来源：http://xgg.shuidangran.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://unt.ydzc1.top

[Q54] 清空表
来源：http://xla.cqqwz.cn

TRUNCATE TABLE logs;
来源：http://nvs.9152youxi.cn

[Q55] 排名（并列占位）
来源：http://tti.jinqigfzy.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://kmb.hcnkem.com

[Q56] 密集排名（并列不占位）
来源：http://kfv.jinghuilouyu.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://sid.yueranfly.top

[Q57] 行号
来源：http://hcs.zhongyouzk.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ryv.shanyushiyangtech.top

[Q58] 累计求和
来源：http://akl.fzhhl.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ftq.tian-w.cn

[Q59] 分组内累计
来源：http://zeo.birdmap.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://jtr.dianchejie.cn

[Q60] 取上一行 / 下一行
来源：http://slr.sxryk.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://pkb.andypj.xyz

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hwf.xylfe.cn

[Q61] 移动平均
来源：http://egg.tanke756.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://dqe.yj202588.top

[Q62] 分组占比
来源：http://zkq.birdmap.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://xqq.guowangkeji.top

[Q63] 开启事务
来源：http://bxs.uphjek.com

START TRANSACTION;                -- 或 BEGIN
来源：http://tuj.yongpay.top

[Q64] 提交事务
来源：http://wtp.hcnkem.com

COMMIT;
来源：http://hxf.svipenyu.cn

[Q65] 回滚事务
来源：http://ckx.9152youxi.cn

ROLLBACK;
来源：http://icx.ehwqpu.com

[Q66] 行锁查询
来源：http://dbg.ywan-chungtsiang.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://gsq.ppjwa.cn

[Q67] 设置隔离级别
来源：http://exn.sxryk.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mcc.ehwqpu.com

[Q68] 保存点
来源：http://ftk.mhx1999.top

SAVEPOINT sp1;
来源：http://lhg.316326.xyz

ROLLBACK TO sp1;
来源：http://bdb.vqdsnc.cn

[Q69] 查看执行计划
来源：http://nzq.pycfn.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://okk.redwolf501.top

[Q70] 更新统计信息
来源：http://ejk.iojbl.cn

ANALYZE TABLE users;
来源：http://sfv.jyoumei.cn

[Q71] 查看建表语句
来源：http://tbf.jiagoushi.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://lvw.ehwqpu.com

[Q72] 查看索引
来源：http://wxo.daxiang520.top

SHOW INDEX FROM users;
来源：http://vjh.pengpengdd.cyou

[Q73] 查看表状态
来源：http://pjy.fehbvm.com

SHOW TABLE STATUS LIKE 'users';
来源：http://etp.fanxiaobao.xyz

[Q74] 强制使用索引
来源：http://yze.xuanzx.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://gwp.sysykeji.top

[Q75] 日期格式化
来源：http://fyz.sweek.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mut.jinyuanbaomall.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://eoa.yj20258.top

[Q76] 按天统计
来源：http://agj.chenzaomai.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://aqc.snrcjt.cn

[Q77] 时间加减
来源：http://tip.xuanzx.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://kaf.gaohongyu789.top

[Q78] 当前时间
来源：http://yer.guowangkeji.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://rxb.ppjwa.cn

[Q79] 字符串拼接
来源：http://ovs.sweek.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://amp.c1oappe.top

[Q80] 字符串截取
来源：http://klp.shzxlz.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://sbt.fktsv.cn

[Q81] 字符串替换
来源：http://yja.hnqzz.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://avy.jinyuanbaomall.cn

[Q82] 字符长度与字节长度
来源：http://tpz.fktsv.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mtd.jinqigufen.top

[Q83] 大小写转换
来源：http://vrs.ydjk.org.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://qoz.ctjpmb.com

[Q84] 去除首尾空格
来源：http://cim.hcnkem.com

SELECT TRIM(name) FROM users;
来源：http://esl.meibo888.top

[Q85] 数值取整
来源：http://pih.zycfv.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://jqv.zdqjudy.top

[Q86] 读取 JSON 字段
来源：http://pwc.aizwys.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://rby.feifeiyinyue.top

[Q87] JSON 字段做条件
来源：http://qku.kuanghao11.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://pov.yj20258.top

[Q88] 行转列（条件聚合）
来源：http://zop.zdqjudy.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://czw.nwbrower.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wgv.jinqigfzy.top

[Q89] 判断表是否存在
来源：http://cha.sweek.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://zsp.zhixingplan.top

[Q90] 生成序号列
来源：http://vtt.shuidangran.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://sau.sweek.top

================================================================================
来源：http://dyw.yanxiufei.cn

R. Bash 专题
来源：http://dey.meibo888.top

================================================================================
来源：http://zgy.shanyushiyangtech.top

[R01] shebang 与严格模式
来源：http://ybt.daxiang520.top

#!/usr/bin/env bash
来源：http://zyo.tianlin.xyz

set -euo pipefail
来源：http://tjb.fzhhl.top

[R02] 变量赋值与使用
来源：http://bfs.fehbvm.com

name="Tom"; echo "$name"
来源：http://fgx.zhiwuduotai.top

[R03] 只读变量
来源：http://jot.xylfe.cn

readonly PI=3.14
来源：http://waj.chenjidiqi.icu

[R04] 位置参数
来源：http://edb.hesvh.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://pgn.vehdjk.com

[R05] 参数默认值
来源：http://avw.fzhhl.top

name="${1:-default}"
来源：http://bfn.hesvh.cn

[R06] 判断命令是否存在
来源：http://cxf.zhaomingkeji.xyz

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mna.fengsongda.top

[R07] if 判断文件
来源：http://wfi.fanxiaobao.xyz

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://tei.yanxiufei.cn

[R08] 数值比较
来源：http://zve.bjfxy.top

if (( a > b )); then echo "a 更大"; fi
来源：http://mgn.shuidangran.top

[R09] 字符串比较
来源：http://hcm.vehdjk.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://dan.hongshengwenyu.top

[R10] 正则匹配
来源：http://ocx.jianghu66.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ylw.fzhhl.top

[R11] case 多分支
来源：http://cbn.zhijiandao.cn

case "$1" in
来源：http://zfh.fanxiaobao.xyz

start) echo "启动" ;;
来源：http://lax.316326.xyz

stop)  echo "停止" ;;
来源：http://xwc.daria6918.cn

*)     echo "未知命令" ;;
来源：http://jyv.hnqzz.top

esac
来源：http://vaq.ydzc1.top

[R12] for 遍历文件
来源：http://fsl.birdmap.top

for f in *.txt; do echo "$f"; done
来源：http://yjw.feifeiyinyue.top

[R13] for 计数循环
来源：http://ndw.nanxuanxn.top

for i in {1..10}; do echo "$i"; done
来源：http://meo.xinyue.icu

[R14] C 风格 for
来源：http://xsy.yvedp.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://owa.zhijiandao.cn

[R15] while 逐行读文件
来源：http://zvc.jinqigfzy.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://obw.cqqwz.cn

[R16] until 等待条件
来源：http://div.cdnleiting.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wyb.bbcook.cn

[R17] 数组定义与取值
来源：http://vbi.ivvv.top

arr=(a b c); echo "${arr[0]}"
来源：http://wbm.hysaishi.cn

[R18] 遍历数组
来源：http://ssu.ivvv.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wjn.ybcxt.top

[R19] 数组长度
来源：http://hqu.bjfxy.top

echo "${#arr[@]}"
来源：http://pgu.tian-w.cn

[R20] 关联数组（字典）
来源：http://hmd.redwolf501.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hbl.uphjek.com

[R21] 字符串长度
来源：http://cbk.nwbrower.top

echo "${#s}"
来源：http://pbk.fanxiaobao.xyz

[R22] 截取子串
来源：http://sqn.xuetiantiany.cn

echo "${s:0:5}"
来源：http://xcj.chenjidiqi.icu

[R23] 字符串替换
来源：http://ysh.0kj1m.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://nes.9152youxi.cn

[R24] 大小写转换
来源：http://rcv.cheryme.top

echo "${s^^}"; echo "${s,,}"
来源：http://dxi.tianlin.xyz

[R25] 去后缀 / 去前缀
来源：http://uxz.meibo888.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://scd.xziqi.cn

[R26] 命令替换
来源：http://waf.fzhhl.top

now=$(date +%F); echo "$now"
来源：http://qxv.xinyue.icu

[R27] 算术展开
来源：http://soi.xylfe.cn

echo $((1 + 2 * 3))
来源：http://esu.sysykeji.top

[R28] 浮点运算
来源：http://zsh.chenjidiqi.icu

echo "scale=2; 10/3" | bc
来源：http://eqs.jqgfzy.top

[R29] 定义函数
来源：http://sps.jlsjyb.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://idt.sjlbkw.cn

[R30] 函数返回状态码
来源：http://xvq.shzxlz.cn

f() { return 0; }; f || echo "失败了"
来源：http://rfw.iojbl.cn

[R31] 局部变量
来源：http://hds.yuxming.cn

f() { local x=1; echo "$x"; }
来源：http://noz.9152youxi.cn

[R32] 参数个数校验
来源：http://kuu.hesvh.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://vce.hfpthk.cn

[R33] 捕获错误并提示行号
来源：http://kos.cqqwz.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://uaf.ydjk.org.cn

[R34] 退出时清理
来源：http://huw.wangdashe.top

trap 'rm -f "$tmp"' EXIT
来源：http://gud.bjfxy.top

[R35] 后台执行并等待
来源：http://oyw.ywan-chungtsiang.top

sleep 5 & pid=$!; wait "$pid"
来源：http://fqx.haohaochexian.top

[R36] 并发执行多个任务
来源：http://gcq.nanxinkj.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://fcq.hfpthk.cn

[R37] 把输出赋给变量
来源：http://vxy.cucudq.cn

files=$(ls -1)
来源：http://rij.fzhhl.top

[R38] 管道串联
来源：http://yfr.snrcjt.cn

cat a.txt | grep -i error | wc -l
来源：http://jyq.hywenlv.cn

[R39] 重定向标准输出与错误
来源：http://boh.wangdashe.top

cmd > out.log 2>&1
来源：http://zuj.vqdsnc.cn

[R40] 追加写日志
来源：http://ifn.cucudq.cn

echo "log" >> out.log
来源：http://wjo.yonumen.top

[R41] 丢弃输出
来源：http://jgw.xuanzx.com

cmd >/dev/null 2>&1
来源：http://zfd.epnwcf.com

[R42] 输入重定向
来源：http://wni.0kj1m.cn

wc -l < a.txt
来源：http://sgp.tian-w.cn

[R43] 按名字查找文件
来源：http://rtf.snrcjt.cn

find . -name "*.log" -type f
来源：http://pxd.shanyushiyangkeji.top

[R44] 按修改时间查找
来源：http://woi.birdmap.top

find . -mtime -7 -type f
来源：http://bbx.pycfn.com

[R45] 批量删除
来源：http://veu.fktsv.cn

find . -name "*.tmp" -delete
来源：http://bur.zhoulong.xyz

[R46] 递归替换文件内容
来源：http://bog.feifeiyinyue.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://agh.tian-w.cn

[R47] sed 单行替换
来源：http://msm.52xcode.cn

sed -i 's/foo/bar/g' a.txt
来源：http://cvo.fzhhl.top

[R48] awk 取指定列
来源：http://tis.316326.xyz

awk '{print $1, $3}' a.txt
来源：http://wry.meibo888.top

[R49] awk 带条件
来源：http://qxs.hcnkem.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://yhs.iojbl.cn

[R50] awk 求和
来源：http://bju.cucudq.cn

awk '{s += $2} END {print s}' a.txt
来源：http://quv.zhiwuduotai.top

[R51] 排序去重取前几
来源：http://aui.ehwqpu.com

sort a.txt | uniq -c | sort -rn | head
来源：http://ncj.pengpengdd.cyou

[R52] 统计行数
来源：http://wgy.dashuyun.cn

wc -l a.txt
来源：http://esb.jinqigfzy.top

[R53] 查看文件头与实时尾
来源：http://jvs.sjlbkw.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://sor.yvedp.cn

[R54] 比较两个文件
来源：http://dth.hammf.cn

diff a.txt b.txt
来源：http://tbe.jqgufenzy.top

[R55] 压缩与解压
来源：http://gig.meibo888.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://xxy.zycfv.cn

[R56] 远程拷贝
来源：http://hle.nanxinkj.top

scp file user@host:/path/
来源：http://rue.fktsv.cn

[R57] 远程执行命令
来源：http://ntt.cucudq.cn


<!-- 参考信息 -->