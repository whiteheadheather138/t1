代发 wailian999

CREATE INDEX idx_users_email ON users(email);
来源：http://bup.vqdsnc.cn

[Q09] 创建唯一索引
来源：http://vsi.nanxinkj.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://plq.shangyingyoupin.top

[Q10] 插入单行
来源：http://ofb.ydjk.org.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://zcj.chenlongwang.top

[Q11] 一次插入多行
来源：http://nnt.cheryme.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://xwi.9152youxi.cn

[Q12] 插入后取自增 ID
来源：http://ksq.0kj1m.cn

INSERT INTO users (name) VALUES ('C');
来源：http://jik.jinqigfzy.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://kyt.ydjk.org.cn

[Q13] 忽略重复插入
来源：http://zvy.0kj1m.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://zfk.tanke756.top

[Q14] 存在则更新（upsert）
来源：http://gdd.gzhubu.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://kwp.tarul.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://lcm.yanxiufei.cn

[Q15] 查询全部
来源：http://tuj.fktsv.cn

SELECT * FROM users;
来源：http://atz.shzxlz.cn

[Q16] 查询指定列
来源：http://knw.ywan-chungtsiang.top

SELECT id, name FROM users;
来源：http://ytu.nanxuanxn.top

[Q17] 条件查询
来源：http://ask.xylfe.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wyk.52xcode.cn

[Q18] 模糊匹配
来源：http://pks.jinqigufen.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ioe.gotoacloud.top

[Q19] 范围查询
来源：http://xkl.hcnkem.com

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://cvm.nanxinkj.top

[Q20] IN 列表
来源：http://pun.c1oappe.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://kdd.shangyingyoupin.top

[Q21] 空值判断
来源：http://zce.jinghuilouyu.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://fdy.jinqigfzy.top

[Q22] 排序
来源：http://ovd.daxiang520.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://efx.yongpay.top

[Q23] 分页
来源：http://sec.shzxlz.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://bxj.9152youxi.cn

[Q24] 去重
来源：http://ymo.cheryme.top

SELECT DISTINCT city FROM users;
来源：http://upf.hammf.cn

[Q25] 只取前 N 条
来源：http://vir.yongpay.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://eta.nanxuanxn.top

[Q26] 计数
来源：http://utb.svipenyu.cn

SELECT COUNT(*) FROM users;
来源：http://ptq.mhx1999.top

[Q27] 条件计数
来源：http://maz.bbcook.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://tqy.mhx1999.top

[Q28] 求和与平均
来源：http://odu.fzhhl.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://dwj.zhixingplan.top

[Q29] 最大最小值
来源：http://lhs.tanke756.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://xzv.jianghu66.top

[Q30] 分组统计
来源：http://tlo.haohaochexian.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://aef.quarkkingdee.top

[Q31] 分组后过滤
来源：http://bro.aibaodan.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://bnl.ctjpmb.com

[Q32] 分组拼接字符串
来源：http://nnn.316326.xyz

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://iub.zycfv.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://khr.tarul.cn

[Q33] 多列分组
来源：http://gjv.yj20258888.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://nvq.nanxuanxn.top

[Q34] 每组取第一条
来源：http://tck.fktsv.cn

SELECT * FROM (
来源：http://huo.cashguo.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://kbz.uphjek.com

) t WHERE rn = 1;
来源：http://qll.xinyue.icu

[Q35] 内连接
来源：http://qsn.tianlin.xyz

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://fag.yuanzhike.top

[Q36] 左连接
来源：http://qln.52xcode.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://iok.gzhubu.top

[Q37] 右连接
来源：http://brx.jqgfzy.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://qtv.jqgufenzy.top

[Q38] 全外连接（PostgreSQL）
来源：http://oun.jlsjyb.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://zae.hnxiangtu.top

[Q39] 自连接（查上下级）
来源：http://nub.zhoulong.xyz

SELECT e.name, m.name AS manager FROM employees e
来源：http://pjr.yuanzhike.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://xoo.9152youxi.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://pan.pengpengdd.cyou

SELECT * FROM colors CROSS JOIN sizes;
来源：http://jif.fktsv.cn

[Q41] 多表连接
来源：http://siq.jqgufenzy.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://kdu.andypj.xyz

JOIN users u ON u.id = o.user_id
来源：http://gmb.epnwcf.com

JOIN products p ON p.id = o.product_id;
来源：http://svt.yj20258.top

[Q42] 连接条件附加过滤
来源：http://lsr.fengsongda.top

SELECT u.name, o.amount FROM users u
来源：http://ssw.yanxiufei.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://bop.pengpengdd.cyou

[Q43] 标量子查询
来源：http://ipf.hnxiangtu.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://uua.xingfuxueyuan.xyz

[Q44] IN 子查询
来源：http://kcy.jinyuanbaomall.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wus.aibaodan.cn

[Q45] EXISTS 判断存在
来源：http://abz.ctjpmb.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mrm.xinyue.icu

[Q46] NOT EXISTS 判断不存在
来源：http://djy.haohaochexian.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fjq.zhaomingkeji.xyz

[Q47] 与平均值比较
来源：http://tdd.fzhhl.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://prh.hfpthk.cn

[Q48] CTE 公用表表达式
来源：http://dyg.chenzaomai.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://yky.hnqzz.top

SELECT * FROM t WHERE c > 5;
来源：http://hzv.smart0.xyz

[Q49] 更新单行
来源：http://xmy.zhijiandao.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://oni.hfpthk.cn

[Q50] 批量更新
来源：http://nre.shanyushiyangkeji.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://boa.chenjidiqi.icu

[Q51] 用子查询更新
来源：http://qsg.nwbrower.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://tjo.cashguo.top

[Q52] 删除指定行
来源：http://bqk.dianchejie.cn

DELETE FROM users WHERE id = 10;
来源：http://lek.snrcjt.cn

[Q53] 按条件删除
来源：http://tia.sufxvd.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://nra.redwolf501.top

[Q54] 清空表
来源：http://xav.zhaomingkeji.xyz

TRUNCATE TABLE logs;
来源：http://jhm.meibo888.top

[Q55] 排名（并列占位）
来源：http://cbc.vehdjk.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://kha.haohaochexian.top

[Q56] 密集排名（并列不占位）
来源：http://unr.pycfn.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wim.sysykeji.top

[Q57] 行号
来源：http://pxi.hongshengwenyu.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://lkp.yanxiufei.cn

[Q58] 累计求和
来源：http://hev.yj20258888.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mue.iojbl.cn

[Q59] 分组内累计
来源：http://ltu.zhongyouzk.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://swr.xinyue.icu

[Q60] 取上一行 / 下一行
来源：http://zyk.tanke756.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://keo.cqqwz.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://pyy.zdbjq.cn

[Q61] 移动平均
来源：http://kvx.fengsongda.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ykz.smart0.xyz

[Q62] 分组占比
来源：http://iaj.yvedp.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://lcd.yuanzhike.top

[Q63] 开启事务
来源：http://vzg.jinqigufen.top

START TRANSACTION;                -- 或 BEGIN
来源：http://ncm.xuanzx.com

[Q64] 提交事务
来源：http://evo.nwbrower.top

COMMIT;
来源：http://zuk.vqdsnc.cn

[Q65] 回滚事务
来源：http://kkk.yfazqb.com

ROLLBACK;
来源：http://crp.redwolf501.top

[Q66] 行锁查询
来源：http://xwh.pycfn.com

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://kvt.zdqjudy.top

[Q67] 设置隔离级别
来源：http://wpm.haohaochexian.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://pxb.xingfuxueyuan.xyz

[Q68] 保存点
来源：http://sqp.kuanghao11.cn

SAVEPOINT sp1;
来源：http://qwc.hysaishi.cn

ROLLBACK TO sp1;
来源：http://zzb.bjfxy.top

[Q69] 查看执行计划
来源：http://mcb.cdnleiting.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://dws.andypj.xyz

[Q70] 更新统计信息
来源：http://cyl.fktsv.cn

ANALYZE TABLE users;
来源：http://lpo.sxryk.cn

[Q71] 查看建表语句
来源：http://kxn.yanxiufei.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://flo.xingfuxueyuan.xyz

[Q72] 查看索引
来源：http://dju.fehbvm.com

SHOW INDEX FROM users;
来源：http://liu.quarkkingdee.top

[Q73] 查看表状态
来源：http://zih.yanxiufei.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://vfd.ybcxt.top

[Q74] 强制使用索引
来源：http://mii.zhongyouzk.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://jrd.birdmap.top

[Q75] 日期格式化
来源：http://zoc.fzhhl.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://twl.ybcxt.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ndq.vqdsnc.cn

[Q76] 按天统计
来源：http://oej.yj202588.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://scj.tianlin.xyz

[Q77] 时间加减
来源：http://naw.fktsv.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://whq.tian-w.cn

[Q78] 当前时间
来源：http://rht.kuanghao11.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://gpp.0kj1m.cn

[Q79] 字符串拼接
来源：http://lrs.c1oappe.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://asr.yongpay.top

[Q80] 字符串截取
来源：http://lju.gaohongyu789.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://anp.zhaomingkeji.xyz

[Q81] 字符串替换
来源：http://erh.sysykeji.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hph.jinqigufen.top

[Q82] 字符长度与字节长度
来源：http://dxt.nwbrower.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://grd.jiagoushi.top

[Q83] 大小写转换
来源：http://xas.jiagoushi.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://fgf.pengpengdd.cyou

[Q84] 去除首尾空格
来源：http://kll.havefunace.top

SELECT TRIM(name) FROM users;
来源：http://nbw.wangdashe.top

[Q85] 数值取整
来源：http://nbt.ehwqpu.com

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://oov.bjfxy.top

[Q86] 读取 JSON 字段
来源：http://hrs.aibaodan.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://dms.tian-w.cn

[Q87] JSON 字段做条件
来源：http://zes.yfazqb.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wwq.yonumen.top

[Q88] 行转列（条件聚合）
来源：http://yer.sufxvd.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ajz.ehwqpu.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ciz.uphjek.com

[Q89] 判断表是否存在
来源：http://bvc.ydzc1.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://rsy.shangyingyoupin.top

[Q90] 生成序号列
来源：http://wuh.jqgfzy.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wwx.shuidangran.top

================================================================================
来源：http://xwu.hywenlv.cn

R. Bash 专题
来源：http://kcq.haohaochexian.top

================================================================================
来源：http://wfj.daxiang520.top

[R01] shebang 与严格模式
来源：http://neg.guowangkeji.top

#!/usr/bin/env bash
来源：http://rlw.sxryk.cn

set -euo pipefail
来源：http://xae.jiagoushi.top

[R02] 变量赋值与使用
来源：http://gca.fktsv.cn

name="Tom"; echo "$name"
来源：http://pdt.gotoacloud.top

[R03] 只读变量
来源：http://pbd.yanxiufei.cn

readonly PI=3.14
来源：http://lso.chenlongwang.top

[R04] 位置参数
来源：http://zve.meibo888.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ujz.guowangkeji.top

[R05] 参数默认值
来源：http://ybe.hesvh.cn

name="${1:-default}"
来源：http://ttz.snrcjt.cn

[R06] 判断命令是否存在
来源：http://wvd.birdmap.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://bek.yuxming.cn

[R07] if 判断文件
来源：http://ing.jinqigufen.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://cvc.gaohongyu789.top

[R08] 数值比较
来源：http://iah.shanyushiyangtech.top

if (( a > b )); then echo "a 更大"; fi
来源：http://tua.aibaodan.cn

[R09] 字符串比较
来源：http://aih.chenlongwang.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://kpk.fanxiaobao.xyz

[R10] 正则匹配
来源：http://rji.epnwcf.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://irs.jinghuilouyu.cn

[R11] case 多分支
来源：http://atn.feifeiyinyue.top

case "$1" in
来源：http://ykk.ctjpmb.com

start) echo "启动" ;;
来源：http://dlt.ivvv.top

stop)  echo "停止" ;;
来源：http://dbj.smart0.xyz

*)     echo "未知命令" ;;
来源：http://uly.mhx1999.top

esac
来源：http://uto.hongshengwenyu.top

[R12] for 遍历文件
来源：http://ulk.iojbl.cn

for f in *.txt; do echo "$f"; done
来源：http://qjb.cdnleiting.top

[R13] for 计数循环
来源：http://nuy.yj20258.top

for i in {1..10}; do echo "$i"; done
来源：http://uty.ppjwa.cn

[R14] C 风格 for
来源：http://jop.vehdjk.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://bfv.cashguo.top

[R15] while 逐行读文件
来源：http://wqr.yj20258.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mea.ivvv.top

[R16] until 等待条件
来源：http://ljz.zhijiandao.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://cwb.fehbvm.com

[R17] 数组定义与取值
来源：http://gcj.chenjidiqi.icu

arr=(a b c); echo "${arr[0]}"
来源：http://fbn.jlsjyb.cn

[R18] 遍历数组
来源：http://egk.tarul.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ueb.daria6918.cn

[R19] 数组长度
来源：http://kxh.yongpay.top

echo "${#arr[@]}"
来源：http://fps.gogol.net.cn

[R20] 关联数组（字典）
来源：http://ypi.zhengqikj.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://meq.pycfn.com

[R21] 字符串长度
来源：http://kru.sjlbkw.cn

echo "${#s}"
来源：http://vwa.hysaishi.cn

[R22] 截取子串
来源：http://eau.havefunace.top

echo "${s:0:5}"
来源：http://lgd.jiagoushi.top

[R23] 字符串替换
来源：http://ylw.xuetiantiany.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://oaw.cqqwz.cn

[R24] 大小写转换
来源：http://wrc.bbcook.cn

echo "${s^^}"; echo "${s,,}"
来源：http://wey.shanyushiyangtech.top

[R25] 去后缀 / 去前缀
来源：http://jej.xylfe.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://lco.fanxiaobao.xyz

[R26] 命令替换
来源：http://alk.bbcook.cn

now=$(date +%F); echo "$now"
来源：http://vit.jianghu66.top

[R27] 算术展开
来源：http://zyt.iojbl.cn

echo $((1 + 2 * 3))
来源：http://amg.hesvh.cn

[R28] 浮点运算
来源：http://jon.yanxiufei.cn

echo "scale=2; 10/3" | bc
来源：http://bca.tian-w.cn

[R29] 定义函数
来源：http://aza.birdmap.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ofw.guowangkeji.top

[R30] 函数返回状态码
来源：http://egr.vqdsnc.cn

f() { return 0; }; f || echo "失败了"
来源：http://cdu.uphjek.com

[R31] 局部变量
来源：http://knd.fzhhl.top

f() { local x=1; echo "$x"; }
来源：http://qwa.guowangkeji.top

[R32] 参数个数校验
来源：http://bgk.redwolf501.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://prw.sxryk.cn

[R33] 捕获错误并提示行号
来源：http://wrr.zhiwuduotai.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://srs.jinqigufen.top

[R34] 退出时清理
来源：http://sbu.fengsongda.top

trap 'rm -f "$tmp"' EXIT
来源：http://bda.zycfv.cn

[R35] 后台执行并等待
来源：http://ixj.cashguo.top

sleep 5 & pid=$!; wait "$pid"
来源：http://ypl.sweek.top

[R36] 并发执行多个任务
来源：http://hve.hongshengwenyu.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://dgc.vqdsnc.cn

[R37] 把输出赋给变量
来源：http://kiy.vehdjk.com

files=$(ls -1)
来源：http://idp.aizwys.cn

[R38] 管道串联
来源：http://otd.zycfv.cn

cat a.txt | grep -i error | wc -l
来源：http://hsx.yangfankeji.com

[R39] 重定向标准输出与错误
来源：http://zbi.bbcook.cn

cmd > out.log 2>&1
来源：http://gww.jinghuilouyu.cn

[R40] 追加写日志
来源：http://uog.ybcxt.top

echo "log" >> out.log
来源：http://ssh.hcnkem.com

[R41] 丢弃输出
来源：http://yft.cucudq.cn

cmd >/dev/null 2>&1
来源：http://hbu.dashuyun.cn

[R42] 输入重定向
来源：http://stt.jinqigufen.top

wc -l < a.txt
来源：http://mrl.cqqwz.cn

[R43] 按名字查找文件
来源：http://uie.jqgufenzy.top

find . -name "*.log" -type f
来源：http://xyh.sufxvd.cn

[R44] 按修改时间查找
来源：http://gsh.wangdashe.top

find . -mtime -7 -type f
来源：http://pyk.hfpthk.cn

[R45] 批量删除
来源：http://odo.zdbjq.cn

find . -name "*.tmp" -delete
来源：http://zqa.epnwcf.com

[R46] 递归替换文件内容
来源：http://pxp.cheryme.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hce.fehbvm.com

[R47] sed 单行替换
来源：http://asd.jyoumei.cn

sed -i 's/foo/bar/g' a.txt
来源：http://wyq.aibaodan.cn

[R48] awk 取指定列
来源：http://egu.zhiwuduotai.top

awk '{print $1, $3}' a.txt
来源：http://uee.zdbjq.cn

[R49] awk 带条件
来源：http://vcn.zhijiandao.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://eem.ctjpmb.com

[R50] awk 求和
来源：http://nxm.ybcxt.top

awk '{s += $2} END {print s}' a.txt
来源：http://wkj.shanyushiyangtech.top

[R51] 排序去重取前几
来源：http://bxg.andypj.xyz

sort a.txt | uniq -c | sort -rn | head
来源：http://xvo.shanyushiyangtech.top

[R52] 统计行数
来源：http://ser.snrcjt.cn

wc -l a.txt
来源：http://eft.havefunace.top

[R53] 查看文件头与实时尾
来源：http://bqw.hnqzz.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wpr.yangfankeji.com

[R54] 比较两个文件
来源：http://fre.meibo888.top

diff a.txt b.txt
来源：http://loi.hnxiangtu.top

[R55] 压缩与解压
来源：http://ofr.ydzc1.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://maw.mhx1999.top

[R56] 远程拷贝
来源：http://wul.yueranfly.top

scp file user@host:/path/
来源：http://gzj.ehwqpu.com

[R57] 远程执行命令
来源：http://udq.yj20258888.top


<!-- 参考信息 -->