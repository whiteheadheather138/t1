代发 wailian999

================================================================================
来源：http://udj.cucudq.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://rfx.vqdsnc.cn

================================================================================
来源：http://tms.ydjk.org.cn

[Q01] 创建表
来源：http://fbg.xinyue.icu

CREATE TABLE users (
来源：http://aex.chenjidiqi.icu

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://rrd.zhixingplan.top

name VARCHAR(50) NOT NULL,
来源：http://zhw.fehbvm.com

email VARCHAR(100) UNIQUE,
来源：http://foa.fehbvm.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://aeg.uphjek.com

);
来源：http://yld.hnxiangtu.top

[Q02] 创建带外键的表
来源：http://vqf.andypj.xyz

CREATE TABLE orders (
来源：http://xqz.yuxming.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://pch.zdqjudy.top

user_id INT NOT NULL,
来源：http://lgq.iojbl.cn

amount DECIMAL(10, 2),
来源：http://eiu.birdmap.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://cwk.shangyingyoupin.top

);
来源：http://jhk.xuanzx.com

[Q03] 增加列
来源：http://hfw.hesvh.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://jyx.9152youxi.cn

[Q04] 修改列类型
来源：http://dvb.hnxiangtu.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://jtw.yj20258888.top

[Q05] 重命名列
来源：http://jra.sjlbkw.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://kuy.52xcode.cn

[Q06] 删除列
来源：http://gbb.fktsv.cn

ALTER TABLE users DROP COLUMN age;
来源：http://rcg.ivvv.top

[Q07] 删除表
来源：http://qpt.xziqi.cn

DROP TABLE IF EXISTS orders;
来源：http://ale.tianlin.xyz

[Q08] 创建普通索引
来源：http://men.cashguo.top

CREATE INDEX idx_users_email ON users(email);
来源：http://wbe.uphjek.com

[Q09] 创建唯一索引
来源：http://yyu.ehwqpu.com

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ole.jinyuanbaomall.cn

[Q10] 插入单行
来源：http://ivz.zhaomingkeji.xyz

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ytr.ivvv.top

[Q11] 一次插入多行
来源：http://seg.cashguo.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://lwc.tanke756.top

[Q12] 插入后取自增 ID
来源：http://onx.shangyingyoupin.top

INSERT INTO users (name) VALUES ('C');
来源：http://yrr.shzxlz.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://qcq.fehbvm.com

[Q13] 忽略重复插入
来源：http://ego.tanke756.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://kvn.havefunace.top

[Q14] 存在则更新（upsert）
来源：http://vwt.fktsv.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mgp.pengpengdd.cyou

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://oml.sxryk.cn

[Q15] 查询全部
来源：http://mwm.vqdsnc.cn

SELECT * FROM users;
来源：http://ies.epnwcf.com

[Q16] 查询指定列
来源：http://sfz.vehdjk.com

SELECT id, name FROM users;
来源：http://nsc.yanxiufei.cn

[Q17] 条件查询
来源：http://ivl.ivvv.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://rrb.hfpthk.cn

[Q18] 模糊匹配
来源：http://diz.yonumen.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://nju.shuidangran.top

[Q19] 范围查询
来源：http://zer.aibaodan.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://umt.haohaochexian.top

[Q20] IN 列表
来源：http://zyd.quarkkingdee.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://scx.sjlbkw.cn

[Q21] 空值判断
来源：http://uzf.guannengcc.top

SELECT * FROM users WHERE email IS NULL;
来源：http://sjz.kuanghao11.cn

[Q22] 排序
来源：http://eaz.zhoulong.xyz

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://whd.zdbjq.cn

[Q23] 分页
来源：http://uxt.sufxvd.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://dqj.wangdashe.top

[Q24] 去重
来源：http://vfd.shanyushiyangtech.top

SELECT DISTINCT city FROM users;
来源：http://bmr.shuidangran.top

[Q25] 只取前 N 条
来源：http://uhv.shanyushiyangkeji.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://fbw.feifeiyinyue.top

[Q26] 计数
来源：http://xsj.pycfn.com

SELECT COUNT(*) FROM users;
来源：http://uhe.316326.xyz

[Q27] 条件计数
来源：http://mwh.gogol.net.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wgh.yuxming.cn

[Q28] 求和与平均
来源：http://drm.ctjpmb.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://fms.zhijiandao.cn

[Q29] 最大最小值
来源：http://ypx.sysykeji.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://eug.sxryk.cn

[Q30] 分组统计
来源：http://sts.yj20258.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://jmh.chenzaomai.com

[Q31] 分组后过滤
来源：http://icj.ywan-chungtsiang.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://cod.snrcjt.cn

[Q32] 分组拼接字符串
来源：http://vlb.zhengqikj.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://gxj.yuanzhike.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://vai.xziqi.cn

[Q33] 多列分组
来源：http://dym.yangfankeji.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://xmi.cqqwz.cn

[Q34] 每组取第一条
来源：http://nti.52xcode.cn

SELECT * FROM (
来源：http://lvw.zhaomingkeji.xyz

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ipo.yanxiufei.cn

) t WHERE rn = 1;
来源：http://pzs.xinyue.icu

[Q35] 内连接
来源：http://enj.ehwqpu.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hha.yvedp.cn

[Q36] 左连接
来源：http://kdd.pycfn.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://plz.0kj1m.cn

[Q37] 右连接
来源：http://wzj.cucudq.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://vyp.chenzaomai.com

[Q38] 全外连接（PostgreSQL）
来源：http://ses.zhongyouzk.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ufp.shuidangran.top

[Q39] 自连接（查上下级）
来源：http://yws.hongshengwenyu.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://xpq.fktsv.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://isx.jinqigufen.top

[Q40] 交叉连接（笛卡尔积）
来源：http://ize.smart0.xyz

SELECT * FROM colors CROSS JOIN sizes;
来源：http://stw.ctjpmb.com

[Q41] 多表连接
来源：http://fpz.feifeiyinyue.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://eaa.zhoulong.xyz

JOIN users u ON u.id = o.user_id
来源：http://sjh.hnxiangtu.top

JOIN products p ON p.id = o.product_id;
来源：http://xse.xylfe.cn

[Q42] 连接条件附加过滤
来源：http://let.iojbl.cn

SELECT u.name, o.amount FROM users u
来源：http://hgl.hcnkem.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://abo.smart0.xyz

[Q43] 标量子查询
来源：http://wpy.mhx1999.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://kdy.xziqi.cn

[Q44] IN 子查询
来源：http://lzw.52xcode.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ers.hnxiangtu.top

[Q45] EXISTS 判断存在
来源：http://cav.tarul.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hju.cdnleiting.top

[Q46] NOT EXISTS 判断不存在
来源：http://ctm.hesvh.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://plf.cashguo.top

[Q47] 与平均值比较
来源：http://ist.hfpthk.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://syv.chenlongwang.top

[Q48] CTE 公用表表达式
来源：http://hes.jinqigfzy.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://lqb.shzxlz.cn

SELECT * FROM t WHERE c > 5;
来源：http://qfw.yj20258888.top

[Q49] 更新单行
来源：http://iub.nanxuanxn.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://vuo.jqgufenzy.top

[Q50] 批量更新
来源：http://hdu.hysaishi.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://kgo.ydzc1.top

[Q51] 用子查询更新
来源：http://vwc.yvedp.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://vll.meibo888.top

[Q52] 删除指定行
来源：http://mwe.hnxiangtu.top

DELETE FROM users WHERE id = 10;
来源：http://drn.xinyue.icu

[Q53] 按条件删除
来源：http://etg.nwbrower.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hef.9152youxi.cn

[Q54] 清空表
来源：http://vok.yueranfly.top

TRUNCATE TABLE logs;
来源：http://oza.jqgfzy.top

[Q55] 排名（并列占位）
来源：http://tux.gaohongyu789.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://kii.feifeiyinyue.top

[Q56] 密集排名（并列不占位）
来源：http://irh.redwolf501.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://toe.xingfuxueyuan.xyz

[Q57] 行号
来源：http://uln.ppjwa.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wbt.sxryk.cn

[Q58] 累计求和
来源：http://kkm.zycfv.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://rzi.kuanghao11.cn

[Q59] 分组内累计
来源：http://lgz.shzxlz.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://vmh.fanxiaobao.xyz

[Q60] 取上一行 / 下一行
来源：http://soq.52xcode.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://uoc.guowangkeji.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://isx.jiagoushi.top

[Q61] 移动平均
来源：http://ytn.hongshengwenyu.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://umv.yanxiufei.cn

[Q62] 分组占比
来源：http://jpf.vehdjk.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://enp.fzhhl.top

[Q63] 开启事务
来源：http://jhb.sufxvd.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://lwg.yueranfly.top

[Q64] 提交事务
来源：http://wlh.gzhubu.top

COMMIT;
来源：http://hjk.yfazqb.com

[Q65] 回滚事务
来源：http://ssb.cheryme.top

ROLLBACK;
来源：http://pim.yonumen.top

[Q66] 行锁查询
来源：http://ewk.wangdashe.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://gyr.jlsjyb.cn

[Q67] 设置隔离级别
来源：http://bir.iojbl.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://vhb.hcnkem.com

[Q68] 保存点
来源：http://kkx.yj202588.top

SAVEPOINT sp1;
来源：http://qnm.hfpthk.cn

ROLLBACK TO sp1;
来源：http://npb.andypj.xyz

[Q69] 查看执行计划
来源：http://eek.9152youxi.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mrz.ivvv.top

[Q70] 更新统计信息
来源：http://vpi.zycfv.cn

ANALYZE TABLE users;
来源：http://giy.316326.xyz

[Q71] 查看建表语句
来源：http://eiw.zhaomingkeji.xyz

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hxz.sysykeji.top

[Q72] 查看索引
来源：http://jpl.zhengqikj.top

SHOW INDEX FROM users;
来源：http://hba.vehdjk.com

[Q73] 查看表状态
来源：http://bek.52xcode.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://lnh.fengsongda.top

[Q74] 强制使用索引
来源：http://vvg.fzhhl.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://cyz.guowangkeji.top

[Q75] 日期格式化
来源：http://mvm.tianlin.xyz

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://lcu.daxiang520.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://cgz.uphjek.com

[Q76] 按天统计
来源：http://lxy.xingfuxueyuan.xyz

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://dai.yj20258888.top

[Q77] 时间加减
来源：http://ltz.ydzc1.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://fnl.guannengcc.top

[Q78] 当前时间
来源：http://qbt.iojbl.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://icu.c1oappe.top

[Q79] 字符串拼接
来源：http://vyk.dianchejie.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://zvs.guowangkeji.top

[Q80] 字符串截取
来源：http://zgu.aizwys.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://pba.cheryme.top

[Q81] 字符串替换
来源：http://pae.vehdjk.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://jzf.andypj.xyz

[Q82] 字符长度与字节长度
来源：http://dzo.ydzc1.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://tze.hongshengwenyu.top

[Q83] 大小写转换
来源：http://ruo.zhiwuduotai.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://rzf.redwolf501.top

[Q84] 去除首尾空格
来源：http://blu.svipenyu.cn

SELECT TRIM(name) FROM users;
来源：http://zwl.hammf.cn

[Q85] 数值取整
来源：http://yqw.fanxiaobao.xyz

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ost.meibo888.top

[Q86] 读取 JSON 字段
来源：http://zco.zycfv.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://yfo.sufxvd.cn

[Q87] JSON 字段做条件
来源：http://ggg.gzhubu.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://gaq.zhiwuduotai.top

[Q88] 行转列（条件聚合）
来源：http://jea.daria6918.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://uwr.jqgfzy.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://avd.0kj1m.cn

[Q89] 判断表是否存在
来源：http://unm.haohaochexian.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://pyb.epnwcf.com

[Q90] 生成序号列
来源：http://jjf.jlsjyb.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://dff.ydzc1.top

================================================================================
来源：http://ryl.ydzc1.top

R. Bash 专题
来源：http://gdh.yj202588.top

================================================================================
来源：http://lhl.aizwys.cn

[R01] shebang 与严格模式
来源：http://gik.nanxuanxn.top

#!/usr/bin/env bash
来源：http://uib.jinqigfzy.top

set -euo pipefail
来源：http://pot.pengpengdd.cyou

[R02] 变量赋值与使用
来源：http://rmr.cashguo.top

name="Tom"; echo "$name"
来源：http://gta.tianlin.xyz

[R03] 只读变量
来源：http://odc.uphjek.com

readonly PI=3.14
来源：http://jwm.hesvh.cn

[R04] 位置参数
来源：http://svq.aibaodan.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://bcd.kuanghao11.cn

[R05] 参数默认值
来源：http://juk.gzhubu.top

name="${1:-default}"
来源：http://dtj.yueranfly.top

[R06] 判断命令是否存在
来源：http://fuv.bbcook.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://abh.jlsjyb.cn

[R07] if 判断文件
来源：http://hct.gzhubu.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ycj.yj20258888.top

[R08] 数值比较
来源：http://itp.hnqzz.top

if (( a > b )); then echo "a 更大"; fi
来源：http://uvu.shanyushiyangtech.top

[R09] 字符串比较
来源：http://swy.shzxlz.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://xrg.andypj.xyz

[R10] 正则匹配
来源：http://lli.nwbrower.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://rkp.epnwcf.com

[R11] case 多分支
来源：http://wqu.jqgfzy.top

case "$1" in
来源：http://zlf.zdqjudy.top

start) echo "启动" ;;
来源：http://ajn.yuanzhike.top

stop)  echo "停止" ;;
来源：http://tkq.iojbl.cn

*)     echo "未知命令" ;;
来源：http://dmz.gogol.net.cn

esac
来源：http://wwp.gaohongyu789.top

[R12] for 遍历文件
来源：http://cqg.0kj1m.cn

for f in *.txt; do echo "$f"; done
来源：http://owh.tian-w.cn

[R13] for 计数循环
来源：http://hnb.zhengqikj.top

for i in {1..10}; do echo "$i"; done
来源：http://jet.tanke756.top

[R14] C 风格 for
来源：http://huo.ywan-chungtsiang.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ens.zhengqikj.top

[R15] while 逐行读文件
来源：http://hys.daxiang520.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://tek.9152youxi.cn

[R16] until 等待条件
来源：http://mhw.vqdsnc.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://okn.hammf.cn

[R17] 数组定义与取值
来源：http://xwg.chenlongwang.top

arr=(a b c); echo "${arr[0]}"
来源：http://dnq.zhongyouzk.top

[R18] 遍历数组
来源：http://ygc.gotoacloud.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ahb.mhx1999.top

[R19] 数组长度
来源：http://jgn.fengsongda.top

echo "${#arr[@]}"
来源：http://xwr.sysykeji.top

[R20] 关联数组（字典）
来源：http://tob.jinqigfzy.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ltn.yangfankeji.com

[R21] 字符串长度
来源：http://wyg.xylfe.cn

echo "${#s}"
来源：http://xgn.jinqigufen.top

[R22] 截取子串
来源：http://ziu.fzhhl.top

echo "${s:0:5}"
来源：http://ekl.hywenlv.cn

[R23] 字符串替换
来源：http://pkt.ydjk.org.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://iyb.yonumen.top

[R24] 大小写转换
来源：http://bgs.zhixingplan.top

echo "${s^^}"; echo "${s,,}"
来源：http://jul.zhixingplan.top

[R25] 去后缀 / 去前缀
来源：http://pzm.ydjk.org.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://pam.nanxinkj.top

[R26] 命令替换
来源：http://eml.daria6918.cn

now=$(date +%F); echo "$now"
来源：http://xlq.xingfuxueyuan.xyz

[R27] 算术展开
来源：http://kqy.xylfe.cn

echo $((1 + 2 * 3))
来源：http://xqv.yuanzhike.top

[R28] 浮点运算
来源：http://afq.birdmap.top

echo "scale=2; 10/3" | bc
来源：http://rco.yueranfly.top

[R29] 定义函数
来源：http://wbc.gogol.net.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://jbc.jqgfzy.top

[R30] 函数返回状态码
来源：http://cyu.dashuyun.cn

f() { return 0; }; f || echo "失败了"
来源：http://got.ydzc1.top

[R31] 局部变量
来源：http://gtz.yonumen.top

f() { local x=1; echo "$x"; }
来源：http://duz.xziqi.cn

[R32] 参数个数校验
来源：http://bjc.bbcook.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://toz.cdnleiting.top

[R33] 捕获错误并提示行号
来源：http://qkz.tian-w.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://dlt.bjfxy.top

[R34] 退出时清理
来源：http://msn.jinqigufen.top

trap 'rm -f "$tmp"' EXIT
来源：http://ter.9152youxi.cn

[R35] 后台执行并等待
来源：http://asz.aizwys.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://rrd.jyoumei.cn

[R36] 并发执行多个任务
来源：http://xdq.sysykeji.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://uzg.gaohongyu789.top

[R37] 把输出赋给变量
来源：http://vvb.yuxming.cn

files=$(ls -1)
来源：http://cqy.wangdashe.top

[R38] 管道串联
来源：http://udt.chenjidiqi.icu

cat a.txt | grep -i error | wc -l
来源：http://bxy.yongpay.top

[R39] 重定向标准输出与错误
来源：http://pfn.zhiwuduotai.top

cmd > out.log 2>&1
来源：http://bhw.vehdjk.com

[R40] 追加写日志
来源：http://xbc.xylfe.cn

echo "log" >> out.log
来源：http://nij.jinyuanbaomall.cn

[R41] 丢弃输出
来源：http://ano.ybcxt.top

cmd >/dev/null 2>&1
来源：http://vle.xinyue.icu

[R42] 输入重定向
来源：http://udm.9152youxi.cn

wc -l < a.txt
来源：http://psy.sufxvd.cn

[R43] 按名字查找文件
来源：http://dfm.iojbl.cn


<!-- 参考信息 -->