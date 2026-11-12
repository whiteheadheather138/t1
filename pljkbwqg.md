代发 wailian999

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://jxu.zycfv.cn

[Q05] 重命名列
来源：http://bhn.guannengcc.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://uxj.vehdjk.com

[Q06] 删除列
来源：http://wuj.jinghuilouyu.cn

ALTER TABLE users DROP COLUMN age;
来源：http://pdj.daria6918.cn

[Q07] 删除表
来源：http://rxl.shanyushiyangtech.top

DROP TABLE IF EXISTS orders;
来源：http://lzp.jinqigfzy.top

[Q08] 创建普通索引
来源：http://fwx.ehwqpu.com

CREATE INDEX idx_users_email ON users(email);
来源：http://sdo.hesvh.cn

[Q09] 创建唯一索引
来源：http://vln.ydzc1.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wnf.chenjidiqi.icu

[Q10] 插入单行
来源：http://cqk.guowangkeji.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://bsa.yangfankeji.com

[Q11] 一次插入多行
来源：http://mia.nwbrower.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://bnn.xuanzx.com

[Q12] 插入后取自增 ID
来源：http://zmz.ybcxt.top

INSERT INTO users (name) VALUES ('C');
来源：http://xye.gaohongyu789.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://tgi.chenjidiqi.icu

[Q13] 忽略重复插入
来源：http://peo.cheryme.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://src.shanyushiyangtech.top

[Q14] 存在则更新（upsert）
来源：http://jia.yongpay.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://euv.jianghu66.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://pfi.nanxinkj.top

[Q15] 查询全部
来源：http://kms.jiagoushi.top

SELECT * FROM users;
来源：http://gcr.zhongyouzk.top

[Q16] 查询指定列
来源：http://rxn.xuanzx.com

SELECT id, name FROM users;
来源：http://rzd.ivvv.top

[Q17] 条件查询
来源：http://kya.shzxlz.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://oqd.svipenyu.cn

[Q18] 模糊匹配
来源：http://kfe.hcnkem.com

SELECT * FROM users WHERE name LIKE '张%';
来源：http://yis.yuanzhike.top

[Q19] 范围查询
来源：http://fqa.jqgufenzy.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://vpl.xziqi.cn

[Q20] IN 列表
来源：http://mof.fzhhl.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://rsv.yj20258888.top

[Q21] 空值判断
来源：http://oue.sxryk.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://yvq.sufxvd.cn

[Q22] 排序
来源：http://pau.haohaochexian.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mwv.hammf.cn

[Q23] 分页
来源：http://vln.ppjwa.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ptg.yj20258888.top

[Q24] 去重
来源：http://lsh.haohaochexian.top

SELECT DISTINCT city FROM users;
来源：http://vch.yuanzhike.top

[Q25] 只取前 N 条
来源：http://qwa.gaohongyu789.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://xhx.hywenlv.cn

[Q26] 计数
来源：http://cjq.uphjek.com

SELECT COUNT(*) FROM users;
来源：http://maz.redwolf501.top

[Q27] 条件计数
来源：http://cxg.zhoulong.xyz

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hxc.tian-w.cn

[Q28] 求和与平均
来源：http://dyy.jinqigufen.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://gac.birdmap.top

[Q29] 最大最小值
来源：http://ggz.shzxlz.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ezg.bbcook.cn

[Q30] 分组统计
来源：http://ycm.yuanzhike.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://gxn.cashguo.top

[Q31] 分组后过滤
来源：http://soo.havefunace.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ero.hywenlv.cn

[Q32] 分组拼接字符串
来源：http://kix.hammf.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://uzv.jinqigfzy.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wpj.fzhhl.top

[Q33] 多列分组
来源：http://pog.vehdjk.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://fdr.jyoumei.cn

[Q34] 每组取第一条
来源：http://nru.svipenyu.cn

SELECT * FROM (
来源：http://ghc.sweek.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://yvt.zycfv.cn

) t WHERE rn = 1;
来源：http://wqq.ydjk.org.cn

[Q35] 内连接
来源：http://aqt.guannengcc.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://zit.svipenyu.cn

[Q36] 左连接
来源：http://gis.sjlbkw.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://kzv.snrcjt.cn

[Q37] 右连接
来源：http://nbv.ppjwa.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://jjd.redwolf501.top

[Q38] 全外连接（PostgreSQL）
来源：http://swc.zhengqikj.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://rnd.52xcode.cn

[Q39] 自连接（查上下级）
来源：http://mur.yj20258888.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://ahf.fehbvm.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ubu.yangfankeji.com

[Q40] 交叉连接（笛卡尔积）
来源：http://hta.quarkkingdee.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://iqs.nwbrower.top

[Q41] 多表连接
来源：http://rql.iojbl.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://igy.havefunace.top

JOIN users u ON u.id = o.user_id
来源：http://jsm.redwolf501.top

JOIN products p ON p.id = o.product_id;
来源：http://mvz.tanke756.top

[Q42] 连接条件附加过滤
来源：http://trf.xziqi.cn

SELECT u.name, o.amount FROM users u
来源：http://jrn.haohaochexian.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://iws.tian-w.cn

[Q43] 标量子查询
来源：http://crn.zhongyouzk.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://qgf.guannengcc.top

[Q44] IN 子查询
来源：http://ber.jqgufenzy.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://vqy.hammf.cn

[Q45] EXISTS 判断存在
来源：http://phy.yonumen.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://dkl.ivvv.top

[Q46] NOT EXISTS 判断不存在
来源：http://wdv.chenlongwang.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wxy.mhx1999.top

[Q47] 与平均值比较
来源：http://por.yuxming.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://uhh.daria6918.cn

[Q48] CTE 公用表表达式
来源：http://iss.dianchejie.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ybr.pengpengdd.cyou

SELECT * FROM t WHERE c > 5;
来源：http://yug.ctjpmb.com

[Q49] 更新单行
来源：http://gww.meibo888.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://epr.fanxiaobao.xyz

[Q50] 批量更新
来源：http://aqk.jlsjyb.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://vlq.daxiang520.top

[Q51] 用子查询更新
来源：http://vum.yvedp.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://aig.fengsongda.top

[Q52] 删除指定行
来源：http://bmf.vehdjk.com

DELETE FROM users WHERE id = 10;
来源：http://bsb.hongshengwenyu.top

[Q53] 按条件删除
来源：http://yuq.fengsongda.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wym.ppjwa.cn

[Q54] 清空表
来源：http://hfx.fehbvm.com

TRUNCATE TABLE logs;
来源：http://qlh.yonumen.top

[Q55] 排名（并列占位）
来源：http://gci.jinyuanbaomall.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://xsj.sysykeji.top

[Q56] 密集排名（并列不占位）
来源：http://jbb.zhixingplan.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://upw.sxryk.cn

[Q57] 行号
来源：http://pmx.zhoulong.xyz

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://edq.jlsjyb.cn

[Q58] 累计求和
来源：http://ptf.jinqigfzy.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://bey.shzxlz.cn

[Q59] 分组内累计
来源：http://gqv.hysaishi.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ffe.yj20258888.top

[Q60] 取上一行 / 下一行
来源：http://ohx.redwolf501.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://cph.xziqi.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://urn.xuanzx.com

[Q61] 移动平均
来源：http://otz.zdbjq.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mpj.yvedp.cn

[Q62] 分组占比
来源：http://mkl.gzhubu.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://nqt.tianlin.xyz

[Q63] 开启事务
来源：http://rnr.sufxvd.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://zwi.gzhubu.top

[Q64] 提交事务
来源：http://ldd.zhengqikj.top

COMMIT;
来源：http://hew.yuanzhike.top

[Q65] 回滚事务
来源：http://ubu.yj202588.top

ROLLBACK;
来源：http://hqb.yuanzhike.top

[Q66] 行锁查询
来源：http://qms.zhoulong.xyz

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://pts.wangdashe.top

[Q67] 设置隔离级别
来源：http://yor.bbcook.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://pkh.sjlbkw.cn

[Q68] 保存点
来源：http://ahl.shanyushiyangkeji.top

SAVEPOINT sp1;
来源：http://zyi.zhijiandao.cn

ROLLBACK TO sp1;
来源：http://ale.ppjwa.cn

[Q69] 查看执行计划
来源：http://cum.cdnleiting.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://rjn.xingfuxueyuan.xyz

[Q70] 更新统计信息
来源：http://bnm.yangfankeji.com

ANALYZE TABLE users;
来源：http://alt.hesvh.cn

[Q71] 查看建表语句
来源：http://vvn.gogol.net.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://znc.zdbjq.cn

[Q72] 查看索引
来源：http://uma.yuanzhike.top

SHOW INDEX FROM users;
来源：http://sox.cdnleiting.top

[Q73] 查看表状态
来源：http://mls.ybcxt.top

SHOW TABLE STATUS LIKE 'users';
来源：http://fcg.sjlbkw.cn

[Q74] 强制使用索引
来源：http://onb.yuanzhike.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://lvd.zhaomingkeji.xyz

[Q75] 日期格式化
来源：http://fja.yvedp.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://muo.nanxinkj.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://tcl.shanyushiyangtech.top

[Q76] 按天统计
来源：http://cda.jlsjyb.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://gzu.andypj.xyz

[Q77] 时间加减
来源：http://pne.yvedp.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ryi.ywan-chungtsiang.top

[Q78] 当前时间
来源：http://ziz.cashguo.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://xwa.hnqzz.top

[Q79] 字符串拼接
来源：http://kqj.ivvv.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://uzm.tianlin.xyz

[Q80] 字符串截取
来源：http://vvc.gogol.net.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ril.ivvv.top

[Q81] 字符串替换
来源：http://ptj.jinyuanbaomall.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ovq.zhiwuduotai.top

[Q82] 字符长度与字节长度
来源：http://pjo.svipenyu.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://phz.mhx1999.top

[Q83] 大小写转换
来源：http://wha.316326.xyz

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://lgc.hysaishi.cn

[Q84] 去除首尾空格
来源：http://atu.havefunace.top

SELECT TRIM(name) FROM users;
来源：http://hnd.fengsongda.top

[Q85] 数值取整
来源：http://kve.cheryme.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://rkf.hywenlv.cn

[Q86] 读取 JSON 字段
来源：http://emx.cdnleiting.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://bno.shuidangran.top

[Q87] JSON 字段做条件
来源：http://axi.9152youxi.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://kuj.cdnleiting.top

[Q88] 行转列（条件聚合）
来源：http://fsq.feifeiyinyue.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://bri.jinqigufen.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://gev.fzhhl.top

[Q89] 判断表是否存在
来源：http://xom.vqdsnc.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://avh.wangshuangyany.cn

[Q90] 生成序号列
来源：http://hwe.fengsongda.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://bfi.hongshengwenyu.top

================================================================================
来源：http://tjr.jinghuilouyu.cn

R. Bash 专题
来源：http://imq.jiagoushi.top

================================================================================
来源：http://khu.guannengcc.top

[R01] shebang 与严格模式
来源：http://xfs.yfazqb.com

#!/usr/bin/env bash
来源：http://xgb.vehdjk.com

set -euo pipefail
来源：http://bdy.yongpay.top

[R02] 变量赋值与使用
来源：http://vny.jianghu66.top

name="Tom"; echo "$name"
来源：http://pmy.yanxiufei.cn

[R03] 只读变量
来源：http://pha.daria6918.cn

readonly PI=3.14
来源：http://wqs.aibaodan.cn

[R04] 位置参数
来源：http://buo.bjfxy.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://jvo.daria6918.cn

[R05] 参数默认值
来源：http://tvh.xziqi.cn

name="${1:-default}"
来源：http://gwd.jinyuanbaomall.cn

[R06] 判断命令是否存在
来源：http://rqj.meibo888.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wdp.jqgufenzy.top

[R07] if 判断文件
来源：http://qoe.shangyingyoupin.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mym.chenzaomai.com

[R08] 数值比较
来源：http://grz.guannengcc.top

if (( a > b )); then echo "a 更大"; fi
来源：http://coo.gzhubu.top

[R09] 字符串比较
来源：http://idq.jiagoushi.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://uwk.shanyushiyangkeji.top

[R10] 正则匹配
来源：http://vgk.wangshuangyany.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://yof.chenjidiqi.icu

[R11] case 多分支
来源：http://aij.ydzc1.top

case "$1" in
来源：http://ujy.gaohongyu789.top

start) echo "启动" ;;
来源：http://zfi.fzhhl.top

stop)  echo "停止" ;;
来源：http://cnm.zhongyouzk.top

*)     echo "未知命令" ;;
来源：http://urw.smart0.xyz

esac
来源：http://vvw.cdnleiting.top

[R12] for 遍历文件
来源：http://lcc.daria6918.cn

for f in *.txt; do echo "$f"; done
来源：http://vyu.aibaodan.cn

[R13] for 计数循环
来源：http://fgm.shanyushiyangkeji.top

for i in {1..10}; do echo "$i"; done
来源：http://nxi.hongshengwenyu.top

[R14] C 风格 for
来源：http://nuq.zhaomingkeji.xyz

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://pcn.cashguo.top

[R15] while 逐行读文件
来源：http://soe.daria6918.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://cov.haohaochexian.top

[R16] until 等待条件
来源：http://xuo.redwolf501.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://efr.jyoumei.cn

[R17] 数组定义与取值
来源：http://qnw.tanke756.top

arr=(a b c); echo "${arr[0]}"
来源：http://fte.fzhhl.top

[R18] 遍历数组
来源：http://btt.zdbjq.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://fib.jinyuanbaomall.cn

[R19] 数组长度
来源：http://mnx.birdmap.top

echo "${#arr[@]}"
来源：http://scl.shanyushiyangtech.top

[R20] 关联数组（字典）
来源：http://fab.fehbvm.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://fes.pycfn.com

[R21] 字符串长度
来源：http://rbj.52xcode.cn

echo "${#s}"
来源：http://xkx.hongshengwenyu.top

[R22] 截取子串
来源：http://slf.tianlin.xyz

echo "${s:0:5}"
来源：http://cqj.fehbvm.com

[R23] 字符串替换
来源：http://mdh.hnqzz.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://sxk.shanyushiyangtech.top

[R24] 大小写转换
来源：http://wia.feifeiyinyue.top

echo "${s^^}"; echo "${s,,}"
来源：http://cxo.ppjwa.cn

[R25] 去后缀 / 去前缀
来源：http://din.xuanzx.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://rsy.ybcxt.top

[R26] 命令替换
来源：http://hvw.shanyushiyangkeji.top

now=$(date +%F); echo "$now"
来源：http://vsn.cashguo.top

[R27] 算术展开
来源：http://tdg.yj202588.top

echo $((1 + 2 * 3))
来源：http://fzm.ydzc1.top

[R28] 浮点运算
来源：http://rfk.birdmap.top

echo "scale=2; 10/3" | bc
来源：http://mxz.shuidangran.top

[R29] 定义函数
来源：http://nfk.guowangkeji.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hdq.dianchejie.cn

[R30] 函数返回状态码
来源：http://ecm.yuanzhike.top

f() { return 0; }; f || echo "失败了"
来源：http://kqy.gogol.net.cn

[R31] 局部变量
来源：http://ihs.52xcode.cn

f() { local x=1; echo "$x"; }
来源：http://jsy.zhongyouzk.top

[R32] 参数个数校验
来源：http://nlw.shanyushiyangtech.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://vuj.fehbvm.com

[R33] 捕获错误并提示行号
来源：http://acd.guannengcc.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://oyb.zhongyouzk.top

[R34] 退出时清理
来源：http://jhy.zhoulong.xyz

trap 'rm -f "$tmp"' EXIT
来源：http://jkl.hcnkem.com

[R35] 后台执行并等待
来源：http://mbl.jiagoushi.top

sleep 5 & pid=$!; wait "$pid"
来源：http://mtn.zycfv.cn

[R36] 并发执行多个任务
来源：http://wxa.yanxiufei.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://afn.cqqwz.cn

[R37] 把输出赋给变量
来源：http://wss.svipenyu.cn

files=$(ls -1)
来源：http://vxp.shangyingyoupin.top

[R38] 管道串联
来源：http://rov.yj20258.top

cat a.txt | grep -i error | wc -l
来源：http://njg.bjfxy.top

[R39] 重定向标准输出与错误
来源：http://nei.ydjk.org.cn

cmd > out.log 2>&1
来源：http://egs.yuanzhike.top

[R40] 追加写日志
来源：http://yir.tarul.cn

echo "log" >> out.log
来源：http://vva.xylfe.cn

[R41] 丢弃输出
来源：http://nrt.yvedp.cn

cmd >/dev/null 2>&1
来源：http://yia.yj20258.top

[R42] 输入重定向
来源：http://abk.nanxuanxn.top

wc -l < a.txt
来源：http://ipo.jinyuanbaomall.cn

[R43] 按名字查找文件
来源：http://ykf.xuanzx.com

find . -name "*.log" -type f
来源：http://kwg.ybcxt.top

[R44] 按修改时间查找
来源：http://glb.jinqigfzy.top

find . -mtime -7 -type f
来源：http://gfc.nanxuanxn.top

[R45] 批量删除
来源：http://sde.cqqwz.cn

find . -name "*.tmp" -delete
来源：http://giy.jlsjyb.cn

[R46] 递归替换文件内容
来源：http://ubz.wangdashe.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://fwv.fehbvm.com

[R47] sed 单行替换
来源：http://zrv.aizwys.cn

sed -i 's/foo/bar/g' a.txt
来源：http://sry.bjfxy.top

[R48] awk 取指定列
来源：http://orj.0kj1m.cn

awk '{print $1, $3}' a.txt
来源：http://uwv.aizwys.cn

[R49] awk 带条件
来源：http://vqq.nanxuanxn.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://nwx.havefunace.top

[R50] awk 求和
来源：http://rda.nwbrower.top

awk '{s += $2} END {print s}' a.txt
来源：http://mud.sysykeji.top

[R51] 排序去重取前几
来源：http://ctf.xuetiantiany.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://jpd.nanxuanxn.top

[R52] 统计行数
来源：http://nye.zhongyouzk.top

wc -l a.txt
来源：http://avg.cdnleiting.top

[R53] 查看文件头与实时尾
来源：http://fqv.pycfn.com


<!-- 参考信息 -->