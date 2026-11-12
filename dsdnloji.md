代发 wailian999

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://nwd.tian-w.cn

[Q05] 重命名列
来源：http://iok.wangshuangyany.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hwq.aibaodan.cn

[Q06] 删除列
来源：http://pac.fzhhl.top

ALTER TABLE users DROP COLUMN age;
来源：http://vzk.nanxinkj.top

[Q07] 删除表
来源：http://mor.hammf.cn

DROP TABLE IF EXISTS orders;
来源：http://wei.yanxiufei.cn

[Q08] 创建普通索引
来源：http://hhp.yfazqb.com

CREATE INDEX idx_users_email ON users(email);
来源：http://qmm.zdbjq.cn

[Q09] 创建唯一索引
来源：http://tak.shuidangran.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://uzf.kuanghao11.cn

[Q10] 插入单行
来源：http://ymq.bbcook.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://kpd.yongpay.top

[Q11] 一次插入多行
来源：http://uxb.yangfankeji.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://jav.hongshengwenyu.top

[Q12] 插入后取自增 ID
来源：http://xak.gzhubu.top

INSERT INTO users (name) VALUES ('C');
来源：http://yvs.jinghuilouyu.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://yag.jlsjyb.cn

[Q13] 忽略重复插入
来源：http://nln.ywan-chungtsiang.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://fel.zhixingplan.top

[Q14] 存在则更新（upsert）
来源：http://qmc.52xcode.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ihl.cheryme.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://piw.tanke756.top

[Q15] 查询全部
来源：http://tbr.epnwcf.com

SELECT * FROM users;
来源：http://pso.daria6918.cn

[Q16] 查询指定列
来源：http://xip.xinyue.icu

SELECT id, name FROM users;
来源：http://tuk.gogol.net.cn

[Q17] 条件查询
来源：http://paa.jlsjyb.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://vcy.guannengcc.top

[Q18] 模糊匹配
来源：http://yal.shuidangran.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://lus.pengpengdd.cyou

[Q19] 范围查询
来源：http://pjh.wangshuangyany.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://uso.cucudq.cn

[Q20] IN 列表
来源：http://xgg.52xcode.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://otb.xingfuxueyuan.xyz

[Q21] 空值判断
来源：http://kup.kuanghao11.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://oso.bjfxy.top

[Q22] 排序
来源：http://bki.9152youxi.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ygc.guowangkeji.top

[Q23] 分页
来源：http://xfk.havefunace.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://zas.ctjpmb.com

[Q24] 去重
来源：http://oyp.feifeiyinyue.top

SELECT DISTINCT city FROM users;
来源：http://qqk.iojbl.cn

[Q25] 只取前 N 条
来源：http://hyn.fzhhl.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://bmk.zhijiandao.cn

[Q26] 计数
来源：http://kqs.gaohongyu789.top

SELECT COUNT(*) FROM users;
来源：http://aqs.vqdsnc.cn

[Q27] 条件计数
来源：http://cxa.fktsv.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://eap.vqdsnc.cn

[Q28] 求和与平均
来源：http://pgc.gogol.net.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://dnj.guowangkeji.top

[Q29] 最大最小值
来源：http://bzm.ywan-chungtsiang.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://eka.hammf.cn

[Q30] 分组统计
来源：http://dio.jqgufenzy.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://kma.dashuyun.cn

[Q31] 分组后过滤
来源：http://ian.fanxiaobao.xyz

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://nti.shuidangran.top

[Q32] 分组拼接字符串
来源：http://ubt.gotoacloud.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://oco.yj202588.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://dbv.guowangkeji.top

[Q33] 多列分组
来源：http://cwi.shuidangran.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://qbs.guannengcc.top

[Q34] 每组取第一条
来源：http://isk.shanyushiyangkeji.top

SELECT * FROM (
来源：http://yqk.hcnkem.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://lao.yj20258888.top

) t WHERE rn = 1;
来源：http://wdl.sweek.top

[Q35] 内连接
来源：http://xvv.ppjwa.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://zrj.sjlbkw.cn

[Q36] 左连接
来源：http://odf.shangyingyoupin.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://bah.chenlongwang.top

[Q37] 右连接
来源：http://dec.nanxuanxn.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://tlc.dashuyun.cn

[Q38] 全外连接（PostgreSQL）
来源：http://hfq.redwolf501.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://pob.yj20258.top

[Q39] 自连接（查上下级）
来源：http://rvk.yj202588.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://alw.fktsv.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://zww.haohaochexian.top

[Q40] 交叉连接（笛卡尔积）
来源：http://rdk.c1oappe.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://kpr.hfpthk.cn

[Q41] 多表连接
来源：http://xcz.dashuyun.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://rsf.cqqwz.cn

JOIN users u ON u.id = o.user_id
来源：http://gcd.hnxiangtu.top

JOIN products p ON p.id = o.product_id;
来源：http://ksy.xziqi.cn

[Q42] 连接条件附加过滤
来源：http://zgx.hesvh.cn

SELECT u.name, o.amount FROM users u
来源：http://eit.yuxming.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://dfo.vehdjk.com

[Q43] 标量子查询
来源：http://yit.redwolf501.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mmd.smart0.xyz

[Q44] IN 子查询
来源：http://onm.ehwqpu.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://miy.jqgfzy.top

[Q45] EXISTS 判断存在
来源：http://nel.xingfuxueyuan.xyz

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://erc.dianchejie.cn

[Q46] NOT EXISTS 判断不存在
来源：http://lnz.yanxiufei.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qxq.jinqigufen.top

[Q47] 与平均值比较
来源：http://dkn.hammf.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ghd.yj20258.top

[Q48] CTE 公用表表达式
来源：http://uuh.daria6918.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wwz.ppjwa.cn

SELECT * FROM t WHERE c > 5;
来源：http://oyp.ydzc1.top

[Q49] 更新单行
来源：http://ceg.bjfxy.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ixr.gzhubu.top

[Q50] 批量更新
来源：http://lln.guowangkeji.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://vla.zycfv.cn

[Q51] 用子查询更新
来源：http://npu.feifeiyinyue.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://gci.iojbl.cn

[Q52] 删除指定行
来源：http://mef.cucudq.cn

DELETE FROM users WHERE id = 10;
来源：http://nfb.c1oappe.top

[Q53] 按条件删除
来源：http://hlt.ivvv.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ttd.hammf.cn

[Q54] 清空表
来源：http://jdv.fzhhl.top

TRUNCATE TABLE logs;
来源：http://yru.jinqigufen.top

[Q55] 排名（并列占位）
来源：http://dzu.daria6918.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://uuk.tian-w.cn

[Q56] 密集排名（并列不占位）
来源：http://mxn.iojbl.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hrs.iojbl.cn

[Q57] 行号
来源：http://nre.chenjidiqi.icu

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hin.chenjidiqi.icu

[Q58] 累计求和
来源：http://cqm.jqgfzy.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wiy.xylfe.cn

[Q59] 分组内累计
来源：http://bnq.ivvv.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://rxo.fehbvm.com

[Q60] 取上一行 / 下一行
来源：http://url.haohaochexian.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://fyf.chenzaomai.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://xln.dashuyun.cn

[Q61] 移动平均
来源：http://eyc.shanyushiyangtech.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://jzy.jinqigufen.top

[Q62] 分组占比
来源：http://sxf.sxryk.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wvr.sxryk.cn

[Q63] 开启事务
来源：http://kho.nanxuanxn.top

START TRANSACTION;                -- 或 BEGIN
来源：http://pwk.tanke756.top

[Q64] 提交事务
来源：http://yoo.xziqi.cn

COMMIT;
来源：http://wmv.quarkkingdee.top

[Q65] 回滚事务
来源：http://mvp.hesvh.cn

ROLLBACK;
来源：http://lpg.zycfv.cn

[Q66] 行锁查询
来源：http://ekm.cashguo.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://evd.hcnkem.com

[Q67] 设置隔离级别
来源：http://aeu.guannengcc.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://smr.yonumen.top

[Q68] 保存点
来源：http://hxn.daria6918.cn

SAVEPOINT sp1;
来源：http://kvh.fanxiaobao.xyz

ROLLBACK TO sp1;
来源：http://dya.yueranfly.top

[Q69] 查看执行计划
来源：http://msr.pycfn.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://oow.smart0.xyz

[Q70] 更新统计信息
来源：http://azw.shzxlz.cn

ANALYZE TABLE users;
来源：http://erh.jyoumei.cn

[Q71] 查看建表语句
来源：http://dey.chenjidiqi.icu

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://qka.mhx1999.top

[Q72] 查看索引
来源：http://jjb.shzxlz.cn

SHOW INDEX FROM users;
来源：http://dle.yuanzhike.top

[Q73] 查看表状态
来源：http://wua.birdmap.top

SHOW TABLE STATUS LIKE 'users';
来源：http://esy.bbcook.cn

[Q74] 强制使用索引
来源：http://txn.nanxinkj.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://lyw.gotoacloud.top

[Q75] 日期格式化
来源：http://pme.yuxming.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://tsl.jinqigfzy.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://vhc.9152youxi.cn

[Q76] 按天统计
来源：http://tla.shanyushiyangkeji.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://cpy.bjfxy.top

[Q77] 时间加减
来源：http://hsu.guowangkeji.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://aqs.zycfv.cn

[Q78] 当前时间
来源：http://ikd.ydzc1.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://zmf.cheryme.top

[Q79] 字符串拼接
来源：http://cdf.hcnkem.com

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://zyw.fengsongda.top

[Q80] 字符串截取
来源：http://btx.uphjek.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://pwg.ywan-chungtsiang.top

[Q81] 字符串替换
来源：http://gll.yj20258888.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://cvv.shanyushiyangkeji.top

[Q82] 字符长度与字节长度
来源：http://kas.xziqi.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://fvf.dashuyun.cn

[Q83] 大小写转换
来源：http://rtq.yangfankeji.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://frz.vqdsnc.cn

[Q84] 去除首尾空格
来源：http://agk.gzhubu.top

SELECT TRIM(name) FROM users;
来源：http://swh.shanyushiyangtech.top

[Q85] 数值取整
来源：http://whj.birdmap.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ghi.jinghuilouyu.cn

[Q86] 读取 JSON 字段
来源：http://zfn.fanxiaobao.xyz

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://qrr.aizwys.cn

[Q87] JSON 字段做条件
来源：http://cfb.sysykeji.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mvl.nwbrower.top

[Q88] 行转列（条件聚合）
来源：http://cyk.vqdsnc.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://fgg.daria6918.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://pht.yanxiufei.cn

[Q89] 判断表是否存在
来源：http://trr.zhoulong.xyz

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://dtx.gaohongyu789.top

[Q90] 生成序号列
来源：http://psb.nwbrower.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://veq.tian-w.cn

================================================================================
来源：http://byq.redwolf501.top

R. Bash 专题
来源：http://kys.vqdsnc.cn

================================================================================
来源：http://tzw.zhijiandao.cn

[R01] shebang 与严格模式
来源：http://bfc.xuetiantiany.cn

#!/usr/bin/env bash
来源：http://znl.nwbrower.top

set -euo pipefail
来源：http://ogy.zhongyouzk.top

[R02] 变量赋值与使用
来源：http://ddr.uphjek.com

name="Tom"; echo "$name"
来源：http://lfu.zhongyouzk.top

[R03] 只读变量
来源：http://nmy.nanxinkj.top

readonly PI=3.14
来源：http://wll.yj20258888.top

[R04] 位置参数
来源：http://rwm.jinqigufen.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://lrr.mhx1999.top

[R05] 参数默认值
来源：http://xkd.tanke756.top

name="${1:-default}"
来源：http://pdy.chenlongwang.top

[R06] 判断命令是否存在
来源：http://zgt.yuanzhike.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://fux.zhongyouzk.top

[R07] if 判断文件
来源：http://job.ydjk.org.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ukx.cqqwz.cn

[R08] 数值比较
来源：http://est.wangdashe.top

if (( a > b )); then echo "a 更大"; fi
来源：http://fla.hnxiangtu.top

[R09] 字符串比较
来源：http://qdd.ehwqpu.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ccy.tian-w.cn

[R10] 正则匹配
来源：http://cmc.jyoumei.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://qge.jyoumei.cn

[R11] case 多分支
来源：http://ldc.guowangkeji.top

case "$1" in
来源：http://imj.yangfankeji.com

start) echo "启动" ;;
来源：http://jco.yuanzhike.top

stop)  echo "停止" ;;
来源：http://pym.jianghu66.top

*)     echo "未知命令" ;;
来源：http://lhv.c1oappe.top

esac
来源：http://hru.bbcook.cn

[R12] for 遍历文件
来源：http://zas.gzhubu.top

for f in *.txt; do echo "$f"; done
来源：http://vhj.tarul.cn

[R13] for 计数循环
来源：http://ukb.zdbjq.cn

for i in {1..10}; do echo "$i"; done
来源：http://img.jinqigufen.top

[R14] C 风格 for
来源：http://nvs.316326.xyz

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://pwt.dianchejie.cn

[R15] while 逐行读文件
来源：http://qay.yj20258.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://stb.hfpthk.cn

[R16] until 等待条件
来源：http://ivg.ppjwa.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://kyf.dianchejie.cn

[R17] 数组定义与取值
来源：http://oid.yueranfly.top

arr=(a b c); echo "${arr[0]}"
来源：http://otu.nanxinkj.top

[R18] 遍历数组
来源：http://wra.zhongyouzk.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://irz.quarkkingdee.top

[R19] 数组长度
来源：http://krg.bjfxy.top

echo "${#arr[@]}"
来源：http://eub.zhaomingkeji.xyz

[R20] 关联数组（字典）
来源：http://ani.uphjek.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mli.jqgfzy.top

[R21] 字符串长度
来源：http://eao.yfazqb.com

echo "${#s}"
来源：http://bnx.aizwys.cn

[R22] 截取子串
来源：http://suy.epnwcf.com

echo "${s:0:5}"
来源：http://mfr.nanxinkj.top

[R23] 字符串替换
来源：http://yxk.daxiang520.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://zns.0kj1m.cn

[R24] 大小写转换
来源：http://ruu.jianghu66.top

echo "${s^^}"; echo "${s,,}"
来源：http://lms.sxryk.cn

[R25] 去后缀 / 去前缀
来源：http://lqx.yonumen.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://ntz.zhongyouzk.top

[R26] 命令替换
来源：http://ujg.yuxming.cn

now=$(date +%F); echo "$now"
来源：http://xdi.birdmap.top

[R27] 算术展开
来源：http://vcb.cashguo.top

echo $((1 + 2 * 3))
来源：http://odt.sweek.top

[R28] 浮点运算
来源：http://qyb.bjfxy.top

echo "scale=2; 10/3" | bc
来源：http://lih.gaohongyu789.top

[R29] 定义函数
来源：http://wne.9152youxi.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://zaa.ydzc1.top

[R30] 函数返回状态码
来源：http://zxu.shuidangran.top

f() { return 0; }; f || echo "失败了"
来源：http://fnv.hfpthk.cn

[R31] 局部变量
来源：http://tmh.quarkkingdee.top

f() { local x=1; echo "$x"; }
来源：http://pxu.0kj1m.cn

[R32] 参数个数校验
来源：http://mxj.tianlin.xyz

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://byg.hnqzz.top

[R33] 捕获错误并提示行号
来源：http://nhq.gogol.net.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://vbq.fengsongda.top

[R34] 退出时清理
来源：http://jno.bbcook.cn

trap 'rm -f "$tmp"' EXIT
来源：http://bak.aibaodan.cn

[R35] 后台执行并等待
来源：http://jvg.shuidangran.top

sleep 5 & pid=$!; wait "$pid"
来源：http://vnw.0kj1m.cn

[R36] 并发执行多个任务
来源：http://szm.zhengqikj.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://age.ybcxt.top

[R37] 把输出赋给变量
来源：http://wei.uphjek.com

files=$(ls -1)
来源：http://fnh.havefunace.top

[R38] 管道串联
来源：http://lpz.daxiang520.top

cat a.txt | grep -i error | wc -l
来源：http://bph.iojbl.cn

[R39] 重定向标准输出与错误
来源：http://gpx.yueranfly.top

cmd > out.log 2>&1
来源：http://wdx.ppjwa.cn

[R40] 追加写日志
来源：http://zyt.yanxiufei.cn

echo "log" >> out.log
来源：http://woo.mhx1999.top

[R41] 丢弃输出
来源：http://sqp.daria6918.cn

cmd >/dev/null 2>&1
来源：http://nqb.tarul.cn

[R42] 输入重定向
来源：http://vpn.guannengcc.top

wc -l < a.txt
来源：http://sqk.zdqjudy.top

[R43] 按名字查找文件
来源：http://bmv.ywan-chungtsiang.top

find . -name "*.log" -type f
来源：http://vgu.shanyushiyangkeji.top

[R44] 按修改时间查找
来源：http://unc.316326.xyz

find . -mtime -7 -type f
来源：http://fsk.gaohongyu789.top

[R45] 批量删除
来源：http://aqp.snrcjt.cn

find . -name "*.tmp" -delete
来源：http://ylx.yuxming.cn

[R46] 递归替换文件内容
来源：http://yjd.meibo888.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://nii.chenjidiqi.icu

[R47] sed 单行替换
来源：http://zax.bjfxy.top

sed -i 's/foo/bar/g' a.txt
来源：http://def.epnwcf.com

[R48] awk 取指定列
来源：http://ije.ywan-chungtsiang.top

awk '{print $1, $3}' a.txt
来源：http://var.snrcjt.cn

[R49] awk 带条件
来源：http://abr.fehbvm.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wcy.guowangkeji.top

[R50] awk 求和
来源：http://qyx.nanxuanxn.top

awk '{s += $2} END {print s}' a.txt
来源：http://dia.zycfv.cn

[R51] 排序去重取前几
来源：http://czm.sjlbkw.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://lys.shangyingyoupin.top

[R52] 统计行数
来源：http://osr.shuidangran.top

wc -l a.txt
来源：http://cob.andypj.xyz

[R53] 查看文件头与实时尾
来源：http://emj.zycfv.cn


<!-- 参考信息 -->