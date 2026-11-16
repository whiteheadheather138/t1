代发 wailian999

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://tpo.svipenyu.cn

[Q05] 重命名列
来源：http://hbq.shanyushiyangtech.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://jvm.nanxuanxn.top

[Q06] 删除列
来源：http://nwi.yanxiufei.cn

ALTER TABLE users DROP COLUMN age;
来源：http://jbi.zdqjudy.top

[Q07] 删除表
来源：http://kud.shanyushiyangkeji.top

DROP TABLE IF EXISTS orders;
来源：http://fja.zdbjq.cn

[Q08] 创建普通索引
来源：http://uol.jianghu66.top

CREATE INDEX idx_users_email ON users(email);
来源：http://rwt.jyoumei.cn

[Q09] 创建唯一索引
来源：http://hqe.shzxlz.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hot.sufxvd.cn

[Q10] 插入单行
来源：http://pip.shanyushiyangkeji.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://joe.pycfn.com

[Q11] 一次插入多行
来源：http://xrf.sxryk.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://iai.dianchejie.cn

[Q12] 插入后取自增 ID
来源：http://wpg.hnxiangtu.top

INSERT INTO users (name) VALUES ('C');
来源：http://xfk.nanxinkj.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://jvj.gzhubu.top

[Q13] 忽略重复插入
来源：http://iqb.hywenlv.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://pnb.guannengcc.top

[Q14] 存在则更新（upsert）
来源：http://doa.jiagoushi.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://qcr.kuanghao11.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://dny.hcnkem.com

[Q15] 查询全部
来源：http://bhd.epnwcf.com

SELECT * FROM users;
来源：http://fho.hammf.cn

[Q16] 查询指定列
来源：http://oqv.sxryk.cn

SELECT id, name FROM users;
来源：http://cew.jinqigfzy.top

[Q17] 条件查询
来源：http://yvy.zhongyouzk.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ops.vehdjk.com

[Q18] 模糊匹配
来源：http://qww.cheryme.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://dte.kuanghao11.cn

[Q19] 范围查询
来源：http://ilx.zdqjudy.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://egh.shangyingyoupin.top

[Q20] IN 列表
来源：http://grz.tarul.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hod.hysaishi.cn

[Q21] 空值判断
来源：http://dtk.chenlongwang.top

SELECT * FROM users WHERE email IS NULL;
来源：http://zon.meibo888.top

[Q22] 排序
来源：http://zue.hywenlv.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://kul.yj202588.top

[Q23] 分页
来源：http://kab.zhixingplan.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://xpa.xylfe.cn

[Q24] 去重
来源：http://ned.ppjwa.cn

SELECT DISTINCT city FROM users;
来源：http://jgr.ydjk.org.cn

[Q25] 只取前 N 条
来源：http://eqt.jianghu66.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ydn.jianghu66.top

[Q26] 计数
来源：http://oqh.guannengcc.top

SELECT COUNT(*) FROM users;
来源：http://kjm.hesvh.cn

[Q27] 条件计数
来源：http://zlt.redwolf501.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://cdq.shangyingyoupin.top

[Q28] 求和与平均
来源：http://pdi.bjfxy.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://vmy.jianghu66.top

[Q29] 最大最小值
来源：http://eat.nanxuanxn.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://laz.xuetiantiany.cn

[Q30] 分组统计
来源：http://jjf.shuidangran.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://rpg.ybcxt.top

[Q31] 分组后过滤
来源：http://jls.zdqjudy.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://nhf.xinyue.icu

[Q32] 分组拼接字符串
来源：http://qie.ppjwa.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://rct.nanxuanxn.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://sjn.0kj1m.cn

[Q33] 多列分组
来源：http://qwk.tarul.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://tdb.gaohongyu789.top

[Q34] 每组取第一条
来源：http://jix.zycfv.cn

SELECT * FROM (
来源：http://gzi.cqqwz.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://dxf.jinghuilouyu.cn

) t WHERE rn = 1;
来源：http://hov.ywan-chungtsiang.top

[Q35] 内连接
来源：http://nqv.jqgufenzy.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wmo.aibaodan.cn

[Q36] 左连接
来源：http://rcg.shzxlz.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://vqk.bbcook.cn

[Q37] 右连接
来源：http://mpt.ppjwa.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mcb.gogol.net.cn

[Q38] 全外连接（PostgreSQL）
来源：http://pkq.zhaomingkeji.xyz

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://smx.jinyuanbaomall.cn

[Q39] 自连接（查上下级）
来源：http://ccz.ydzc1.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://uwr.guannengcc.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://nft.havefunace.top

[Q40] 交叉连接（笛卡尔积）
来源：http://aya.smart0.xyz

SELECT * FROM colors CROSS JOIN sizes;
来源：http://frk.nanxinkj.top

[Q41] 多表连接
来源：http://tty.hcnkem.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://jfh.hysaishi.cn

JOIN users u ON u.id = o.user_id
来源：http://qnd.tian-w.cn

JOIN products p ON p.id = o.product_id;
来源：http://ach.jinqigufen.top

[Q42] 连接条件附加过滤
来源：http://lha.zycfv.cn

SELECT u.name, o.amount FROM users u
来源：http://nyl.xuetiantiany.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://kuo.aibaodan.cn

[Q43] 标量子查询
来源：http://fce.ybcxt.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://was.ehwqpu.com

[Q44] IN 子查询
来源：http://vnr.52xcode.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mlh.vqdsnc.cn

[Q45] EXISTS 判断存在
来源：http://jwq.yfazqb.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ciu.jqgufenzy.top

[Q46] NOT EXISTS 判断不存在
来源：http://lxx.hcnkem.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hqn.tarul.cn

[Q47] 与平均值比较
来源：http://ceb.zhixingplan.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://vwj.tian-w.cn

[Q48] CTE 公用表表达式
来源：http://brw.hfpthk.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ewr.cdnleiting.top

SELECT * FROM t WHERE c > 5;
来源：http://bfz.jlsjyb.cn

[Q49] 更新单行
来源：http://plf.nanxuanxn.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://tzj.yj20258.top

[Q50] 批量更新
来源：http://wvq.jinqigufen.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wov.ctjpmb.com

[Q51] 用子查询更新
来源：http://kwf.yonumen.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mbb.chenjidiqi.icu

[Q52] 删除指定行
来源：http://lyq.shanyushiyangkeji.top

DELETE FROM users WHERE id = 10;
来源：http://adg.cheryme.top

[Q53] 按条件删除
来源：http://abw.jiagoushi.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://tav.sufxvd.cn

[Q54] 清空表
来源：http://law.shanyushiyangtech.top

TRUNCATE TABLE logs;
来源：http://mcs.cheryme.top

[Q55] 排名（并列占位）
来源：http://agk.jiagoushi.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ulu.jqgufenzy.top

[Q56] 密集排名（并列不占位）
来源：http://gix.fehbvm.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://sbt.yueranfly.top

[Q57] 行号
来源：http://hwf.sysykeji.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://eow.bbcook.cn

[Q58] 累计求和
来源：http://sof.zhoulong.xyz

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ehq.0kj1m.cn

[Q59] 分组内累计
来源：http://ypk.mhx1999.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://zmh.vqdsnc.cn

[Q60] 取上一行 / 下一行
来源：http://mas.gaohongyu789.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://svz.sxryk.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://qen.ydzc1.top

[Q61] 移动平均
来源：http://vxn.jinqigfzy.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://flr.zhaomingkeji.xyz

[Q62] 分组占比
来源：http://skt.yuxming.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://yhd.fktsv.cn

[Q63] 开启事务
来源：http://dyo.hesvh.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://sxc.cheryme.top

[Q64] 提交事务
来源：http://unx.havefunace.top

COMMIT;
来源：http://hnb.jinghuilouyu.cn

[Q65] 回滚事务
来源：http://ovc.hesvh.cn

ROLLBACK;
来源：http://msz.jqgfzy.top

[Q66] 行锁查询
来源：http://swj.sysykeji.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://eyb.316326.xyz

[Q67] 设置隔离级别
来源：http://hoz.zdbjq.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://dkx.ybcxt.top

[Q68] 保存点
来源：http://oua.birdmap.top

SAVEPOINT sp1;
来源：http://mrs.xziqi.cn

ROLLBACK TO sp1;
来源：http://mmn.shuidangran.top

[Q69] 查看执行计划
来源：http://xsu.gaohongyu789.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://rlo.meibo888.top

[Q70] 更新统计信息
来源：http://rku.havefunace.top

ANALYZE TABLE users;
来源：http://thw.hongshengwenyu.top

[Q71] 查看建表语句
来源：http://eik.yanxiufei.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ihe.xuetiantiany.cn

[Q72] 查看索引
来源：http://ftl.nwbrower.top

SHOW INDEX FROM users;
来源：http://usj.wangdashe.top

[Q73] 查看表状态
来源：http://xin.c1oappe.top

SHOW TABLE STATUS LIKE 'users';
来源：http://vli.yangfankeji.com

[Q74] 强制使用索引
来源：http://lal.jqgufenzy.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://qwv.jiagoushi.top

[Q75] 日期格式化
来源：http://pbt.snrcjt.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://zcl.jyoumei.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://uql.hfpthk.cn

[Q76] 按天统计
来源：http://mkj.yuxming.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hae.cashguo.top

[Q77] 时间加减
来源：http://zdw.quarkkingdee.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ftz.gogol.net.cn

[Q78] 当前时间
来源：http://mrz.yonumen.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hib.feifeiyinyue.top

[Q79] 字符串拼接
来源：http://omz.havefunace.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ykc.svipenyu.cn

[Q80] 字符串截取
来源：http://fks.hnqzz.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://dst.fktsv.cn

[Q81] 字符串替换
来源：http://qkw.9152youxi.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://vao.vqdsnc.cn

[Q82] 字符长度与字节长度
来源：http://anu.shuidangran.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ohs.jianghu66.top

[Q83] 大小写转换
来源：http://fon.yanxiufei.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://rhq.jinyuanbaomall.cn

[Q84] 去除首尾空格
来源：http://noz.yonumen.top

SELECT TRIM(name) FROM users;
来源：http://wlo.ywan-chungtsiang.top

[Q85] 数值取整
来源：http://gvf.birdmap.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://dmp.wangdashe.top

[Q86] 读取 JSON 字段
来源：http://vtj.jianghu66.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mot.ehwqpu.com

[Q87] JSON 字段做条件
来源：http://gyh.ydzc1.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://bdz.chenlongwang.top

[Q88] 行转列（条件聚合）
来源：http://gzv.jiagoushi.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://zbx.tian-w.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://lom.yueranfly.top

[Q89] 判断表是否存在
来源：http://gfb.hammf.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://dmd.kuanghao11.cn

[Q90] 生成序号列
来源：http://yjq.zhiwuduotai.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://kic.bjfxy.top

================================================================================
来源：http://uwe.yueranfly.top

R. Bash 专题
来源：http://pbu.zhoulong.xyz

================================================================================
来源：http://lfg.0kj1m.cn

[R01] shebang 与严格模式
来源：http://tso.sufxvd.cn

#!/usr/bin/env bash
来源：http://ika.c1oappe.top

set -euo pipefail
来源：http://xpi.zdqjudy.top

[R02] 变量赋值与使用
来源：http://kcd.tarul.cn

name="Tom"; echo "$name"
来源：http://kah.9152youxi.cn

[R03] 只读变量
来源：http://kbf.zhoulong.xyz

readonly PI=3.14
来源：http://wgt.tian-w.cn

[R04] 位置参数
来源：http://mph.dashuyun.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://zux.ivvv.top

[R05] 参数默认值
来源：http://xtv.fzhhl.top

name="${1:-default}"
来源：http://cpu.cucudq.cn

[R06] 判断命令是否存在
来源：http://umc.yanxiufei.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://vxi.pycfn.com

[R07] if 判断文件
来源：http://xjz.cqqwz.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://qma.kuanghao11.cn

[R08] 数值比较
来源：http://aoa.hnqzz.top

if (( a > b )); then echo "a 更大"; fi
来源：http://mca.ehwqpu.com

[R09] 字符串比较
来源：http://ybz.sysykeji.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://syz.guannengcc.top

[R10] 正则匹配
来源：http://kbu.cheryme.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ndi.sxryk.cn

[R11] case 多分支
来源：http://umw.vehdjk.com

case "$1" in
来源：http://vje.jinqigfzy.top

start) echo "启动" ;;
来源：http://eth.gzhubu.top

stop)  echo "停止" ;;
来源：http://jlb.fzhhl.top

*)     echo "未知命令" ;;
来源：http://fqi.ivvv.top

esac
来源：http://gdp.andypj.xyz

[R12] for 遍历文件
来源：http://lto.daria6918.cn

for f in *.txt; do echo "$f"; done
来源：http://gus.havefunace.top

[R13] for 计数循环
来源：http://nps.daxiang520.top

for i in {1..10}; do echo "$i"; done
来源：http://tfz.jqgfzy.top

[R14] C 风格 for
来源：http://ycm.ppjwa.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://zcf.chenlongwang.top

[R15] while 逐行读文件
来源：http://aop.dashuyun.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://lot.zycfv.cn

[R16] until 等待条件
来源：http://efm.hesvh.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hax.xingfuxueyuan.xyz

[R17] 数组定义与取值
来源：http://ilp.fehbvm.com

arr=(a b c); echo "${arr[0]}"
来源：http://brz.yuxming.cn

[R18] 遍历数组
来源：http://yuo.yvedp.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://yfn.hnxiangtu.top

[R19] 数组长度
来源：http://zzp.gotoacloud.top

echo "${#arr[@]}"
来源：http://glq.cucudq.cn

[R20] 关联数组（字典）
来源：http://rgn.9152youxi.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://qrv.zdqjudy.top

[R21] 字符串长度
来源：http://wkx.yongpay.top

echo "${#s}"
来源：http://yjb.iojbl.cn

[R22] 截取子串
来源：http://gvw.ehwqpu.com

echo "${s:0:5}"
来源：http://ivx.sysykeji.top

[R23] 字符串替换
来源：http://jeb.tianlin.xyz

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://zrt.shanyushiyangkeji.top

[R24] 大小写转换
来源：http://aiy.haohaochexian.top

echo "${s^^}"; echo "${s,,}"
来源：http://uya.haohaochexian.top

[R25] 去后缀 / 去前缀
来源：http://nnp.shangyingyoupin.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://ptp.wangshuangyany.cn

[R26] 命令替换
来源：http://whs.epnwcf.com

now=$(date +%F); echo "$now"
来源：http://yju.sufxvd.cn

[R27] 算术展开
来源：http://zer.cdnleiting.top

echo $((1 + 2 * 3))
来源：http://rax.shangyingyoupin.top

[R28] 浮点运算
来源：http://vro.tianlin.xyz

echo "scale=2; 10/3" | bc
来源：http://zwu.sjlbkw.cn

[R29] 定义函数
来源：http://nat.sjlbkw.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://kav.yuxming.cn

[R30] 函数返回状态码
来源：http://qul.zdqjudy.top

f() { return 0; }; f || echo "失败了"
来源：http://qwv.fanxiaobao.xyz

[R31] 局部变量
来源：http://akl.gotoacloud.top

f() { local x=1; echo "$x"; }
来源：http://hso.cdnleiting.top

[R32] 参数个数校验
来源：http://yiu.hfpthk.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ucr.shanyushiyangkeji.top

[R33] 捕获错误并提示行号
来源：http://cob.xinyue.icu

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ayt.hnqzz.top

[R34] 退出时清理
来源：http://sab.aizwys.cn

trap 'rm -f "$tmp"' EXIT
来源：http://yga.jiagoushi.top

[R35] 后台执行并等待
来源：http://qyh.dianchejie.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://xae.yanxiufei.cn

[R36] 并发执行多个任务
来源：http://jbf.yuxming.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ums.fehbvm.com

[R37] 把输出赋给变量
来源：http://swy.gaohongyu789.top

files=$(ls -1)
来源：http://uzd.yuanzhike.top

[R38] 管道串联
来源：http://upz.xinyue.icu

cat a.txt | grep -i error | wc -l
来源：http://fyo.hesvh.cn

[R39] 重定向标准输出与错误
来源：http://zco.hesvh.cn

cmd > out.log 2>&1
来源：http://xhx.mhx1999.top

[R40] 追加写日志
来源：http://sgw.jianghu66.top

echo "log" >> out.log
来源：http://ovn.ivvv.top

[R41] 丢弃输出
来源：http://eex.hongshengwenyu.top

cmd >/dev/null 2>&1
来源：http://tvf.fktsv.cn

[R42] 输入重定向
来源：http://zcd.zycfv.cn

wc -l < a.txt
来源：http://omr.aizwys.cn

[R43] 按名字查找文件
来源：http://buz.yfazqb.com

find . -name "*.log" -type f
来源：http://ivi.yueranfly.top

[R44] 按修改时间查找
来源：http://qvh.zycfv.cn

find . -mtime -7 -type f
来源：http://hts.sxryk.cn

[R45] 批量删除
来源：http://ovn.cashguo.top

find . -name "*.tmp" -delete
来源：http://qaq.shanyushiyangkeji.top

[R46] 递归替换文件内容
来源：http://oui.shanyushiyangkeji.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://gpo.zdqjudy.top

[R47] sed 单行替换
来源：http://nnj.gotoacloud.top

sed -i 's/foo/bar/g' a.txt
来源：http://met.bbcook.cn

[R48] awk 取指定列
来源：http://wgz.jinqigfzy.top

awk '{print $1, $3}' a.txt
来源：http://sjv.chenzaomai.com

[R49] awk 带条件
来源：http://puz.sysykeji.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://nsv.yanxiufei.cn

[R50] awk 求和
来源：http://woe.feifeiyinyue.top

awk '{s += $2} END {print s}' a.txt
来源：http://dmu.kuanghao11.cn

[R51] 排序去重取前几
来源：http://fjr.jianghu66.top

sort a.txt | uniq -c | sort -rn | head
来源：http://shi.yongpay.top

[R52] 统计行数
来源：http://ojq.xinyue.icu

wc -l a.txt
来源：http://sze.hnxiangtu.top

[R53] 查看文件头与实时尾
来源：http://cli.zycfv.cn


<!-- 参考信息 -->