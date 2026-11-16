代发 wailian999

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://vvs.gaohongyu789.top

[Q05] 重命名列
来源：http://dbk.sufxvd.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://vwk.guannengcc.top

[Q06] 删除列
来源：http://uxs.ehwqpu.com

ALTER TABLE users DROP COLUMN age;
来源：http://xxo.xuetiantiany.cn

[Q07] 删除表
来源：http://yvv.sweek.top

DROP TABLE IF EXISTS orders;
来源：http://lxp.daxiang520.top

[Q08] 创建普通索引
来源：http://ilb.9152youxi.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://hza.zhijiandao.cn

[Q09] 创建唯一索引
来源：http://uuw.iojbl.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://tgo.jinghuilouyu.cn

[Q10] 插入单行
来源：http://tec.feifeiyinyue.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://llo.fktsv.cn

[Q11] 一次插入多行
来源：http://lyp.ppjwa.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://rme.ctjpmb.com

[Q12] 插入后取自增 ID
来源：http://cat.gaohongyu789.top

INSERT INTO users (name) VALUES ('C');
来源：http://lds.gzhubu.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://qaq.wangdashe.top

[Q13] 忽略重复插入
来源：http://ztx.hammf.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ntf.daxiang520.top

[Q14] 存在则更新（upsert）
来源：http://paz.316326.xyz

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hxu.ydjk.org.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://xxc.xziqi.cn

[Q15] 查询全部
来源：http://rzm.quarkkingdee.top

SELECT * FROM users;
来源：http://mii.xylfe.cn

[Q16] 查询指定列
来源：http://ehg.kuanghao11.cn

SELECT id, name FROM users;
来源：http://kli.xingfuxueyuan.xyz

[Q17] 条件查询
来源：http://bgk.yfazqb.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://niy.meibo888.top

[Q18] 模糊匹配
来源：http://wzr.hcnkem.com

SELECT * FROM users WHERE name LIKE '张%';
来源：http://xmn.sweek.top

[Q19] 范围查询
来源：http://vrb.jianghu66.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://bfn.shzxlz.cn

[Q20] IN 列表
来源：http://ysf.yonumen.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mrf.smart0.xyz

[Q21] 空值判断
来源：http://elt.andypj.xyz

SELECT * FROM users WHERE email IS NULL;
来源：http://dlk.316326.xyz

[Q22] 排序
来源：http://zla.gaohongyu789.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://gkb.ydzc1.top

[Q23] 分页
来源：http://jhc.hcnkem.com

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://luv.nanxuanxn.top

[Q24] 去重
来源：http://jcd.iojbl.cn

SELECT DISTINCT city FROM users;
来源：http://cqn.hfpthk.cn

[Q25] 只取前 N 条
来源：http://jdl.fehbvm.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://tcu.gotoacloud.top

[Q26] 计数
来源：http://gmi.ydzc1.top

SELECT COUNT(*) FROM users;
来源：http://gzn.aibaodan.cn

[Q27] 条件计数
来源：http://zqr.jinyuanbaomall.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://fkd.pycfn.com

[Q28] 求和与平均
来源：http://wlm.nanxuanxn.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://jai.haohaochexian.top

[Q29] 最大最小值
来源：http://shv.uphjek.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://wtg.shzxlz.cn

[Q30] 分组统计
来源：http://obk.nwbrower.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wxb.zycfv.cn

[Q31] 分组后过滤
来源：http://dez.shuidangran.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://rpf.iojbl.cn

[Q32] 分组拼接字符串
来源：http://wwh.birdmap.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://apb.dianchejie.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://gsg.yongpay.top

[Q33] 多列分组
来源：http://smo.haohaochexian.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ztg.tian-w.cn

[Q34] 每组取第一条
来源：http://zvu.sysykeji.top

SELECT * FROM (
来源：http://mej.aizwys.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://phy.yangfankeji.com

) t WHERE rn = 1;
来源：http://veb.ppjwa.cn

[Q35] 内连接
来源：http://orn.jqgufenzy.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://xyc.hywenlv.cn

[Q36] 左连接
来源：http://ixd.haohaochexian.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ajq.hywenlv.cn

[Q37] 右连接
来源：http://ywp.cqqwz.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://xgj.chenlongwang.top

[Q38] 全外连接（PostgreSQL）
来源：http://vkz.0kj1m.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://yuq.yuanzhike.top

[Q39] 自连接（查上下级）
来源：http://ndp.hammf.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://baa.wangdashe.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://yqn.yj20258.top

[Q40] 交叉连接（笛卡尔积）
来源：http://eds.shanyushiyangkeji.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://usq.aibaodan.cn

[Q41] 多表连接
来源：http://fbt.hongshengwenyu.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://ese.shanyushiyangkeji.top

JOIN users u ON u.id = o.user_id
来源：http://ppf.jinghuilouyu.cn

JOIN products p ON p.id = o.product_id;
来源：http://jqr.316326.xyz

[Q42] 连接条件附加过滤
来源：http://wsq.ctjpmb.com

SELECT u.name, o.amount FROM users u
来源：http://czp.zdqjudy.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://oka.52xcode.cn

[Q43] 标量子查询
来源：http://cfj.hammf.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://afg.cdnleiting.top

[Q44] IN 子查询
来源：http://pwt.ydjk.org.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://kig.jinqigufen.top

[Q45] EXISTS 判断存在
来源：http://dwb.jianghu66.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fhk.fktsv.cn

[Q46] NOT EXISTS 判断不存在
来源：http://jbs.ivvv.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://apd.fanxiaobao.xyz

[Q47] 与平均值比较
来源：http://gvt.fehbvm.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://vyi.hnqzz.top

[Q48] CTE 公用表表达式
来源：http://fpi.svipenyu.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wvj.uphjek.com

SELECT * FROM t WHERE c > 5;
来源：http://yha.cheryme.top

[Q49] 更新单行
来源：http://yii.dianchejie.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://qqw.yuanzhike.top

[Q50] 批量更新
来源：http://dmj.chenjidiqi.icu

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://lua.hnqzz.top

[Q51] 用子查询更新
来源：http://frd.jinqigufen.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mix.fehbvm.com

[Q52] 删除指定行
来源：http://dal.hnxiangtu.top

DELETE FROM users WHERE id = 10;
来源：http://nlm.cqqwz.cn

[Q53] 按条件删除
来源：http://vik.ydzc1.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ypr.tarul.cn

[Q54] 清空表
来源：http://gud.ywan-chungtsiang.top

TRUNCATE TABLE logs;
来源：http://rvn.tian-w.cn

[Q55] 排名（并列占位）
来源：http://xdr.gogol.net.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://tgx.sjlbkw.cn

[Q56] 密集排名（并列不占位）
来源：http://iyp.chenzaomai.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mur.hongshengwenyu.top

[Q57] 行号
来源：http://bez.c1oappe.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ews.sxryk.cn

[Q58] 累计求和
来源：http://put.zhijiandao.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://kdq.redwolf501.top

[Q59] 分组内累计
来源：http://fae.jianghu66.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ftw.meibo888.top

[Q60] 取上一行 / 下一行
来源：http://ifi.316326.xyz

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://csb.zhiwuduotai.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://grz.gzhubu.top

[Q61] 移动平均
来源：http://fwt.jinghuilouyu.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://vhv.zhijiandao.cn

[Q62] 分组占比
来源：http://ezg.wangshuangyany.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ace.snrcjt.cn

[Q63] 开启事务
来源：http://usp.hnqzz.top

START TRANSACTION;                -- 或 BEGIN
来源：http://mla.yonumen.top

[Q64] 提交事务
来源：http://kje.hesvh.cn

COMMIT;
来源：http://uyv.kuanghao11.cn

[Q65] 回滚事务
来源：http://lak.fzhhl.top

ROLLBACK;
来源：http://hqy.jyoumei.cn

[Q66] 行锁查询
来源：http://gjt.tianlin.xyz

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://iyp.nwbrower.top

[Q67] 设置隔离级别
来源：http://rrq.chenlongwang.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://qhu.svipenyu.cn

[Q68] 保存点
来源：http://sxt.daxiang520.top

SAVEPOINT sp1;
来源：http://wul.zhengqikj.top

ROLLBACK TO sp1;
来源：http://ncq.zycfv.cn

[Q69] 查看执行计划
来源：http://jwv.zdbjq.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://zra.sweek.top

[Q70] 更新统计信息
来源：http://jss.sweek.top

ANALYZE TABLE users;
来源：http://frh.sweek.top

[Q71] 查看建表语句
来源：http://yzb.daxiang520.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://plq.yvedp.cn

[Q72] 查看索引
来源：http://psl.fehbvm.com

SHOW INDEX FROM users;
来源：http://oew.bbcook.cn

[Q73] 查看表状态
来源：http://fbp.hammf.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://cfl.fengsongda.top

[Q74] 强制使用索引
来源：http://snx.chenlongwang.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://gjz.zhixingplan.top

[Q75] 日期格式化
来源：http://opf.jyoumei.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://egz.ydjk.org.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://gjg.cdnleiting.top

[Q76] 按天统计
来源：http://ixp.shuidangran.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wyd.yj20258888.top

[Q77] 时间加减
来源：http://pti.aizwys.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://zhf.gzhubu.top

[Q78] 当前时间
来源：http://tcv.dashuyun.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://sub.mhx1999.top

[Q79] 字符串拼接
来源：http://fyi.aibaodan.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://jcy.xuanzx.com

[Q80] 字符串截取
来源：http://fin.iojbl.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://nqa.pengpengdd.cyou

[Q81] 字符串替换
来源：http://ksq.dianchejie.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ucf.havefunace.top

[Q82] 字符长度与字节长度
来源：http://mjh.mhx1999.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://qtu.haohaochexian.top

[Q83] 大小写转换
来源：http://yoy.snrcjt.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mkr.yueranfly.top

[Q84] 去除首尾空格
来源：http://pha.zhijiandao.cn

SELECT TRIM(name) FROM users;
来源：http://rsn.fzhhl.top

[Q85] 数值取整
来源：http://pht.zhixingplan.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://obw.gzhubu.top

[Q86] 读取 JSON 字段
来源：http://urx.hywenlv.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://xwh.quarkkingdee.top

[Q87] JSON 字段做条件
来源：http://nsa.chenjidiqi.icu

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wml.9152youxi.cn

[Q88] 行转列（条件聚合）
来源：http://nip.hcnkem.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://duv.hfpthk.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://nea.jinghuilouyu.cn

[Q89] 判断表是否存在
来源：http://sgj.yongpay.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ndo.ppjwa.cn

[Q90] 生成序号列
来源：http://fzs.tanke756.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ngi.redwolf501.top

================================================================================
来源：http://yqk.zdqjudy.top

R. Bash 专题
来源：http://lwa.c1oappe.top

================================================================================
来源：http://eqj.jinghuilouyu.cn

[R01] shebang 与严格模式
来源：http://mhx.ppjwa.cn

#!/usr/bin/env bash
来源：http://jpv.haohaochexian.top

set -euo pipefail
来源：http://adm.jinyuanbaomall.cn

[R02] 变量赋值与使用
来源：http://hgp.ywan-chungtsiang.top

name="Tom"; echo "$name"
来源：http://eig.hysaishi.cn

[R03] 只读变量
来源：http://vau.cucudq.cn

readonly PI=3.14
来源：http://dun.jianghu66.top

[R04] 位置参数
来源：http://kql.ctjpmb.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://dhm.chenlongwang.top

[R05] 参数默认值
来源：http://ces.9152youxi.cn

name="${1:-default}"
来源：http://edh.fktsv.cn

[R06] 判断命令是否存在
来源：http://omj.shanyushiyangkeji.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://owd.yuanzhike.top

[R07] if 判断文件
来源：http://afq.316326.xyz

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://fvd.chenlongwang.top

[R08] 数值比较
来源：http://ddh.cucudq.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://vbg.zycfv.cn

[R09] 字符串比较
来源：http://uch.yuxming.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://xwt.feifeiyinyue.top

[R10] 正则匹配
来源：http://yxa.jlsjyb.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://lpn.zhongyouzk.top

[R11] case 多分支
来源：http://ugt.zhoulong.xyz

case "$1" in
来源：http://lam.hysaishi.cn

start) echo "启动" ;;
来源：http://mgf.zycfv.cn

stop)  echo "停止" ;;
来源：http://rqd.jinqigfzy.top

*)     echo "未知命令" ;;
来源：http://jlb.sufxvd.cn

esac
来源：http://xly.pengpengdd.cyou

[R12] for 遍历文件
来源：http://prh.cdnleiting.top

for f in *.txt; do echo "$f"; done
来源：http://enj.havefunace.top

[R13] for 计数循环
来源：http://jqi.sjlbkw.cn

for i in {1..10}; do echo "$i"; done
来源：http://paw.fktsv.cn

[R14] C 风格 for
来源：http://isz.fanxiaobao.xyz

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://omk.hnxiangtu.top

[R15] while 逐行读文件
来源：http://uev.bbcook.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wxg.yuanzhike.top

[R16] until 等待条件
来源：http://aze.sufxvd.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://qvt.sjlbkw.cn

[R17] 数组定义与取值
来源：http://sba.smart0.xyz

arr=(a b c); echo "${arr[0]}"
来源：http://bkn.cashguo.top

[R18] 遍历数组
来源：http://jrg.hcnkem.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://lmt.fanxiaobao.xyz

[R19] 数组长度
来源：http://ahs.tarul.cn

echo "${#arr[@]}"
来源：http://teu.sxryk.cn

[R20] 关联数组（字典）
来源：http://hmy.zdbjq.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://jdc.0kj1m.cn

[R21] 字符串长度
来源：http://znm.xingfuxueyuan.xyz

echo "${#s}"
来源：http://jbg.jinghuilouyu.cn

[R22] 截取子串
来源：http://beo.hammf.cn

echo "${s:0:5}"
来源：http://mxp.hfpthk.cn

[R23] 字符串替换
来源：http://tcg.yanxiufei.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://xdi.cashguo.top

[R24] 大小写转换
来源：http://ldi.ybcxt.top

echo "${s^^}"; echo "${s,,}"
来源：http://wny.haohaochexian.top

[R25] 去后缀 / 去前缀
来源：http://pkq.zhengqikj.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://dew.guannengcc.top

[R26] 命令替换
来源：http://dep.fzhhl.top

now=$(date +%F); echo "$now"
来源：http://jqz.gogol.net.cn

[R27] 算术展开
来源：http://brb.zhiwuduotai.top

echo $((1 + 2 * 3))
来源：http://mei.zhixingplan.top

[R28] 浮点运算
来源：http://dmh.zhoulong.xyz

echo "scale=2; 10/3" | bc
来源：http://nnw.gogol.net.cn

[R29] 定义函数
来源：http://rmt.fanxiaobao.xyz

add() { echo $(($1 + $2)); }; add 1 2
来源：http://oje.gaohongyu789.top

[R30] 函数返回状态码
来源：http://ixi.gogol.net.cn

f() { return 0; }; f || echo "失败了"
来源：http://evq.jlsjyb.cn

[R31] 局部变量
来源：http://mwo.wangdashe.top

f() { local x=1; echo "$x"; }
来源：http://reo.birdmap.top

[R32] 参数个数校验
来源：http://xys.havefunace.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://qgp.epnwcf.com

[R33] 捕获错误并提示行号
来源：http://cqr.dianchejie.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://vbu.yj20258888.top

[R34] 退出时清理
来源：http://pvt.hesvh.cn

trap 'rm -f "$tmp"' EXIT
来源：http://kls.ydjk.org.cn

[R35] 后台执行并等待
来源：http://pez.c1oappe.top

sleep 5 & pid=$!; wait "$pid"
来源：http://woy.snrcjt.cn

[R36] 并发执行多个任务
来源：http://njl.nanxinkj.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://zbg.sweek.top

[R37] 把输出赋给变量
来源：http://yxp.fzhhl.top

files=$(ls -1)
来源：http://ewj.jqgfzy.top

[R38] 管道串联
来源：http://dvm.hfpthk.cn

cat a.txt | grep -i error | wc -l
来源：http://wgt.zhengqikj.top

[R39] 重定向标准输出与错误
来源：http://lhy.chenlongwang.top

cmd > out.log 2>&1
来源：http://ent.vqdsnc.cn

[R40] 追加写日志
来源：http://lcq.uphjek.com

echo "log" >> out.log
来源：http://mju.snrcjt.cn

[R41] 丢弃输出
来源：http://irr.yonumen.top

cmd >/dev/null 2>&1
来源：http://xxm.wangdashe.top

[R42] 输入重定向
来源：http://jyc.ehwqpu.com

wc -l < a.txt
来源：http://jnu.svipenyu.cn

[R43] 按名字查找文件
来源：http://rpz.ydzc1.top

find . -name "*.log" -type f
来源：http://ycc.cqqwz.cn

[R44] 按修改时间查找
来源：http://svo.redwolf501.top

find . -mtime -7 -type f
来源：http://ver.zdbjq.cn

[R45] 批量删除
来源：http://ofv.jianghu66.top

find . -name "*.tmp" -delete
来源：http://uif.yuxming.cn

[R46] 递归替换文件内容
来源：http://qqs.zhoulong.xyz

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mhw.meibo888.top

[R47] sed 单行替换
来源：http://pse.hywenlv.cn

sed -i 's/foo/bar/g' a.txt
来源：http://rsn.yj202588.top

[R48] awk 取指定列
来源：http://dal.haohaochexian.top

awk '{print $1, $3}' a.txt
来源：http://ntr.wangshuangyany.cn

[R49] awk 带条件
来源：http://krj.zhijiandao.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://kzg.zhongyouzk.top

[R50] awk 求和
来源：http://zjf.shanyushiyangtech.top

awk '{s += $2} END {print s}' a.txt
来源：http://rte.ppjwa.cn

[R51] 排序去重取前几
来源：http://fwi.shanyushiyangkeji.top

sort a.txt | uniq -c | sort -rn | head
来源：http://urc.guowangkeji.top

[R52] 统计行数
来源：http://dyq.fengsongda.top

wc -l a.txt
来源：http://okx.zdbjq.cn

[R53] 查看文件头与实时尾
来源：http://gjt.dianchejie.cn


<!-- 参考信息 -->