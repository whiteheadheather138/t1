代发 wailian999

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://npd.redwolf501.top

);
来源：http://bpt.cashguo.top

[Q02] 创建带外键的表
来源：http://llj.jqgufenzy.top

CREATE TABLE orders (
来源：http://nuq.ywan-chungtsiang.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wim.zdqjudy.top

user_id INT NOT NULL,
来源：http://vli.dashuyun.cn

amount DECIMAL(10, 2),
来源：http://wab.yueranfly.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://jwb.hcnkem.com

);
来源：http://vfi.ydjk.org.cn

[Q03] 增加列
来源：http://zix.vehdjk.com

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://pbk.shanyushiyangtech.top

[Q04] 修改列类型
来源：http://pod.quarkkingdee.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://afq.mhx1999.top

[Q05] 重命名列
来源：http://rnm.jqgfzy.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://obi.yuxming.cn

[Q06] 删除列
来源：http://tqp.epnwcf.com

ALTER TABLE users DROP COLUMN age;
来源：http://ixg.yangfankeji.com

[Q07] 删除表
来源：http://sfa.iojbl.cn

DROP TABLE IF EXISTS orders;
来源：http://tet.xuetiantiany.cn

[Q08] 创建普通索引
来源：http://ymv.sufxvd.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://pkk.shanyushiyangtech.top

[Q09] 创建唯一索引
来源：http://eek.gogol.net.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://poq.jinghuilouyu.cn

[Q10] 插入单行
来源：http://dbg.cheryme.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ijz.quarkkingdee.top

[Q11] 一次插入多行
来源：http://iit.pengpengdd.cyou

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://jab.jqgfzy.top

[Q12] 插入后取自增 ID
来源：http://umk.pengpengdd.cyou

INSERT INTO users (name) VALUES ('C');
来源：http://dmq.jinqigufen.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mma.zhoulong.xyz

[Q13] 忽略重复插入
来源：http://dnt.jlsjyb.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://nkt.ppjwa.cn

[Q14] 存在则更新（upsert）
来源：http://vht.pengpengdd.cyou

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://yuw.yonumen.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://xgg.jiagoushi.top

[Q15] 查询全部
来源：http://opv.ivvv.top

SELECT * FROM users;
来源：http://coa.gzhubu.top

[Q16] 查询指定列
来源：http://cnx.0kj1m.cn

SELECT id, name FROM users;
来源：http://htg.yfazqb.com

[Q17] 条件查询
来源：http://ypw.yonumen.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://rwh.quarkkingdee.top

[Q18] 模糊匹配
来源：http://ivr.xinyue.icu

SELECT * FROM users WHERE name LIKE '张%';
来源：http://dcu.dashuyun.cn

[Q19] 范围查询
来源：http://ywt.wangdashe.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://dug.mhx1999.top

[Q20] IN 列表
来源：http://tgl.yonumen.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ziy.yanxiufei.cn

[Q21] 空值判断
来源：http://vpj.pycfn.com

SELECT * FROM users WHERE email IS NULL;
来源：http://djk.cucudq.cn

[Q22] 排序
来源：http://jbg.jinqigfzy.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://end.pycfn.com

[Q23] 分页
来源：http://lit.redwolf501.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://lnl.ivvv.top

[Q24] 去重
来源：http://jkw.yueranfly.top

SELECT DISTINCT city FROM users;
来源：http://ccc.shangyingyoupin.top

[Q25] 只取前 N 条
来源：http://jwo.hysaishi.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://brn.hammf.cn

[Q26] 计数
来源：http://mbw.ehwqpu.com

SELECT COUNT(*) FROM users;
来源：http://rpq.yueranfly.top

[Q27] 条件计数
来源：http://lzd.hcnkem.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://bpu.jyoumei.cn

[Q28] 求和与平均
来源：http://tew.hnxiangtu.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://don.xylfe.cn

[Q29] 最大最小值
来源：http://ksb.snrcjt.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://tej.gogol.net.cn

[Q30] 分组统计
来源：http://yjs.zhoulong.xyz

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://rck.meibo888.top

[Q31] 分组后过滤
来源：http://fta.ydjk.org.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://inp.nanxuanxn.top

[Q32] 分组拼接字符串
来源：http://oik.aizwys.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://eap.jqgufenzy.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ajk.sweek.top

[Q33] 多列分组
来源：http://ueh.xylfe.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://qny.pengpengdd.cyou

[Q34] 每组取第一条
来源：http://mjk.gzhubu.top

SELECT * FROM (
来源：http://ucp.xingfuxueyuan.xyz

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://puv.hywenlv.cn

) t WHERE rn = 1;
来源：http://xue.zhoulong.xyz

[Q35] 内连接
来源：http://ppc.c1oappe.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://uyy.jyoumei.cn

[Q36] 左连接
来源：http://ina.wangdashe.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://kjw.zhijiandao.cn

[Q37] 右连接
来源：http://scw.jinghuilouyu.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://anl.tarul.cn

[Q38] 全外连接（PostgreSQL）
来源：http://dgi.ppjwa.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://jry.daria6918.cn

[Q39] 自连接（查上下级）
来源：http://oeu.epnwcf.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://joc.fengsongda.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://kjr.sufxvd.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://xte.zhijiandao.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://erj.hywenlv.cn

[Q41] 多表连接
来源：http://vwm.yonumen.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://ggf.quarkkingdee.top

JOIN users u ON u.id = o.user_id
来源：http://gfy.daria6918.cn

JOIN products p ON p.id = o.product_id;
来源：http://kwq.hammf.cn

[Q42] 连接条件附加过滤
来源：http://qmi.yvedp.cn

SELECT u.name, o.amount FROM users u
来源：http://vjp.chenjidiqi.icu

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://yse.nwbrower.top

[Q43] 标量子查询
来源：http://lpg.wangshuangyany.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hls.yj20258888.top

[Q44] IN 子查询
来源：http://cln.zhengqikj.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://fmr.hnxiangtu.top

[Q45] EXISTS 判断存在
来源：http://iob.redwolf501.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qdr.birdmap.top

[Q46] NOT EXISTS 判断不存在
来源：http://vlh.316326.xyz

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rtb.9152youxi.cn

[Q47] 与平均值比较
来源：http://fic.fanxiaobao.xyz

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://zmr.cdnleiting.top

[Q48] CTE 公用表表达式
来源：http://eer.zhixingplan.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ahq.ctjpmb.com

SELECT * FROM t WHERE c > 5;
来源：http://pfs.gaohongyu789.top

[Q49] 更新单行
来源：http://kku.0kj1m.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://xha.0kj1m.cn

[Q50] 批量更新
来源：http://cdj.ybcxt.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://orw.zhongyouzk.top

[Q51] 用子查询更新
来源：http://utz.0kj1m.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://olx.jyoumei.cn

[Q52] 删除指定行
来源：http://zza.shzxlz.cn

DELETE FROM users WHERE id = 10;
来源：http://yvs.hammf.cn

[Q53] 按条件删除
来源：http://frt.gotoacloud.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://fkh.yj20258888.top

[Q54] 清空表
来源：http://bbw.hywenlv.cn

TRUNCATE TABLE logs;
来源：http://cix.yuxming.cn

[Q55] 排名（并列占位）
来源：http://prx.nwbrower.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hfn.cdnleiting.top

[Q56] 密集排名（并列不占位）
来源：http://qfp.yueranfly.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://rqw.cucudq.cn

[Q57] 行号
来源：http://dbk.hfpthk.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://jxo.zhixingplan.top

[Q58] 累计求和
来源：http://dtp.quarkkingdee.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://gav.jqgfzy.top

[Q59] 分组内累计
来源：http://buh.snrcjt.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://icx.pycfn.com

[Q60] 取上一行 / 下一行
来源：http://xpc.guannengcc.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://aww.xingfuxueyuan.xyz

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://iqu.sufxvd.cn

[Q61] 移动平均
来源：http://maw.zhaomingkeji.xyz

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wbd.gogol.net.cn

[Q62] 分组占比
来源：http://kzm.zycfv.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://bkz.jinyuanbaomall.cn

[Q63] 开启事务
来源：http://cra.ywan-chungtsiang.top

START TRANSACTION;                -- 或 BEGIN
来源：http://shn.shanyushiyangkeji.top

[Q64] 提交事务
来源：http://kyl.fzhhl.top

COMMIT;
来源：http://btg.zhoulong.xyz

[Q65] 回滚事务
来源：http://qke.jinyuanbaomall.cn

ROLLBACK;
来源：http://veu.yuxming.cn

[Q66] 行锁查询
来源：http://dce.shanyushiyangkeji.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://tmr.chenjidiqi.icu

[Q67] 设置隔离级别
来源：http://kbt.hfpthk.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://xce.guannengcc.top

[Q68] 保存点
来源：http://ngm.fanxiaobao.xyz

SAVEPOINT sp1;
来源：http://njk.hcnkem.com

ROLLBACK TO sp1;
来源：http://vss.hongshengwenyu.top

[Q69] 查看执行计划
来源：http://vuo.shuidangran.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wjj.uphjek.com

[Q70] 更新统计信息
来源：http://mjg.zhiwuduotai.top

ANALYZE TABLE users;
来源：http://kzq.chenjidiqi.icu

[Q71] 查看建表语句
来源：http://bui.zhaomingkeji.xyz

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://uuu.jinyuanbaomall.cn

[Q72] 查看索引
来源：http://cdc.bjfxy.top

SHOW INDEX FROM users;
来源：http://mjw.316326.xyz

[Q73] 查看表状态
来源：http://hds.svipenyu.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://xam.yueranfly.top

[Q74] 强制使用索引
来源：http://gdy.hnxiangtu.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ytc.jqgufenzy.top

[Q75] 日期格式化
来源：http://nqh.zhongyouzk.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hof.quarkkingdee.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ucz.jqgfzy.top

[Q76] 按天统计
来源：http://mcn.birdmap.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://qob.sxryk.cn

[Q77] 时间加减
来源：http://yes.sysykeji.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://dwm.iojbl.cn

[Q78] 当前时间
来源：http://pir.sweek.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://fpr.yanxiufei.cn

[Q79] 字符串拼接
来源：http://fmu.yueranfly.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://seh.fehbvm.com

[Q80] 字符串截取
来源：http://kib.shzxlz.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://lfg.tanke756.top

[Q81] 字符串替换
来源：http://ltl.haohaochexian.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://skf.zhijiandao.cn

[Q82] 字符长度与字节长度
来源：http://fqj.jyoumei.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hxd.yvedp.cn

[Q83] 大小写转换
来源：http://bdj.shanyushiyangtech.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://vtt.hywenlv.cn

[Q84] 去除首尾空格
来源：http://qjg.yanxiufei.cn

SELECT TRIM(name) FROM users;
来源：http://omr.yonumen.top

[Q85] 数值取整
来源：http://iqg.shanyushiyangkeji.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://lwe.hammf.cn

[Q86] 读取 JSON 字段
来源：http://dkq.xingfuxueyuan.xyz

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mza.jinyuanbaomall.cn

[Q87] JSON 字段做条件
来源：http://noq.daxiang520.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://drn.mhx1999.top

[Q88] 行转列（条件聚合）
来源：http://uoo.iojbl.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://rnp.xingfuxueyuan.xyz

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://bzw.pycfn.com

[Q89] 判断表是否存在
来源：http://rnl.ydzc1.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mvl.cashguo.top

[Q90] 生成序号列
来源：http://cnk.dashuyun.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://qeu.vqdsnc.cn

================================================================================
来源：http://pps.zhiwuduotai.top

R. Bash 专题
来源：http://uie.gogol.net.cn

================================================================================
来源：http://psn.guowangkeji.top

[R01] shebang 与严格模式
来源：http://pfp.mhx1999.top

#!/usr/bin/env bash
来源：http://uun.ivvv.top

set -euo pipefail
来源：http://tik.zhongyouzk.top

[R02] 变量赋值与使用
来源：http://ohb.shangyingyoupin.top

name="Tom"; echo "$name"
来源：http://spt.zycfv.cn

[R03] 只读变量
来源：http://feg.vqdsnc.cn

readonly PI=3.14
来源：http://tlk.ppjwa.cn

[R04] 位置参数
来源：http://vfn.zhiwuduotai.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wdw.hammf.cn

[R05] 参数默认值
来源：http://hvm.zdqjudy.top

name="${1:-default}"
来源：http://hsr.tian-w.cn

[R06] 判断命令是否存在
来源：http://azd.bjfxy.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ibp.xingfuxueyuan.xyz

[R07] if 判断文件
来源：http://cwh.vehdjk.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hnc.jinyuanbaomall.cn

[R08] 数值比较
来源：http://zzw.cheryme.top

if (( a > b )); then echo "a 更大"; fi
来源：http://tll.gotoacloud.top

[R09] 字符串比较
来源：http://wrl.tian-w.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ktz.hesvh.cn

[R10] 正则匹配
来源：http://utk.zhoulong.xyz

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://yzg.sysykeji.top

[R11] case 多分支
来源：http://rhi.hammf.cn

case "$1" in
来源：http://yji.yj20258.top

start) echo "启动" ;;
来源：http://ciq.pycfn.com

stop)  echo "停止" ;;
来源：http://pqm.nanxuanxn.top

*)     echo "未知命令" ;;
来源：http://njd.hongshengwenyu.top

esac
来源：http://gez.dianchejie.cn

[R12] for 遍历文件
来源：http://qbl.gaohongyu789.top

for f in *.txt; do echo "$f"; done
来源：http://xlw.nanxinkj.top

[R13] for 计数循环
来源：http://tku.hcnkem.com

for i in {1..10}; do echo "$i"; done
来源：http://yxt.zdqjudy.top

[R14] C 风格 for
来源：http://aqw.yvedp.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://rfs.jqgufenzy.top

[R15] while 逐行读文件
来源：http://hhf.svipenyu.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://noy.52xcode.cn

[R16] until 等待条件
来源：http://dgc.c1oappe.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ohy.andypj.xyz

[R17] 数组定义与取值
来源：http://dxm.52xcode.cn

arr=(a b c); echo "${arr[0]}"
来源：http://bpp.cucudq.cn

[R18] 遍历数组
来源：http://zvg.redwolf501.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ilv.0kj1m.cn

[R19] 数组长度
来源：http://xjg.gzhubu.top

echo "${#arr[@]}"
来源：http://rln.sweek.top

[R20] 关联数组（字典）
来源：http://fib.guannengcc.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://red.jinyuanbaomall.cn

[R21] 字符串长度
来源：http://vku.ybcxt.top

echo "${#s}"
来源：http://ayt.daria6918.cn

[R22] 截取子串
来源：http://qhv.dianchejie.cn

echo "${s:0:5}"
来源：http://amr.daxiang520.top

[R23] 字符串替换
来源：http://kac.quarkkingdee.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://bsw.shanyushiyangtech.top

[R24] 大小写转换
来源：http://fyb.c1oappe.top

echo "${s^^}"; echo "${s,,}"
来源：http://gub.gzhubu.top

[R25] 去后缀 / 去前缀
来源：http://giu.xuanzx.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://ssc.svipenyu.cn

[R26] 命令替换
来源：http://qrh.yj20258.top

now=$(date +%F); echo "$now"
来源：http://dmy.hammf.cn

[R27] 算术展开
来源：http://qih.shanyushiyangkeji.top

echo $((1 + 2 * 3))
来源：http://ahj.ppjwa.cn

[R28] 浮点运算
来源：http://ppq.zhaomingkeji.xyz

echo "scale=2; 10/3" | bc
来源：http://fjc.aibaodan.cn

[R29] 定义函数
来源：http://pty.zhijiandao.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hlr.tarul.cn

[R30] 函数返回状态码
来源：http://xtz.meibo888.top

f() { return 0; }; f || echo "失败了"
来源：http://fqx.wangdashe.top

[R31] 局部变量
来源：http://uiz.sweek.top

f() { local x=1; echo "$x"; }
来源：http://vsk.yanxiufei.cn

[R32] 参数个数校验
来源：http://qzc.jinghuilouyu.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://etl.c1oappe.top

[R33] 捕获错误并提示行号
来源：http://bex.cdnleiting.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://pgu.hnxiangtu.top

[R34] 退出时清理
来源：http://osg.jinghuilouyu.cn

trap 'rm -f "$tmp"' EXIT
来源：http://kal.shanyushiyangtech.top

[R35] 后台执行并等待
来源：http://plb.chenjidiqi.icu

sleep 5 & pid=$!; wait "$pid"
来源：http://riz.fzhhl.top

[R36] 并发执行多个任务
来源：http://jys.cashguo.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://uvz.ehwqpu.com

[R37] 把输出赋给变量
来源：http://wlf.svipenyu.cn

files=$(ls -1)
来源：http://hyw.yj202588.top

[R38] 管道串联
来源：http://fld.c1oappe.top

cat a.txt | grep -i error | wc -l
来源：http://rzd.uphjek.com

[R39] 重定向标准输出与错误
来源：http://mkf.zhijiandao.cn

cmd > out.log 2>&1
来源：http://bij.vqdsnc.cn

[R40] 追加写日志
来源：http://tse.ctjpmb.com

echo "log" >> out.log
来源：http://rlg.vehdjk.com

[R41] 丢弃输出
来源：http://sks.cucudq.cn

cmd >/dev/null 2>&1
来源：http://pom.wangshuangyany.cn

[R42] 输入重定向
来源：http://gvu.xingfuxueyuan.xyz

wc -l < a.txt
来源：http://gxh.shzxlz.cn

[R43] 按名字查找文件
来源：http://ujl.fehbvm.com

find . -name "*.log" -type f
来源：http://pdp.hnxiangtu.top

[R44] 按修改时间查找
来源：http://uiy.cdnleiting.top

find . -mtime -7 -type f
来源：http://ank.mhx1999.top

[R45] 批量删除
来源：http://tyv.yuxming.cn

find . -name "*.tmp" -delete
来源：http://rme.gotoacloud.top

[R46] 递归替换文件内容
来源：http://ibo.hnqzz.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://che.yueranfly.top

[R47] sed 单行替换
来源：http://lzk.hfpthk.cn


<!-- 参考信息 -->