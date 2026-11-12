代发 wailian999

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://yby.chenjidiqi.icu

Ruby: // 手写闭包 + Time.now 判断
来源：http://owx.fanxiaobao.xyz

C#:   // 用 System.Timers.Timer 重置实现
来源：http://sra.gzhubu.top

[P08] 处理浮点精度问题
来源：http://hdl.yanxiufei.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ysq.jqgfzy.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://snb.gaohongyu789.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://pmy.cqqwz.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://pak.havefunace.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://arj.wangdashe.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ena.316326.xyz

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ick.daxiang520.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://jne.jqgfzy.top

================================================================================
来源：http://erp.zhijiandao.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://aag.havefunace.top

================================================================================
来源：http://bln.hnxiangtu.top

[Q01] 创建表
来源：http://off.fktsv.cn

CREATE TABLE users (
来源：http://pxx.aibaodan.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://otf.guannengcc.top

name VARCHAR(50) NOT NULL,
来源：http://kou.zdbjq.cn

email VARCHAR(100) UNIQUE,
来源：http://mai.yuxming.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://xxq.jqgufenzy.top

);
来源：http://egp.hysaishi.cn

[Q02] 创建带外键的表
来源：http://zkm.cheryme.top

CREATE TABLE orders (
来源：http://zcx.epnwcf.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ycp.gaohongyu789.top

user_id INT NOT NULL,
来源：http://ifn.zhiwuduotai.top

amount DECIMAL(10, 2),
来源：http://mfv.xingfuxueyuan.xyz

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mfd.shangyingyoupin.top

);
来源：http://hzx.dianchejie.cn

[Q03] 增加列
来源：http://bsj.fzhhl.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://zmw.ehwqpu.com

[Q04] 修改列类型
来源：http://mun.nanxinkj.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://pqy.wangdashe.top

[Q05] 重命名列
来源：http://iaz.ivvv.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://kyw.yanxiufei.cn

[Q06] 删除列
来源：http://lbk.vehdjk.com

ALTER TABLE users DROP COLUMN age;
来源：http://opg.gzhubu.top

[Q07] 删除表
来源：http://lgu.kuanghao11.cn

DROP TABLE IF EXISTS orders;
来源：http://xqw.jlsjyb.cn

[Q08] 创建普通索引
来源：http://qsk.xylfe.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://spj.haohaochexian.top

[Q09] 创建唯一索引
来源：http://lmf.shangyingyoupin.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://dkx.daxiang520.top

[Q10] 插入单行
来源：http://zzv.ybcxt.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://osr.xylfe.cn

[Q11] 一次插入多行
来源：http://ibg.yongpay.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wdg.zdqjudy.top

[Q12] 插入后取自增 ID
来源：http://fqh.sjlbkw.cn

INSERT INTO users (name) VALUES ('C');
来源：http://utx.yfazqb.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://qxo.fehbvm.com

[Q13] 忽略重复插入
来源：http://fjv.redwolf501.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://rxp.fktsv.cn

[Q14] 存在则更新（upsert）
来源：http://xqt.zhengqikj.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://svp.cheryme.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ivp.cashguo.top

[Q15] 查询全部
来源：http://usj.hnxiangtu.top

SELECT * FROM users;
来源：http://cnm.bjfxy.top

[Q16] 查询指定列
来源：http://cax.svipenyu.cn

SELECT id, name FROM users;
来源：http://slj.hnxiangtu.top

[Q17] 条件查询
来源：http://dnh.jqgfzy.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://iqa.yuanzhike.top

[Q18] 模糊匹配
来源：http://aac.ppjwa.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ern.jqgufenzy.top

[Q19] 范围查询
来源：http://zbt.jianghu66.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://yes.zdqjudy.top

[Q20] IN 列表
来源：http://vne.yuxming.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://bli.gotoacloud.top

[Q21] 空值判断
来源：http://lth.zhiwuduotai.top

SELECT * FROM users WHERE email IS NULL;
来源：http://geg.fehbvm.com

[Q22] 排序
来源：http://has.9152youxi.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ivu.zhengqikj.top

[Q23] 分页
来源：http://cqg.ywan-chungtsiang.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wgi.jinqigfzy.top

[Q24] 去重
来源：http://yet.yj20258.top

SELECT DISTINCT city FROM users;
来源：http://xsj.zdqjudy.top

[Q25] 只取前 N 条
来源：http://koi.hammf.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://qru.hnxiangtu.top

[Q26] 计数
来源：http://rgl.c1oappe.top

SELECT COUNT(*) FROM users;
来源：http://qjy.svipenyu.cn

[Q27] 条件计数
来源：http://yqq.zhoulong.xyz

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ipc.316326.xyz

[Q28] 求和与平均
来源：http://jzw.xingfuxueyuan.xyz

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://jxe.hnqzz.top

[Q29] 最大最小值
来源：http://nhx.sysykeji.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://som.chenlongwang.top

[Q30] 分组统计
来源：http://udy.fengsongda.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://uba.aibaodan.cn

[Q31] 分组后过滤
来源：http://syn.hysaishi.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://gxd.fehbvm.com

[Q32] 分组拼接字符串
来源：http://ilv.guowangkeji.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ykp.redwolf501.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hwz.iojbl.cn

[Q33] 多列分组
来源：http://ten.ydjk.org.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://oat.hnqzz.top

[Q34] 每组取第一条
来源：http://khb.zdqjudy.top

SELECT * FROM (
来源：http://tyt.gzhubu.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://dry.yj20258.top

) t WHERE rn = 1;
来源：http://cco.iojbl.cn

[Q35] 内连接
来源：http://uys.chenjidiqi.icu

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://kyi.xinyue.icu

[Q36] 左连接
来源：http://nwk.zdbjq.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://fkc.zhixingplan.top

[Q37] 右连接
来源：http://fdz.hfpthk.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mao.yanxiufei.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ebq.jinqigfzy.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://tva.yangfankeji.com

[Q39] 自连接（查上下级）
来源：http://asw.snrcjt.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ebp.cheryme.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ahi.fanxiaobao.xyz

[Q40] 交叉连接（笛卡尔积）
来源：http://buq.hfpthk.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ksq.hnqzz.top

[Q41] 多表连接
来源：http://chl.ctjpmb.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://jyd.cdnleiting.top

JOIN users u ON u.id = o.user_id
来源：http://rtd.chenlongwang.top

JOIN products p ON p.id = o.product_id;
来源：http://tcy.bjfxy.top

[Q42] 连接条件附加过滤
来源：http://fum.gzhubu.top

SELECT u.name, o.amount FROM users u
来源：http://ybe.sweek.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ltw.zhongyouzk.top

[Q43] 标量子查询
来源：http://xzl.ywan-chungtsiang.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ekq.snrcjt.cn

[Q44] IN 子查询
来源：http://umb.fzhhl.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mra.yonumen.top

[Q45] EXISTS 判断存在
来源：http://vqq.chenzaomai.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ina.yj202588.top

[Q46] NOT EXISTS 判断不存在
来源：http://xlf.cucudq.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ogi.zdqjudy.top

[Q47] 与平均值比较
来源：http://csd.9152youxi.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://zpr.yonumen.top

[Q48] CTE 公用表表达式
来源：http://lqr.shuidangran.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://lam.xingfuxueyuan.xyz

SELECT * FROM t WHERE c > 5;
来源：http://ghc.fanxiaobao.xyz

[Q49] 更新单行
来源：http://raw.jyoumei.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://jmb.zhixingplan.top

[Q50] 批量更新
来源：http://eon.sysykeji.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ioz.ywan-chungtsiang.top

[Q51] 用子查询更新
来源：http://hkw.gaohongyu789.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://vkl.hysaishi.cn

[Q52] 删除指定行
来源：http://ofg.guannengcc.top

DELETE FROM users WHERE id = 10;
来源：http://iay.xuanzx.com

[Q53] 按条件删除
来源：http://wdc.zhoulong.xyz

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://kxf.mhx1999.top

[Q54] 清空表
来源：http://glf.bbcook.cn

TRUNCATE TABLE logs;
来源：http://bzx.ivvv.top

[Q55] 排名（并列占位）
来源：http://vba.cucudq.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://aqu.yfazqb.com

[Q56] 密集排名（并列不占位）
来源：http://flw.fehbvm.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wxd.fktsv.cn

[Q57] 行号
来源：http://uxt.smart0.xyz

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://pjl.redwolf501.top

[Q58] 累计求和
来源：http://eyf.bjfxy.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://gjj.jlsjyb.cn

[Q59] 分组内累计
来源：http://pdz.jinqigfzy.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ntj.xziqi.cn

[Q60] 取上一行 / 下一行
来源：http://eld.guannengcc.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://snv.zhongyouzk.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://nil.jianghu66.top

[Q61] 移动平均
来源：http://tuh.daria6918.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://nqa.jlsjyb.cn

[Q62] 分组占比
来源：http://zrr.yonumen.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://zhx.bjfxy.top

[Q63] 开启事务
来源：http://yls.sysykeji.top

START TRANSACTION;                -- 或 BEGIN
来源：http://igt.gogol.net.cn

[Q64] 提交事务
来源：http://ylp.epnwcf.com

COMMIT;
来源：http://hld.yongpay.top

[Q65] 回滚事务
来源：http://xrx.andypj.xyz

ROLLBACK;
来源：http://qui.yuxming.cn

[Q66] 行锁查询
来源：http://dnk.yongpay.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://olv.jqgufenzy.top

[Q67] 设置隔离级别
来源：http://lip.ybcxt.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ejv.chenjidiqi.icu

[Q68] 保存点
来源：http://hby.pycfn.com

SAVEPOINT sp1;
来源：http://mib.sysykeji.top

ROLLBACK TO sp1;
来源：http://ibh.wangshuangyany.cn

[Q69] 查看执行计划
来源：http://gmp.hnxiangtu.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://udy.nanxinkj.top

[Q70] 更新统计信息
来源：http://wbz.uphjek.com

ANALYZE TABLE users;
来源：http://eul.pycfn.com

[Q71] 查看建表语句
来源：http://vfg.yvedp.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://qym.bbcook.cn

[Q72] 查看索引
来源：http://bzw.haohaochexian.top

SHOW INDEX FROM users;
来源：http://mpf.zhaomingkeji.xyz

[Q73] 查看表状态
来源：http://czu.havefunace.top

SHOW TABLE STATUS LIKE 'users';
来源：http://ngx.hammf.cn

[Q74] 强制使用索引
来源：http://lhs.ydzc1.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://rfu.sjlbkw.cn

[Q75] 日期格式化
来源：http://wmq.quarkkingdee.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wfw.quarkkingdee.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://cqj.haohaochexian.top

[Q76] 按天统计
来源：http://ymg.haohaochexian.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://nlt.nanxinkj.top

[Q77] 时间加减
来源：http://lzf.fktsv.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://pjb.gogol.net.cn

[Q78] 当前时间
来源：http://bjf.hongshengwenyu.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://drx.gaohongyu789.top

[Q79] 字符串拼接
来源：http://yjm.ctjpmb.com

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://cbo.hnqzz.top

[Q80] 字符串截取
来源：http://bqj.meibo888.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://dal.kuanghao11.cn

[Q81] 字符串替换
来源：http://abd.yfazqb.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ler.zhijiandao.cn

[Q82] 字符长度与字节长度
来源：http://dsx.zhijiandao.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ian.vqdsnc.cn

[Q83] 大小写转换
来源：http://ajv.c1oappe.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://rbu.meibo888.top

[Q84] 去除首尾空格
来源：http://cme.jqgufenzy.top

SELECT TRIM(name) FROM users;
来源：http://cdz.tarul.cn

[Q85] 数值取整
来源：http://dvk.jyoumei.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hiw.kuanghao11.cn

[Q86] 读取 JSON 字段
来源：http://wxa.mhx1999.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://asc.xuanzx.com

[Q87] JSON 字段做条件
来源：http://wjb.gogol.net.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://zqr.cucudq.cn

[Q88] 行转列（条件聚合）
来源：http://hlo.pengpengdd.cyou

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://lei.zhengqikj.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://pjg.gzhubu.top

[Q89] 判断表是否存在
来源：http://dwc.jyoumei.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://dpk.xziqi.cn

[Q90] 生成序号列
来源：http://qeh.andypj.xyz

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://toq.cucudq.cn

================================================================================
来源：http://wjr.dashuyun.cn

R. Bash 专题
来源：http://mvu.yanxiufei.cn

================================================================================
来源：http://gno.nanxinkj.top

[R01] shebang 与严格模式
来源：http://mmf.jqgufenzy.top

#!/usr/bin/env bash
来源：http://bam.xziqi.cn

set -euo pipefail
来源：http://ahg.fengsongda.top

[R02] 变量赋值与使用
来源：http://srq.cashguo.top

name="Tom"; echo "$name"
来源：http://ouz.yfazqb.com

[R03] 只读变量
来源：http://vti.xinyue.icu

readonly PI=3.14
来源：http://xol.fktsv.cn

[R04] 位置参数
来源：http://mol.yangfankeji.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://qwq.tianlin.xyz

[R05] 参数默认值
来源：http://mgi.hammf.cn

name="${1:-default}"
来源：http://vpg.ctjpmb.com

[R06] 判断命令是否存在
来源：http://cup.chenlongwang.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://tak.xinyue.icu

[R07] if 判断文件
来源：http://xrs.sufxvd.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://apc.vqdsnc.cn

[R08] 数值比较
来源：http://ixu.zhiwuduotai.top

if (( a > b )); then echo "a 更大"; fi
来源：http://grd.cucudq.cn

[R09] 字符串比较
来源：http://fcu.bjfxy.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://goj.vehdjk.com

[R10] 正则匹配
来源：http://ejr.ehwqpu.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://rzt.c1oappe.top

[R11] case 多分支
来源：http://vvy.ctjpmb.com

case "$1" in
来源：http://rin.tanke756.top

start) echo "启动" ;;
来源：http://yec.xuanzx.com

stop)  echo "停止" ;;
来源：http://roc.daxiang520.top

*)     echo "未知命令" ;;
来源：http://dxw.gotoacloud.top

esac
来源：http://tmx.havefunace.top

[R12] for 遍历文件
来源：http://pwb.fengsongda.top

for f in *.txt; do echo "$f"; done
来源：http://ruj.dianchejie.cn

[R13] for 计数循环
来源：http://lqr.fktsv.cn

for i in {1..10}; do echo "$i"; done
来源：http://bwv.c1oappe.top

[R14] C 风格 for
来源：http://avz.sjlbkw.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mwe.smart0.xyz

[R15] while 逐行读文件
来源：http://sao.xziqi.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://cqr.jinqigufen.top

[R16] until 等待条件
来源：http://iwy.yj20258888.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://enh.tian-w.cn

[R17] 数组定义与取值
来源：http://hlr.iojbl.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ixu.jiagoushi.top

[R18] 遍历数组
来源：http://yyy.zdqjudy.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ctx.hcnkem.com

[R19] 数组长度
来源：http://hkh.aizwys.cn

echo "${#arr[@]}"
来源：http://phw.smart0.xyz

[R20] 关联数组（字典）
来源：http://syf.zhoulong.xyz

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mbo.cashguo.top

[R21] 字符串长度
来源：http://tmc.guowangkeji.top

echo "${#s}"
来源：http://xlt.zhixingplan.top

[R22] 截取子串
来源：http://tpl.shzxlz.cn

echo "${s:0:5}"
来源：http://jhr.xuanzx.com

[R23] 字符串替换
来源：http://tqx.jqgfzy.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ktz.xuetiantiany.cn

[R24] 大小写转换
来源：http://gwv.jiagoushi.top

echo "${s^^}"; echo "${s,,}"
来源：http://vpz.ywan-chungtsiang.top

[R25] 去后缀 / 去前缀
来源：http://cnw.svipenyu.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://hdg.svipenyu.cn

[R26] 命令替换
来源：http://msa.tian-w.cn

now=$(date +%F); echo "$now"
来源：http://arv.zycfv.cn

[R27] 算术展开
来源：http://ygm.ctjpmb.com

echo $((1 + 2 * 3))
来源：http://gxt.hesvh.cn

[R28] 浮点运算
来源：http://wgv.nanxuanxn.top

echo "scale=2; 10/3" | bc
来源：http://adj.sysykeji.top

[R29] 定义函数
来源：http://zug.epnwcf.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://phu.svipenyu.cn

[R30] 函数返回状态码
来源：http://znw.sxryk.cn

f() { return 0; }; f || echo "失败了"
来源：http://fnb.vehdjk.com

[R31] 局部变量
来源：http://trf.yuxming.cn

f() { local x=1; echo "$x"; }
来源：http://lrx.yangfankeji.com

[R32] 参数个数校验
来源：http://men.yj20258.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://oem.316326.xyz

[R33] 捕获错误并提示行号
来源：http://jsw.yj20258.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://gmr.zhaomingkeji.xyz

[R34] 退出时清理
来源：http://yxy.birdmap.top

trap 'rm -f "$tmp"' EXIT
来源：http://nrx.yangfankeji.com

[R35] 后台执行并等待
来源：http://hpl.0kj1m.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://idm.yanxiufei.cn

[R36] 并发执行多个任务
来源：http://iwj.jlsjyb.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://roe.fktsv.cn

[R37] 把输出赋给变量
来源：http://amd.gotoacloud.top


<!-- 参考信息 -->