代发 wailian999

CREATE INDEX idx_users_email ON users(email);
来源：http://rxe.epnwcf.com

[Q09] 创建唯一索引
来源：http://vkf.chenjidiqi.icu

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://dms.yj202588.top

[Q10] 插入单行
来源：http://owu.shanyushiyangkeji.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mvu.vehdjk.com

[Q11] 一次插入多行
来源：http://dmq.xingfuxueyuan.xyz

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://sfw.yueranfly.top

[Q12] 插入后取自增 ID
来源：http://pgk.chenzaomai.com

INSERT INTO users (name) VALUES ('C');
来源：http://yoz.tarul.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://rhf.hesvh.cn

[Q13] 忽略重复插入
来源：http://dkj.tarul.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://jxl.ctjpmb.com

[Q14] 存在则更新（upsert）
来源：http://iwe.aibaodan.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://cad.redwolf501.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://azl.tarul.cn

[Q15] 查询全部
来源：http://tff.jinghuilouyu.cn

SELECT * FROM users;
来源：http://zej.shuidangran.top

[Q16] 查询指定列
来源：http://ovh.zhiwuduotai.top

SELECT id, name FROM users;
来源：http://bde.zdqjudy.top

[Q17] 条件查询
来源：http://fcg.feifeiyinyue.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://cvw.daxiang520.top

[Q18] 模糊匹配
来源：http://bpe.sxryk.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://vba.tian-w.cn

[Q19] 范围查询
来源：http://xvq.zdbjq.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://cen.bbcook.cn

[Q20] IN 列表
来源：http://bmu.daxiang520.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://jjg.zhongyouzk.top

[Q21] 空值判断
来源：http://aik.chenzaomai.com

SELECT * FROM users WHERE email IS NULL;
来源：http://cis.zhongyouzk.top

[Q22] 排序
来源：http://paz.9152youxi.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://uaj.hammf.cn

[Q23] 分页
来源：http://ota.yuxming.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://dyu.hesvh.cn

[Q24] 去重
来源：http://ava.ydjk.org.cn

SELECT DISTINCT city FROM users;
来源：http://bbm.cucudq.cn

[Q25] 只取前 N 条
来源：http://jzp.gotoacloud.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://kjo.hysaishi.cn

[Q26] 计数
来源：http://swr.shzxlz.cn

SELECT COUNT(*) FROM users;
来源：http://xbz.quarkkingdee.top

[Q27] 条件计数
来源：http://hhf.yueranfly.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://jqn.zhengqikj.top

[Q28] 求和与平均
来源：http://ysq.birdmap.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://nwk.shanyushiyangkeji.top

[Q29] 最大最小值
来源：http://lzv.chenlongwang.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://jzp.fehbvm.com

[Q30] 分组统计
来源：http://brk.jyoumei.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hwq.gotoacloud.top

[Q31] 分组后过滤
来源：http://xxh.shangyingyoupin.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://rco.ydzc1.top

[Q32] 分组拼接字符串
来源：http://bqr.havefunace.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mcp.52xcode.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://jng.shanyushiyangtech.top

[Q33] 多列分组
来源：http://igh.yanxiufei.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ktp.cqqwz.cn

[Q34] 每组取第一条
来源：http://sam.yonumen.top

SELECT * FROM (
来源：http://oli.mhx1999.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hes.jqgufenzy.top

) t WHERE rn = 1;
来源：http://axz.nanxuanxn.top

[Q35] 内连接
来源：http://eku.chenlongwang.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://rtm.cashguo.top

[Q36] 左连接
来源：http://sep.aibaodan.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://bva.shangyingyoupin.top

[Q37] 右连接
来源：http://ylu.shzxlz.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://htp.zdqjudy.top

[Q38] 全外连接（PostgreSQL）
来源：http://vuv.316326.xyz

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://cdo.ivvv.top

[Q39] 自连接（查上下级）
来源：http://pbe.jlsjyb.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ghj.ywan-chungtsiang.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mki.hysaishi.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://lsm.ydjk.org.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://luj.c1oappe.top

[Q41] 多表连接
来源：http://qvx.meibo888.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://qts.haohaochexian.top

JOIN users u ON u.id = o.user_id
来源：http://mva.hesvh.cn

JOIN products p ON p.id = o.product_id;
来源：http://jpk.zhongyouzk.top

[Q42] 连接条件附加过滤
来源：http://ppd.hesvh.cn

SELECT u.name, o.amount FROM users u
来源：http://dwz.jiagoushi.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://jrl.jiagoushi.top

[Q43] 标量子查询
来源：http://ofs.shangyingyoupin.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://dxa.fehbvm.com

[Q44] IN 子查询
来源：http://ydk.zhijiandao.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://jxp.316326.xyz

[Q45] EXISTS 判断存在
来源：http://kjk.yfazqb.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://csl.aibaodan.cn

[Q46] NOT EXISTS 判断不存在
来源：http://lmd.hesvh.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kkh.nanxinkj.top

[Q47] 与平均值比较
来源：http://wrq.jinqigufen.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://tzn.snrcjt.cn

[Q48] CTE 公用表表达式
来源：http://qmh.zhijiandao.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://vny.vqdsnc.cn

SELECT * FROM t WHERE c > 5;
来源：http://wwt.vqdsnc.cn

[Q49] 更新单行
来源：http://duk.xziqi.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://zlv.yvedp.cn

[Q50] 批量更新
来源：http://ssi.xinyue.icu

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://zix.pengpengdd.cyou

[Q51] 用子查询更新
来源：http://zeq.tanke756.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://udx.yj20258888.top

[Q52] 删除指定行
来源：http://qkn.fanxiaobao.xyz

DELETE FROM users WHERE id = 10;
来源：http://bxs.iojbl.cn

[Q53] 按条件删除
来源：http://xkz.gotoacloud.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://onq.guannengcc.top

[Q54] 清空表
来源：http://ago.kuanghao11.cn

TRUNCATE TABLE logs;
来源：http://gjn.jinqigfzy.top

[Q55] 排名（并列占位）
来源：http://dly.c1oappe.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://btn.nanxinkj.top

[Q56] 密集排名（并列不占位）
来源：http://ixh.tianlin.xyz

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://cht.0kj1m.cn

[Q57] 行号
来源：http://fbv.shzxlz.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://bkd.jianghu66.top

[Q58] 累计求和
来源：http://aal.meibo888.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://fqg.vqdsnc.cn

[Q59] 分组内累计
来源：http://xdk.shanyushiyangtech.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ysa.jianghu66.top

[Q60] 取上一行 / 下一行
来源：http://kmd.cheryme.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://jcr.uphjek.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://zrg.zhaomingkeji.xyz

[Q61] 移动平均
来源：http://knv.fehbvm.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://elg.chenjidiqi.icu

[Q62] 分组占比
来源：http://fsx.nwbrower.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://fap.xinyue.icu

[Q63] 开启事务
来源：http://ker.fengsongda.top

START TRANSACTION;                -- 或 BEGIN
来源：http://jyk.yueranfly.top

[Q64] 提交事务
来源：http://tep.xylfe.cn

COMMIT;
来源：http://wku.wangdashe.top

[Q65] 回滚事务
来源：http://bax.snrcjt.cn

ROLLBACK;
来源：http://yfq.epnwcf.com

[Q66] 行锁查询
来源：http://cqw.fengsongda.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://sbw.vehdjk.com

[Q67] 设置隔离级别
来源：http://oyu.jinghuilouyu.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://lsn.zhengqikj.top

[Q68] 保存点
来源：http://iip.0kj1m.cn

SAVEPOINT sp1;
来源：http://qnf.tianlin.xyz

ROLLBACK TO sp1;
来源：http://rsg.yuxming.cn

[Q69] 查看执行计划
来源：http://mgu.dianchejie.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://zgm.jianghu66.top

[Q70] 更新统计信息
来源：http://zwm.fehbvm.com

ANALYZE TABLE users;
来源：http://qki.gzhubu.top

[Q71] 查看建表语句
来源：http://qcc.zdqjudy.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://rjt.316326.xyz

[Q72] 查看索引
来源：http://wrc.daxiang520.top

SHOW INDEX FROM users;
来源：http://sqk.yj202588.top

[Q73] 查看表状态
来源：http://cps.zhaomingkeji.xyz

SHOW TABLE STATUS LIKE 'users';
来源：http://dbo.daxiang520.top

[Q74] 强制使用索引
来源：http://jrz.hywenlv.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://tvp.ctjpmb.com

[Q75] 日期格式化
来源：http://jai.zhengqikj.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://tig.cheryme.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ats.hywenlv.cn

[Q76] 按天统计
来源：http://mnr.ehwqpu.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hbz.iojbl.cn

[Q77] 时间加减
来源：http://pwo.ppjwa.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://qve.feifeiyinyue.top

[Q78] 当前时间
来源：http://myd.redwolf501.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wtp.sysykeji.top

[Q79] 字符串拼接
来源：http://dlf.cucudq.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://nlo.vqdsnc.cn

[Q80] 字符串截取
来源：http://iyx.yj20258888.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://nuh.hesvh.cn

[Q81] 字符串替换
来源：http://sql.daria6918.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wzn.jinyuanbaomall.cn

[Q82] 字符长度与字节长度
来源：http://lcn.zhengqikj.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ajt.shanyushiyangtech.top

[Q83] 大小写转换
来源：http://afu.hywenlv.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://zaq.yanxiufei.cn

[Q84] 去除首尾空格
来源：http://vog.jyoumei.cn

SELECT TRIM(name) FROM users;
来源：http://cop.cheryme.top

[Q85] 数值取整
来源：http://wob.jqgufenzy.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://eop.quarkkingdee.top

[Q86] 读取 JSON 字段
来源：http://jvl.ivvv.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://usu.shangyingyoupin.top

[Q87] JSON 字段做条件
来源：http://owb.cucudq.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://qip.gogol.net.cn

[Q88] 行转列（条件聚合）
来源：http://vob.zhengqikj.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://uui.bjfxy.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ofy.haohaochexian.top

[Q89] 判断表是否存在
来源：http://mbm.52xcode.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://kqm.cucudq.cn

[Q90] 生成序号列
来源：http://hwj.meibo888.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://zsw.ctjpmb.com

================================================================================
来源：http://enb.jqgufenzy.top

R. Bash 专题
来源：http://kej.cucudq.cn

================================================================================
来源：http://nzt.daria6918.cn

[R01] shebang 与严格模式
来源：http://vqr.uphjek.com

#!/usr/bin/env bash
来源：http://ess.zhengqikj.top

set -euo pipefail
来源：http://lax.guowangkeji.top

[R02] 变量赋值与使用
来源：http://cpw.shanyushiyangkeji.top

name="Tom"; echo "$name"
来源：http://mbe.yfazqb.com

[R03] 只读变量
来源：http://orc.ywan-chungtsiang.top

readonly PI=3.14
来源：http://meg.yangfankeji.com

[R04] 位置参数
来源：http://ncg.jinqigufen.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wlv.dashuyun.cn

[R05] 参数默认值
来源：http://wir.jlsjyb.cn

name="${1:-default}"
来源：http://hkc.guowangkeji.top

[R06] 判断命令是否存在
来源：http://cfy.guannengcc.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ccs.zhiwuduotai.top

[R07] if 判断文件
来源：http://msf.andypj.xyz

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ctw.tanke756.top

[R08] 数值比较
来源：http://psw.meibo888.top

if (( a > b )); then echo "a 更大"; fi
来源：http://cxp.xinyue.icu

[R09] 字符串比较
来源：http://igc.fehbvm.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://cbg.yj20258888.top

[R10] 正则匹配
来源：http://jni.sweek.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://qyg.pycfn.com

[R11] case 多分支
来源：http://fhg.yvedp.cn

case "$1" in
来源：http://gvx.daxiang520.top

start) echo "启动" ;;
来源：http://cts.xuanzx.com

stop)  echo "停止" ;;
来源：http://qse.chenjidiqi.icu

*)     echo "未知命令" ;;
来源：http://ien.yonumen.top

esac
来源：http://ajf.redwolf501.top

[R12] for 遍历文件
来源：http://ulc.zhijiandao.cn

for f in *.txt; do echo "$f"; done
来源：http://vbe.jlsjyb.cn

[R13] for 计数循环
来源：http://baz.wangdashe.top

for i in {1..10}; do echo "$i"; done
来源：http://mal.yj20258.top

[R14] C 风格 for
来源：http://rtr.zhiwuduotai.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ape.hfpthk.cn

[R15] while 逐行读文件
来源：http://xvh.yj20258888.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://qpa.aizwys.cn

[R16] until 等待条件
来源：http://udq.sweek.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://vil.shangyingyoupin.top

[R17] 数组定义与取值
来源：http://ovx.zhixingplan.top

arr=(a b c); echo "${arr[0]}"
来源：http://dvn.0kj1m.cn

[R18] 遍历数组
来源：http://rwi.shzxlz.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://end.aizwys.cn

[R19] 数组长度
来源：http://opv.redwolf501.top

echo "${#arr[@]}"
来源：http://dke.zhijiandao.cn

[R20] 关联数组（字典）
来源：http://kme.mhx1999.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wsn.jqgfzy.top

[R21] 字符串长度
来源：http://ukj.hongshengwenyu.top

echo "${#s}"
来源：http://swm.zdbjq.cn

[R22] 截取子串
来源：http://zva.ivvv.top

echo "${s:0:5}"
来源：http://ynm.wangdashe.top

[R23] 字符串替换
来源：http://fxq.zhengqikj.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://cdc.yfazqb.com

[R24] 大小写转换
来源：http://gfd.svipenyu.cn

echo "${s^^}"; echo "${s,,}"
来源：http://xlg.zhoulong.xyz

[R25] 去后缀 / 去前缀
来源：http://cyz.chenlongwang.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://fkg.52xcode.cn

[R26] 命令替换
来源：http://vdp.quarkkingdee.top

now=$(date +%F); echo "$now"
来源：http://shq.shanyushiyangtech.top

[R27] 算术展开
来源：http://knp.gaohongyu789.top

echo $((1 + 2 * 3))
来源：http://ynt.ywan-chungtsiang.top

[R28] 浮点运算
来源：http://ubb.hywenlv.cn

echo "scale=2; 10/3" | bc
来源：http://ymc.ivvv.top

[R29] 定义函数
来源：http://suu.gzhubu.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://icw.jinqigfzy.top

[R30] 函数返回状态码
来源：http://kqo.yvedp.cn

f() { return 0; }; f || echo "失败了"
来源：http://bei.quarkkingdee.top

[R31] 局部变量
来源：http://cfj.fehbvm.com

f() { local x=1; echo "$x"; }
来源：http://fce.aibaodan.cn

[R32] 参数个数校验
来源：http://myr.ydzc1.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://xcq.vehdjk.com

[R33] 捕获错误并提示行号
来源：http://rhe.fengsongda.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://aci.dashuyun.cn

[R34] 退出时清理
来源：http://wcd.redwolf501.top

trap 'rm -f "$tmp"' EXIT
来源：http://qdd.shzxlz.cn

[R35] 后台执行并等待
来源：http://gqf.9152youxi.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ykx.xuetiantiany.cn

[R36] 并发执行多个任务
来源：http://lyx.zycfv.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://tll.hammf.cn

[R37] 把输出赋给变量
来源：http://ive.ehwqpu.com

files=$(ls -1)
来源：http://wfe.jyoumei.cn

[R38] 管道串联
来源：http://ghn.iojbl.cn

cat a.txt | grep -i error | wc -l
来源：http://feb.shuidangran.top

[R39] 重定向标准输出与错误
来源：http://wmg.hfpthk.cn

cmd > out.log 2>&1
来源：http://vdf.daria6918.cn

[R40] 追加写日志
来源：http://bgl.xingfuxueyuan.xyz

echo "log" >> out.log
来源：http://uvg.gaohongyu789.top

[R41] 丢弃输出
来源：http://jnd.bjfxy.top

cmd >/dev/null 2>&1
来源：http://ukw.guannengcc.top

[R42] 输入重定向
来源：http://shv.redwolf501.top

wc -l < a.txt
来源：http://rrq.fehbvm.com

[R43] 按名字查找文件
来源：http://exo.svipenyu.cn

find . -name "*.log" -type f
来源：http://pqc.guannengcc.top

[R44] 按修改时间查找
来源：http://dai.yuanzhike.top

find . -mtime -7 -type f
来源：http://kdz.mhx1999.top

[R45] 批量删除
来源：http://lug.hongshengwenyu.top

find . -name "*.tmp" -delete
来源：http://uoa.zhixingplan.top

[R46] 递归替换文件内容
来源：http://hli.jlsjyb.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://qzw.zycfv.cn

[R47] sed 单行替换
来源：http://lbq.chenlongwang.top

sed -i 's/foo/bar/g' a.txt
来源：http://fcu.chenlongwang.top

[R48] awk 取指定列
来源：http://ctc.haohaochexian.top

awk '{print $1, $3}' a.txt
来源：http://tqx.shangyingyoupin.top

[R49] awk 带条件
来源：http://djw.smart0.xyz

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://tom.tanke756.top

[R50] awk 求和
来源：http://nkp.fzhhl.top

awk '{s += $2} END {print s}' a.txt
来源：http://wjv.zdbjq.cn

[R51] 排序去重取前几
来源：http://rgi.hesvh.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://yym.zhijiandao.cn

[R52] 统计行数
来源：http://aqr.shzxlz.cn

wc -l a.txt
来源：http://zty.zhaomingkeji.xyz

[R53] 查看文件头与实时尾
来源：http://cna.tian-w.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://fiw.jyoumei.cn

[R54] 比较两个文件
来源：http://ftk.cashguo.top

diff a.txt b.txt
来源：http://rso.c1oappe.top

[R55] 压缩与解压
来源：http://btm.shanyushiyangtech.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://rdc.jyoumei.cn

[R56] 远程拷贝
来源：http://pfh.havefunace.top

scp file user@host:/path/
来源：http://loz.jinghuilouyu.cn

[R57] 远程执行命令
来源：http://syb.jinqigufen.top


<!-- 参考信息 -->