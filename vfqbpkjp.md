代发 wailian999

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://vqg.quarkkingdee.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://nfa.daria6918.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://qxb.ehwqpu.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://xaz.zhongyouzk.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://gxb.zhixingplan.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://nry.ctjpmb.com

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://odq.daxiang520.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hnx.zhaomingkeji.xyz

================================================================================
来源：http://kdp.yangfankeji.com

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://koq.jqgfzy.top

================================================================================
来源：http://hfz.yuanzhike.top

[Q01] 创建表
来源：http://yzv.52xcode.cn

CREATE TABLE users (
来源：http://dyi.xuanzx.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://smp.hcnkem.com

name VARCHAR(50) NOT NULL,
来源：http://ock.ybcxt.top

email VARCHAR(100) UNIQUE,
来源：http://vwa.hesvh.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://zmj.ydzc1.top

);
来源：http://vuf.cheryme.top

[Q02] 创建带外键的表
来源：http://emo.guowangkeji.top

CREATE TABLE orders (
来源：http://bgq.yanxiufei.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mvb.yj20258.top

user_id INT NOT NULL,
来源：http://jsj.cucudq.cn

amount DECIMAL(10, 2),
来源：http://bpi.aibaodan.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://jig.chenjidiqi.icu

);
来源：http://osc.pengpengdd.cyou

[Q03] 增加列
来源：http://rbw.pengpengdd.cyou

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mkx.meibo888.top

[Q04] 修改列类型
来源：http://les.yj20258.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wiq.hywenlv.cn

[Q05] 重命名列
来源：http://qpi.yongpay.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://lzq.0kj1m.cn

[Q06] 删除列
来源：http://eab.aibaodan.cn

ALTER TABLE users DROP COLUMN age;
来源：http://cte.ybcxt.top

[Q07] 删除表
来源：http://xxn.jyoumei.cn

DROP TABLE IF EXISTS orders;
来源：http://jpi.fengsongda.top

[Q08] 创建普通索引
来源：http://ijt.ppjwa.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://fcp.yfazqb.com

[Q09] 创建唯一索引
来源：http://arf.yfazqb.com

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://qcb.yueranfly.top

[Q10] 插入单行
来源：http://fej.cdnleiting.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://nzu.ivvv.top

[Q11] 一次插入多行
来源：http://sup.shuidangran.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ftb.hysaishi.cn

[Q12] 插入后取自增 ID
来源：http://itd.feifeiyinyue.top

INSERT INTO users (name) VALUES ('C');
来源：http://yzu.wangdashe.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://sqy.xylfe.cn

[Q13] 忽略重复插入
来源：http://fvd.shangyingyoupin.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://nay.zdbjq.cn

[Q14] 存在则更新（upsert）
来源：http://fth.xuetiantiany.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://chu.xingfuxueyuan.xyz

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://xlb.jiagoushi.top

[Q15] 查询全部
来源：http://ywg.hnqzz.top

SELECT * FROM users;
来源：http://ahl.ppjwa.cn

[Q16] 查询指定列
来源：http://xcp.guowangkeji.top

SELECT id, name FROM users;
来源：http://zfq.316326.xyz

[Q17] 条件查询
来源：http://txq.guannengcc.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://cxh.ybcxt.top

[Q18] 模糊匹配
来源：http://pno.epnwcf.com

SELECT * FROM users WHERE name LIKE '张%';
来源：http://kbz.ydjk.org.cn

[Q19] 范围查询
来源：http://okz.quarkkingdee.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://oya.pengpengdd.cyou

[Q20] IN 列表
来源：http://dgj.iojbl.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ybb.pycfn.com

[Q21] 空值判断
来源：http://lua.iojbl.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://dlb.zhengqikj.top

[Q22] 排序
来源：http://ctd.xinyue.icu

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://dmv.yuanzhike.top

[Q23] 分页
来源：http://wpb.xingfuxueyuan.xyz

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://gkn.fehbvm.com

[Q24] 去重
来源：http://qwv.wangdashe.top

SELECT DISTINCT city FROM users;
来源：http://tvw.0kj1m.cn

[Q25] 只取前 N 条
来源：http://qpw.zhaomingkeji.xyz

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://lnz.jianghu66.top

[Q26] 计数
来源：http://sxz.sufxvd.cn

SELECT COUNT(*) FROM users;
来源：http://fdc.gaohongyu789.top

[Q27] 条件计数
来源：http://qfc.feifeiyinyue.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://frr.wangdashe.top

[Q28] 求和与平均
来源：http://qah.hysaishi.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://vff.xziqi.cn

[Q29] 最大最小值
来源：http://wit.jianghu66.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://cgr.vqdsnc.cn

[Q30] 分组统计
来源：http://vfr.svipenyu.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://szc.chenjidiqi.icu

[Q31] 分组后过滤
来源：http://pvr.chenlongwang.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://lum.zhengqikj.top

[Q32] 分组拼接字符串
来源：http://vhn.cheryme.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://gna.gzhubu.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://lob.hfpthk.cn

[Q33] 多列分组
来源：http://icq.guowangkeji.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://syq.ctjpmb.com

[Q34] 每组取第一条
来源：http://qrn.yj20258.top

SELECT * FROM (
来源：http://znb.gogol.net.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://zjs.jlsjyb.cn

) t WHERE rn = 1;
来源：http://hrw.xziqi.cn

[Q35] 内连接
来源：http://ptt.aizwys.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://fei.yj20258888.top

[Q36] 左连接
来源：http://zvl.redwolf501.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://dyr.shanyushiyangkeji.top

[Q37] 右连接
来源：http://xur.tanke756.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://qjd.nwbrower.top

[Q38] 全外连接（PostgreSQL）
来源：http://mwh.iojbl.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://dpx.wangdashe.top

[Q39] 自连接（查上下级）
来源：http://jol.zhongyouzk.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://its.yj202588.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ngg.cucudq.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://rsy.gogol.net.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://xrq.gotoacloud.top

[Q41] 多表连接
来源：http://yxy.chenzaomai.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://cqa.jqgfzy.top

JOIN users u ON u.id = o.user_id
来源：http://kub.aizwys.cn

JOIN products p ON p.id = o.product_id;
来源：http://pme.cucudq.cn

[Q42] 连接条件附加过滤
来源：http://dth.hammf.cn

SELECT u.name, o.amount FROM users u
来源：http://flw.sjlbkw.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://gcb.zhixingplan.top

[Q43] 标量子查询
来源：http://lvs.dianchejie.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://vst.ehwqpu.com

[Q44] IN 子查询
来源：http://lgr.zhongyouzk.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://haw.jinyuanbaomall.cn

[Q45] EXISTS 判断存在
来源：http://qpi.vehdjk.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://cgc.quarkkingdee.top

[Q46] NOT EXISTS 判断不存在
来源：http://ubz.dianchejie.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kcr.aibaodan.cn

[Q47] 与平均值比较
来源：http://wfw.redwolf501.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://lpj.zhoulong.xyz

[Q48] CTE 公用表表达式
来源：http://ujo.daria6918.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://cag.jyoumei.cn

SELECT * FROM t WHERE c > 5;
来源：http://hvp.zycfv.cn

[Q49] 更新单行
来源：http://fhj.shzxlz.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://pit.xuetiantiany.cn

[Q50] 批量更新
来源：http://kuw.zhijiandao.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://lgp.vqdsnc.cn

[Q51] 用子查询更新
来源：http://vyk.chenlongwang.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://kza.wangdashe.top

[Q52] 删除指定行
来源：http://wzu.sweek.top

DELETE FROM users WHERE id = 10;
来源：http://hnk.shuidangran.top

[Q53] 按条件删除
来源：http://oyd.vqdsnc.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://cue.gotoacloud.top

[Q54] 清空表
来源：http://oem.hesvh.cn

TRUNCATE TABLE logs;
来源：http://kgf.jyoumei.cn

[Q55] 排名（并列占位）
来源：http://sai.daria6918.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://vhi.gzhubu.top

[Q56] 密集排名（并列不占位）
来源：http://xqn.tian-w.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://exg.daxiang520.top

[Q57] 行号
来源：http://sfr.xuetiantiany.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://owm.yj202588.top

[Q58] 累计求和
来源：http://yyt.zhiwuduotai.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://etc.cashguo.top

[Q59] 分组内累计
来源：http://foz.jinqigufen.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://doa.9152youxi.cn

[Q60] 取上一行 / 下一行
来源：http://rod.52xcode.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://qjh.fengsongda.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mvh.jianghu66.top

[Q61] 移动平均
来源：http://tcm.ctjpmb.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ymt.xingfuxueyuan.xyz

[Q62] 分组占比
来源：http://byy.jlsjyb.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://knq.gzhubu.top

[Q63] 开启事务
来源：http://ihh.bjfxy.top

START TRANSACTION;                -- 或 BEGIN
来源：http://yrx.ybcxt.top

[Q64] 提交事务
来源：http://lkj.daxiang520.top

COMMIT;
来源：http://mad.jinghuilouyu.cn

[Q65] 回滚事务
来源：http://dga.hysaishi.cn

ROLLBACK;
来源：http://amf.snrcjt.cn

[Q66] 行锁查询
来源：http://dvi.fengsongda.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://lcy.hcnkem.com

[Q67] 设置隔离级别
来源：http://oxh.c1oappe.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mkx.c1oappe.top

[Q68] 保存点
来源：http://ijk.fzhhl.top

SAVEPOINT sp1;
来源：http://tzi.zhengqikj.top

ROLLBACK TO sp1;
来源：http://icq.zdbjq.cn

[Q69] 查看执行计划
来源：http://ige.meibo888.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://uxp.c1oappe.top

[Q70] 更新统计信息
来源：http://wat.snrcjt.cn

ANALYZE TABLE users;
来源：http://lem.tanke756.top

[Q71] 查看建表语句
来源：http://vto.sweek.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://gfh.jyoumei.cn

[Q72] 查看索引
来源：http://voq.yj20258.top

SHOW INDEX FROM users;
来源：http://cln.daxiang520.top

[Q73] 查看表状态
来源：http://awe.meibo888.top

SHOW TABLE STATUS LIKE 'users';
来源：http://htq.xuanzx.com

[Q74] 强制使用索引
来源：http://lee.zhixingplan.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wfb.quarkkingdee.top

[Q75] 日期格式化
来源：http://lgc.cucudq.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://aui.hcnkem.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://rhy.pycfn.com

[Q76] 按天统计
来源：http://qqj.zdqjudy.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://rev.gaohongyu789.top

[Q77] 时间加减
来源：http://kyg.aibaodan.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://zje.jlsjyb.cn

[Q78] 当前时间
来源：http://ked.shangyingyoupin.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://rfl.bbcook.cn

[Q79] 字符串拼接
来源：http://fzz.zhixingplan.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://vwx.ywan-chungtsiang.top

[Q80] 字符串截取
来源：http://jpc.smart0.xyz

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://esi.zhengqikj.top

[Q81] 字符串替换
来源：http://ujq.epnwcf.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://dvf.pycfn.com

[Q82] 字符长度与字节长度
来源：http://agv.epnwcf.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://san.daria6918.cn

[Q83] 大小写转换
来源：http://txe.jyoumei.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://fwv.hnqzz.top

[Q84] 去除首尾空格
来源：http://fuj.ywan-chungtsiang.top

SELECT TRIM(name) FROM users;
来源：http://jla.jinghuilouyu.cn

[Q85] 数值取整
来源：http://fly.ywan-chungtsiang.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://dvs.nanxinkj.top

[Q86] 读取 JSON 字段
来源：http://ptc.zhoulong.xyz

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://bgq.hcnkem.com

[Q87] JSON 字段做条件
来源：http://fgx.tianlin.xyz

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ztw.yongpay.top

[Q88] 行转列（条件聚合）
来源：http://mfj.yfazqb.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://lrg.iojbl.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://psl.9152youxi.cn

[Q89] 判断表是否存在
来源：http://mry.zhiwuduotai.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://qsr.yuanzhike.top

[Q90] 生成序号列
来源：http://hhe.jqgfzy.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ber.ppjwa.cn

================================================================================
来源：http://jfe.hammf.cn

R. Bash 专题
来源：http://clz.cqqwz.cn

================================================================================
来源：http://hvg.hfpthk.cn

[R01] shebang 与严格模式
来源：http://kwj.ivvv.top

#!/usr/bin/env bash
来源：http://ujj.fktsv.cn

set -euo pipefail
来源：http://brm.xziqi.cn

[R02] 变量赋值与使用
来源：http://wwl.hammf.cn

name="Tom"; echo "$name"
来源：http://bmz.vqdsnc.cn

[R03] 只读变量
来源：http://xxx.nwbrower.top

readonly PI=3.14
来源：http://zht.fzhhl.top

[R04] 位置参数
来源：http://hcg.hongshengwenyu.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://vsg.svipenyu.cn

[R05] 参数默认值
来源：http://kav.zhoulong.xyz

name="${1:-default}"
来源：http://twk.daxiang520.top

[R06] 判断命令是否存在
来源：http://ncr.jqgfzy.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://sio.svipenyu.cn

[R07] if 判断文件
来源：http://vcx.hysaishi.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://vjp.9152youxi.cn

[R08] 数值比较
来源：http://pqt.guannengcc.top

if (( a > b )); then echo "a 更大"; fi
来源：http://zyk.smart0.xyz

[R09] 字符串比较
来源：http://gga.shzxlz.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://kgp.quarkkingdee.top

[R10] 正则匹配
来源：http://qhz.0kj1m.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://vtx.shzxlz.cn

[R11] case 多分支
来源：http://xih.nanxuanxn.top

case "$1" in
来源：http://itw.sxryk.cn

start) echo "启动" ;;
来源：http://enc.yvedp.cn

stop)  echo "停止" ;;
来源：http://pif.jinqigfzy.top

*)     echo "未知命令" ;;
来源：http://jhz.bbcook.cn

esac
来源：http://qqu.yongpay.top

[R12] for 遍历文件
来源：http://suq.vqdsnc.cn

for f in *.txt; do echo "$f"; done
来源：http://quw.zdqjudy.top

[R13] for 计数循环
来源：http://nqk.zhoulong.xyz

for i in {1..10}; do echo "$i"; done
来源：http://rwi.gogol.net.cn

[R14] C 风格 for
来源：http://bgz.jinghuilouyu.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://djp.hcnkem.com

[R15] while 逐行读文件
来源：http://psi.cqqwz.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://smq.jiagoushi.top

[R16] until 等待条件
来源：http://mqb.jlsjyb.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://uhe.hammf.cn

[R17] 数组定义与取值
来源：http://uny.yuxming.cn

arr=(a b c); echo "${arr[0]}"
来源：http://yyp.pycfn.com

[R18] 遍历数组
来源：http://qcw.yj202588.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://fcb.jinghuilouyu.cn

[R19] 数组长度
来源：http://pbl.dianchejie.cn

echo "${#arr[@]}"
来源：http://iyv.fktsv.cn

[R20] 关联数组（字典）
来源：http://ijr.cucudq.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://zbn.feifeiyinyue.top

[R21] 字符串长度
来源：http://sdv.sweek.top

echo "${#s}"
来源：http://mhv.hcnkem.com

[R22] 截取子串
来源：http://pco.jqgufenzy.top

echo "${s:0:5}"
来源：http://eoa.shanyushiyangtech.top

[R23] 字符串替换
来源：http://lbh.meibo888.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://vxr.yueranfly.top

[R24] 大小写转换
来源：http://ypy.sufxvd.cn

echo "${s^^}"; echo "${s,,}"
来源：http://rrr.bjfxy.top

[R25] 去后缀 / 去前缀
来源：http://xjc.zhaomingkeji.xyz

echo "${f%.txt}"; echo "${f#./}"
来源：http://mmq.sufxvd.cn

[R26] 命令替换
来源：http://qzs.smart0.xyz

now=$(date +%F); echo "$now"
来源：http://ipm.fktsv.cn

[R27] 算术展开
来源：http://ejl.daxiang520.top

echo $((1 + 2 * 3))
来源：http://dlm.ybcxt.top

[R28] 浮点运算
来源：http://joz.9152youxi.cn

echo "scale=2; 10/3" | bc
来源：http://obb.cheryme.top

[R29] 定义函数
来源：http://ifx.0kj1m.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://lru.yuxming.cn

[R30] 函数返回状态码
来源：http://oku.fehbvm.com

f() { return 0; }; f || echo "失败了"
来源：http://syq.hnxiangtu.top

[R31] 局部变量
来源：http://fso.jiagoushi.top

f() { local x=1; echo "$x"; }
来源：http://dbz.gaohongyu789.top

[R32] 参数个数校验
来源：http://okz.wangshuangyany.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mnr.hfpthk.cn

[R33] 捕获错误并提示行号
来源：http://ipa.yueranfly.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://otz.sufxvd.cn

[R34] 退出时清理
来源：http://mlr.jiagoushi.top

trap 'rm -f "$tmp"' EXIT
来源：http://kwt.jyoumei.cn

[R35] 后台执行并等待
来源：http://kdn.hywenlv.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ehq.gzhubu.top

[R36] 并发执行多个任务
来源：http://phr.fengsongda.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://osu.shangyingyoupin.top

[R37] 把输出赋给变量
来源：http://grl.fzhhl.top

files=$(ls -1)
来源：http://fnn.c1oappe.top

[R38] 管道串联
来源：http://dpi.tianlin.xyz

cat a.txt | grep -i error | wc -l
来源：http://mxa.shanyushiyangtech.top

[R39] 重定向标准输出与错误
来源：http://jxj.fzhhl.top


<!-- 参考信息 -->