代发 wailian999

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ujk.cucudq.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://cuk.andypj.xyz

C#:   // 用 System.Timers.Timer 重置实现
来源：http://sls.snrcjt.cn

[P08] 处理浮点精度问题
来源：http://xnv.jinqigufen.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hfw.pycfn.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://nbq.hongshengwenyu.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://kns.ywan-chungtsiang.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ife.nanxuanxn.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://nah.ywan-chungtsiang.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://sxy.ehwqpu.com

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://dnk.gzhubu.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://joi.zhengqikj.top

================================================================================
来源：http://xzb.yonumen.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://moj.tian-w.cn

================================================================================
来源：http://wmy.bbcook.cn

[Q01] 创建表
来源：http://hzc.guowangkeji.top

CREATE TABLE users (
来源：http://aqs.tian-w.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://avr.chenzaomai.com

name VARCHAR(50) NOT NULL,
来源：http://lcf.cucudq.cn

email VARCHAR(100) UNIQUE,
来源：http://zgz.ctjpmb.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://vsh.fktsv.cn

);
来源：http://pgy.yuanzhike.top

[Q02] 创建带外键的表
来源：http://isf.chenjidiqi.icu

CREATE TABLE orders (
来源：http://ybo.ybcxt.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ibg.jiagoushi.top

user_id INT NOT NULL,
来源：http://geg.epnwcf.com

amount DECIMAL(10, 2),
来源：http://fzw.zhoulong.xyz

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://oby.chenzaomai.com

);
来源：http://bcx.wangshuangyany.cn

[Q03] 增加列
来源：http://pia.tianlin.xyz

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wuh.jqgfzy.top

[Q04] 修改列类型
来源：http://koj.mhx1999.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://coz.52xcode.cn

[Q05] 重命名列
来源：http://mhq.birdmap.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hdq.meibo888.top

[Q06] 删除列
来源：http://jyl.zhengqikj.top

ALTER TABLE users DROP COLUMN age;
来源：http://set.fzhhl.top

[Q07] 删除表
来源：http://odq.yuxming.cn

DROP TABLE IF EXISTS orders;
来源：http://ect.jinqigufen.top

[Q08] 创建普通索引
来源：http://bmh.cheryme.top

CREATE INDEX idx_users_email ON users(email);
来源：http://ezl.yj20258.top

[Q09] 创建唯一索引
来源：http://oih.kuanghao11.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://tze.mhx1999.top

[Q10] 插入单行
来源：http://lut.tarul.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ehq.fengsongda.top

[Q11] 一次插入多行
来源：http://ero.nwbrower.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hrb.jlsjyb.cn

[Q12] 插入后取自增 ID
来源：http://gyd.fktsv.cn

INSERT INTO users (name) VALUES ('C');
来源：http://cro.uphjek.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://vcs.xuetiantiany.cn

[Q13] 忽略重复插入
来源：http://mdp.cashguo.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://lar.hongshengwenyu.top

[Q14] 存在则更新（upsert）
来源：http://zss.jqgfzy.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://bcm.daxiang520.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://tph.yuxming.cn

[Q15] 查询全部
来源：http://cnk.sweek.top

SELECT * FROM users;
来源：http://xke.0kj1m.cn

[Q16] 查询指定列
来源：http://ayu.jlsjyb.cn

SELECT id, name FROM users;
来源：http://nkx.ywan-chungtsiang.top

[Q17] 条件查询
来源：http://mca.hcnkem.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://udi.hnxiangtu.top

[Q18] 模糊匹配
来源：http://dxh.nwbrower.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ttd.yangfankeji.com

[Q19] 范围查询
来源：http://oyd.jiagoushi.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ood.sysykeji.top

[Q20] IN 列表
来源：http://umt.316326.xyz

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://jpq.kuanghao11.cn

[Q21] 空值判断
来源：http://ssp.mhx1999.top

SELECT * FROM users WHERE email IS NULL;
来源：http://yvd.havefunace.top

[Q22] 排序
来源：http://aoi.316326.xyz

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ovv.jinqigufen.top

[Q23] 分页
来源：http://fmz.svipenyu.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://eiv.xinyue.icu

[Q24] 去重
来源：http://imj.jqgfzy.top

SELECT DISTINCT city FROM users;
来源：http://pmn.guowangkeji.top

[Q25] 只取前 N 条
来源：http://rlj.mhx1999.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wqs.zhaomingkeji.xyz

[Q26] 计数
来源：http://jfn.yuanzhike.top

SELECT COUNT(*) FROM users;
来源：http://ljx.xuanzx.com

[Q27] 条件计数
来源：http://xor.meibo888.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://kth.tarul.cn

[Q28] 求和与平均
来源：http://jjz.ybcxt.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mmn.zhixingplan.top

[Q29] 最大最小值
来源：http://qwd.shzxlz.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://rsp.gogol.net.cn

[Q30] 分组统计
来源：http://ylm.xinyue.icu

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://omx.daria6918.cn

[Q31] 分组后过滤
来源：http://mfe.iojbl.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wql.bbcook.cn

[Q32] 分组拼接字符串
来源：http://zpf.chenjidiqi.icu

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://opc.bjfxy.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mwn.shanyushiyangtech.top

[Q33] 多列分组
来源：http://qvl.yj202588.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://znb.fengsongda.top

[Q34] 每组取第一条
来源：http://cus.nanxuanxn.top

SELECT * FROM (
来源：http://jli.shanyushiyangtech.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://zaj.xinyue.icu

) t WHERE rn = 1;
来源：http://lfy.cdnleiting.top

[Q35] 内连接
来源：http://emy.epnwcf.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://tuv.hfpthk.cn

[Q36] 左连接
来源：http://jqw.316326.xyz

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://swb.zhengqikj.top

[Q37] 右连接
来源：http://tee.haohaochexian.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://jbe.epnwcf.com

[Q38] 全外连接（PostgreSQL）
来源：http://xtc.gzhubu.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://gxy.iojbl.cn

[Q39] 自连接（查上下级）
来源：http://rla.zycfv.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://vmn.xuanzx.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://dqy.tian-w.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://zlg.jiagoushi.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://raj.epnwcf.com

[Q41] 多表连接
来源：http://drb.zdbjq.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ati.nanxuanxn.top

JOIN users u ON u.id = o.user_id
来源：http://sda.iojbl.cn

JOIN products p ON p.id = o.product_id;
来源：http://ooi.9152youxi.cn

[Q42] 连接条件附加过滤
来源：http://lcb.dianchejie.cn

SELECT u.name, o.amount FROM users u
来源：http://iet.xuanzx.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://xdo.havefunace.top

[Q43] 标量子查询
来源：http://egs.cdnleiting.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://qmx.meibo888.top

[Q44] IN 子查询
来源：http://fum.daxiang520.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://lpj.jyoumei.cn

[Q45] EXISTS 判断存在
来源：http://jad.ydzc1.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://skz.guowangkeji.top

[Q46] NOT EXISTS 判断不存在
来源：http://ipt.hcnkem.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://lgt.guowangkeji.top

[Q47] 与平均值比较
来源：http://vhz.cqqwz.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://anf.cucudq.cn

[Q48] CTE 公用表表达式
来源：http://gzm.feifeiyinyue.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://kte.sxryk.cn

SELECT * FROM t WHERE c > 5;
来源：http://vzy.epnwcf.com

[Q49] 更新单行
来源：http://ufv.jinqigfzy.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://pqt.cqqwz.cn

[Q50] 批量更新
来源：http://exg.sjlbkw.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mtt.bbcook.cn

[Q51] 用子查询更新
来源：http://une.hongshengwenyu.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ezx.redwolf501.top

[Q52] 删除指定行
来源：http://oih.xziqi.cn

DELETE FROM users WHERE id = 10;
来源：http://lnn.zhaomingkeji.xyz

[Q53] 按条件删除
来源：http://qnn.fktsv.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://azu.zdbjq.cn

[Q54] 清空表
来源：http://wdb.ywan-chungtsiang.top

TRUNCATE TABLE logs;
来源：http://tqb.tian-w.cn

[Q55] 排名（并列占位）
来源：http://jeq.yangfankeji.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://qkw.tarul.cn

[Q56] 密集排名（并列不占位）
来源：http://etp.jiagoushi.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://vsd.uphjek.com

[Q57] 行号
来源：http://blb.zhoulong.xyz

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://gay.ppjwa.cn

[Q58] 累计求和
来源：http://bdj.ppjwa.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://qvj.fanxiaobao.xyz

[Q59] 分组内累计
来源：http://znc.dianchejie.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://fzh.52xcode.cn

[Q60] 取上一行 / 下一行
来源：http://uaf.svipenyu.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://qzj.yangfankeji.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://cxq.ivvv.top

[Q61] 移动平均
来源：http://ppu.fzhhl.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://nnh.daxiang520.top

[Q62] 分组占比
来源：http://xut.aizwys.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ngu.kuanghao11.cn

[Q63] 开启事务
来源：http://bpz.ywan-chungtsiang.top

START TRANSACTION;                -- 或 BEGIN
来源：http://jlq.chenlongwang.top

[Q64] 提交事务
来源：http://ysx.hnqzz.top

COMMIT;
来源：http://bwn.jinqigufen.top

[Q65] 回滚事务
来源：http://ers.316326.xyz

ROLLBACK;
来源：http://sab.havefunace.top

[Q66] 行锁查询
来源：http://ojj.zhixingplan.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://sqv.pycfn.com

[Q67] 设置隔离级别
来源：http://rdk.dashuyun.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://dnz.tarul.cn

[Q68] 保存点
来源：http://vsu.fehbvm.com

SAVEPOINT sp1;
来源：http://udp.zhijiandao.cn

ROLLBACK TO sp1;
来源：http://utw.gogol.net.cn

[Q69] 查看执行计划
来源：http://eik.kuanghao11.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://pxw.bjfxy.top

[Q70] 更新统计信息
来源：http://kms.cucudq.cn

ANALYZE TABLE users;
来源：http://prx.daxiang520.top

[Q71] 查看建表语句
来源：http://sbo.nanxuanxn.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://yxg.yangfankeji.com

[Q72] 查看索引
来源：http://rvp.c1oappe.top

SHOW INDEX FROM users;
来源：http://kup.hongshengwenyu.top

[Q73] 查看表状态
来源：http://dnl.xuetiantiany.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://dro.shanyushiyangtech.top

[Q74] 强制使用索引
来源：http://pjy.zhongyouzk.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://age.cucudq.cn

[Q75] 日期格式化
来源：http://mcn.sjlbkw.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://xrv.sysykeji.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://kyn.mhx1999.top

[Q76] 按天统计
来源：http://rcy.yj20258888.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ywl.xziqi.cn

[Q77] 时间加减
来源：http://gay.hywenlv.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ywm.gogol.net.cn

[Q78] 当前时间
来源：http://mln.cucudq.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://evp.yj20258888.top

[Q79] 字符串拼接
来源：http://kus.yj20258888.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://bnw.jiagoushi.top

[Q80] 字符串截取
来源：http://eue.quarkkingdee.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://vlu.ctjpmb.com

[Q81] 字符串替换
来源：http://iww.epnwcf.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://sgd.zhaomingkeji.xyz

[Q82] 字符长度与字节长度
来源：http://oci.dianchejie.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://qex.zhiwuduotai.top

[Q83] 大小写转换
来源：http://fnl.gotoacloud.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://rsj.zycfv.cn

[Q84] 去除首尾空格
来源：http://knc.ydzc1.top

SELECT TRIM(name) FROM users;
来源：http://llc.fengsongda.top

[Q85] 数值取整
来源：http://xme.sweek.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://tgf.hesvh.cn

[Q86] 读取 JSON 字段
来源：http://hkx.cucudq.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mdl.aibaodan.cn

[Q87] JSON 字段做条件
来源：http://roy.ctjpmb.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://htb.andypj.xyz

[Q88] 行转列（条件聚合）
来源：http://bon.ivvv.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hsm.xziqi.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://lmr.jqgfzy.top

[Q89] 判断表是否存在
来源：http://rwn.zhengqikj.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://eou.sweek.top

[Q90] 生成序号列
来源：http://vpy.vqdsnc.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://jju.xingfuxueyuan.xyz

================================================================================
来源：http://llw.zhengqikj.top

R. Bash 专题
来源：http://ytt.jyoumei.cn

================================================================================
来源：http://wgo.hnqzz.top

[R01] shebang 与严格模式
来源：http://kur.cdnleiting.top

#!/usr/bin/env bash
来源：http://azn.aibaodan.cn

set -euo pipefail
来源：http://lfp.fehbvm.com

[R02] 变量赋值与使用
来源：http://bea.zhoulong.xyz

name="Tom"; echo "$name"
来源：http://zmc.mhx1999.top

[R03] 只读变量
来源：http://sbw.cqqwz.cn

readonly PI=3.14
来源：http://ztz.jianghu66.top

[R04] 位置参数
来源：http://gpz.nwbrower.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://khv.nanxuanxn.top

[R05] 参数默认值
来源：http://dcl.redwolf501.top

name="${1:-default}"
来源：http://yzt.yj20258888.top

[R06] 判断命令是否存在
来源：http://hnx.yj20258888.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://cvo.sysykeji.top

[R07] if 判断文件
来源：http://nzd.zhixingplan.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://qsn.xziqi.cn

[R08] 数值比较
来源：http://hmq.ehwqpu.com

if (( a > b )); then echo "a 更大"; fi
来源：http://lzg.wangshuangyany.cn

[R09] 字符串比较
来源：http://iqa.yj202588.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://uhv.hfpthk.cn

[R10] 正则匹配
来源：http://qau.svipenyu.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hwv.nwbrower.top

[R11] case 多分支
来源：http://bii.wangdashe.top

case "$1" in
来源：http://oex.wangshuangyany.cn

start) echo "启动" ;;
来源：http://dpk.xingfuxueyuan.xyz

stop)  echo "停止" ;;
来源：http://duu.fengsongda.top

*)     echo "未知命令" ;;
来源：http://nly.vqdsnc.cn

esac
来源：http://uts.zdqjudy.top

[R12] for 遍历文件
来源：http://amc.birdmap.top

for f in *.txt; do echo "$f"; done
来源：http://bqj.tianlin.xyz

[R13] for 计数循环
来源：http://nkg.0kj1m.cn

for i in {1..10}; do echo "$i"; done
来源：http://oix.ybcxt.top

[R14] C 风格 for
来源：http://uzt.andypj.xyz

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://pga.yj20258888.top

[R15] while 逐行读文件
来源：http://ahk.wangdashe.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://vdj.shzxlz.cn

[R16] until 等待条件
来源：http://pne.vqdsnc.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://zsf.smart0.xyz

[R17] 数组定义与取值
来源：http://ibr.sweek.top

arr=(a b c); echo "${arr[0]}"
来源：http://ekj.iojbl.cn

[R18] 遍历数组
来源：http://jjs.chenzaomai.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://nop.jiagoushi.top

[R19] 数组长度
来源：http://yzb.daxiang520.top

echo "${#arr[@]}"
来源：http://gxs.aizwys.cn

[R20] 关联数组（字典）
来源：http://wmm.c1oappe.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://edq.epnwcf.com

[R21] 字符串长度
来源：http://nhf.tianlin.xyz

echo "${#s}"
来源：http://wvu.tarul.cn

[R22] 截取子串
来源：http://bvk.chenlongwang.top

echo "${s:0:5}"
来源：http://qnr.sxryk.cn

[R23] 字符串替换
来源：http://wid.ywan-chungtsiang.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://poo.shzxlz.cn

[R24] 大小写转换
来源：http://uih.aizwys.cn

echo "${s^^}"; echo "${s,,}"
来源：http://rmx.gotoacloud.top

[R25] 去后缀 / 去前缀
来源：http://egj.xingfuxueyuan.xyz

echo "${f%.txt}"; echo "${f#./}"
来源：http://xct.jiagoushi.top

[R26] 命令替换
来源：http://hhd.epnwcf.com

now=$(date +%F); echo "$now"
来源：http://irv.ivvv.top

[R27] 算术展开
来源：http://pab.nwbrower.top

echo $((1 + 2 * 3))
来源：http://fjs.jinqigfzy.top

[R28] 浮点运算
来源：http://wcs.yj202588.top

echo "scale=2; 10/3" | bc
来源：http://gyc.xziqi.cn

[R29] 定义函数
来源：http://hvh.hesvh.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://kev.zhiwuduotai.top

[R30] 函数返回状态码
来源：http://qfq.fehbvm.com

f() { return 0; }; f || echo "失败了"
来源：http://agf.haohaochexian.top

[R31] 局部变量
来源：http://dxf.jqgufenzy.top

f() { local x=1; echo "$x"; }
来源：http://ocz.snrcjt.cn

[R32] 参数个数校验
来源：http://qxl.yuanzhike.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://zgv.52xcode.cn

[R33] 捕获错误并提示行号
来源：http://rok.yj20258.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://rai.dashuyun.cn

[R34] 退出时清理
来源：http://zal.316326.xyz

trap 'rm -f "$tmp"' EXIT
来源：http://ppf.hcnkem.com

[R35] 后台执行并等待
来源：http://ukk.shanyushiyangkeji.top

sleep 5 & pid=$!; wait "$pid"
来源：http://bcr.yongpay.top

[R36] 并发执行多个任务
来源：http://zvh.jinqigufen.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ojq.fzhhl.top

[R37] 把输出赋给变量
来源：http://bbb.bbcook.cn


<!-- 参考信息 -->