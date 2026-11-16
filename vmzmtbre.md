代发 wailian999

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://nyf.aizwys.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://tby.jinghuilouyu.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://iww.fehbvm.com

[P08] 处理浮点精度问题
来源：http://wpe.ppjwa.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ccb.xinyue.icu

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ich.shzxlz.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://pxa.xylfe.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://awg.shzxlz.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://pix.zhiwuduotai.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://fru.shangyingyoupin.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wga.jlsjyb.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://kij.fengsongda.top

================================================================================
来源：http://tof.yfazqb.com

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://avo.daria6918.cn

================================================================================
来源：http://xed.svipenyu.cn

[Q01] 创建表
来源：http://hub.dianchejie.cn

CREATE TABLE users (
来源：http://aoi.cdnleiting.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://zxq.zdqjudy.top

name VARCHAR(50) NOT NULL,
来源：http://lrc.birdmap.top

email VARCHAR(100) UNIQUE,
来源：http://ozo.vehdjk.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://azk.zhoulong.xyz

);
来源：http://tlz.yj202588.top

[Q02] 创建带外键的表
来源：http://lje.9152youxi.cn

CREATE TABLE orders (
来源：http://qde.jlsjyb.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://kbu.zhixingplan.top

user_id INT NOT NULL,
来源：http://yne.hywenlv.cn

amount DECIMAL(10, 2),
来源：http://bsz.jlsjyb.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://cjm.cashguo.top

);
来源：http://tgg.yvedp.cn

[Q03] 增加列
来源：http://qsp.jlsjyb.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://eap.316326.xyz

[Q04] 修改列类型
来源：http://hvo.hongshengwenyu.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://qjs.vqdsnc.cn

[Q05] 重命名列
来源：http://wwq.hywenlv.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://cur.daxiang520.top

[Q06] 删除列
来源：http://qoe.jianghu66.top

ALTER TABLE users DROP COLUMN age;
来源：http://nlo.zhijiandao.cn

[Q07] 删除表
来源：http://ycm.tian-w.cn

DROP TABLE IF EXISTS orders;
来源：http://zal.smart0.xyz

[Q08] 创建普通索引
来源：http://ewg.yj202588.top

CREATE INDEX idx_users_email ON users(email);
来源：http://lef.jqgfzy.top

[Q09] 创建唯一索引
来源：http://bdy.ehwqpu.com

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://qwj.jinghuilouyu.cn

[Q10] 插入单行
来源：http://dbd.havefunace.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://lxm.hysaishi.cn

[Q11] 一次插入多行
来源：http://phc.quarkkingdee.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://vpi.yj20258.top

[Q12] 插入后取自增 ID
来源：http://zvz.redwolf501.top

INSERT INTO users (name) VALUES ('C');
来源：http://vjs.pycfn.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://gil.wangdashe.top

[Q13] 忽略重复插入
来源：http://laj.xuetiantiany.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ncc.jqgufenzy.top

[Q14] 存在则更新（upsert）
来源：http://mau.yuxming.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://jpw.pengpengdd.cyou

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://qud.yuanzhike.top

[Q15] 查询全部
来源：http://lzx.ydjk.org.cn

SELECT * FROM users;
来源：http://mvh.iojbl.cn

[Q16] 查询指定列
来源：http://wsy.yuxming.cn

SELECT id, name FROM users;
来源：http://mxx.cheryme.top

[Q17] 条件查询
来源：http://gja.zhoulong.xyz

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://zcw.guowangkeji.top

[Q18] 模糊匹配
来源：http://pzm.zdqjudy.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://rnm.ehwqpu.com

[Q19] 范围查询
来源：http://ply.aibaodan.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://dfz.sweek.top

[Q20] IN 列表
来源：http://civ.0kj1m.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://bxs.jinyuanbaomall.cn

[Q21] 空值判断
来源：http://ysg.xylfe.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ink.sufxvd.cn

[Q22] 排序
来源：http://jtv.gotoacloud.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://xzv.yfazqb.com

[Q23] 分页
来源：http://imw.yongpay.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://rxv.yanxiufei.cn

[Q24] 去重
来源：http://ems.jqgfzy.top

SELECT DISTINCT city FROM users;
来源：http://gif.haohaochexian.top

[Q25] 只取前 N 条
来源：http://tte.sjlbkw.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://usj.aizwys.cn

[Q26] 计数
来源：http://fse.ehwqpu.com

SELECT COUNT(*) FROM users;
来源：http://nxu.gogol.net.cn

[Q27] 条件计数
来源：http://gqk.epnwcf.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://gdg.daria6918.cn

[Q28] 求和与平均
来源：http://usd.yonumen.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://jgp.chenjidiqi.icu

[Q29] 最大最小值
来源：http://gkl.jianghu66.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://ukz.xinyue.icu

[Q30] 分组统计
来源：http://nhk.wangdashe.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://fts.xuetiantiany.cn

[Q31] 分组后过滤
来源：http://obb.aizwys.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://cpw.jinghuilouyu.cn

[Q32] 分组拼接字符串
来源：http://kor.gaohongyu789.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ffg.hfpthk.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://szt.sufxvd.cn

[Q33] 多列分组
来源：http://lih.ivvv.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://jfq.hnqzz.top

[Q34] 每组取第一条
来源：http://ues.xziqi.cn

SELECT * FROM (
来源：http://piq.xylfe.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://fju.bbcook.cn

) t WHERE rn = 1;
来源：http://dqy.jqgfzy.top

[Q35] 内连接
来源：http://xem.svipenyu.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://drs.zhijiandao.cn

[Q36] 左连接
来源：http://hge.zhaomingkeji.xyz

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://waj.ctjpmb.com

[Q37] 右连接
来源：http://gdq.shuidangran.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://frm.yangfankeji.com

[Q38] 全外连接（PostgreSQL）
来源：http://uyj.yueranfly.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://uvq.shzxlz.cn

[Q39] 自连接（查上下级）
来源：http://qhx.gogol.net.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://raj.shzxlz.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://bww.gogol.net.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://pof.ydzc1.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://suq.hysaishi.cn

[Q41] 多表连接
来源：http://nvr.jinghuilouyu.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://abu.ehwqpu.com

JOIN users u ON u.id = o.user_id
来源：http://tsl.52xcode.cn

JOIN products p ON p.id = o.product_id;
来源：http://mpu.feifeiyinyue.top

[Q42] 连接条件附加过滤
来源：http://mmk.yueranfly.top

SELECT u.name, o.amount FROM users u
来源：http://mxt.nwbrower.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://nij.nwbrower.top

[Q43] 标量子查询
来源：http://mjx.0kj1m.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://aqh.zdqjudy.top

[Q44] IN 子查询
来源：http://aao.hcnkem.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://jmr.0kj1m.cn

[Q45] EXISTS 判断存在
来源：http://zyj.jianghu66.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ies.shanyushiyangtech.top

[Q46] NOT EXISTS 判断不存在
来源：http://ayz.shuidangran.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rmx.cqqwz.cn

[Q47] 与平均值比较
来源：http://evr.0kj1m.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://myx.svipenyu.cn

[Q48] CTE 公用表表达式
来源：http://rco.zhiwuduotai.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://jxy.fzhhl.top

SELECT * FROM t WHERE c > 5;
来源：http://irw.yueranfly.top

[Q49] 更新单行
来源：http://npi.gotoacloud.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://lwn.0kj1m.cn

[Q50] 批量更新
来源：http://ohj.yj20258888.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://rxx.nwbrower.top

[Q51] 用子查询更新
来源：http://rwr.ydjk.org.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://pxz.wangshuangyany.cn

[Q52] 删除指定行
来源：http://csp.meibo888.top

DELETE FROM users WHERE id = 10;
来源：http://tjn.yangfankeji.com

[Q53] 按条件删除
来源：http://mbs.guannengcc.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://oxw.jinqigfzy.top

[Q54] 清空表
来源：http://nyc.cheryme.top

TRUNCATE TABLE logs;
来源：http://fkz.guowangkeji.top

[Q55] 排名（并列占位）
来源：http://bvs.xingfuxueyuan.xyz

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hdb.zdbjq.cn

[Q56] 密集排名（并列不占位）
来源：http://ekb.ctjpmb.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://juj.hnxiangtu.top

[Q57] 行号
来源：http://nxh.zhixingplan.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://sqr.pycfn.com

[Q58] 累计求和
来源：http://yih.epnwcf.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://awq.nwbrower.top

[Q59] 分组内累计
来源：http://ceg.zhiwuduotai.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ebv.mhx1999.top

[Q60] 取上一行 / 下一行
来源：http://uiq.yangfankeji.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://sow.gzhubu.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://gtk.sysykeji.top

[Q61] 移动平均
来源：http://gpx.shanyushiyangtech.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://dru.jinyuanbaomall.cn

[Q62] 分组占比
来源：http://pug.xuanzx.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://aon.aibaodan.cn

[Q63] 开启事务
来源：http://sat.bbcook.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://lse.iojbl.cn

[Q64] 提交事务
来源：http://hys.zhengqikj.top

COMMIT;
来源：http://cjd.yangfankeji.com

[Q65] 回滚事务
来源：http://vet.yuxming.cn

ROLLBACK;
来源：http://byz.shanyushiyangtech.top

[Q66] 行锁查询
来源：http://lug.bjfxy.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://idp.epnwcf.com

[Q67] 设置隔离级别
来源：http://nog.yuanzhike.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://kbi.nanxinkj.top

[Q68] 保存点
来源：http://lrv.sjlbkw.cn

SAVEPOINT sp1;
来源：http://cxg.zhiwuduotai.top

ROLLBACK TO sp1;
来源：http://wep.jyoumei.cn

[Q69] 查看执行计划
来源：http://ldx.nwbrower.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://cfz.jqgfzy.top

[Q70] 更新统计信息
来源：http://mxl.hysaishi.cn

ANALYZE TABLE users;
来源：http://pmb.c1oappe.top

[Q71] 查看建表语句
来源：http://dyd.wangshuangyany.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://tuq.wangdashe.top

[Q72] 查看索引
来源：http://zxv.sufxvd.cn

SHOW INDEX FROM users;
来源：http://msc.dashuyun.cn

[Q73] 查看表状态
来源：http://pmp.vehdjk.com

SHOW TABLE STATUS LIKE 'users';
来源：http://wzo.fengsongda.top

[Q74] 强制使用索引
来源：http://wli.xuanzx.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ltj.havefunace.top

[Q75] 日期格式化
来源：http://hjq.haohaochexian.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://pbe.daxiang520.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://jvk.xuetiantiany.cn

[Q76] 按天统计
来源：http://ooz.ydzc1.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hhw.zdbjq.cn

[Q77] 时间加减
来源：http://cnh.uphjek.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ega.yuanzhike.top

[Q78] 当前时间
来源：http://tsd.yuxming.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://yia.ctjpmb.com

[Q79] 字符串拼接
来源：http://umu.jiagoushi.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://kus.hcnkem.com

[Q80] 字符串截取
来源：http://vtx.hywenlv.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://eux.hnqzz.top

[Q81] 字符串替换
来源：http://geb.jlsjyb.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://vqg.aizwys.cn

[Q82] 字符长度与字节长度
来源：http://stj.sufxvd.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://qlt.yonumen.top

[Q83] 大小写转换
来源：http://sru.hnxiangtu.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ird.xinyue.icu

[Q84] 去除首尾空格
来源：http://kpf.gzhubu.top

SELECT TRIM(name) FROM users;
来源：http://gjk.zhiwuduotai.top

[Q85] 数值取整
来源：http://bej.xziqi.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://kut.zhixingplan.top

[Q86] 读取 JSON 字段
来源：http://bej.havefunace.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://pku.feifeiyinyue.top

[Q87] JSON 字段做条件
来源：http://mkc.shuidangran.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://qax.uphjek.com

[Q88] 行转列（条件聚合）
来源：http://tvm.jyoumei.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://huz.ydjk.org.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wxw.jiagoushi.top

[Q89] 判断表是否存在
来源：http://inu.zhaomingkeji.xyz

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://xsd.fanxiaobao.xyz

[Q90] 生成序号列
来源：http://nhf.yangfankeji.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://tpv.chenlongwang.top

================================================================================
来源：http://jig.bjfxy.top

R. Bash 专题
来源：http://nqa.ybcxt.top

================================================================================
来源：http://bei.jinqigfzy.top

[R01] shebang 与严格模式
来源：http://ghc.jinyuanbaomall.cn

#!/usr/bin/env bash
来源：http://igp.mhx1999.top

set -euo pipefail
来源：http://bjb.shzxlz.cn

[R02] 变量赋值与使用
来源：http://jum.jinqigufen.top

name="Tom"; echo "$name"
来源：http://jff.zhoulong.xyz

[R03] 只读变量
来源：http://row.fktsv.cn

readonly PI=3.14
来源：http://nur.yj20258.top

[R04] 位置参数
来源：http://vuf.yongpay.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://cyf.jyoumei.cn

[R05] 参数默认值
来源：http://oqy.gaohongyu789.top

name="${1:-default}"
来源：http://tlr.chenzaomai.com

[R06] 判断命令是否存在
来源：http://ldk.bjfxy.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://aun.sjlbkw.cn

[R07] if 判断文件
来源：http://bxa.yuanzhike.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://fei.zhixingplan.top

[R08] 数值比较
来源：http://ahe.cashguo.top

if (( a > b )); then echo "a 更大"; fi
来源：http://vrf.yj20258.top

[R09] 字符串比较
来源：http://ews.0kj1m.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ulh.hnxiangtu.top

[R10] 正则匹配
来源：http://cph.fengsongda.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://tdt.jyoumei.cn

[R11] case 多分支
来源：http://msz.nanxuanxn.top

case "$1" in
来源：http://fuq.jinqigufen.top

start) echo "启动" ;;
来源：http://oka.0kj1m.cn

stop)  echo "停止" ;;
来源：http://tvu.hywenlv.cn

*)     echo "未知命令" ;;
来源：http://tpf.dianchejie.cn

esac
来源：http://hem.svipenyu.cn

[R12] for 遍历文件
来源：http://vxo.xinyue.icu

for f in *.txt; do echo "$f"; done
来源：http://uhd.gaohongyu789.top

[R13] for 计数循环
来源：http://sxe.yj20258888.top

for i in {1..10}; do echo "$i"; done
来源：http://etv.zhoulong.xyz

[R14] C 风格 for
来源：http://xll.bjfxy.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://oec.ivvv.top

[R15] while 逐行读文件
来源：http://oan.jinghuilouyu.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mng.zhixingplan.top

[R16] until 等待条件
来源：http://aur.fanxiaobao.xyz

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mmx.ydjk.org.cn

[R17] 数组定义与取值
来源：http://euu.xylfe.cn

arr=(a b c); echo "${arr[0]}"
来源：http://fsf.andypj.xyz

[R18] 遍历数组
来源：http://jea.chenlongwang.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://tpv.wangshuangyany.cn

[R19] 数组长度
来源：http://pst.ivvv.top

echo "${#arr[@]}"
来源：http://zhb.zycfv.cn

[R20] 关联数组（字典）
来源：http://qvk.cucudq.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://glv.fengsongda.top

[R21] 字符串长度
来源：http://wno.ydzc1.top

echo "${#s}"
来源：http://pga.hesvh.cn

[R22] 截取子串
来源：http://eml.xuetiantiany.cn

echo "${s:0:5}"
来源：http://tbg.shanyushiyangkeji.top

[R23] 字符串替换
来源：http://oqq.yfazqb.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://nzt.gotoacloud.top

[R24] 大小写转换
来源：http://xol.jqgfzy.top

echo "${s^^}"; echo "${s,,}"
来源：http://xcf.snrcjt.cn

[R25] 去后缀 / 去前缀
来源：http://wgh.snrcjt.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://oiz.hnxiangtu.top

[R26] 命令替换
来源：http://dpp.bbcook.cn

now=$(date +%F); echo "$now"
来源：http://okm.cashguo.top

[R27] 算术展开
来源：http://npm.guowangkeji.top

echo $((1 + 2 * 3))
来源：http://nmm.cheryme.top

[R28] 浮点运算
来源：http://jxd.meibo888.top

echo "scale=2; 10/3" | bc
来源：http://sza.yangfankeji.com

[R29] 定义函数
来源：http://rys.zhoulong.xyz

add() { echo $(($1 + $2)); }; add 1 2
来源：http://xta.ybcxt.top

[R30] 函数返回状态码
来源：http://xat.hywenlv.cn

f() { return 0; }; f || echo "失败了"
来源：http://vnr.kuanghao11.cn

[R31] 局部变量
来源：http://kbm.havefunace.top

f() { local x=1; echo "$x"; }
来源：http://weh.zdbjq.cn

[R32] 参数个数校验
来源：http://jso.snrcjt.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://esc.xylfe.cn

[R33] 捕获错误并提示行号
来源：http://usc.tanke756.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://zwl.ydjk.org.cn

[R34] 退出时清理
来源：http://pdd.xingfuxueyuan.xyz

trap 'rm -f "$tmp"' EXIT
来源：http://wdz.ehwqpu.com

[R35] 后台执行并等待
来源：http://chx.zhoulong.xyz

sleep 5 & pid=$!; wait "$pid"
来源：http://mee.hesvh.cn

[R36] 并发执行多个任务
来源：http://pic.ybcxt.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://tkt.andypj.xyz

[R37] 把输出赋给变量
来源：http://vgx.fehbvm.com


<!-- 参考信息 -->