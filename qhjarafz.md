代发 wailian999

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://cpq.jyoumei.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://cgu.haohaochexian.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wyx.mhx1999.top

[P08] 处理浮点精度问题
来源：http://plx.bbcook.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://xdo.andypj.xyz

PHP:  bcadd("0.1", "0.2", 2);
来源：http://zjr.xuanzx.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ygj.yueranfly.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ehp.jlsjyb.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://gvg.gogol.net.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ylr.yj20258.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://crr.0kj1m.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hew.jinqigfzy.top

================================================================================
来源：http://vue.ydzc1.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://xoh.hesvh.cn

================================================================================
来源：http://tdy.tanke756.top

[Q01] 创建表
来源：http://xfx.redwolf501.top

CREATE TABLE users (
来源：http://dkp.jinghuilouyu.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ryf.pengpengdd.cyou

name VARCHAR(50) NOT NULL,
来源：http://txv.yanxiufei.cn

email VARCHAR(100) UNIQUE,
来源：http://hsc.smart0.xyz

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://pul.svipenyu.cn

);
来源：http://luy.sweek.top

[Q02] 创建带外键的表
来源：http://bja.ywan-chungtsiang.top

CREATE TABLE orders (
来源：http://qas.zhixingplan.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ttz.mhx1999.top

user_id INT NOT NULL,
来源：http://vwz.fengsongda.top

amount DECIMAL(10, 2),
来源：http://qyc.cheryme.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://auq.316326.xyz

);
来源：http://ewq.316326.xyz

[Q03] 增加列
来源：http://rbj.shanyushiyangkeji.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://zeq.fzhhl.top

[Q04] 修改列类型
来源：http://hww.jqgufenzy.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mhu.jinqigfzy.top

[Q05] 重命名列
来源：http://wdk.epnwcf.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://qst.yanxiufei.cn

[Q06] 删除列
来源：http://olo.ydzc1.top

ALTER TABLE users DROP COLUMN age;
来源：http://hze.hesvh.cn

[Q07] 删除表
来源：http://vit.feifeiyinyue.top

DROP TABLE IF EXISTS orders;
来源：http://jet.epnwcf.com

[Q08] 创建普通索引
来源：http://bzu.hfpthk.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://xdn.wangdashe.top

[Q09] 创建唯一索引
来源：http://ref.316326.xyz

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://rcl.birdmap.top

[Q10] 插入单行
来源：http://toh.gotoacloud.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://lfz.yongpay.top

[Q11] 一次插入多行
来源：http://pds.snrcjt.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://zsv.hywenlv.cn

[Q12] 插入后取自增 ID
来源：http://ybb.ydjk.org.cn

INSERT INTO users (name) VALUES ('C');
来源：http://niu.zhongyouzk.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://rnv.jlsjyb.cn

[Q13] 忽略重复插入
来源：http://mos.jinghuilouyu.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://rpc.svipenyu.cn

[Q14] 存在则更新（upsert）
来源：http://gkg.jqgufenzy.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://uba.hesvh.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://xrw.fzhhl.top

[Q15] 查询全部
来源：http://ntk.hnxiangtu.top

SELECT * FROM users;
来源：http://rkh.cheryme.top

[Q16] 查询指定列
来源：http://ibg.gotoacloud.top

SELECT id, name FROM users;
来源：http://vbq.yongpay.top

[Q17] 条件查询
来源：http://tyr.shanyushiyangkeji.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://qoj.sxryk.cn

[Q18] 模糊匹配
来源：http://hsj.hcnkem.com

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wzw.gaohongyu789.top

[Q19] 范围查询
来源：http://csc.hfpthk.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://nrr.shuidangran.top

[Q20] IN 列表
来源：http://oem.tian-w.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://uwg.shanyushiyangtech.top

[Q21] 空值判断
来源：http://ihf.daxiang520.top

SELECT * FROM users WHERE email IS NULL;
来源：http://mnz.tianlin.xyz

[Q22] 排序
来源：http://wkw.ctjpmb.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ggm.ydzc1.top

[Q23] 分页
来源：http://bnj.fktsv.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://che.zhiwuduotai.top

[Q24] 去重
来源：http://whi.ydjk.org.cn

SELECT DISTINCT city FROM users;
来源：http://vaj.gogol.net.cn

[Q25] 只取前 N 条
来源：http://hiz.fehbvm.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://fgj.ydzc1.top

[Q26] 计数
来源：http://hno.hfpthk.cn

SELECT COUNT(*) FROM users;
来源：http://wln.chenzaomai.com

[Q27] 条件计数
来源：http://swt.gaohongyu789.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hgw.redwolf501.top

[Q28] 求和与平均
来源：http://vdo.haohaochexian.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://lic.yongpay.top

[Q29] 最大最小值
来源：http://hlc.redwolf501.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://geq.epnwcf.com

[Q30] 分组统计
来源：http://lya.smart0.xyz

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ecs.andypj.xyz

[Q31] 分组后过滤
来源：http://pxk.jlsjyb.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://qwf.ppjwa.cn

[Q32] 分组拼接字符串
来源：http://kxm.andypj.xyz

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://abs.nwbrower.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://pse.fanxiaobao.xyz

[Q33] 多列分组
来源：http://rmm.wangdashe.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://lva.sjlbkw.cn

[Q34] 每组取第一条
来源：http://mcs.hysaishi.cn

SELECT * FROM (
来源：http://qvw.yongpay.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://iqv.yvedp.cn

) t WHERE rn = 1;
来源：http://akz.aibaodan.cn

[Q35] 内连接
来源：http://emn.daria6918.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://lvg.tianlin.xyz

[Q36] 左连接
来源：http://lyy.jiagoushi.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://kod.shanyushiyangkeji.top

[Q37] 右连接
来源：http://ueh.jlsjyb.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://nqs.mhx1999.top

[Q38] 全外连接（PostgreSQL）
来源：http://stm.vehdjk.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://cdi.yongpay.top

[Q39] 自连接（查上下级）
来源：http://afc.yj20258.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://psw.ivvv.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://dvx.ydjk.org.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://sai.zycfv.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ozn.yj202588.top

[Q41] 多表连接
来源：http://zzf.shzxlz.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://xfy.ppjwa.cn

JOIN users u ON u.id = o.user_id
来源：http://edp.quarkkingdee.top

JOIN products p ON p.id = o.product_id;
来源：http://fhy.redwolf501.top

[Q42] 连接条件附加过滤
来源：http://lns.svipenyu.cn

SELECT u.name, o.amount FROM users u
来源：http://kns.yuanzhike.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://sve.andypj.xyz

[Q43] 标量子查询
来源：http://ruo.ydjk.org.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://lsi.yvedp.cn

[Q44] IN 子查询
来源：http://fdx.fktsv.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://osu.shangyingyoupin.top

[Q45] EXISTS 判断存在
来源：http://tyh.zhijiandao.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qsi.sxryk.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ndu.havefunace.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://aoz.dashuyun.cn

[Q47] 与平均值比较
来源：http://gcd.pengpengdd.cyou

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://elr.quarkkingdee.top

[Q48] CTE 公用表表达式
来源：http://tms.cheryme.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://fop.vqdsnc.cn

SELECT * FROM t WHERE c > 5;
来源：http://pxz.yonumen.top

[Q49] 更新单行
来源：http://vgn.ywan-chungtsiang.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://pso.dianchejie.cn

[Q50] 批量更新
来源：http://gap.tanke756.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://qth.vqdsnc.cn

[Q51] 用子查询更新
来源：http://lof.sufxvd.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://cmx.hesvh.cn

[Q52] 删除指定行
来源：http://lkn.yj20258888.top

DELETE FROM users WHERE id = 10;
来源：http://sae.yfazqb.com

[Q53] 按条件删除
来源：http://uns.bbcook.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://tpr.meibo888.top

[Q54] 清空表
来源：http://vsb.feifeiyinyue.top

TRUNCATE TABLE logs;
来源：http://joo.cqqwz.cn

[Q55] 排名（并列占位）
来源：http://gan.dashuyun.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://fji.chenlongwang.top

[Q56] 密集排名（并列不占位）
来源：http://bfx.pycfn.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://tnq.yanxiufei.cn

[Q57] 行号
来源：http://daa.nanxinkj.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mhg.shzxlz.cn

[Q58] 累计求和
来源：http://yjo.yueranfly.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ydc.yueranfly.top

[Q59] 分组内累计
来源：http://zax.hnqzz.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://yff.fzhhl.top

[Q60] 取上一行 / 下一行
来源：http://dlg.havefunace.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wik.cheryme.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://gvq.jianghu66.top

[Q61] 移动平均
来源：http://zkg.wangshuangyany.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://daq.tarul.cn

[Q62] 分组占比
来源：http://vvg.pycfn.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://vlm.hfpthk.cn

[Q63] 开启事务
来源：http://fxb.aizwys.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://kiu.xuanzx.com

[Q64] 提交事务
来源：http://lip.jlsjyb.cn

COMMIT;
来源：http://qri.iojbl.cn

[Q65] 回滚事务
来源：http://lrm.ydzc1.top

ROLLBACK;
来源：http://qhc.jiagoushi.top

[Q66] 行锁查询
来源：http://lsg.mhx1999.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://aaz.xziqi.cn

[Q67] 设置隔离级别
来源：http://bpj.jiagoushi.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ldt.andypj.xyz

[Q68] 保存点
来源：http://fkn.ctjpmb.com

SAVEPOINT sp1;
来源：http://nwy.hysaishi.cn

ROLLBACK TO sp1;
来源：http://fuq.aibaodan.cn

[Q69] 查看执行计划
来源：http://dtr.0kj1m.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://txr.cucudq.cn

[Q70] 更新统计信息
来源：http://pbf.yj20258.top

ANALYZE TABLE users;
来源：http://adr.316326.xyz

[Q71] 查看建表语句
来源：http://wbw.iojbl.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://pqt.hesvh.cn

[Q72] 查看索引
来源：http://cuq.sjlbkw.cn

SHOW INDEX FROM users;
来源：http://kkv.yongpay.top

[Q73] 查看表状态
来源：http://ijf.jlsjyb.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ype.sxryk.cn

[Q74] 强制使用索引
来源：http://idb.fehbvm.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://cql.yj20258.top

[Q75] 日期格式化
来源：http://dja.cucudq.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://nht.tianlin.xyz

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://isi.jiagoushi.top

[Q76] 按天统计
来源：http://krg.c1oappe.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://lru.hongshengwenyu.top

[Q77] 时间加减
来源：http://sdl.hysaishi.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://uaz.daxiang520.top

[Q78] 当前时间
来源：http://kas.hesvh.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://gye.shanyushiyangtech.top

[Q79] 字符串拼接
来源：http://zag.guowangkeji.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://zuw.yonumen.top

[Q80] 字符串截取
来源：http://ywk.fktsv.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://dzi.jlsjyb.cn

[Q81] 字符串替换
来源：http://sst.zhoulong.xyz

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ucx.nwbrower.top

[Q82] 字符长度与字节长度
来源：http://oom.yvedp.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hkm.zhengqikj.top

[Q83] 大小写转换
来源：http://ifq.zhixingplan.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://vxl.kuanghao11.cn

[Q84] 去除首尾空格
来源：http://ppg.yvedp.cn

SELECT TRIM(name) FROM users;
来源：http://icx.yvedp.cn

[Q85] 数值取整
来源：http://rkx.daxiang520.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://kvl.fehbvm.com

[Q86] 读取 JSON 字段
来源：http://rbp.kuanghao11.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://krh.sysykeji.top

[Q87] JSON 字段做条件
来源：http://gcg.yonumen.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://pbp.havefunace.top

[Q88] 行转列（条件聚合）
来源：http://vjj.sweek.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ffd.xuanzx.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://jjz.jlsjyb.cn

[Q89] 判断表是否存在
来源：http://ofz.ydjk.org.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://lcg.birdmap.top

[Q90] 生成序号列
来源：http://pzp.aibaodan.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://iqq.yangfankeji.com

================================================================================
来源：http://azv.sjlbkw.cn

R. Bash 专题
来源：http://ckx.cqqwz.cn

================================================================================
来源：http://jxu.bjfxy.top

[R01] shebang 与严格模式
来源：http://ykz.zycfv.cn

#!/usr/bin/env bash
来源：http://ceu.sufxvd.cn

set -euo pipefail
来源：http://pko.hnxiangtu.top

[R02] 变量赋值与使用
来源：http://ozz.jlsjyb.cn

name="Tom"; echo "$name"
来源：http://pol.tanke756.top

[R03] 只读变量
来源：http://pxm.ctjpmb.com

readonly PI=3.14
来源：http://kim.yuanzhike.top

[R04] 位置参数
来源：http://fcf.hnqzz.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://oin.zdqjudy.top

[R05] 参数默认值
来源：http://fkz.ydjk.org.cn

name="${1:-default}"
来源：http://cze.hongshengwenyu.top

[R06] 判断命令是否存在
来源：http://kvm.ybcxt.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://rtf.xziqi.cn

[R07] if 判断文件
来源：http://xzs.tanke756.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://kvl.havefunace.top

[R08] 数值比较
来源：http://ffw.haohaochexian.top

if (( a > b )); then echo "a 更大"; fi
来源：http://hwy.quarkkingdee.top

[R09] 字符串比较
来源：http://nuc.gotoacloud.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ars.xinyue.icu

[R10] 正则匹配
来源：http://tyb.hongshengwenyu.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://cap.bjfxy.top

[R11] case 多分支
来源：http://gqk.shuidangran.top

case "$1" in
来源：http://knx.bjfxy.top

start) echo "启动" ;;
来源：http://yvv.daxiang520.top

stop)  echo "停止" ;;
来源：http://pgz.jinyuanbaomall.cn

*)     echo "未知命令" ;;
来源：http://itd.zhaomingkeji.xyz

esac
来源：http://cbe.jyoumei.cn

[R12] for 遍历文件
来源：http://wka.9152youxi.cn

for f in *.txt; do echo "$f"; done
来源：http://nub.shangyingyoupin.top

[R13] for 计数循环
来源：http://dcn.zhiwuduotai.top

for i in {1..10}; do echo "$i"; done
来源：http://lae.jinyuanbaomall.cn

[R14] C 风格 for
来源：http://ftc.9152youxi.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://gzc.hcnkem.com

[R15] while 逐行读文件
来源：http://yta.zhongyouzk.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://cyu.jinghuilouyu.cn

[R16] until 等待条件
来源：http://lto.hesvh.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mfd.0kj1m.cn

[R17] 数组定义与取值
来源：http://hes.jlsjyb.cn

arr=(a b c); echo "${arr[0]}"
来源：http://owf.uphjek.com

[R18] 遍历数组
来源：http://ngp.haohaochexian.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hjo.sweek.top

[R19] 数组长度
来源：http://rsw.redwolf501.top

echo "${#arr[@]}"
来源：http://hhm.jianghu66.top

[R20] 关联数组（字典）
来源：http://vbf.jlsjyb.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://xvc.guowangkeji.top

[R21] 字符串长度
来源：http://ixu.chenzaomai.com

echo "${#s}"
来源：http://gjk.hysaishi.cn

[R22] 截取子串
来源：http://cnv.chenlongwang.top

echo "${s:0:5}"
来源：http://dck.jinghuilouyu.cn

[R23] 字符串替换
来源：http://sse.sjlbkw.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://onr.cheryme.top

[R24] 大小写转换
来源：http://rbh.pycfn.com

echo "${s^^}"; echo "${s,,}"
来源：http://psd.hfpthk.cn

[R25] 去后缀 / 去前缀
来源：http://gvs.hesvh.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://oqq.jlsjyb.cn

[R26] 命令替换
来源：http://bku.yuxming.cn

now=$(date +%F); echo "$now"
来源：http://ujb.gaohongyu789.top

[R27] 算术展开
来源：http://jeu.dashuyun.cn

echo $((1 + 2 * 3))
来源：http://ylg.jqgufenzy.top

[R28] 浮点运算
来源：http://ndl.jqgufenzy.top

echo "scale=2; 10/3" | bc
来源：http://vux.shanyushiyangtech.top

[R29] 定义函数
来源：http://hhy.jinghuilouyu.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://nzh.dashuyun.cn

[R30] 函数返回状态码
来源：http://pwl.xylfe.cn

f() { return 0; }; f || echo "失败了"
来源：http://zer.316326.xyz

[R31] 局部变量
来源：http://jpv.c1oappe.top

f() { local x=1; echo "$x"; }
来源：http://mhr.52xcode.cn

[R32] 参数个数校验
来源：http://xze.birdmap.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mdw.chenlongwang.top

[R33] 捕获错误并提示行号
来源：http://sxa.ctjpmb.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://rfw.tanke756.top

[R34] 退出时清理
来源：http://xww.fehbvm.com

trap 'rm -f "$tmp"' EXIT
来源：http://fot.feifeiyinyue.top

[R35] 后台执行并等待
来源：http://wsv.vqdsnc.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://tjy.hcnkem.com

[R36] 并发执行多个任务
来源：http://ann.aibaodan.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://uvv.zhongyouzk.top

[R37] 把输出赋给变量
来源：http://gom.hongshengwenyu.top


<!-- 参考信息 -->