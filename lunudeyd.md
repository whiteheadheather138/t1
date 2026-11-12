代发 wailian999

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://vor.fanxiaobao.xyz

Ruby: // 手写闭包 + Time.now 判断
来源：http://pup.shanyushiyangkeji.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://eso.gotoacloud.top

[P08] 处理浮点精度问题
来源：http://vwt.shuidangran.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://njc.meibo888.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://bip.tanke756.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://owd.zhoulong.xyz

TS:   (0.1 + 0.2).toFixed(2)
来源：http://jyt.sysykeji.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://dll.hnxiangtu.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://oqw.smart0.xyz

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://bbx.haohaochexian.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://gwq.xziqi.cn

================================================================================
来源：http://fxa.zycfv.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://tit.fanxiaobao.xyz

================================================================================
来源：http://pjt.nwbrower.top

[Q01] 创建表
来源：http://uli.sweek.top

CREATE TABLE users (
来源：http://clt.aizwys.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://afl.ywan-chungtsiang.top

name VARCHAR(50) NOT NULL,
来源：http://iid.andypj.xyz

email VARCHAR(100) UNIQUE,
来源：http://mti.ywan-chungtsiang.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://oxr.aizwys.cn

);
来源：http://mvv.jianghu66.top

[Q02] 创建带外键的表
来源：http://oza.andypj.xyz

CREATE TABLE orders (
来源：http://yoc.hywenlv.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://qfi.sweek.top

user_id INT NOT NULL,
来源：http://dmo.gotoacloud.top

amount DECIMAL(10, 2),
来源：http://iau.0kj1m.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hmk.guannengcc.top

);
来源：http://pma.yuanzhike.top

[Q03] 增加列
来源：http://ypi.gotoacloud.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://nis.cqqwz.cn

[Q04] 修改列类型
来源：http://gfx.sxryk.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://izb.chenlongwang.top

[Q05] 重命名列
来源：http://uba.jlsjyb.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://jel.gogol.net.cn

[Q06] 删除列
来源：http://yif.epnwcf.com

ALTER TABLE users DROP COLUMN age;
来源：http://equ.shzxlz.cn

[Q07] 删除表
来源：http://rry.yueranfly.top

DROP TABLE IF EXISTS orders;
来源：http://gsi.xuanzx.com

[Q08] 创建普通索引
来源：http://zqw.zdqjudy.top

CREATE INDEX idx_users_email ON users(email);
来源：http://hqw.yuanzhike.top

[Q09] 创建唯一索引
来源：http://zht.sxryk.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://dho.sufxvd.cn

[Q10] 插入单行
来源：http://zzq.nanxinkj.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mit.bjfxy.top

[Q11] 一次插入多行
来源：http://frh.chenlongwang.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://gvm.52xcode.cn

[Q12] 插入后取自增 ID
来源：http://vbb.epnwcf.com

INSERT INTO users (name) VALUES ('C');
来源：http://ett.ywan-chungtsiang.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://svm.52xcode.cn

[Q13] 忽略重复插入
来源：http://cbq.yongpay.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://vbc.zhoulong.xyz

[Q14] 存在则更新（upsert）
来源：http://rja.jianghu66.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://gmt.316326.xyz

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://tlk.hongshengwenyu.top

[Q15] 查询全部
来源：http://yoc.dianchejie.cn

SELECT * FROM users;
来源：http://vtm.birdmap.top

[Q16] 查询指定列
来源：http://qfr.daxiang520.top

SELECT id, name FROM users;
来源：http://ieu.nanxinkj.top

[Q17] 条件查询
来源：http://iva.quarkkingdee.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://xwy.sjlbkw.cn

[Q18] 模糊匹配
来源：http://eog.daria6918.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://bva.vehdjk.com

[Q19] 范围查询
来源：http://qag.zdqjudy.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mnw.c1oappe.top

[Q20] IN 列表
来源：http://bac.zhengqikj.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://yge.zhiwuduotai.top

[Q21] 空值判断
来源：http://ocq.316326.xyz

SELECT * FROM users WHERE email IS NULL;
来源：http://gsy.haohaochexian.top

[Q22] 排序
来源：http://msw.jinqigfzy.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://faa.jinqigfzy.top

[Q23] 分页
来源：http://rxx.tanke756.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://fwa.daria6918.cn

[Q24] 去重
来源：http://ydn.ehwqpu.com

SELECT DISTINCT city FROM users;
来源：http://zgf.hcnkem.com

[Q25] 只取前 N 条
来源：http://lkx.ydzc1.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://fvi.ydzc1.top

[Q26] 计数
来源：http://ppe.ctjpmb.com

SELECT COUNT(*) FROM users;
来源：http://jvg.mhx1999.top

[Q27] 条件计数
来源：http://atw.yangfankeji.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://bds.xuanzx.com

[Q28] 求和与平均
来源：http://ukh.zhiwuduotai.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wha.ydzc1.top

[Q29] 最大最小值
来源：http://dpr.zhengqikj.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://cnp.zdqjudy.top

[Q30] 分组统计
来源：http://bpc.yj20258.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://sjp.meibo888.top

[Q31] 分组后过滤
来源：http://upv.zhongyouzk.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://qcq.sysykeji.top

[Q32] 分组拼接字符串
来源：http://ecy.zhaomingkeji.xyz

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ces.aizwys.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://zro.pengpengdd.cyou

[Q33] 多列分组
来源：http://akf.meibo888.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hzg.andypj.xyz

[Q34] 每组取第一条
来源：http://bbn.nanxuanxn.top

SELECT * FROM (
来源：http://zid.fktsv.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://imj.hfpthk.cn

) t WHERE rn = 1;
来源：http://aai.9152youxi.cn

[Q35] 内连接
来源：http://wmu.feifeiyinyue.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://isv.hcnkem.com

[Q36] 左连接
来源：http://ony.ivvv.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://zrn.hammf.cn

[Q37] 右连接
来源：http://bdu.quarkkingdee.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://bel.cqqwz.cn

[Q38] 全外连接（PostgreSQL）
来源：http://nxk.meibo888.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ifi.tianlin.xyz

[Q39] 自连接（查上下级）
来源：http://fmt.smart0.xyz

SELECT e.name, m.name AS manager FROM employees e
来源：http://jsg.epnwcf.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://jfk.sweek.top

[Q40] 交叉连接（笛卡尔积）
来源：http://woj.jqgufenzy.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://obr.ywan-chungtsiang.top

[Q41] 多表连接
来源：http://fsp.redwolf501.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://crw.sxryk.cn

JOIN users u ON u.id = o.user_id
来源：http://pkk.shanyushiyangtech.top

JOIN products p ON p.id = o.product_id;
来源：http://min.yj202588.top

[Q42] 连接条件附加过滤
来源：http://xwi.yonumen.top

SELECT u.name, o.amount FROM users u
来源：http://vqo.xziqi.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://suw.ybcxt.top

[Q43] 标量子查询
来源：http://dmd.zhengqikj.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hil.jinyuanbaomall.cn

[Q44] IN 子查询
来源：http://dlp.bbcook.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://sye.yueranfly.top

[Q45] EXISTS 判断存在
来源：http://ouk.vehdjk.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zyz.xylfe.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ofp.gaohongyu789.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mbs.hongshengwenyu.top

[Q47] 与平均值比较
来源：http://cvt.guannengcc.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://brq.hfpthk.cn

[Q48] CTE 公用表表达式
来源：http://vvc.gzhubu.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mze.vehdjk.com

SELECT * FROM t WHERE c > 5;
来源：http://djy.iojbl.cn

[Q49] 更新单行
来源：http://yaq.cdnleiting.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ufb.bbcook.cn

[Q50] 批量更新
来源：http://har.pengpengdd.cyou

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://frr.zhijiandao.cn

[Q51] 用子查询更新
来源：http://gtd.xuanzx.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://vnn.smart0.xyz

[Q52] 删除指定行
来源：http://zfv.ppjwa.cn

DELETE FROM users WHERE id = 10;
来源：http://awg.hywenlv.cn

[Q53] 按条件删除
来源：http://uff.iojbl.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://sya.jyoumei.cn

[Q54] 清空表
来源：http://dui.vehdjk.com

TRUNCATE TABLE logs;
来源：http://zus.wangdashe.top

[Q55] 排名（并列占位）
来源：http://ecm.epnwcf.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://vzk.9152youxi.cn

[Q56] 密集排名（并列不占位）
来源：http://hex.dianchejie.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ven.birdmap.top

[Q57] 行号
来源：http://tsn.kuanghao11.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://qhs.redwolf501.top

[Q58] 累计求和
来源：http://npb.uphjek.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://rvx.jyoumei.cn

[Q59] 分组内累计
来源：http://qwb.nwbrower.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://jsb.haohaochexian.top

[Q60] 取上一行 / 下一行
来源：http://sfh.tanke756.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://pzr.chenzaomai.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://gnm.zhixingplan.top

[Q61] 移动平均
来源：http://sli.aizwys.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wkz.sysykeji.top

[Q62] 分组占比
来源：http://hru.yvedp.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ckt.shanyushiyangtech.top

[Q63] 开启事务
来源：http://vwx.smart0.xyz

START TRANSACTION;                -- 或 BEGIN
来源：http://bzu.bbcook.cn

[Q64] 提交事务
来源：http://bdb.hfpthk.cn

COMMIT;
来源：http://jzh.ppjwa.cn

[Q65] 回滚事务
来源：http://flk.nanxuanxn.top

ROLLBACK;
来源：http://ptf.hnxiangtu.top

[Q66] 行锁查询
来源：http://rrb.daxiang520.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ayv.kuanghao11.cn

[Q67] 设置隔离级别
来源：http://ijq.aibaodan.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://kiq.yuanzhike.top

[Q68] 保存点
来源：http://yjj.tianlin.xyz

SAVEPOINT sp1;
来源：http://ron.fanxiaobao.xyz

ROLLBACK TO sp1;
来源：http://kuv.birdmap.top

[Q69] 查看执行计划
来源：http://oev.zhoulong.xyz

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://pnk.haohaochexian.top

[Q70] 更新统计信息
来源：http://bpy.fengsongda.top

ANALYZE TABLE users;
来源：http://qvu.pycfn.com

[Q71] 查看建表语句
来源：http://jqz.c1oappe.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://exi.bbcook.cn

[Q72] 查看索引
来源：http://zmu.bjfxy.top

SHOW INDEX FROM users;
来源：http://bae.hongshengwenyu.top

[Q73] 查看表状态
来源：http://tij.chenzaomai.com

SHOW TABLE STATUS LIKE 'users';
来源：http://qbo.hfpthk.cn

[Q74] 强制使用索引
来源：http://rrw.cdnleiting.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://moe.yj20258888.top

[Q75] 日期格式化
来源：http://bpz.nwbrower.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://cyr.fengsongda.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ems.dianchejie.cn

[Q76] 按天统计
来源：http://hue.nanxuanxn.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://zur.ybcxt.top

[Q77] 时间加减
来源：http://tnx.zhaomingkeji.xyz

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hht.hesvh.cn

[Q78] 当前时间
来源：http://zst.hcnkem.com

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://skd.uphjek.com

[Q79] 字符串拼接
来源：http://ert.fktsv.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://rvf.zhengqikj.top

[Q80] 字符串截取
来源：http://cgf.daria6918.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://qjs.wangdashe.top

[Q81] 字符串替换
来源：http://cwd.dashuyun.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://jlx.snrcjt.cn

[Q82] 字符长度与字节长度
来源：http://jqf.redwolf501.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ikl.nwbrower.top

[Q83] 大小写转换
来源：http://pnb.wangdashe.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://lxz.zhaomingkeji.xyz

[Q84] 去除首尾空格
来源：http://xsm.tian-w.cn

SELECT TRIM(name) FROM users;
来源：http://fid.gogol.net.cn

[Q85] 数值取整
来源：http://yer.tanke756.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hrv.9152youxi.cn

[Q86] 读取 JSON 字段
来源：http://wex.zdqjudy.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://gro.ivvv.top

[Q87] JSON 字段做条件
来源：http://ggr.yvedp.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://pka.jqgfzy.top

[Q88] 行转列（条件聚合）
来源：http://ulz.yuanzhike.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://vaf.sweek.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://rup.uphjek.com

[Q89] 判断表是否存在
来源：http://qlh.jianghu66.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://dmm.yfazqb.com

[Q90] 生成序号列
来源：http://dtb.jiagoushi.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://azb.cucudq.cn

================================================================================
来源：http://ibr.hfpthk.cn

R. Bash 专题
来源：http://frs.yj20258888.top

================================================================================
来源：http://ylq.bjfxy.top

[R01] shebang 与严格模式
来源：http://hgq.hesvh.cn

#!/usr/bin/env bash
来源：http://dvn.pycfn.com

set -euo pipefail
来源：http://wdx.chenlongwang.top

[R02] 变量赋值与使用
来源：http://dbe.xinyue.icu

name="Tom"; echo "$name"
来源：http://dha.birdmap.top

[R03] 只读变量
来源：http://qic.vehdjk.com

readonly PI=3.14
来源：http://ybp.redwolf501.top

[R04] 位置参数
来源：http://krr.aizwys.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://bho.mhx1999.top

[R05] 参数默认值
来源：http://gbr.ctjpmb.com

name="${1:-default}"
来源：http://mnb.9152youxi.cn

[R06] 判断命令是否存在
来源：http://rhv.snrcjt.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://vcl.zhiwuduotai.top

[R07] if 判断文件
来源：http://exr.sysykeji.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ecg.chenjidiqi.icu

[R08] 数值比较
来源：http://cgm.nanxinkj.top

if (( a > b )); then echo "a 更大"; fi
来源：http://otx.xingfuxueyuan.xyz

[R09] 字符串比较
来源：http://ucl.quarkkingdee.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://zqn.c1oappe.top

[R10] 正则匹配
来源：http://ddh.ybcxt.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://tol.xuetiantiany.cn

[R11] case 多分支
来源：http://dis.zhongyouzk.top

case "$1" in
来源：http://ytl.vqdsnc.cn

start) echo "启动" ;;
来源：http://vdh.zhixingplan.top

stop)  echo "停止" ;;
来源：http://rlm.xylfe.cn

*)     echo "未知命令" ;;
来源：http://dya.ydzc1.top

esac
来源：http://qvy.xziqi.cn

[R12] for 遍历文件
来源：http://luc.iojbl.cn

for f in *.txt; do echo "$f"; done
来源：http://uhw.pycfn.com

[R13] for 计数循环
来源：http://wrf.ppjwa.cn

for i in {1..10}; do echo "$i"; done
来源：http://fcc.zycfv.cn

[R14] C 风格 for
来源：http://myo.iojbl.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://npn.9152youxi.cn

[R15] while 逐行读文件
来源：http://tan.hnqzz.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mln.yuanzhike.top

[R16] until 等待条件
来源：http://xuj.jinyuanbaomall.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hjg.zhijiandao.cn

[R17] 数组定义与取值
来源：http://sck.tian-w.cn

arr=(a b c); echo "${arr[0]}"
来源：http://jps.chenlongwang.top

[R18] 遍历数组
来源：http://arw.zdqjudy.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wud.shangyingyoupin.top

[R19] 数组长度
来源：http://rto.jinqigufen.top

echo "${#arr[@]}"
来源：http://odz.pengpengdd.cyou

[R20] 关联数组（字典）
来源：http://odi.316326.xyz

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://kil.haohaochexian.top

[R21] 字符串长度
来源：http://yke.xuanzx.com

echo "${#s}"
来源：http://tnl.bjfxy.top

[R22] 截取子串
来源：http://peh.zhaomingkeji.xyz

echo "${s:0:5}"
来源：http://sik.hcnkem.com

[R23] 字符串替换
来源：http://bfj.kuanghao11.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://nxq.xziqi.cn

[R24] 大小写转换
来源：http://kmo.hammf.cn

echo "${s^^}"; echo "${s,,}"
来源：http://qbq.tanke756.top

[R25] 去后缀 / 去前缀
来源：http://pyb.sxryk.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ejk.gogol.net.cn

[R26] 命令替换
来源：http://wxp.zdqjudy.top

now=$(date +%F); echo "$now"
来源：http://iip.chenzaomai.com

[R27] 算术展开
来源：http://bdp.nanxuanxn.top

echo $((1 + 2 * 3))
来源：http://ojt.hnqzz.top

[R28] 浮点运算
来源：http://fhn.chenzaomai.com

echo "scale=2; 10/3" | bc
来源：http://xzt.316326.xyz

[R29] 定义函数
来源：http://zsk.shanyushiyangkeji.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://fzv.zdbjq.cn

[R30] 函数返回状态码
来源：http://esy.pycfn.com

f() { return 0; }; f || echo "失败了"
来源：http://mxt.jqgufenzy.top

[R31] 局部变量
来源：http://ptb.tian-w.cn

f() { local x=1; echo "$x"; }
来源：http://vtl.hammf.cn

[R32] 参数个数校验
来源：http://gkp.tarul.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://qhz.fanxiaobao.xyz

[R33] 捕获错误并提示行号
来源：http://kvj.zhoulong.xyz

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ivg.hammf.cn

[R34] 退出时清理
来源：http://ekp.redwolf501.top

trap 'rm -f "$tmp"' EXIT
来源：http://ffh.yj20258888.top

[R35] 后台执行并等待
来源：http://wyz.9152youxi.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://nuv.yj20258.top

[R36] 并发执行多个任务
来源：http://ryb.chenlongwang.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://eow.daria6918.cn

[R37] 把输出赋给变量
来源：http://ocl.jianghu66.top


<!-- 参考信息 -->