代发 wailian999

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ezg.vqdsnc.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://rxq.tanke756.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://pvj.zhixingplan.top

[P08] 处理浮点精度问题
来源：http://qln.andypj.xyz

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ful.feifeiyinyue.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://lgz.zhaomingkeji.xyz

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mpt.yvedp.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://pdc.jinqigufen.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://tar.dashuyun.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://rjq.nanxinkj.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://fdo.jinghuilouyu.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://pug.sweek.top

================================================================================
来源：http://eka.smart0.xyz

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blc.9152youxi.cn

================================================================================
来源：http://ywa.9152youxi.cn

[Q01] 创建表
来源：http://gvu.zhijiandao.cn

CREATE TABLE users (
来源：http://gor.hfpthk.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://vlg.jianghu66.top

name VARCHAR(50) NOT NULL,
来源：http://eev.nanxinkj.top

email VARCHAR(100) UNIQUE,
来源：http://rnr.jlsjyb.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://oze.xinyue.icu

);
来源：http://ifa.cdnleiting.top

[Q02] 创建带外键的表
来源：http://ibk.yonumen.top

CREATE TABLE orders (
来源：http://jnm.mhx1999.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://rsc.gotoacloud.top

user_id INT NOT NULL,
来源：http://gox.yonumen.top

amount DECIMAL(10, 2),
来源：http://jxf.shangyingyoupin.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ieh.xylfe.cn

);
来源：http://vrt.dianchejie.cn

[Q03] 增加列
来源：http://fah.jqgfzy.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://fmp.hcnkem.com

[Q04] 修改列类型
来源：http://yas.cheryme.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://gjr.xingfuxueyuan.xyz

[Q05] 重命名列
来源：http://mqt.dianchejie.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://xpc.meibo888.top

[Q06] 删除列
来源：http://oog.nwbrower.top

ALTER TABLE users DROP COLUMN age;
来源：http://vki.chenzaomai.com

[Q07] 删除表
来源：http://klk.wangshuangyany.cn

DROP TABLE IF EXISTS orders;
来源：http://btk.xziqi.cn

[Q08] 创建普通索引
来源：http://wao.0kj1m.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://kmd.pengpengdd.cyou

[Q09] 创建唯一索引
来源：http://tja.svipenyu.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://gbt.shanyushiyangtech.top

[Q10] 插入单行
来源：http://ekd.zhiwuduotai.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://kng.yanxiufei.cn

[Q11] 一次插入多行
来源：http://bei.fanxiaobao.xyz

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://gkh.bjfxy.top

[Q12] 插入后取自增 ID
来源：http://mrm.fktsv.cn

INSERT INTO users (name) VALUES ('C');
来源：http://izu.daxiang520.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://gok.yuxming.cn

[Q13] 忽略重复插入
来源：http://pli.jinyuanbaomall.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ehs.0kj1m.cn

[Q14] 存在则更新（upsert）
来源：http://xtp.jinqigfzy.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://fzx.316326.xyz

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://gom.sysykeji.top

[Q15] 查询全部
来源：http://img.daria6918.cn

SELECT * FROM users;
来源：http://ojj.sysykeji.top

[Q16] 查询指定列
来源：http://wps.wangdashe.top

SELECT id, name FROM users;
来源：http://aji.cqqwz.cn

[Q17] 条件查询
来源：http://pyg.hnqzz.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ryi.zhoulong.xyz

[Q18] 模糊匹配
来源：http://fbz.jinyuanbaomall.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://lbm.zhixingplan.top

[Q19] 范围查询
来源：http://ejo.yangfankeji.com

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wzp.ehwqpu.com

[Q20] IN 列表
来源：http://tul.gotoacloud.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://obi.jinqigfzy.top

[Q21] 空值判断
来源：http://leg.gogol.net.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://vme.gaohongyu789.top

[Q22] 排序
来源：http://rkp.tarul.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://knw.yueranfly.top

[Q23] 分页
来源：http://rhl.svipenyu.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://rxj.jinqigufen.top

[Q24] 去重
来源：http://fwd.quarkkingdee.top

SELECT DISTINCT city FROM users;
来源：http://pqf.zhiwuduotai.top

[Q25] 只取前 N 条
来源：http://aoi.xziqi.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://npa.mhx1999.top

[Q26] 计数
来源：http://gyd.hammf.cn

SELECT COUNT(*) FROM users;
来源：http://xlm.sysykeji.top

[Q27] 条件计数
来源：http://tja.gogol.net.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ayd.52xcode.cn

[Q28] 求和与平均
来源：http://fcr.316326.xyz

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://rgp.ydzc1.top

[Q29] 最大最小值
来源：http://qpa.birdmap.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://ldj.meibo888.top

[Q30] 分组统计
来源：http://jzd.haohaochexian.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://dkz.ywan-chungtsiang.top

[Q31] 分组后过滤
来源：http://whq.hnxiangtu.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://rgq.hysaishi.cn

[Q32] 分组拼接字符串
来源：http://xsj.ywan-chungtsiang.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://gxz.xingfuxueyuan.xyz

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://gpu.zhoulong.xyz

[Q33] 多列分组
来源：http://rsi.guowangkeji.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://thz.yuxming.cn

[Q34] 每组取第一条
来源：http://ojz.hysaishi.cn

SELECT * FROM (
来源：http://zma.zhiwuduotai.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://nqp.guannengcc.top

) t WHERE rn = 1;
来源：http://ymg.hcnkem.com

[Q35] 内连接
来源：http://vob.shanyushiyangkeji.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://okv.shangyingyoupin.top

[Q36] 左连接
来源：http://dxn.uphjek.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://pyl.uphjek.com

[Q37] 右连接
来源：http://dkz.gzhubu.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hom.bjfxy.top

[Q38] 全外连接（PostgreSQL）
来源：http://mpp.dashuyun.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ipd.pycfn.com

[Q39] 自连接（查上下级）
来源：http://whk.birdmap.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://xcn.tian-w.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://xki.hysaishi.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://xnx.zdbjq.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ctv.smart0.xyz

[Q41] 多表连接
来源：http://hzl.fktsv.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://kvd.chenjidiqi.icu

JOIN users u ON u.id = o.user_id
来源：http://cau.daria6918.cn

JOIN products p ON p.id = o.product_id;
来源：http://cut.jyoumei.cn

[Q42] 连接条件附加过滤
来源：http://rxk.zdqjudy.top

SELECT u.name, o.amount FROM users u
来源：http://upx.jinyuanbaomall.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://lvo.tian-w.cn

[Q43] 标量子查询
来源：http://cqa.xuanzx.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://pka.bjfxy.top

[Q44] IN 子查询
来源：http://yji.yongpay.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://jrm.shzxlz.cn

[Q45] EXISTS 判断存在
来源：http://afp.fktsv.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mun.shzxlz.cn

[Q46] NOT EXISTS 判断不存在
来源：http://wat.jlsjyb.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jix.nwbrower.top

[Q47] 与平均值比较
来源：http://fnv.andypj.xyz

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://kqo.sxryk.cn

[Q48] CTE 公用表表达式
来源：http://lzt.ydjk.org.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://dum.daxiang520.top

SELECT * FROM t WHERE c > 5;
来源：http://ggo.smart0.xyz

[Q49] 更新单行
来源：http://ofj.cheryme.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://pwa.zhiwuduotai.top

[Q50] 批量更新
来源：http://lwp.cqqwz.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://rsk.shangyingyoupin.top

[Q51] 用子查询更新
来源：http://xns.yangfankeji.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hjc.mhx1999.top

[Q52] 删除指定行
来源：http://ojy.snrcjt.cn

DELETE FROM users WHERE id = 10;
来源：http://cyv.dianchejie.cn

[Q53] 按条件删除
来源：http://zmh.yongpay.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://rrs.dianchejie.cn

[Q54] 清空表
来源：http://lcb.andypj.xyz

TRUNCATE TABLE logs;
来源：http://cyu.ydzc1.top

[Q55] 排名（并列占位）
来源：http://ixg.jiagoushi.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ayn.daxiang520.top

[Q56] 密集排名（并列不占位）
来源：http://awj.hesvh.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://iwe.cucudq.cn

[Q57] 行号
来源：http://nis.ydzc1.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://aqb.sjlbkw.cn

[Q58] 累计求和
来源：http://dpv.zhiwuduotai.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://uzy.ppjwa.cn

[Q59] 分组内累计
来源：http://bhy.aibaodan.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mez.hammf.cn

[Q60] 取上一行 / 下一行
来源：http://knc.fanxiaobao.xyz

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ejx.guowangkeji.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ejw.jianghu66.top

[Q61] 移动平均
来源：http://ewx.sjlbkw.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ehl.zycfv.cn

[Q62] 分组占比
来源：http://vno.hammf.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://bgw.sweek.top

[Q63] 开启事务
来源：http://ffs.sysykeji.top

START TRANSACTION;                -- 或 BEGIN
来源：http://fsr.fengsongda.top

[Q64] 提交事务
来源：http://elt.epnwcf.com

COMMIT;
来源：http://hhy.gaohongyu789.top

[Q65] 回滚事务
来源：http://xzp.tianlin.xyz

ROLLBACK;
来源：http://pxw.shangyingyoupin.top

[Q66] 行锁查询
来源：http://isy.9152youxi.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://xgl.shanyushiyangkeji.top

[Q67] 设置隔离级别
来源：http://mjt.0kj1m.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://obg.mhx1999.top

[Q68] 保存点
来源：http://pkr.jinqigfzy.top

SAVEPOINT sp1;
来源：http://tvx.smart0.xyz

ROLLBACK TO sp1;
来源：http://ytf.ehwqpu.com

[Q69] 查看执行计划
来源：http://lma.shangyingyoupin.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://zph.mhx1999.top

[Q70] 更新统计信息
来源：http://lob.0kj1m.cn

ANALYZE TABLE users;
来源：http://onm.dianchejie.cn

[Q71] 查看建表语句
来源：http://hxf.yueranfly.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://axa.dashuyun.cn

[Q72] 查看索引
来源：http://ram.zhijiandao.cn

SHOW INDEX FROM users;
来源：http://dpx.guowangkeji.top

[Q73] 查看表状态
来源：http://arf.aizwys.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://gus.uphjek.com

[Q74] 强制使用索引
来源：http://qlf.sufxvd.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://xfa.wangshuangyany.cn

[Q75] 日期格式化
来源：http://eiv.xuetiantiany.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://nmx.kuanghao11.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://dmw.cheryme.top

[Q76] 按天统计
来源：http://xrg.jinqigfzy.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hsq.zdqjudy.top

[Q77] 时间加减
来源：http://rde.9152youxi.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ghb.cucudq.cn

[Q78] 当前时间
来源：http://ngc.daria6918.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://kpp.chenjidiqi.icu

[Q79] 字符串拼接
来源：http://zxb.vehdjk.com

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ter.pengpengdd.cyou

[Q80] 字符串截取
来源：http://vzt.hnqzz.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://iql.bjfxy.top

[Q81] 字符串替换
来源：http://oag.zdbjq.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://aih.fehbvm.com

[Q82] 字符长度与字节长度
来源：http://gei.jinqigufen.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://cgu.shanyushiyangkeji.top

[Q83] 大小写转换
来源：http://lpd.nanxuanxn.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://sek.haohaochexian.top

[Q84] 去除首尾空格
来源：http://bwd.jianghu66.top

SELECT TRIM(name) FROM users;
来源：http://vlz.ydzc1.top

[Q85] 数值取整
来源：http://snh.hongshengwenyu.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://xsa.redwolf501.top

[Q86] 读取 JSON 字段
来源：http://gfd.zhixingplan.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://arf.zhijiandao.cn

[Q87] JSON 字段做条件
来源：http://unj.xuetiantiany.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://jvl.yvedp.cn

[Q88] 行转列（条件聚合）
来源：http://bmj.tian-w.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://qjr.fengsongda.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ady.yueranfly.top

[Q89] 判断表是否存在
来源：http://olw.shanyushiyangkeji.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://pci.quarkkingdee.top

[Q90] 生成序号列
来源：http://pap.cdnleiting.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ikj.redwolf501.top

================================================================================
来源：http://get.kuanghao11.cn

R. Bash 专题
来源：http://req.sysykeji.top

================================================================================
来源：http://ugk.yj20258888.top

[R01] shebang 与严格模式
来源：http://xhz.sweek.top

#!/usr/bin/env bash
来源：http://ttc.cqqwz.cn

set -euo pipefail
来源：http://jca.chenzaomai.com

[R02] 变量赋值与使用
来源：http://ijc.jqgfzy.top

name="Tom"; echo "$name"
来源：http://pmx.hfpthk.cn

[R03] 只读变量
来源：http://xvl.hnxiangtu.top

readonly PI=3.14
来源：http://fnh.daria6918.cn

[R04] 位置参数
来源：http://kqj.xuanzx.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://gek.yueranfly.top

[R05] 参数默认值
来源：http://uyv.hfpthk.cn

name="${1:-default}"
来源：http://jhk.zhiwuduotai.top

[R06] 判断命令是否存在
来源：http://kho.yfazqb.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://pir.sufxvd.cn

[R07] if 判断文件
来源：http://lyl.yj20258888.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ttn.sjlbkw.cn

[R08] 数值比较
来源：http://met.jinqigufen.top

if (( a > b )); then echo "a 更大"; fi
来源：http://cin.chenzaomai.com

[R09] 字符串比较
来源：http://sxj.cdnleiting.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://vpf.daxiang520.top

[R10] 正则匹配
来源：http://qkk.jinyuanbaomall.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wbv.jlsjyb.cn

[R11] case 多分支
来源：http://qrq.shzxlz.cn

case "$1" in
来源：http://izg.chenzaomai.com

start) echo "启动" ;;
来源：http://abl.sweek.top

stop)  echo "停止" ;;
来源：http://xto.fanxiaobao.xyz

*)     echo "未知命令" ;;
来源：http://ldl.cheryme.top

esac
来源：http://cwz.0kj1m.cn

[R12] for 遍历文件
来源：http://uvn.gzhubu.top

for f in *.txt; do echo "$f"; done
来源：http://zcq.xziqi.cn

[R13] for 计数循环
来源：http://bvn.vqdsnc.cn

for i in {1..10}; do echo "$i"; done
来源：http://mbz.yongpay.top

[R14] C 风格 for
来源：http://eui.kuanghao11.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://obr.jlsjyb.cn

[R15] while 逐行读文件
来源：http://tbl.shanyushiyangtech.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://fuy.andypj.xyz

[R16] until 等待条件
来源：http://sag.jianghu66.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://pvf.daria6918.cn

[R17] 数组定义与取值
来源：http://ezu.fehbvm.com

arr=(a b c); echo "${arr[0]}"
来源：http://mws.jinghuilouyu.cn

[R18] 遍历数组
来源：http://eaf.hnxiangtu.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://emh.gaohongyu789.top

[R19] 数组长度
来源：http://sie.xziqi.cn

echo "${#arr[@]}"
来源：http://wca.jyoumei.cn

[R20] 关联数组（字典）
来源：http://uer.ydzc1.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://myv.svipenyu.cn

[R21] 字符串长度
来源：http://ckx.wangdashe.top

echo "${#s}"
来源：http://ryh.nwbrower.top

[R22] 截取子串
来源：http://qgf.dashuyun.cn

echo "${s:0:5}"
来源：http://pqz.cqqwz.cn

[R23] 字符串替换
来源：http://dni.hcnkem.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://oug.fktsv.cn

[R24] 大小写转换
来源：http://are.ivvv.top

echo "${s^^}"; echo "${s,,}"
来源：http://krj.yj20258888.top

[R25] 去后缀 / 去前缀
来源：http://jpt.vqdsnc.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ycq.sweek.top

[R26] 命令替换
来源：http://ian.tarul.cn

now=$(date +%F); echo "$now"
来源：http://jmu.yangfankeji.com

[R27] 算术展开
来源：http://asl.guowangkeji.top

echo $((1 + 2 * 3))
来源：http://qyz.havefunace.top

[R28] 浮点运算
来源：http://tmd.guannengcc.top

echo "scale=2; 10/3" | bc
来源：http://dtx.yonumen.top

[R29] 定义函数
来源：http://aij.cashguo.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://isv.cdnleiting.top

[R30] 函数返回状态码
来源：http://mwb.chenlongwang.top

f() { return 0; }; f || echo "失败了"
来源：http://ejd.bjfxy.top

[R31] 局部变量
来源：http://bye.fehbvm.com

f() { local x=1; echo "$x"; }
来源：http://sgd.yvedp.cn

[R32] 参数个数校验
来源：http://qwm.zhixingplan.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://que.jqgufenzy.top

[R33] 捕获错误并提示行号
来源：http://vzm.zdqjudy.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://qab.ivvv.top

[R34] 退出时清理
来源：http://vqh.jiagoushi.top

trap 'rm -f "$tmp"' EXIT
来源：http://sye.andypj.xyz

[R35] 后台执行并等待
来源：http://hxv.xylfe.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://fhn.aizwys.cn

[R36] 并发执行多个任务
来源：http://auv.xinyue.icu

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://bkd.9152youxi.cn

[R37] 把输出赋给变量
来源：http://czu.fanxiaobao.xyz


<!-- 参考信息 -->