代发 wailian999

================================================================================
来源：http://rck.bbcook.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://gah.wangdashe.top

================================================================================
来源：http://rog.hfpthk.cn

[Q01] 创建表
来源：http://ujo.yj20258888.top

CREATE TABLE users (
来源：http://vry.jqgufenzy.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://smy.vehdjk.com

name VARCHAR(50) NOT NULL,
来源：http://dus.haohaochexian.top

email VARCHAR(100) UNIQUE,
来源：http://vjz.gotoacloud.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://fnj.yueranfly.top

);
来源：http://hsu.daria6918.cn

[Q02] 创建带外键的表
来源：http://dqz.ppjwa.cn

CREATE TABLE orders (
来源：http://jgo.xuanzx.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wqd.aibaodan.cn

user_id INT NOT NULL,
来源：http://jvz.hesvh.cn

amount DECIMAL(10, 2),
来源：http://wih.zdqjudy.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://pjs.yuanzhike.top

);
来源：http://dsj.zhoulong.xyz

[Q03] 增加列
来源：http://kmo.yuanzhike.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://lfw.jinqigfzy.top

[Q04] 修改列类型
来源：http://hrr.meibo888.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://fsr.vqdsnc.cn

[Q05] 重命名列
来源：http://wvb.gzhubu.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://xmt.birdmap.top

[Q06] 删除列
来源：http://udy.yuanzhike.top

ALTER TABLE users DROP COLUMN age;
来源：http://rzc.iojbl.cn

[Q07] 删除表
来源：http://hgj.epnwcf.com

DROP TABLE IF EXISTS orders;
来源：http://ply.zhongyouzk.top

[Q08] 创建普通索引
来源：http://qyr.xinyue.icu

CREATE INDEX idx_users_email ON users(email);
来源：http://czo.shangyingyoupin.top

[Q09] 创建唯一索引
来源：http://gzs.svipenyu.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hpr.zhengqikj.top

[Q10] 插入单行
来源：http://osk.fanxiaobao.xyz

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://gee.kuanghao11.cn

[Q11] 一次插入多行
来源：http://evk.sweek.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://tpn.52xcode.cn

[Q12] 插入后取自增 ID
来源：http://jsg.daxiang520.top

INSERT INTO users (name) VALUES ('C');
来源：http://tfr.gogol.net.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://bni.jinghuilouyu.cn

[Q13] 忽略重复插入
来源：http://ufq.xinyue.icu

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mwh.sufxvd.cn

[Q14] 存在则更新（upsert）
来源：http://nez.dashuyun.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wsx.tianlin.xyz

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://gym.shuidangran.top

[Q15] 查询全部
来源：http://xyh.jianghu66.top

SELECT * FROM users;
来源：http://ftg.nanxinkj.top

[Q16] 查询指定列
来源：http://jud.ehwqpu.com

SELECT id, name FROM users;
来源：http://wxr.fanxiaobao.xyz

[Q17] 条件查询
来源：http://sav.redwolf501.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://sqq.jinghuilouyu.cn

[Q18] 模糊匹配
来源：http://xnb.daria6918.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://fxv.shzxlz.cn

[Q19] 范围查询
来源：http://syr.xuanzx.com

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://slj.meibo888.top

[Q20] IN 列表
来源：http://ouo.ybcxt.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mry.cashguo.top

[Q21] 空值判断
来源：http://rog.daria6918.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://icy.dashuyun.cn

[Q22] 排序
来源：http://udj.zhoulong.xyz

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://dut.shanyushiyangtech.top

[Q23] 分页
来源：http://gwg.guowangkeji.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://jao.zdbjq.cn

[Q24] 去重
来源：http://ifb.sweek.top

SELECT DISTINCT city FROM users;
来源：http://vqk.ivvv.top

[Q25] 只取前 N 条
来源：http://xyo.wangshuangyany.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://xlz.zhaomingkeji.xyz

[Q26] 计数
来源：http://kuj.xylfe.cn

SELECT COUNT(*) FROM users;
来源：http://hqo.mhx1999.top

[Q27] 条件计数
来源：http://apz.vehdjk.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://yqh.xuanzx.com

[Q28] 求和与平均
来源：http://bfr.sweek.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://pbl.cqqwz.cn

[Q29] 最大最小值
来源：http://fqk.bbcook.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://slw.redwolf501.top

[Q30] 分组统计
来源：http://sdp.zhengqikj.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://pvc.nwbrower.top

[Q31] 分组后过滤
来源：http://ogm.zdbjq.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://pxw.jyoumei.cn

[Q32] 分组拼接字符串
来源：http://vuz.yj20258888.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://dfc.zhongyouzk.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://dbc.cheryme.top

[Q33] 多列分组
来源：http://pom.hammf.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ccn.yfazqb.com

[Q34] 每组取第一条
来源：http://mqs.shuidangran.top

SELECT * FROM (
来源：http://vxh.yueranfly.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://dcf.hysaishi.cn

) t WHERE rn = 1;
来源：http://fls.yonumen.top

[Q35] 内连接
来源：http://bme.yonumen.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://nlh.bbcook.cn

[Q36] 左连接
来源：http://rdt.bjfxy.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://inp.tianlin.xyz

[Q37] 右连接
来源：http://ckm.hnqzz.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://vpu.dashuyun.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ejw.daria6918.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ita.nanxinkj.top

[Q39] 自连接（查上下级）
来源：http://vsv.birdmap.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://htq.hysaishi.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://jcs.epnwcf.com

[Q40] 交叉连接（笛卡尔积）
来源：http://tee.xuetiantiany.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ngn.zhengqikj.top

[Q41] 多表连接
来源：http://omx.fktsv.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://owl.yanxiufei.cn

JOIN users u ON u.id = o.user_id
来源：http://bhr.xziqi.cn

JOIN products p ON p.id = o.product_id;
来源：http://lcy.pengpengdd.cyou

[Q42] 连接条件附加过滤
来源：http://utj.c1oappe.top

SELECT u.name, o.amount FROM users u
来源：http://hje.yangfankeji.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://oys.yangfankeji.com

[Q43] 标量子查询
来源：http://cuy.shangyingyoupin.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ted.nanxinkj.top

[Q44] IN 子查询
来源：http://izk.bbcook.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ydm.aibaodan.cn

[Q45] EXISTS 判断存在
来源：http://cxu.hnqzz.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://sxh.hnxiangtu.top

[Q46] NOT EXISTS 判断不存在
来源：http://cgi.hnxiangtu.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ray.wangdashe.top

[Q47] 与平均值比较
来源：http://ydz.nanxuanxn.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://vsy.52xcode.cn

[Q48] CTE 公用表表达式
来源：http://fen.jinghuilouyu.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://qjk.vehdjk.com

SELECT * FROM t WHERE c > 5;
来源：http://tqj.pengpengdd.cyou

[Q49] 更新单行
来源：http://kto.chenlongwang.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://vfj.zycfv.cn

[Q50] 批量更新
来源：http://kgd.pycfn.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ble.meibo888.top

[Q51] 用子查询更新
来源：http://xcs.birdmap.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://lbn.zycfv.cn

[Q52] 删除指定行
来源：http://ceu.hesvh.cn

DELETE FROM users WHERE id = 10;
来源：http://ceh.zhoulong.xyz

[Q53] 按条件删除
来源：http://xhm.tianlin.xyz

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://jie.fktsv.cn

[Q54] 清空表
来源：http://rln.chenlongwang.top

TRUNCATE TABLE logs;
来源：http://ygn.fengsongda.top

[Q55] 排名（并列占位）
来源：http://rsz.xylfe.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://qws.ivvv.top

[Q56] 密集排名（并列不占位）
来源：http://ocu.mhx1999.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://agr.c1oappe.top

[Q57] 行号
来源：http://kal.birdmap.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mgv.yueranfly.top

[Q58] 累计求和
来源：http://mnw.hammf.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ojm.zhiwuduotai.top

[Q59] 分组内累计
来源：http://yvt.shuidangran.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://lpc.tanke756.top

[Q60] 取上一行 / 下一行
来源：http://hqz.tanke756.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://kys.dianchejie.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wql.zhengqikj.top

[Q61] 移动平均
来源：http://hnk.redwolf501.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://zye.bjfxy.top

[Q62] 分组占比
来源：http://uie.jinghuilouyu.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://lnn.fanxiaobao.xyz

[Q63] 开启事务
来源：http://ypx.fanxiaobao.xyz

START TRANSACTION;                -- 或 BEGIN
来源：http://mxq.gzhubu.top

[Q64] 提交事务
来源：http://emi.zhengqikj.top

COMMIT;
来源：http://niz.jiagoushi.top

[Q65] 回滚事务
来源：http://omz.jinqigfzy.top

ROLLBACK;
来源：http://zfw.xingfuxueyuan.xyz

[Q66] 行锁查询
来源：http://str.tanke756.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://qhk.snrcjt.cn

[Q67] 设置隔离级别
来源：http://qlb.zdbjq.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://qyr.svipenyu.cn

[Q68] 保存点
来源：http://idr.0kj1m.cn

SAVEPOINT sp1;
来源：http://iec.aizwys.cn

ROLLBACK TO sp1;
来源：http://cmq.pengpengdd.cyou

[Q69] 查看执行计划
来源：http://qvl.wangdashe.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://lmj.uphjek.com

[Q70] 更新统计信息
来源：http://tow.daria6918.cn

ANALYZE TABLE users;
来源：http://gzl.cucudq.cn

[Q71] 查看建表语句
来源：http://yzv.uphjek.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://qav.fktsv.cn

[Q72] 查看索引
来源：http://rtq.epnwcf.com

SHOW INDEX FROM users;
来源：http://bep.sweek.top

[Q73] 查看表状态
来源：http://znv.0kj1m.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://rwf.pycfn.com

[Q74] 强制使用索引
来源：http://ffa.shanyushiyangtech.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://kkf.birdmap.top

[Q75] 日期格式化
来源：http://cgy.zhoulong.xyz

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://lei.pycfn.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://rgq.tian-w.cn

[Q76] 按天统计
来源：http://rqx.jqgfzy.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://gwq.jlsjyb.cn

[Q77] 时间加减
来源：http://hpk.sxryk.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://uxu.gogol.net.cn

[Q78] 当前时间
来源：http://qzu.ehwqpu.com

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://jfi.hnqzz.top

[Q79] 字符串拼接
来源：http://sxt.jinghuilouyu.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mhf.cashguo.top

[Q80] 字符串截取
来源：http://irh.fehbvm.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mnh.guannengcc.top

[Q81] 字符串替换
来源：http://omr.hnqzz.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://trk.yj20258888.top

[Q82] 字符长度与字节长度
来源：http://tpo.yanxiufei.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ihz.cucudq.cn

[Q83] 大小写转换
来源：http://sdq.pycfn.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://vcy.zhijiandao.cn

[Q84] 去除首尾空格
来源：http://uhi.hongshengwenyu.top

SELECT TRIM(name) FROM users;
来源：http://kjr.yfazqb.com

[Q85] 数值取整
来源：http://dhc.dashuyun.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://bzz.yfazqb.com

[Q86] 读取 JSON 字段
来源：http://dft.andypj.xyz

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://cbr.ydzc1.top

[Q87] JSON 字段做条件
来源：http://yrt.aibaodan.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hlw.uphjek.com

[Q88] 行转列（条件聚合）
来源：http://yxe.ctjpmb.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://xfm.hnxiangtu.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://lxe.nwbrower.top

[Q89] 判断表是否存在
来源：http://ktm.xinyue.icu

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://rof.sjlbkw.cn

[Q90] 生成序号列
来源：http://yha.yonumen.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://yld.epnwcf.com

================================================================================
来源：http://qdl.chenzaomai.com

R. Bash 专题
来源：http://kdf.yongpay.top

================================================================================
来源：http://lnv.316326.xyz

[R01] shebang 与严格模式
来源：http://goo.tarul.cn

#!/usr/bin/env bash
来源：http://upf.yuanzhike.top

set -euo pipefail
来源：http://sqz.redwolf501.top

[R02] 变量赋值与使用
来源：http://ore.bjfxy.top

name="Tom"; echo "$name"
来源：http://mdt.havefunace.top

[R03] 只读变量
来源：http://xcs.quarkkingdee.top

readonly PI=3.14
来源：http://wdw.redwolf501.top

[R04] 位置参数
来源：http://awr.jinyuanbaomall.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://xlq.chenlongwang.top

[R05] 参数默认值
来源：http://yul.zycfv.cn

name="${1:-default}"
来源：http://syp.fengsongda.top

[R06] 判断命令是否存在
来源：http://ibe.cqqwz.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://vhw.dashuyun.cn

[R07] if 判断文件
来源：http://ueg.xuetiantiany.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://lry.andypj.xyz

[R08] 数值比较
来源：http://eoe.zhengqikj.top

if (( a > b )); then echo "a 更大"; fi
来源：http://isl.sweek.top

[R09] 字符串比较
来源：http://rzh.gaohongyu789.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://fly.xylfe.cn

[R10] 正则匹配
来源：http://kwq.xingfuxueyuan.xyz

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://sgm.shuidangran.top

[R11] case 多分支
来源：http://yov.sweek.top

case "$1" in
来源：http://rrd.fengsongda.top

start) echo "启动" ;;
来源：http://dbw.guannengcc.top

stop)  echo "停止" ;;
来源：http://ygp.nanxinkj.top

*)     echo "未知命令" ;;
来源：http://zug.fehbvm.com

esac
来源：http://upc.shanyushiyangtech.top

[R12] for 遍历文件
来源：http://utq.zhiwuduotai.top

for f in *.txt; do echo "$f"; done
来源：http://tyk.sufxvd.cn

[R13] for 计数循环
来源：http://iwv.nanxinkj.top

for i in {1..10}; do echo "$i"; done
来源：http://yzm.316326.xyz

[R14] C 风格 for
来源：http://gje.jinqigfzy.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ycr.fktsv.cn

[R15] while 逐行读文件
来源：http://uqi.dianchejie.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://vns.ppjwa.cn

[R16] until 等待条件
来源：http://jxa.jinqigfzy.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wsy.xuetiantiany.cn

[R17] 数组定义与取值
来源：http://thk.chenjidiqi.icu

arr=(a b c); echo "${arr[0]}"
来源：http://mdr.mhx1999.top

[R18] 遍历数组
来源：http://yxc.yj20258.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://yyf.yongpay.top

[R19] 数组长度
来源：http://rqu.yj20258888.top

echo "${#arr[@]}"
来源：http://yzq.xylfe.cn

[R20] 关联数组（字典）
来源：http://als.wangdashe.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://pyb.gaohongyu789.top

[R21] 字符串长度
来源：http://miq.tian-w.cn

echo "${#s}"
来源：http://uoj.tianlin.xyz

[R22] 截取子串
来源：http://fvd.zhoulong.xyz

echo "${s:0:5}"
来源：http://edv.fanxiaobao.xyz

[R23] 字符串替换
来源：http://mpi.smart0.xyz

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://xow.hfpthk.cn

[R24] 大小写转换
来源：http://rwk.xziqi.cn

echo "${s^^}"; echo "${s,,}"
来源：http://udq.shzxlz.cn

[R25] 去后缀 / 去前缀
来源：http://cck.birdmap.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://vue.gzhubu.top

[R26] 命令替换
来源：http://rtd.cashguo.top

now=$(date +%F); echo "$now"
来源：http://rwd.c1oappe.top

[R27] 算术展开
来源：http://gum.pycfn.com

echo $((1 + 2 * 3))
来源：http://stk.xziqi.cn

[R28] 浮点运算
来源：http://imv.wangdashe.top

echo "scale=2; 10/3" | bc
来源：http://ooi.bbcook.cn

[R29] 定义函数
来源：http://yjj.hysaishi.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://cjw.yj20258888.top

[R30] 函数返回状态码
来源：http://wgt.ybcxt.top

f() { return 0; }; f || echo "失败了"
来源：http://zoj.hesvh.cn

[R31] 局部变量
来源：http://cok.chenjidiqi.icu

f() { local x=1; echo "$x"; }
来源：http://ahb.shuidangran.top

[R32] 参数个数校验
来源：http://uif.ybcxt.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://fbs.tanke756.top

[R33] 捕获错误并提示行号
来源：http://bwz.yj202588.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://fbe.epnwcf.com

[R34] 退出时清理
来源：http://jiq.meibo888.top

trap 'rm -f "$tmp"' EXIT
来源：http://uhq.sysykeji.top

[R35] 后台执行并等待
来源：http://pnb.hesvh.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://vgd.aizwys.cn

[R36] 并发执行多个任务
来源：http://fjo.mhx1999.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://bzx.c1oappe.top

[R37] 把输出赋给变量
来源：http://zjk.chenzaomai.com

files=$(ls -1)
来源：http://xkk.gogol.net.cn

[R38] 管道串联
来源：http://ihb.zhengqikj.top

cat a.txt | grep -i error | wc -l
来源：http://dqy.cdnleiting.top

[R39] 重定向标准输出与错误
来源：http://wkf.ehwqpu.com

cmd > out.log 2>&1
来源：http://sjg.aizwys.cn

[R40] 追加写日志
来源：http://nhk.havefunace.top

echo "log" >> out.log
来源：http://ddi.tarul.cn

[R41] 丢弃输出
来源：http://bni.hesvh.cn

cmd >/dev/null 2>&1
来源：http://gtn.hysaishi.cn

[R42] 输入重定向
来源：http://srx.yuanzhike.top

wc -l < a.txt
来源：http://gvc.zhengqikj.top

[R43] 按名字查找文件
来源：http://ahq.52xcode.cn


<!-- 参考信息 -->