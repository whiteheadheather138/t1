代发 wailian999

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://jry.daria6918.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://nhs.andypj.xyz

C#:   // 用 System.Timers.Timer 重置实现
来源：http://fvp.kuanghao11.cn

[P08] 处理浮点精度问题
来源：http://yvk.hysaishi.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://isa.shuidangran.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://gcn.ybcxt.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://gyq.hesvh.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://psu.ywan-chungtsiang.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ght.chenlongwang.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://oqv.zdqjudy.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://iin.zhoulong.xyz

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ety.hysaishi.cn

================================================================================
来源：http://lhi.ybcxt.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ibd.hnqzz.top

================================================================================
来源：http://eou.316326.xyz

[Q01] 创建表
来源：http://bdw.tian-w.cn

CREATE TABLE users (
来源：http://gld.kuanghao11.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://vek.gaohongyu789.top

name VARCHAR(50) NOT NULL,
来源：http://fma.daxiang520.top

email VARCHAR(100) UNIQUE,
来源：http://fhr.nanxinkj.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ybm.ctjpmb.com

);
来源：http://wwc.epnwcf.com

[Q02] 创建带外键的表
来源：http://xhp.jqgfzy.top

CREATE TABLE orders (
来源：http://hrm.hongshengwenyu.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://xlb.yvedp.cn

user_id INT NOT NULL,
来源：http://sie.havefunace.top

amount DECIMAL(10, 2),
来源：http://koa.yuxming.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://yxu.hesvh.cn

);
来源：http://mro.fanxiaobao.xyz

[Q03] 增加列
来源：http://msu.ybcxt.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ftl.zhixingplan.top

[Q04] 修改列类型
来源：http://ijc.tianlin.xyz

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://rdc.cucudq.cn

[Q05] 重命名列
来源：http://muf.havefunace.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hyc.vqdsnc.cn

[Q06] 删除列
来源：http://gdi.yueranfly.top

ALTER TABLE users DROP COLUMN age;
来源：http://qzg.yuanzhike.top

[Q07] 删除表
来源：http://mdy.jiagoushi.top

DROP TABLE IF EXISTS orders;
来源：http://qtf.sxryk.cn

[Q08] 创建普通索引
来源：http://gxh.wangdashe.top

CREATE INDEX idx_users_email ON users(email);
来源：http://pjy.zhijiandao.cn

[Q09] 创建唯一索引
来源：http://cqq.shzxlz.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://lyt.gzhubu.top

[Q10] 插入单行
来源：http://jjw.cucudq.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://pdi.epnwcf.com

[Q11] 一次插入多行
来源：http://zbc.hammf.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://fjc.sysykeji.top

[Q12] 插入后取自增 ID
来源：http://yju.shanyushiyangtech.top

INSERT INTO users (name) VALUES ('C');
来源：http://jpl.guannengcc.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://yan.feifeiyinyue.top

[Q13] 忽略重复插入
来源：http://sdk.bjfxy.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://nyb.yj202588.top

[Q14] 存在则更新（upsert）
来源：http://pxh.snrcjt.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://dyo.ydjk.org.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://rbs.ehwqpu.com

[Q15] 查询全部
来源：http://nbn.zdqjudy.top

SELECT * FROM users;
来源：http://dxg.snrcjt.cn

[Q16] 查询指定列
来源：http://wyg.xuetiantiany.cn

SELECT id, name FROM users;
来源：http://fzj.hammf.cn

[Q17] 条件查询
来源：http://zxr.jqgfzy.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ngl.zhijiandao.cn

[Q18] 模糊匹配
来源：http://jpj.guannengcc.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://amz.jyoumei.cn

[Q19] 范围查询
来源：http://vif.chenjidiqi.icu

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://rje.hesvh.cn

[Q20] IN 列表
来源：http://wqf.fengsongda.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://zes.zhongyouzk.top

[Q21] 空值判断
来源：http://pzt.tanke756.top

SELECT * FROM users WHERE email IS NULL;
来源：http://puq.zdbjq.cn

[Q22] 排序
来源：http://fsk.ehwqpu.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://kgs.gotoacloud.top

[Q23] 分页
来源：http://dfj.bjfxy.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wiu.fengsongda.top

[Q24] 去重
来源：http://aop.daxiang520.top

SELECT DISTINCT city FROM users;
来源：http://zyh.xingfuxueyuan.xyz

[Q25] 只取前 N 条
来源：http://vfc.ivvv.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://jmy.yj202588.top

[Q26] 计数
来源：http://hmu.zycfv.cn

SELECT COUNT(*) FROM users;
来源：http://jzw.yangfankeji.com

[Q27] 条件计数
来源：http://ecr.yvedp.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ldk.nanxinkj.top

[Q28] 求和与平均
来源：http://tgt.316326.xyz

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ifm.ydzc1.top

[Q29] 最大最小值
来源：http://add.fzhhl.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://xjy.tarul.cn

[Q30] 分组统计
来源：http://uqf.hysaishi.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://smg.yj20258888.top

[Q31] 分组后过滤
来源：http://vmb.xinyue.icu

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://bei.yj20258.top

[Q32] 分组拼接字符串
来源：http://knx.gogol.net.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mez.sysykeji.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ibt.zhoulong.xyz

[Q33] 多列分组
来源：http://kcg.jinqigfzy.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://jdy.zhijiandao.cn

[Q34] 每组取第一条
来源：http://cuo.ppjwa.cn

SELECT * FROM (
来源：http://mle.mhx1999.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://lec.ydzc1.top

) t WHERE rn = 1;
来源：http://igr.fktsv.cn

[Q35] 内连接
来源：http://rzr.wangdashe.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://itn.shanyushiyangkeji.top

[Q36] 左连接
来源：http://vab.dianchejie.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://cjt.jiagoushi.top

[Q37] 右连接
来源：http://eti.hesvh.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mcz.xinyue.icu

[Q38] 全外连接（PostgreSQL）
来源：http://zyj.zdbjq.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://nby.316326.xyz

[Q39] 自连接（查上下级）
来源：http://knl.9152youxi.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ctg.yangfankeji.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://udv.jinyuanbaomall.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://rjb.uphjek.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://tee.uphjek.com

[Q41] 多表连接
来源：http://lrf.cqqwz.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://zui.cdnleiting.top

JOIN users u ON u.id = o.user_id
来源：http://yla.bjfxy.top

JOIN products p ON p.id = o.product_id;
来源：http://cup.ivvv.top

[Q42] 连接条件附加过滤
来源：http://est.feifeiyinyue.top

SELECT u.name, o.amount FROM users u
来源：http://ink.nanxuanxn.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://gkm.jqgfzy.top

[Q43] 标量子查询
来源：http://fwi.gogol.net.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://kjx.yangfankeji.com

[Q44] IN 子查询
来源：http://rxr.hnxiangtu.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://fsi.yangfankeji.com

[Q45] EXISTS 判断存在
来源：http://nrc.shuidangran.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kpm.fanxiaobao.xyz

[Q46] NOT EXISTS 判断不存在
来源：http://sif.jinqigufen.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fjj.hnxiangtu.top

[Q47] 与平均值比较
来源：http://hor.aizwys.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://qjt.hesvh.cn

[Q48] CTE 公用表表达式
来源：http://rin.shzxlz.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://vjd.gzhubu.top

SELECT * FROM t WHERE c > 5;
来源：http://ust.dianchejie.cn

[Q49] 更新单行
来源：http://oqd.ydzc1.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://nwx.shanyushiyangtech.top

[Q50] 批量更新
来源：http://gvv.shangyingyoupin.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://emk.nwbrower.top

[Q51] 用子查询更新
来源：http://egs.shzxlz.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://tid.sweek.top

[Q52] 删除指定行
来源：http://dyq.jianghu66.top

DELETE FROM users WHERE id = 10;
来源：http://cvt.uphjek.com

[Q53] 按条件删除
来源：http://ukb.9152youxi.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://nve.sufxvd.cn

[Q54] 清空表
来源：http://ceo.gogol.net.cn

TRUNCATE TABLE logs;
来源：http://pmb.hongshengwenyu.top

[Q55] 排名（并列占位）
来源：http://dgh.xinyue.icu

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ici.shuidangran.top

[Q56] 密集排名（并列不占位）
来源：http://ayw.xylfe.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://goh.yj20258.top

[Q57] 行号
来源：http://fvi.vehdjk.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://vfb.zdqjudy.top

[Q58] 累计求和
来源：http://qqg.yonumen.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mdy.hysaishi.cn

[Q59] 分组内累计
来源：http://ebi.gzhubu.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://anv.hesvh.cn

[Q60] 取上一行 / 下一行
来源：http://ihk.9152youxi.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://rqg.ywan-chungtsiang.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://xsk.sufxvd.cn

[Q61] 移动平均
来源：http://nhk.hnxiangtu.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://can.guowangkeji.top

[Q62] 分组占比
来源：http://yzg.jyoumei.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://xek.ppjwa.cn

[Q63] 开启事务
来源：http://mfb.jyoumei.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://buy.guowangkeji.top

[Q64] 提交事务
来源：http://oxn.andypj.xyz

COMMIT;
来源：http://hxc.cucudq.cn

[Q65] 回滚事务
来源：http://mea.yj20258888.top

ROLLBACK;
来源：http://nql.aibaodan.cn

[Q66] 行锁查询
来源：http://ado.guannengcc.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mbm.ydzc1.top

[Q67] 设置隔离级别
来源：http://sel.jqgfzy.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://twf.redwolf501.top

[Q68] 保存点
来源：http://mgy.iojbl.cn

SAVEPOINT sp1;
来源：http://yho.jiagoushi.top

ROLLBACK TO sp1;
来源：http://smh.yuanzhike.top

[Q69] 查看执行计划
来源：http://vue.jinqigufen.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://dnp.yj20258.top

[Q70] 更新统计信息
来源：http://dxs.dianchejie.cn

ANALYZE TABLE users;
来源：http://ywf.ppjwa.cn

[Q71] 查看建表语句
来源：http://rwy.hysaishi.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://xst.sxryk.cn

[Q72] 查看索引
来源：http://vta.wangshuangyany.cn

SHOW INDEX FROM users;
来源：http://ypy.iojbl.cn

[Q73] 查看表状态
来源：http://bxb.cdnleiting.top

SHOW TABLE STATUS LIKE 'users';
来源：http://snp.zhijiandao.cn

[Q74] 强制使用索引
来源：http://cqv.daxiang520.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ete.jqgufenzy.top

[Q75] 日期格式化
来源：http://yld.yonumen.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://paz.bbcook.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://trs.daxiang520.top

[Q76] 按天统计
来源：http://wfw.ehwqpu.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://qoq.ivvv.top

[Q77] 时间加减
来源：http://svs.fanxiaobao.xyz

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://xzl.chenjidiqi.icu

[Q78] 当前时间
来源：http://cya.yfazqb.com

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://kxu.yj20258888.top

[Q79] 字符串拼接
来源：http://yzb.yonumen.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://btt.ctjpmb.com

[Q80] 字符串截取
来源：http://ihh.meibo888.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://zdx.zycfv.cn

[Q81] 字符串替换
来源：http://yik.shanyushiyangkeji.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://sqf.zhaomingkeji.xyz

[Q82] 字符长度与字节长度
来源：http://fqt.yj20258.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://tto.fehbvm.com

[Q83] 大小写转换
来源：http://pii.meibo888.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://rng.cqqwz.cn

[Q84] 去除首尾空格
来源：http://xnq.gzhubu.top

SELECT TRIM(name) FROM users;
来源：http://ldy.cqqwz.cn

[Q85] 数值取整
来源：http://ijj.cheryme.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://fna.hnqzz.top

[Q86] 读取 JSON 字段
来源：http://kwl.yvedp.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://nod.guannengcc.top

[Q87] JSON 字段做条件
来源：http://fnt.shzxlz.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://gux.yfazqb.com

[Q88] 行转列（条件聚合）
来源：http://qug.redwolf501.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://nei.yueranfly.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wgh.cqqwz.cn

[Q89] 判断表是否存在
来源：http://plj.vqdsnc.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://zwz.gaohongyu789.top

[Q90] 生成序号列
来源：http://rnl.hcnkem.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wib.zdbjq.cn

================================================================================
来源：http://gow.yangfankeji.com

R. Bash 专题
来源：http://vqr.ctjpmb.com

================================================================================
来源：http://bna.quarkkingdee.top

[R01] shebang 与严格模式
来源：http://bor.meibo888.top

#!/usr/bin/env bash
来源：http://fff.yuanzhike.top

set -euo pipefail
来源：http://gcn.wangshuangyany.cn

[R02] 变量赋值与使用
来源：http://feb.chenlongwang.top

name="Tom"; echo "$name"
来源：http://zcy.hcnkem.com

[R03] 只读变量
来源：http://vlj.jinyuanbaomall.cn

readonly PI=3.14
来源：http://kzf.zhongyouzk.top

[R04] 位置参数
来源：http://nyj.0kj1m.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://pha.xziqi.cn

[R05] 参数默认值
来源：http://dqy.yvedp.cn

name="${1:-default}"
来源：http://nxh.yanxiufei.cn

[R06] 判断命令是否存在
来源：http://cpn.wangdashe.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://aid.guannengcc.top

[R07] if 判断文件
来源：http://vdh.cqqwz.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://zts.mhx1999.top

[R08] 数值比较
来源：http://peb.hysaishi.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://cfz.gotoacloud.top

[R09] 字符串比较
来源：http://fhm.jqgufenzy.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://dac.jinqigufen.top

[R10] 正则匹配
来源：http://qar.jinyuanbaomall.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hdp.yvedp.cn

[R11] case 多分支
来源：http://xcy.shanyushiyangkeji.top

case "$1" in
来源：http://qet.xinyue.icu

start) echo "启动" ;;
来源：http://dec.jlsjyb.cn

stop)  echo "停止" ;;
来源：http://njr.hcnkem.com

*)     echo "未知命令" ;;
来源：http://xhp.yj202588.top

esac
来源：http://zai.jlsjyb.cn

[R12] for 遍历文件
来源：http://jvt.shangyingyoupin.top

for f in *.txt; do echo "$f"; done
来源：http://eyo.shangyingyoupin.top

[R13] for 计数循环
来源：http://bdk.316326.xyz

for i in {1..10}; do echo "$i"; done
来源：http://ozi.nanxinkj.top

[R14] C 风格 for
来源：http://xjm.shanyushiyangkeji.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mdf.aizwys.cn

[R15] while 逐行读文件
来源：http://jby.tianlin.xyz

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://xwu.yanxiufei.cn

[R16] until 等待条件
来源：http://fzd.zdbjq.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ssz.tanke756.top

[R17] 数组定义与取值
来源：http://wah.shanyushiyangkeji.top

arr=(a b c); echo "${arr[0]}"
来源：http://lnf.chenjidiqi.icu

[R18] 遍历数组
来源：http://htg.wangshuangyany.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ypc.c1oappe.top

[R19] 数组长度
来源：http://wun.yueranfly.top

echo "${#arr[@]}"
来源：http://amq.fzhhl.top

[R20] 关联数组（字典）
来源：http://sqg.xylfe.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://tqk.kuanghao11.cn

[R21] 字符串长度
来源：http://aol.sysykeji.top

echo "${#s}"
来源：http://kfm.sysykeji.top

[R22] 截取子串
来源：http://aiv.hnxiangtu.top

echo "${s:0:5}"
来源：http://mxg.bjfxy.top

[R23] 字符串替换
来源：http://mqw.zhongyouzk.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://gbf.fengsongda.top

[R24] 大小写转换
来源：http://gls.cqqwz.cn

echo "${s^^}"; echo "${s,,}"
来源：http://hty.zhongyouzk.top

[R25] 去后缀 / 去前缀
来源：http://rdg.hywenlv.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://krd.316326.xyz

[R26] 命令替换
来源：http://yts.birdmap.top

now=$(date +%F); echo "$now"
来源：http://eum.mhx1999.top

[R27] 算术展开
来源：http://xka.zhongyouzk.top

echo $((1 + 2 * 3))
来源：http://ymh.ydzc1.top

[R28] 浮点运算
来源：http://twh.zhixingplan.top

echo "scale=2; 10/3" | bc
来源：http://vve.epnwcf.com

[R29] 定义函数
来源：http://hwe.fehbvm.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://jso.aibaodan.cn

[R30] 函数返回状态码
来源：http://vxr.hesvh.cn

f() { return 0; }; f || echo "失败了"
来源：http://egc.guannengcc.top

[R31] 局部变量
来源：http://gzs.tarul.cn

f() { local x=1; echo "$x"; }
来源：http://qzb.zycfv.cn

[R32] 参数个数校验
来源：http://mii.ctjpmb.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hmq.hongshengwenyu.top

[R33] 捕获错误并提示行号
来源：http://rez.gaohongyu789.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://uqu.yj202588.top

[R34] 退出时清理
来源：http://aoc.jinqigufen.top

trap 'rm -f "$tmp"' EXIT
来源：http://mne.yvedp.cn

[R35] 后台执行并等待
来源：http://kdc.yangfankeji.com

sleep 5 & pid=$!; wait "$pid"
来源：http://hgf.shuidangran.top

[R36] 并发执行多个任务
来源：http://vkc.316326.xyz

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://pxw.cheryme.top

[R37] 把输出赋给变量
来源：http://kxw.fktsv.cn


<!-- 参考信息 -->