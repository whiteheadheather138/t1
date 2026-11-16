代发 wailian999

CREATE INDEX idx_users_email ON users(email);
来源：http://lyw.cdnleiting.top

[Q09] 创建唯一索引
来源：http://obl.hongshengwenyu.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://vlr.fzhhl.top

[Q10] 插入单行
来源：http://fgv.daria6918.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blu.ctjpmb.com

[Q11] 一次插入多行
来源：http://odq.shzxlz.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://vgj.cheryme.top

[Q12] 插入后取自增 ID
来源：http://nzt.hfpthk.cn

INSERT INTO users (name) VALUES ('C');
来源：http://vgk.fanxiaobao.xyz

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://qqy.shanyushiyangtech.top

[Q13] 忽略重复插入
来源：http://rrz.jinqigufen.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://tdq.yuxming.cn

[Q14] 存在则更新（upsert）
来源：http://ake.andypj.xyz

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://kci.daria6918.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://luz.yj20258888.top

[Q15] 查询全部
来源：http://myi.daxiang520.top

SELECT * FROM users;
来源：http://nvv.gogol.net.cn

[Q16] 查询指定列
来源：http://qhc.vehdjk.com

SELECT id, name FROM users;
来源：http://hci.bjfxy.top

[Q17] 条件查询
来源：http://nne.daxiang520.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://qez.jqgfzy.top

[Q18] 模糊匹配
来源：http://zow.yonumen.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://qcz.yfazqb.com

[Q19] 范围查询
来源：http://uvi.aizwys.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://tah.shuidangran.top

[Q20] IN 列表
来源：http://vhm.jyoumei.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://oqu.yvedp.cn

[Q21] 空值判断
来源：http://tuf.meibo888.top

SELECT * FROM users WHERE email IS NULL;
来源：http://isj.yuxming.cn

[Q22] 排序
来源：http://lxq.pengpengdd.cyou

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://fgo.shanyushiyangkeji.top

[Q23] 分页
来源：http://zsr.uphjek.com

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ipy.xziqi.cn

[Q24] 去重
来源：http://tmb.sjlbkw.cn

SELECT DISTINCT city FROM users;
来源：http://rbg.hywenlv.cn

[Q25] 只取前 N 条
来源：http://lvt.yuanzhike.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mlf.fzhhl.top

[Q26] 计数
来源：http://kqc.shanyushiyangtech.top

SELECT COUNT(*) FROM users;
来源：http://rwy.yvedp.cn

[Q27] 条件计数
来源：http://kjg.daria6918.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://bqs.aizwys.cn

[Q28] 求和与平均
来源：http://ary.hcnkem.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://eam.jlsjyb.cn

[Q29] 最大最小值
来源：http://seb.mhx1999.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://gum.gzhubu.top

[Q30] 分组统计
来源：http://qzq.316326.xyz

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://pod.jqgfzy.top

[Q31] 分组后过滤
来源：http://dfd.tianlin.xyz

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://cxd.hesvh.cn

[Q32] 分组拼接字符串
来源：http://wqg.svipenyu.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://fjh.chenzaomai.com

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://fbj.c1oappe.top

[Q33] 多列分组
来源：http://muz.xylfe.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://obl.xuetiantiany.cn

[Q34] 每组取第一条
来源：http://dcp.0kj1m.cn

SELECT * FROM (
来源：http://rjf.yfazqb.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://uke.shangyingyoupin.top

) t WHERE rn = 1;
来源：http://jfv.pengpengdd.cyou

[Q35] 内连接
来源：http://rki.fengsongda.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://vdc.hcnkem.com

[Q36] 左连接
来源：http://rdy.yongpay.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://omd.ybcxt.top

[Q37] 右连接
来源：http://eeo.andypj.xyz

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://nev.nanxinkj.top

[Q38] 全外连接（PostgreSQL）
来源：http://jsf.zhoulong.xyz

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hlm.yj20258888.top

[Q39] 自连接（查上下级）
来源：http://cti.zhengqikj.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://zqq.meibo888.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mmu.hywenlv.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://qwy.meibo888.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ozi.vqdsnc.cn

[Q41] 多表连接
来源：http://tdn.hammf.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://gvo.52xcode.cn

JOIN users u ON u.id = o.user_id
来源：http://eyl.aizwys.cn

JOIN products p ON p.id = o.product_id;
来源：http://xvx.dianchejie.cn

[Q42] 连接条件附加过滤
来源：http://vdf.ydjk.org.cn

SELECT u.name, o.amount FROM users u
来源：http://uxp.cheryme.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://sry.yj20258888.top

[Q43] 标量子查询
来源：http://vqh.fzhhl.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://jgt.fehbvm.com

[Q44] IN 子查询
来源：http://zca.quarkkingdee.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://iuy.9152youxi.cn

[Q45] EXISTS 判断存在
来源：http://qmn.nanxinkj.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hnz.haohaochexian.top

[Q46] NOT EXISTS 判断不存在
来源：http://bys.hnqzz.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://llk.fktsv.cn

[Q47] 与平均值比较
来源：http://okv.ywan-chungtsiang.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://dlr.0kj1m.cn

[Q48] CTE 公用表表达式
来源：http://rdc.chenzaomai.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://npr.vehdjk.com

SELECT * FROM t WHERE c > 5;
来源：http://wzx.ppjwa.cn

[Q49] 更新单行
来源：http://oek.hongshengwenyu.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://kws.haohaochexian.top

[Q50] 批量更新
来源：http://uva.shangyingyoupin.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://sou.fengsongda.top

[Q51] 用子查询更新
来源：http://zbz.nwbrower.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://uox.pengpengdd.cyou

[Q52] 删除指定行
来源：http://pql.mhx1999.top

DELETE FROM users WHERE id = 10;
来源：http://lcx.jlsjyb.cn

[Q53] 按条件删除
来源：http://cca.xziqi.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ews.jqgfzy.top

[Q54] 清空表
来源：http://oqg.snrcjt.cn

TRUNCATE TABLE logs;
来源：http://nly.cqqwz.cn

[Q55] 排名（并列占位）
来源：http://tfe.yuxming.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://pid.fktsv.cn

[Q56] 密集排名（并列不占位）
来源：http://jrz.birdmap.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://pcx.yj20258.top

[Q57] 行号
来源：http://nzn.chenzaomai.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mqp.316326.xyz

[Q58] 累计求和
来源：http://aol.yonumen.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://igp.9152youxi.cn

[Q59] 分组内累计
来源：http://flz.guannengcc.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://szp.gotoacloud.top

[Q60] 取上一行 / 下一行
来源：http://hrn.shzxlz.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://xgq.zhixingplan.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://lym.guowangkeji.top

[Q61] 移动平均
来源：http://axb.iojbl.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://srf.jiagoushi.top

[Q62] 分组占比
来源：http://tll.ydjk.org.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://xxb.hongshengwenyu.top

[Q63] 开启事务
来源：http://bvm.jyoumei.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://dvi.52xcode.cn

[Q64] 提交事务
来源：http://tip.dashuyun.cn

COMMIT;
来源：http://oam.shangyingyoupin.top

[Q65] 回滚事务
来源：http://bom.jqgufenzy.top

ROLLBACK;
来源：http://hml.0kj1m.cn

[Q66] 行锁查询
来源：http://gul.jqgfzy.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://vpo.316326.xyz

[Q67] 设置隔离级别
来源：http://pcv.zhengqikj.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://evd.gogol.net.cn

[Q68] 保存点
来源：http://taw.cheryme.top

SAVEPOINT sp1;
来源：http://hhz.gaohongyu789.top

ROLLBACK TO sp1;
来源：http://lni.andypj.xyz

[Q69] 查看执行计划
来源：http://bxc.yongpay.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://yhb.yuxming.cn

[Q70] 更新统计信息
来源：http://cqp.jyoumei.cn

ANALYZE TABLE users;
来源：http://lgz.haohaochexian.top

[Q71] 查看建表语句
来源：http://aql.kuanghao11.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wbk.yonumen.top

[Q72] 查看索引
来源：http://kuh.ivvv.top

SHOW INDEX FROM users;
来源：http://wpe.yvedp.cn

[Q73] 查看表状态
来源：http://zta.jinqigufen.top

SHOW TABLE STATUS LIKE 'users';
来源：http://qok.fehbvm.com

[Q74] 强制使用索引
来源：http://egx.fktsv.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://qmk.zdqjudy.top

[Q75] 日期格式化
来源：http://mjn.hcnkem.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://pvd.sjlbkw.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://xry.jinqigufen.top

[Q76] 按天统计
来源：http://ihe.guannengcc.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://cum.fktsv.cn

[Q77] 时间加减
来源：http://rfm.ydjk.org.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hso.mhx1999.top

[Q78] 当前时间
来源：http://ukz.jlsjyb.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://dsd.cheryme.top

[Q79] 字符串拼接
来源：http://lmn.chenjidiqi.icu

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://scr.hnxiangtu.top

[Q80] 字符串截取
来源：http://lxq.wangdashe.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://fvo.sysykeji.top

[Q81] 字符串替换
来源：http://vvo.tian-w.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://caj.nanxinkj.top

[Q82] 字符长度与字节长度
来源：http://avr.zdqjudy.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hdz.cucudq.cn

[Q83] 大小写转换
来源：http://opc.feifeiyinyue.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://tki.0kj1m.cn

[Q84] 去除首尾空格
来源：http://qek.havefunace.top

SELECT TRIM(name) FROM users;
来源：http://wqj.sufxvd.cn

[Q85] 数值取整
来源：http://ogu.zhixingplan.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://zoy.jinqigufen.top

[Q86] 读取 JSON 字段
来源：http://qsl.sysykeji.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://lnt.ydzc1.top

[Q87] JSON 字段做条件
来源：http://dka.yueranfly.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wpr.cashguo.top

[Q88] 行转列（条件聚合）
来源：http://xrx.pengpengdd.cyou

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://uwc.aizwys.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://jtx.nanxuanxn.top

[Q89] 判断表是否存在
来源：http://sko.uphjek.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ltu.jinyuanbaomall.cn

[Q90] 生成序号列
来源：http://kpr.quarkkingdee.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://yxh.shuidangran.top

================================================================================
来源：http://ylq.zdqjudy.top

R. Bash 专题
来源：http://kep.hongshengwenyu.top

================================================================================
来源：http://poz.316326.xyz

[R01] shebang 与严格模式
来源：http://omm.iojbl.cn

#!/usr/bin/env bash
来源：http://oov.jinyuanbaomall.cn

set -euo pipefail
来源：http://ejy.aibaodan.cn

[R02] 变量赋值与使用
来源：http://rcy.yuanzhike.top

name="Tom"; echo "$name"
来源：http://hxp.fktsv.cn

[R03] 只读变量
来源：http://znn.zycfv.cn

readonly PI=3.14
来源：http://yhp.aizwys.cn

[R04] 位置参数
来源：http://qhl.sysykeji.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://dvt.fzhhl.top

[R05] 参数默认值
来源：http://fjq.iojbl.cn

name="${1:-default}"
来源：http://cdu.xziqi.cn

[R06] 判断命令是否存在
来源：http://rub.hesvh.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://orf.c1oappe.top

[R07] if 判断文件
来源：http://pbx.dianchejie.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://qfu.wangshuangyany.cn

[R08] 数值比较
来源：http://csf.c1oappe.top

if (( a > b )); then echo "a 更大"; fi
来源：http://hxn.xuetiantiany.cn

[R09] 字符串比较
来源：http://ihs.snrcjt.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://lkz.tarul.cn

[R10] 正则匹配
来源：http://vqt.tarul.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://gzt.yj20258888.top

[R11] case 多分支
来源：http://ule.guannengcc.top

case "$1" in
来源：http://gdz.chenzaomai.com

start) echo "启动" ;;
来源：http://apn.gaohongyu789.top

stop)  echo "停止" ;;
来源：http://lgf.tian-w.cn

*)     echo "未知命令" ;;
来源：http://ugi.nanxuanxn.top

esac
来源：http://umc.hysaishi.cn

[R12] for 遍历文件
来源：http://ydd.hysaishi.cn

for f in *.txt; do echo "$f"; done
来源：http://ggp.316326.xyz

[R13] for 计数循环
来源：http://eik.hammf.cn

for i in {1..10}; do echo "$i"; done
来源：http://whx.quarkkingdee.top

[R14] C 风格 for
来源：http://txn.ywan-chungtsiang.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mlv.xingfuxueyuan.xyz

[R15] while 逐行读文件
来源：http://zgb.yuanzhike.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ezf.0kj1m.cn

[R16] until 等待条件
来源：http://ugr.sufxvd.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://aml.52xcode.cn

[R17] 数组定义与取值
来源：http://ran.shangyingyoupin.top

arr=(a b c); echo "${arr[0]}"
来源：http://hez.wangdashe.top

[R18] 遍历数组
来源：http://wrb.0kj1m.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://zsd.iojbl.cn

[R19] 数组长度
来源：http://kyy.vqdsnc.cn

echo "${#arr[@]}"
来源：http://nik.ydzc1.top

[R20] 关联数组（字典）
来源：http://dzc.pengpengdd.cyou

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://kdp.guannengcc.top

[R21] 字符串长度
来源：http://sjv.wangdashe.top

echo "${#s}"
来源：http://qwv.pycfn.com

[R22] 截取子串
来源：http://abh.andypj.xyz

echo "${s:0:5}"
来源：http://uap.nwbrower.top

[R23] 字符串替换
来源：http://pof.hongshengwenyu.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://eht.andypj.xyz

[R24] 大小写转换
来源：http://huq.hammf.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ukq.zhaomingkeji.xyz

[R25] 去后缀 / 去前缀
来源：http://rfo.cqqwz.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://xht.andypj.xyz

[R26] 命令替换
来源：http://vky.hesvh.cn

now=$(date +%F); echo "$now"
来源：http://wui.yangfankeji.com

[R27] 算术展开
来源：http://frg.pengpengdd.cyou

echo $((1 + 2 * 3))
来源：http://pub.ybcxt.top

[R28] 浮点运算
来源：http://aih.xuanzx.com

echo "scale=2; 10/3" | bc
来源：http://ymv.bbcook.cn

[R29] 定义函数
来源：http://zzm.ctjpmb.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://zdy.pycfn.com

[R30] 函数返回状态码
来源：http://yek.nwbrower.top

f() { return 0; }; f || echo "失败了"
来源：http://iup.chenlongwang.top

[R31] 局部变量
来源：http://oxi.hnqzz.top

f() { local x=1; echo "$x"; }
来源：http://whn.ivvv.top

[R32] 参数个数校验
来源：http://zxb.jinyuanbaomall.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ksv.tian-w.cn

[R33] 捕获错误并提示行号
来源：http://nst.jinghuilouyu.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://dnv.yj202588.top

[R34] 退出时清理
来源：http://kye.cashguo.top

trap 'rm -f "$tmp"' EXIT
来源：http://jze.xuetiantiany.cn

[R35] 后台执行并等待
来源：http://tnc.quarkkingdee.top

sleep 5 & pid=$!; wait "$pid"
来源：http://jir.sxryk.cn

[R36] 并发执行多个任务
来源：http://rpo.jiagoushi.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://cgo.andypj.xyz

[R37] 把输出赋给变量
来源：http://qvr.yj20258.top

files=$(ls -1)
来源：http://vib.yfazqb.com

[R38] 管道串联
来源：http://gez.quarkkingdee.top

cat a.txt | grep -i error | wc -l
来源：http://vsq.daxiang520.top

[R39] 重定向标准输出与错误
来源：http://frz.zhiwuduotai.top

cmd > out.log 2>&1
来源：http://raj.guowangkeji.top

[R40] 追加写日志
来源：http://afo.hesvh.cn

echo "log" >> out.log
来源：http://efd.nanxuanxn.top

[R41] 丢弃输出
来源：http://zkn.bjfxy.top

cmd >/dev/null 2>&1
来源：http://qqx.xuanzx.com

[R42] 输入重定向
来源：http://fcv.gogol.net.cn

wc -l < a.txt
来源：http://pwh.hcnkem.com

[R43] 按名字查找文件
来源：http://rii.mhx1999.top

find . -name "*.log" -type f
来源：http://lkz.yj20258.top

[R44] 按修改时间查找
来源：http://wnj.meibo888.top

find . -mtime -7 -type f
来源：http://yyp.dianchejie.cn

[R45] 批量删除
来源：http://hsg.sxryk.cn

find . -name "*.tmp" -delete
来源：http://uqr.ppjwa.cn

[R46] 递归替换文件内容
来源：http://fyu.sxryk.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://usc.yj202588.top

[R47] sed 单行替换
来源：http://sul.wangdashe.top

sed -i 's/foo/bar/g' a.txt
来源：http://ufj.cucudq.cn

[R48] awk 取指定列
来源：http://oyj.yanxiufei.cn

awk '{print $1, $3}' a.txt
来源：http://lhr.birdmap.top

[R49] awk 带条件
来源：http://wam.iojbl.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://bvk.yongpay.top

[R50] awk 求和
来源：http://jvm.sufxvd.cn

awk '{s += $2} END {print s}' a.txt
来源：http://kmj.yj202588.top

[R51] 排序去重取前几
来源：http://dzs.sysykeji.top

sort a.txt | uniq -c | sort -rn | head
来源：http://jcm.yuxming.cn

[R52] 统计行数
来源：http://hft.zycfv.cn

wc -l a.txt
来源：http://zof.tanke756.top

[R53] 查看文件头与实时尾
来源：http://rlh.cqqwz.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://jjr.aizwys.cn

[R54] 比较两个文件
来源：http://sud.cqqwz.cn

diff a.txt b.txt
来源：http://luv.wangdashe.top

[R55] 压缩与解压
来源：http://wen.yuxming.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://lcg.xylfe.cn

[R56] 远程拷贝
来源：http://qny.tian-w.cn

scp file user@host:/path/
来源：http://muh.ydzc1.top

[R57] 远程执行命令
来源：http://chr.yangfankeji.com


<!-- 参考信息 -->