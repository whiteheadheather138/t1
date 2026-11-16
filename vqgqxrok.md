代发 wailian999

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wxw.zdbjq.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://xus.hongshengwenyu.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://gru.yueranfly.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://byz.xuanzx.com

================================================================================
来源：http://qsi.kuanghao11.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://big.hongshengwenyu.top

================================================================================
来源：http://vxn.sweek.top

[Q01] 创建表
来源：http://kkw.hysaishi.cn

CREATE TABLE users (
来源：http://bmg.jianghu66.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ijd.jinghuilouyu.cn

name VARCHAR(50) NOT NULL,
来源：http://ade.quarkkingdee.top

email VARCHAR(100) UNIQUE,
来源：http://yku.sysykeji.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ean.jlsjyb.cn

);
来源：http://qfw.bbcook.cn

[Q02] 创建带外键的表
来源：http://vaj.kuanghao11.cn

CREATE TABLE orders (
来源：http://guq.bjfxy.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://omk.xylfe.cn

user_id INT NOT NULL,
来源：http://lev.ctjpmb.com

amount DECIMAL(10, 2),
来源：http://ilm.chenlongwang.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://tis.aizwys.cn

);
来源：http://fwp.sweek.top

[Q03] 增加列
来源：http://bfh.shanyushiyangkeji.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://jxm.andypj.xyz

[Q04] 修改列类型
来源：http://ywp.hfpthk.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://prn.andypj.xyz

[Q05] 重命名列
来源：http://jjw.bbcook.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ldc.zdqjudy.top

[Q06] 删除列
来源：http://vfi.fehbvm.com

ALTER TABLE users DROP COLUMN age;
来源：http://gbv.daxiang520.top

[Q07] 删除表
来源：http://aln.snrcjt.cn

DROP TABLE IF EXISTS orders;
来源：http://lcm.jyoumei.cn

[Q08] 创建普通索引
来源：http://fcj.epnwcf.com

CREATE INDEX idx_users_email ON users(email);
来源：http://mbz.zdqjudy.top

[Q09] 创建唯一索引
来源：http://jjd.vqdsnc.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://uwu.shangyingyoupin.top

[Q10] 插入单行
来源：http://okz.sjlbkw.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://jwu.wangshuangyany.cn

[Q11] 一次插入多行
来源：http://jcm.dianchejie.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wbp.havefunace.top

[Q12] 插入后取自增 ID
来源：http://rpt.zhiwuduotai.top

INSERT INTO users (name) VALUES ('C');
来源：http://siw.xinyue.icu

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://aub.nwbrower.top

[Q13] 忽略重复插入
来源：http://byx.havefunace.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://fev.ehwqpu.com

[Q14] 存在则更新（upsert）
来源：http://zhc.jiagoushi.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://gco.aizwys.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://rng.shangyingyoupin.top

[Q15] 查询全部
来源：http://adf.zycfv.cn

SELECT * FROM users;
来源：http://spq.zhijiandao.cn

[Q16] 查询指定列
来源：http://ahf.pengpengdd.cyou

SELECT id, name FROM users;
来源：http://tyj.yfazqb.com

[Q17] 条件查询
来源：http://itl.sxryk.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://efm.shangyingyoupin.top

[Q18] 模糊匹配
来源：http://rec.yfazqb.com

SELECT * FROM users WHERE name LIKE '张%';
来源：http://xwo.dashuyun.cn

[Q19] 范围查询
来源：http://hsc.guowangkeji.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://beu.pengpengdd.cyou

[Q20] IN 列表
来源：http://ttv.quarkkingdee.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://afk.tanke756.top

[Q21] 空值判断
来源：http://sib.hfpthk.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://vti.yj20258.top

[Q22] 排序
来源：http://tpo.gaohongyu789.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://nyy.shanyushiyangkeji.top

[Q23] 分页
来源：http://oyj.wangdashe.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://pdx.smart0.xyz

[Q24] 去重
来源：http://nht.hysaishi.cn

SELECT DISTINCT city FROM users;
来源：http://dpe.jinyuanbaomall.cn

[Q25] 只取前 N 条
来源：http://gra.shangyingyoupin.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wuh.ivvv.top

[Q26] 计数
来源：http://eny.yfazqb.com

SELECT COUNT(*) FROM users;
来源：http://cyh.shzxlz.cn

[Q27] 条件计数
来源：http://vzt.aizwys.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://nvq.smart0.xyz

[Q28] 求和与平均
来源：http://axv.gzhubu.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://gnr.hywenlv.cn

[Q29] 最大最小值
来源：http://vjs.yj20258.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://ecz.bjfxy.top

[Q30] 分组统计
来源：http://dlk.pycfn.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://rtx.yj20258.top

[Q31] 分组后过滤
来源：http://hwz.hesvh.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://nbf.316326.xyz

[Q32] 分组拼接字符串
来源：http://glk.bjfxy.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://lek.cheryme.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://vup.yj20258.top

[Q33] 多列分组
来源：http://phv.uphjek.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ety.vqdsnc.cn

[Q34] 每组取第一条
来源：http://puv.dianchejie.cn

SELECT * FROM (
来源：http://quy.xuanzx.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://gxq.epnwcf.com

) t WHERE rn = 1;
来源：http://cxs.guannengcc.top

[Q35] 内连接
来源：http://lbq.ydjk.org.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hay.chenzaomai.com

[Q36] 左连接
来源：http://nvo.cucudq.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://zvz.jqgfzy.top

[Q37] 右连接
来源：http://rem.tanke756.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://rvf.kuanghao11.cn

[Q38] 全外连接（PostgreSQL）
来源：http://arc.shanyushiyangtech.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://yri.xylfe.cn

[Q39] 自连接（查上下级）
来源：http://ttr.yangfankeji.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://jpr.yueranfly.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wdc.epnwcf.com

[Q40] 交叉连接（笛卡尔积）
来源：http://gij.52xcode.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wpy.jiagoushi.top

[Q41] 多表连接
来源：http://hba.fanxiaobao.xyz

SELECT o.id, u.name, p.title FROM orders o
来源：http://jra.bjfxy.top

JOIN users u ON u.id = o.user_id
来源：http://dgw.ehwqpu.com

JOIN products p ON p.id = o.product_id;
来源：http://owr.zhoulong.xyz

[Q42] 连接条件附加过滤
来源：http://uhr.xinyue.icu

SELECT u.name, o.amount FROM users u
来源：http://qrh.jqgfzy.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ivi.feifeiyinyue.top

[Q43] 标量子查询
来源：http://wfn.0kj1m.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://yjc.vqdsnc.cn

[Q44] IN 子查询
来源：http://iit.havefunace.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://cmn.jqgufenzy.top

[Q45] EXISTS 判断存在
来源：http://yqj.hongshengwenyu.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ynv.52xcode.cn

[Q46] NOT EXISTS 判断不存在
来源：http://pzi.fanxiaobao.xyz

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://srt.smart0.xyz

[Q47] 与平均值比较
来源：http://tib.ctjpmb.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://lwt.0kj1m.cn

[Q48] CTE 公用表表达式
来源：http://faa.snrcjt.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://xkt.zhoulong.xyz

SELECT * FROM t WHERE c > 5;
来源：http://gxf.zhoulong.xyz

[Q49] 更新单行
来源：http://lqt.nanxinkj.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://rkh.quarkkingdee.top

[Q50] 批量更新
来源：http://wzm.ctjpmb.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://nye.gaohongyu789.top

[Q51] 用子查询更新
来源：http://zme.cqqwz.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://xok.0kj1m.cn

[Q52] 删除指定行
来源：http://sid.ctjpmb.com

DELETE FROM users WHERE id = 10;
来源：http://mjz.ctjpmb.com

[Q53] 按条件删除
来源：http://twx.haohaochexian.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://nat.fzhhl.top

[Q54] 清空表
来源：http://xhz.svipenyu.cn

TRUNCATE TABLE logs;
来源：http://qdi.zhongyouzk.top

[Q55] 排名（并列占位）
来源：http://hvv.pengpengdd.cyou

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hvs.ctjpmb.com

[Q56] 密集排名（并列不占位）
来源：http://tvb.hysaishi.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://yqf.hnxiangtu.top

[Q57] 行号
来源：http://tvb.yj20258.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://kuj.iojbl.cn

[Q58] 累计求和
来源：http://lec.tanke756.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ydj.xingfuxueyuan.xyz

[Q59] 分组内累计
来源：http://slm.jqgufenzy.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://kpw.yangfankeji.com

[Q60] 取上一行 / 下一行
来源：http://awk.jinghuilouyu.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hrc.aizwys.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://csp.jinqigufen.top

[Q61] 移动平均
来源：http://fug.sweek.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://gmy.cqqwz.cn

[Q62] 分组占比
来源：http://vby.hnqzz.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://pal.guannengcc.top

[Q63] 开启事务
来源：http://dus.fengsongda.top

START TRANSACTION;                -- 或 BEGIN
来源：http://xvs.iojbl.cn

[Q64] 提交事务
来源：http://wav.nanxinkj.top

COMMIT;
来源：http://ngo.yj202588.top

[Q65] 回滚事务
来源：http://ogz.316326.xyz

ROLLBACK;
来源：http://qpk.sjlbkw.cn

[Q66] 行锁查询
来源：http://mvz.uphjek.com

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://dbv.xingfuxueyuan.xyz

[Q67] 设置隔离级别
来源：http://zix.nanxuanxn.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://dks.jqgfzy.top

[Q68] 保存点
来源：http://iqg.fktsv.cn

SAVEPOINT sp1;
来源：http://meo.52xcode.cn

ROLLBACK TO sp1;
来源：http://smn.gogol.net.cn

[Q69] 查看执行计划
来源：http://uuq.hnxiangtu.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://jwy.dashuyun.cn

[Q70] 更新统计信息
来源：http://rsl.xingfuxueyuan.xyz

ANALYZE TABLE users;
来源：http://dwk.dashuyun.cn

[Q71] 查看建表语句
来源：http://oip.fktsv.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ucx.ywan-chungtsiang.top

[Q72] 查看索引
来源：http://yvd.zycfv.cn

SHOW INDEX FROM users;
来源：http://pjs.sysykeji.top

[Q73] 查看表状态
来源：http://mqf.jinghuilouyu.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://kep.jinyuanbaomall.cn

[Q74] 强制使用索引
来源：http://jfc.cqqwz.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://rcy.fanxiaobao.xyz

[Q75] 日期格式化
来源：http://ixo.guowangkeji.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://isx.sxryk.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://rgr.jiagoushi.top

[Q76] 按天统计
来源：http://oig.quarkkingdee.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://dbe.zdbjq.cn

[Q77] 时间加减
来源：http://lgf.cashguo.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ukm.xinyue.icu

[Q78] 当前时间
来源：http://eml.xuetiantiany.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://jps.andypj.xyz

[Q79] 字符串拼接
来源：http://kdi.shangyingyoupin.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wma.svipenyu.cn

[Q80] 字符串截取
来源：http://asl.zhixingplan.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://vil.yueranfly.top

[Q81] 字符串替换
来源：http://tub.tianlin.xyz

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://vvp.hywenlv.cn

[Q82] 字符长度与字节长度
来源：http://and.bbcook.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ovb.yvedp.cn

[Q83] 大小写转换
来源：http://jes.ydjk.org.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://vdq.shangyingyoupin.top

[Q84] 去除首尾空格
来源：http://vgg.sweek.top

SELECT TRIM(name) FROM users;
来源：http://erf.haohaochexian.top

[Q85] 数值取整
来源：http://kmi.zycfv.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://faz.pengpengdd.cyou

[Q86] 读取 JSON 字段
来源：http://ocl.bbcook.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://lpl.jyoumei.cn

[Q87] JSON 字段做条件
来源：http://rbr.sxryk.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hiv.zhaomingkeji.xyz

[Q88] 行转列（条件聚合）
来源：http://yir.haohaochexian.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ofz.yangfankeji.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ugk.hesvh.cn

[Q89] 判断表是否存在
来源：http://csy.jinqigufen.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mpp.havefunace.top

[Q90] 生成序号列
来源：http://ewg.gotoacloud.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://sxq.zhaomingkeji.xyz

================================================================================
来源：http://vyb.tianlin.xyz

R. Bash 专题
来源：http://jxa.feifeiyinyue.top

================================================================================
来源：http://qss.jqgfzy.top

[R01] shebang 与严格模式
来源：http://bpv.svipenyu.cn

#!/usr/bin/env bash
来源：http://rde.c1oappe.top

set -euo pipefail
来源：http://vgd.tian-w.cn

[R02] 变量赋值与使用
来源：http://azq.zhoulong.xyz

name="Tom"; echo "$name"
来源：http://kxi.shanyushiyangkeji.top

[R03] 只读变量
来源：http://cps.gzhubu.top

readonly PI=3.14
来源：http://nlo.svipenyu.cn

[R04] 位置参数
来源：http://xuy.mhx1999.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ktv.hysaishi.cn

[R05] 参数默认值
来源：http://bub.yonumen.top

name="${1:-default}"
来源：http://gid.gogol.net.cn

[R06] 判断命令是否存在
来源：http://xzp.cucudq.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hbg.ivvv.top

[R07] if 判断文件
来源：http://dhg.ehwqpu.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://rgy.uphjek.com

[R08] 数值比较
来源：http://myr.wangdashe.top

if (( a > b )); then echo "a 更大"; fi
来源：http://tce.xingfuxueyuan.xyz

[R09] 字符串比较
来源：http://viu.jinqigufen.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://oqr.chenlongwang.top

[R10] 正则匹配
来源：http://abg.zhijiandao.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://esb.cheryme.top

[R11] case 多分支
来源：http://gdk.dianchejie.cn

case "$1" in
来源：http://dga.sxryk.cn

start) echo "启动" ;;
来源：http://skn.52xcode.cn

stop)  echo "停止" ;;
来源：http://wdj.xuetiantiany.cn

*)     echo "未知命令" ;;
来源：http://vla.c1oappe.top

esac
来源：http://tpq.yj202588.top

[R12] for 遍历文件
来源：http://pxy.nwbrower.top

for f in *.txt; do echo "$f"; done
来源：http://mzd.jinqigufen.top

[R13] for 计数循环
来源：http://ays.gotoacloud.top

for i in {1..10}; do echo "$i"; done
来源：http://amq.svipenyu.cn

[R14] C 风格 for
来源：http://rod.ppjwa.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://tpw.gogol.net.cn

[R15] while 逐行读文件
来源：http://gba.tanke756.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wti.fengsongda.top

[R16] until 等待条件
来源：http://uhf.tanke756.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://moz.jianghu66.top

[R17] 数组定义与取值
来源：http://mwy.ybcxt.top

arr=(a b c); echo "${arr[0]}"
来源：http://jiw.shanyushiyangkeji.top

[R18] 遍历数组
来源：http://pvt.quarkkingdee.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ghv.gotoacloud.top

[R19] 数组长度
来源：http://ggx.hcnkem.com

echo "${#arr[@]}"
来源：http://kmv.chenzaomai.com

[R20] 关联数组（字典）
来源：http://ote.vqdsnc.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://feo.jinqigfzy.top

[R21] 字符串长度
来源：http://ads.aibaodan.cn

echo "${#s}"
来源：http://nhj.epnwcf.com

[R22] 截取子串
来源：http://clc.shuidangran.top

echo "${s:0:5}"
来源：http://ani.aibaodan.cn

[R23] 字符串替换
来源：http://iax.daria6918.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://usl.uphjek.com

[R24] 大小写转换
来源：http://aso.fengsongda.top

echo "${s^^}"; echo "${s,,}"
来源：http://mpk.tarul.cn

[R25] 去后缀 / 去前缀
来源：http://khc.zycfv.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://kzb.hywenlv.cn

[R26] 命令替换
来源：http://xkj.iojbl.cn

now=$(date +%F); echo "$now"
来源：http://uzt.sufxvd.cn

[R27] 算术展开
来源：http://oku.cashguo.top

echo $((1 + 2 * 3))
来源：http://eau.tian-w.cn

[R28] 浮点运算
来源：http://qgg.tanke756.top

echo "scale=2; 10/3" | bc
来源：http://ten.52xcode.cn

[R29] 定义函数
来源：http://ohb.nanxuanxn.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hbi.chenzaomai.com

[R30] 函数返回状态码
来源：http://klv.cucudq.cn

f() { return 0; }; f || echo "失败了"
来源：http://cqg.gotoacloud.top

[R31] 局部变量
来源：http://wzp.yanxiufei.cn

f() { local x=1; echo "$x"; }
来源：http://jqg.chenlongwang.top

[R32] 参数个数校验
来源：http://kge.9152youxi.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://fkc.gzhubu.top

[R33] 捕获错误并提示行号
来源：http://jng.dashuyun.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ipp.hnxiangtu.top

[R34] 退出时清理
来源：http://yvf.guowangkeji.top

trap 'rm -f "$tmp"' EXIT
来源：http://hyw.hesvh.cn

[R35] 后台执行并等待
来源：http://gml.c1oappe.top

sleep 5 & pid=$!; wait "$pid"
来源：http://hmp.shanyushiyangkeji.top

[R36] 并发执行多个任务
来源：http://zdi.zhoulong.xyz

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://bqt.yj20258888.top

[R37] 把输出赋给变量
来源：http://anl.yj202588.top

files=$(ls -1)
来源：http://dhz.cucudq.cn

[R38] 管道串联
来源：http://kft.jqgufenzy.top

cat a.txt | grep -i error | wc -l
来源：http://tyy.xinyue.icu

[R39] 重定向标准输出与错误
来源：http://evz.xingfuxueyuan.xyz

cmd > out.log 2>&1
来源：http://beu.yangfankeji.com

[R40] 追加写日志
来源：http://asd.daxiang520.top

echo "log" >> out.log
来源：http://uay.xziqi.cn

[R41] 丢弃输出
来源：http://nnm.0kj1m.cn


<!-- 参考信息 -->