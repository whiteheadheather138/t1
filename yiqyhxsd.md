代发 wailian999

ALTER TABLE users DROP COLUMN age;
来源：http://qsn.zycfv.cn

[Q07] 删除表
来源：http://oir.yanxiufei.cn

DROP TABLE IF EXISTS orders;
来源：http://itw.epnwcf.com

[Q08] 创建普通索引
来源：http://sfe.yanxiufei.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://dfk.hfpthk.cn

[Q09] 创建唯一索引
来源：http://swk.havefunace.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mcb.cqqwz.cn

[Q10] 插入单行
来源：http://fbg.fktsv.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ztv.epnwcf.com

[Q11] 一次插入多行
来源：http://ltn.daria6918.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://lbi.snrcjt.cn

[Q12] 插入后取自增 ID
来源：http://jhz.cdnleiting.top

INSERT INTO users (name) VALUES ('C');
来源：http://vej.yueranfly.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://qph.wangdashe.top

[Q13] 忽略重复插入
来源：http://gqm.xylfe.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://tob.epnwcf.com

[Q14] 存在则更新（upsert）
来源：http://hci.zhiwuduotai.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wpo.uphjek.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://klg.aizwys.cn

[Q15] 查询全部
来源：http://vhn.daria6918.cn

SELECT * FROM users;
来源：http://jtd.chenzaomai.com

[Q16] 查询指定列
来源：http://npk.jqgufenzy.top

SELECT id, name FROM users;
来源：http://ofx.hnxiangtu.top

[Q17] 条件查询
来源：http://egm.xinyue.icu

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://rsk.meibo888.top

[Q18] 模糊匹配
来源：http://mbk.meibo888.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://flg.tianlin.xyz

[Q19] 范围查询
来源：http://mvw.bbcook.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wdo.fktsv.cn

[Q20] IN 列表
来源：http://hjv.daxiang520.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://fxj.pycfn.com

[Q21] 空值判断
来源：http://zqi.hesvh.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://var.zhoulong.xyz

[Q22] 排序
来源：http://mfk.fengsongda.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://qfz.0kj1m.cn

[Q23] 分页
来源：http://rqt.jinghuilouyu.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://fwr.vqdsnc.cn

[Q24] 去重
来源：http://gow.tianlin.xyz

SELECT DISTINCT city FROM users;
来源：http://hyy.fengsongda.top

[Q25] 只取前 N 条
来源：http://kkt.316326.xyz

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://usf.ybcxt.top

[Q26] 计数
来源：http://wor.xuetiantiany.cn

SELECT COUNT(*) FROM users;
来源：http://qnq.bbcook.cn

[Q27] 条件计数
来源：http://lhy.hywenlv.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://fyr.yuxming.cn

[Q28] 求和与平均
来源：http://yuz.ywan-chungtsiang.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://xkx.sweek.top

[Q29] 最大最小值
来源：http://lwm.tanke756.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://nhi.hnxiangtu.top

[Q30] 分组统计
来源：http://azb.chenjidiqi.icu

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://gxw.uphjek.com

[Q31] 分组后过滤
来源：http://mkh.yj20258888.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://jfr.meibo888.top

[Q32] 分组拼接字符串
来源：http://ycd.hysaishi.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://tib.haohaochexian.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://bzi.zdqjudy.top

[Q33] 多列分组
来源：http://zqx.zdqjudy.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://xwk.daria6918.cn

[Q34] 每组取第一条
来源：http://mlg.c1oappe.top

SELECT * FROM (
来源：http://gma.zhongyouzk.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://jiv.jinyuanbaomall.cn

) t WHERE rn = 1;
来源：http://pzm.yj202588.top

[Q35] 内连接
来源：http://tye.nanxinkj.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://qyw.tianlin.xyz

[Q36] 左连接
来源：http://zrx.yongpay.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://bgk.xziqi.cn

[Q37] 右连接
来源：http://viw.pengpengdd.cyou

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://sdm.zdqjudy.top

[Q38] 全外连接（PostgreSQL）
来源：http://vwp.sufxvd.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ecw.ivvv.top

[Q39] 自连接（查上下级）
来源：http://wph.jinqigfzy.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://iuv.yfazqb.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ydl.xinyue.icu

[Q40] 交叉连接（笛卡尔积）
来源：http://uus.jqgfzy.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://pqx.sweek.top

[Q41] 多表连接
来源：http://occ.hysaishi.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://tcv.uphjek.com

JOIN users u ON u.id = o.user_id
来源：http://drz.wangdashe.top

JOIN products p ON p.id = o.product_id;
来源：http://blr.sufxvd.cn

[Q42] 连接条件附加过滤
来源：http://euw.chenlongwang.top

SELECT u.name, o.amount FROM users u
来源：http://kgc.feifeiyinyue.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ecx.wangshuangyany.cn

[Q43] 标量子查询
来源：http://yij.andypj.xyz

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hoi.jinyuanbaomall.cn

[Q44] IN 子查询
来源：http://ivp.gaohongyu789.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ril.jinqigfzy.top

[Q45] EXISTS 判断存在
来源：http://pmv.smart0.xyz

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rgz.yvedp.cn

[Q46] NOT EXISTS 判断不存在
来源：http://jlo.shangyingyoupin.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://cvk.yvedp.cn

[Q47] 与平均值比较
来源：http://cmf.feifeiyinyue.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://esp.hesvh.cn

[Q48] CTE 公用表表达式
来源：http://zeo.yj20258888.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://vbd.vqdsnc.cn

SELECT * FROM t WHERE c > 5;
来源：http://ebc.yj202588.top

[Q49] 更新单行
来源：http://udt.shanyushiyangtech.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://xwn.fengsongda.top

[Q50] 批量更新
来源：http://cry.chenlongwang.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://vgh.shanyushiyangkeji.top

[Q51] 用子查询更新
来源：http://etq.fehbvm.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://iiw.zhoulong.xyz

[Q52] 删除指定行
来源：http://ivo.hnqzz.top

DELETE FROM users WHERE id = 10;
来源：http://brz.sufxvd.cn

[Q53] 按条件删除
来源：http://fjy.andypj.xyz

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hgn.yongpay.top

[Q54] 清空表
来源：http://jpd.0kj1m.cn

TRUNCATE TABLE logs;
来源：http://soc.sysykeji.top

[Q55] 排名（并列占位）
来源：http://isw.uphjek.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://gao.zycfv.cn

[Q56] 密集排名（并列不占位）
来源：http://hrb.smart0.xyz

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://jjy.dashuyun.cn

[Q57] 行号
来源：http://phw.fzhhl.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://bmf.gogol.net.cn

[Q58] 累计求和
来源：http://tae.fktsv.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://jaf.ppjwa.cn

[Q59] 分组内累计
来源：http://gyy.aibaodan.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://obi.shuidangran.top

[Q60] 取上一行 / 下一行
来源：http://zwn.52xcode.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://crw.hfpthk.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://tkf.fengsongda.top

[Q61] 移动平均
来源：http://hso.ivvv.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://sxa.cashguo.top

[Q62] 分组占比
来源：http://mrk.ybcxt.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://nfp.andypj.xyz

[Q63] 开启事务
来源：http://wmt.gzhubu.top

START TRANSACTION;                -- 或 BEGIN
来源：http://goi.nwbrower.top

[Q64] 提交事务
来源：http://dur.yvedp.cn

COMMIT;
来源：http://uai.pycfn.com

[Q65] 回滚事务
来源：http://mxi.ctjpmb.com

ROLLBACK;
来源：http://bhm.redwolf501.top

[Q66] 行锁查询
来源：http://xfk.hesvh.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://roo.zdqjudy.top

[Q67] 设置隔离级别
来源：http://key.nanxuanxn.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://fvb.fanxiaobao.xyz

[Q68] 保存点
来源：http://bzn.chenlongwang.top

SAVEPOINT sp1;
来源：http://jth.sxryk.cn

ROLLBACK TO sp1;
来源：http://gpn.jlsjyb.cn

[Q69] 查看执行计划
来源：http://oeq.wangdashe.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://qci.guowangkeji.top

[Q70] 更新统计信息
来源：http://djh.zhaomingkeji.xyz

ANALYZE TABLE users;
来源：http://som.yanxiufei.cn

[Q71] 查看建表语句
来源：http://tnu.zhiwuduotai.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ulq.jinghuilouyu.cn

[Q72] 查看索引
来源：http://ajr.jiagoushi.top

SHOW INDEX FROM users;
来源：http://tne.redwolf501.top

[Q73] 查看表状态
来源：http://lck.xinyue.icu

SHOW TABLE STATUS LIKE 'users';
来源：http://wlf.zdbjq.cn

[Q74] 强制使用索引
来源：http://dov.yj20258888.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://amo.vqdsnc.cn

[Q75] 日期格式化
来源：http://cex.epnwcf.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://imq.jinghuilouyu.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://exz.guowangkeji.top

[Q76] 按天统计
来源：http://gcy.redwolf501.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://xyj.yj202588.top

[Q77] 时间加减
来源：http://jgz.tian-w.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://vcy.kuanghao11.cn

[Q78] 当前时间
来源：http://rkh.jiagoushi.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://dbw.epnwcf.com

[Q79] 字符串拼接
来源：http://sxq.vqdsnc.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://uoa.cheryme.top

[Q80] 字符串截取
来源：http://uqa.yangfankeji.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://iil.xinyue.icu

[Q81] 字符串替换
来源：http://nvc.ybcxt.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://qpx.zhengqikj.top

[Q82] 字符长度与字节长度
来源：http://bpq.zdbjq.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://thu.tian-w.cn

[Q83] 大小写转换
来源：http://zmx.tarul.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://xqc.yuxming.cn

[Q84] 去除首尾空格
来源：http://ykt.aizwys.cn

SELECT TRIM(name) FROM users;
来源：http://xyy.daria6918.cn

[Q85] 数值取整
来源：http://klt.hfpthk.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ogy.ehwqpu.com

[Q86] 读取 JSON 字段
来源：http://aws.smart0.xyz

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://gfj.shzxlz.cn

[Q87] JSON 字段做条件
来源：http://miz.birdmap.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://jdl.aibaodan.cn

[Q88] 行转列（条件聚合）
来源：http://vfs.hammf.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://fev.cheryme.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://raw.jqgufenzy.top

[Q89] 判断表是否存在
来源：http://xxa.52xcode.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://sjw.wangdashe.top

[Q90] 生成序号列
来源：http://pqs.hesvh.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://nng.sufxvd.cn

================================================================================
来源：http://ezy.aizwys.cn

R. Bash 专题
来源：http://dxl.jinqigfzy.top

================================================================================
来源：http://dpb.redwolf501.top

[R01] shebang 与严格模式
来源：http://nek.pengpengdd.cyou

#!/usr/bin/env bash
来源：http://qfw.guowangkeji.top

set -euo pipefail
来源：http://ogi.tian-w.cn

[R02] 变量赋值与使用
来源：http://fdv.chenjidiqi.icu

name="Tom"; echo "$name"
来源：http://hhl.haohaochexian.top

[R03] 只读变量
来源：http://lyk.xinyue.icu

readonly PI=3.14
来源：http://lqf.hnqzz.top

[R04] 位置参数
来源：http://pbp.dianchejie.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://isd.pycfn.com

[R05] 参数默认值
来源：http://ztg.snrcjt.cn

name="${1:-default}"
来源：http://lcd.snrcjt.cn

[R06] 判断命令是否存在
来源：http://oqn.chenzaomai.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://nth.snrcjt.cn

[R07] if 判断文件
来源：http://whz.gogol.net.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://lln.aibaodan.cn

[R08] 数值比较
来源：http://qjc.sufxvd.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ybl.hywenlv.cn

[R09] 字符串比较
来源：http://vsa.zhoulong.xyz

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://xhj.tianlin.xyz

[R10] 正则匹配
来源：http://iir.chenjidiqi.icu

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://rhz.dianchejie.cn

[R11] case 多分支
来源：http://gmh.cdnleiting.top

case "$1" in
来源：http://yws.jinqigufen.top

start) echo "启动" ;;
来源：http://jbu.daria6918.cn

stop)  echo "停止" ;;
来源：http://mhk.chenjidiqi.icu

*)     echo "未知命令" ;;
来源：http://tqz.zhongyouzk.top

esac
来源：http://wvv.snrcjt.cn

[R12] for 遍历文件
来源：http://ixa.yj202588.top

for f in *.txt; do echo "$f"; done
来源：http://sxd.cheryme.top

[R13] for 计数循环
来源：http://nzz.hnqzz.top

for i in {1..10}; do echo "$i"; done
来源：http://isg.zdqjudy.top

[R14] C 风格 for
来源：http://sxy.sysykeji.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://kgd.jqgufenzy.top

[R15] while 逐行读文件
来源：http://gth.sweek.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://utq.xuetiantiany.cn

[R16] until 等待条件
来源：http://ksx.xuanzx.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://lti.vehdjk.com

[R17] 数组定义与取值
来源：http://kgg.xylfe.cn

arr=(a b c); echo "${arr[0]}"
来源：http://jnz.hongshengwenyu.top

[R18] 遍历数组
来源：http://wqp.mhx1999.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hpf.shuidangran.top

[R19] 数组长度
来源：http://yav.meibo888.top

echo "${#arr[@]}"
来源：http://jyq.jianghu66.top

[R20] 关联数组（字典）
来源：http://rcx.daxiang520.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://vpo.vqdsnc.cn

[R21] 字符串长度
来源：http://rmx.mhx1999.top

echo "${#s}"
来源：http://wmg.ivvv.top

[R22] 截取子串
来源：http://tjs.cheryme.top

echo "${s:0:5}"
来源：http://fsx.jinyuanbaomall.cn

[R23] 字符串替换
来源：http://gne.snrcjt.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://btn.nanxuanxn.top

[R24] 大小写转换
来源：http://hmp.gogol.net.cn

echo "${s^^}"; echo "${s,,}"
来源：http://doi.hysaishi.cn

[R25] 去后缀 / 去前缀
来源：http://oam.ydzc1.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://mbk.chenlongwang.top

[R26] 命令替换
来源：http://psk.xinyue.icu

now=$(date +%F); echo "$now"
来源：http://ndt.yuanzhike.top

[R27] 算术展开
来源：http://sdt.tianlin.xyz

echo $((1 + 2 * 3))
来源：http://glx.yanxiufei.cn

[R28] 浮点运算
来源：http://kyf.fktsv.cn

echo "scale=2; 10/3" | bc
来源：http://vaw.mhx1999.top

[R29] 定义函数
来源：http://amc.c1oappe.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mun.svipenyu.cn

[R30] 函数返回状态码
来源：http://dcb.smart0.xyz

f() { return 0; }; f || echo "失败了"
来源：http://cvb.yfazqb.com

[R31] 局部变量
来源：http://nxt.dianchejie.cn

f() { local x=1; echo "$x"; }
来源：http://zgm.chenlongwang.top

[R32] 参数个数校验
来源：http://orh.yanxiufei.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://eze.xingfuxueyuan.xyz

[R33] 捕获错误并提示行号
来源：http://wmo.yueranfly.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://zbm.0kj1m.cn

[R34] 退出时清理
来源：http://cvq.yj20258888.top

trap 'rm -f "$tmp"' EXIT
来源：http://qmj.jinyuanbaomall.cn

[R35] 后台执行并等待
来源：http://sen.fzhhl.top

sleep 5 & pid=$!; wait "$pid"
来源：http://moo.ybcxt.top

[R36] 并发执行多个任务
来源：http://jwd.jqgfzy.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ogo.ppjwa.cn

[R37] 把输出赋给变量
来源：http://eig.cashguo.top

files=$(ls -1)
来源：http://isv.vehdjk.com

[R38] 管道串联
来源：http://zfo.cqqwz.cn

cat a.txt | grep -i error | wc -l
来源：http://fbf.quarkkingdee.top

[R39] 重定向标准输出与错误
来源：http://rpf.fanxiaobao.xyz

cmd > out.log 2>&1
来源：http://kch.ydzc1.top

[R40] 追加写日志
来源：http://lps.yonumen.top

echo "log" >> out.log
来源：http://gbt.yvedp.cn

[R41] 丢弃输出
来源：http://cne.xuetiantiany.cn

cmd >/dev/null 2>&1
来源：http://evw.yuanzhike.top

[R42] 输入重定向
来源：http://hea.yfazqb.com

wc -l < a.txt
来源：http://uoy.mhx1999.top

[R43] 按名字查找文件
来源：http://rgk.zhoulong.xyz

find . -name "*.log" -type f
来源：http://pbk.feifeiyinyue.top

[R44] 按修改时间查找
来源：http://ift.jqgufenzy.top

find . -mtime -7 -type f
来源：http://mxt.wangdashe.top

[R45] 批量删除
来源：http://uxu.jyoumei.cn

find . -name "*.tmp" -delete
来源：http://wvw.zdbjq.cn

[R46] 递归替换文件内容
来源：http://hqv.zycfv.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://rbb.dianchejie.cn

[R47] sed 单行替换
来源：http://kml.cashguo.top

sed -i 's/foo/bar/g' a.txt
来源：http://lxn.ivvv.top

[R48] awk 取指定列
来源：http://ucr.ydjk.org.cn

awk '{print $1, $3}' a.txt
来源：http://yoq.shuidangran.top

[R49] awk 带条件
来源：http://ryw.gogol.net.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://tmb.yongpay.top

[R50] awk 求和
来源：http://hvt.fktsv.cn

awk '{s += $2} END {print s}' a.txt
来源：http://tsd.hnqzz.top

[R51] 排序去重取前几
来源：http://lmd.zhixingplan.top

sort a.txt | uniq -c | sort -rn | head
来源：http://ooy.birdmap.top

[R52] 统计行数
来源：http://rke.smart0.xyz

wc -l a.txt
来源：http://vre.ivvv.top

[R53] 查看文件头与实时尾
来源：http://uxs.yfazqb.com

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://amm.jqgfzy.top

[R54] 比较两个文件
来源：http://thh.chenzaomai.com

diff a.txt b.txt
来源：http://efm.gotoacloud.top

[R55] 压缩与解压
来源：http://zji.jinghuilouyu.cn


<!-- 参考信息 -->