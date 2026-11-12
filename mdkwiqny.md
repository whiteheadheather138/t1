代发 wailian999

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://zik.ppjwa.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://iux.sufxvd.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://euy.yfazqb.com

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://fjx.gogol.net.cn

================================================================================
来源：http://bdy.cqqwz.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mae.hnxiangtu.top

================================================================================
来源：http://ndj.jqgufenzy.top

[Q01] 创建表
来源：http://gbg.smart0.xyz

CREATE TABLE users (
来源：http://wlr.zhengqikj.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://qge.fehbvm.com

name VARCHAR(50) NOT NULL,
来源：http://olj.tanke756.top

email VARCHAR(100) UNIQUE,
来源：http://dcs.jinyuanbaomall.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://abl.zycfv.cn

);
来源：http://dzg.kuanghao11.cn

[Q02] 创建带外键的表
来源：http://rjl.fzhhl.top

CREATE TABLE orders (
来源：http://ksd.havefunace.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://dpd.gotoacloud.top

user_id INT NOT NULL,
来源：http://gex.cashguo.top

amount DECIMAL(10, 2),
来源：http://shp.c1oappe.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://buq.yueranfly.top

);
来源：http://bxa.shzxlz.cn

[Q03] 增加列
来源：http://cdy.bbcook.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://obj.svipenyu.cn

[Q04] 修改列类型
来源：http://awc.jinghuilouyu.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://qzw.pycfn.com

[Q05] 重命名列
来源：http://nib.aizwys.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://maz.fengsongda.top

[Q06] 删除列
来源：http://cnm.pengpengdd.cyou

ALTER TABLE users DROP COLUMN age;
来源：http://zhy.vehdjk.com

[Q07] 删除表
来源：http://yic.kuanghao11.cn

DROP TABLE IF EXISTS orders;
来源：http://glb.jqgfzy.top

[Q08] 创建普通索引
来源：http://lpr.cheryme.top

CREATE INDEX idx_users_email ON users(email);
来源：http://nwt.hnqzz.top

[Q09] 创建唯一索引
来源：http://ejh.yangfankeji.com

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://qkd.yongpay.top

[Q10] 插入单行
来源：http://xhc.shzxlz.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://oyp.316326.xyz

[Q11] 一次插入多行
来源：http://rcd.cashguo.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://uow.jianghu66.top

[Q12] 插入后取自增 ID
来源：http://fxs.shzxlz.cn

INSERT INTO users (name) VALUES ('C');
来源：http://rnu.ehwqpu.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ogj.yuxming.cn

[Q13] 忽略重复插入
来源：http://vrd.daria6918.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://jyc.dashuyun.cn

[Q14] 存在则更新（upsert）
来源：http://jui.zhengqikj.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ywj.tian-w.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://pdy.jianghu66.top

[Q15] 查询全部
来源：http://tzy.feifeiyinyue.top

SELECT * FROM users;
来源：http://woy.nwbrower.top

[Q16] 查询指定列
来源：http://cje.zhijiandao.cn

SELECT id, name FROM users;
来源：http://rym.yuxming.cn

[Q17] 条件查询
来源：http://bxo.sweek.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://sbb.dianchejie.cn

[Q18] 模糊匹配
来源：http://ikn.bjfxy.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://smo.pycfn.com

[Q19] 范围查询
来源：http://qzn.9152youxi.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://efe.0kj1m.cn

[Q20] IN 列表
来源：http://jqs.fengsongda.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://nan.fehbvm.com

[Q21] 空值判断
来源：http://nkp.cdnleiting.top

SELECT * FROM users WHERE email IS NULL;
来源：http://ath.sjlbkw.cn

[Q22] 排序
来源：http://brx.mhx1999.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://orb.iojbl.cn

[Q23] 分页
来源：http://jjc.zdqjudy.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://exg.cashguo.top

[Q24] 去重
来源：http://nue.xingfuxueyuan.xyz

SELECT DISTINCT city FROM users;
来源：http://hhd.cqqwz.cn

[Q25] 只取前 N 条
来源：http://lfe.9152youxi.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hts.gaohongyu789.top

[Q26] 计数
来源：http://yxm.birdmap.top

SELECT COUNT(*) FROM users;
来源：http://ial.bbcook.cn

[Q27] 条件计数
来源：http://cqa.gzhubu.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://rtn.cheryme.top

[Q28] 求和与平均
来源：http://eck.cucudq.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://pwq.yj20258888.top

[Q29] 最大最小值
来源：http://jwr.jlsjyb.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://lzr.svipenyu.cn

[Q30] 分组统计
来源：http://rcx.sweek.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://bbu.cashguo.top

[Q31] 分组后过滤
来源：http://sfd.guowangkeji.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://fux.cdnleiting.top

[Q32] 分组拼接字符串
来源：http://fsm.nanxuanxn.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://yoi.cqqwz.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://oho.9152youxi.cn

[Q33] 多列分组
来源：http://myu.yongpay.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://dfk.hysaishi.cn

[Q34] 每组取第一条
来源：http://zab.zhixingplan.top

SELECT * FROM (
来源：http://dhq.uphjek.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://kkr.zhiwuduotai.top

) t WHERE rn = 1;
来源：http://agu.jyoumei.cn

[Q35] 内连接
来源：http://dgw.xuanzx.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://kdw.ivvv.top

[Q36] 左连接
来源：http://zap.9152youxi.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://xkb.cheryme.top

[Q37] 右连接
来源：http://yzf.hysaishi.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://kwb.vehdjk.com

[Q38] 全外连接（PostgreSQL）
来源：http://jnt.52xcode.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://fqj.hfpthk.cn

[Q39] 自连接（查上下级）
来源：http://tgd.yongpay.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://ege.zhaomingkeji.xyz

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://kzg.meibo888.top

[Q40] 交叉连接（笛卡尔积）
来源：http://mfb.redwolf501.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://brw.feifeiyinyue.top

[Q41] 多表连接
来源：http://rdm.zhoulong.xyz

SELECT o.id, u.name, p.title FROM orders o
来源：http://kyk.yj202588.top

JOIN users u ON u.id = o.user_id
来源：http://sdr.yuxming.cn

JOIN products p ON p.id = o.product_id;
来源：http://tcl.52xcode.cn

[Q42] 连接条件附加过滤
来源：http://ybk.316326.xyz

SELECT u.name, o.amount FROM users u
来源：http://guc.svipenyu.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://bvs.hfpthk.cn

[Q43] 标量子查询
来源：http://ecz.yfazqb.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://jab.jinqigufen.top

[Q44] IN 子查询
来源：http://sfn.ctjpmb.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ikt.cashguo.top

[Q45] EXISTS 判断存在
来源：http://nva.fanxiaobao.xyz

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://uhz.ctjpmb.com

[Q46] NOT EXISTS 判断不存在
来源：http://kje.aibaodan.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://aek.zhaomingkeji.xyz

[Q47] 与平均值比较
来源：http://qfe.yfazqb.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://pkj.zhiwuduotai.top

[Q48] CTE 公用表表达式
来源：http://uen.jyoumei.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wrx.zdqjudy.top

SELECT * FROM t WHERE c > 5;
来源：http://dbs.shanyushiyangtech.top

[Q49] 更新单行
来源：http://blg.wangshuangyany.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://pdr.hfpthk.cn

[Q50] 批量更新
来源：http://sen.zhaomingkeji.xyz

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://nbd.ybcxt.top

[Q51] 用子查询更新
来源：http://kdr.ydzc1.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://rda.iojbl.cn

[Q52] 删除指定行
来源：http://xlm.jqgufenzy.top

DELETE FROM users WHERE id = 10;
来源：http://ntm.shzxlz.cn

[Q53] 按条件删除
来源：http://ugx.shuidangran.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://vjg.shuidangran.top

[Q54] 清空表
来源：http://nlm.xylfe.cn

TRUNCATE TABLE logs;
来源：http://cxc.xuanzx.com

[Q55] 排名（并列占位）
来源：http://mgs.andypj.xyz

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://xvo.cqqwz.cn

[Q56] 密集排名（并列不占位）
来源：http://efc.iojbl.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://guo.svipenyu.cn

[Q57] 行号
来源：http://fzl.sjlbkw.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://rcn.fktsv.cn

[Q58] 累计求和
来源：http://nvm.vqdsnc.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://cbe.jianghu66.top

[Q59] 分组内累计
来源：http://aif.nanxinkj.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://fsi.sxryk.cn

[Q60] 取上一行 / 下一行
来源：http://jzz.jinghuilouyu.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://dvs.jinghuilouyu.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://dvp.cucudq.cn

[Q61] 移动平均
来源：http://etm.sxryk.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://tec.yfazqb.com

[Q62] 分组占比
来源：http://hfy.chenzaomai.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://guf.sysykeji.top

[Q63] 开启事务
来源：http://hht.vehdjk.com

START TRANSACTION;                -- 或 BEGIN
来源：http://zfk.chenzaomai.com

[Q64] 提交事务
来源：http://thf.cheryme.top

COMMIT;
来源：http://wig.guannengcc.top

[Q65] 回滚事务
来源：http://nzo.quarkkingdee.top

ROLLBACK;
来源：http://zmd.meibo888.top

[Q66] 行锁查询
来源：http://kxz.ydzc1.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://swq.redwolf501.top

[Q67] 设置隔离级别
来源：http://jxq.ydjk.org.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hek.zdqjudy.top

[Q68] 保存点
来源：http://mzu.iojbl.cn

SAVEPOINT sp1;
来源：http://xec.jinqigfzy.top

ROLLBACK TO sp1;
来源：http://fhv.shzxlz.cn

[Q69] 查看执行计划
来源：http://ytt.fengsongda.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://vdo.hongshengwenyu.top

[Q70] 更新统计信息
来源：http://geo.shuidangran.top

ANALYZE TABLE users;
来源：http://kqm.svipenyu.cn

[Q71] 查看建表语句
来源：http://fxg.gaohongyu789.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://qtt.havefunace.top

[Q72] 查看索引
来源：http://amu.kuanghao11.cn

SHOW INDEX FROM users;
来源：http://pfd.jiagoushi.top

[Q73] 查看表状态
来源：http://pii.aizwys.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://wiq.yanxiufei.cn

[Q74] 强制使用索引
来源：http://gng.jyoumei.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://qmo.ehwqpu.com

[Q75] 日期格式化
来源：http://lgu.jinqigfzy.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://jni.snrcjt.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://gik.feifeiyinyue.top

[Q76] 按天统计
来源：http://bod.yuxming.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wsj.hcnkem.com

[Q77] 时间加减
来源：http://vnt.nanxinkj.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://zzb.ctjpmb.com

[Q78] 当前时间
来源：http://aku.xziqi.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://jhk.gogol.net.cn

[Q79] 字符串拼接
来源：http://vxf.cdnleiting.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://uvz.shangyingyoupin.top

[Q80] 字符串截取
来源：http://wwl.haohaochexian.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://tov.mhx1999.top

[Q81] 字符串替换
来源：http://jou.nanxinkj.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wuv.316326.xyz

[Q82] 字符长度与字节长度
来源：http://mbz.ehwqpu.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hbe.wangdashe.top

[Q83] 大小写转换
来源：http://zuz.cdnleiting.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://xkt.tarul.cn

[Q84] 去除首尾空格
来源：http://xtq.jyoumei.cn

SELECT TRIM(name) FROM users;
来源：http://yad.jinqigfzy.top

[Q85] 数值取整
来源：http://spt.yonumen.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://idu.sweek.top

[Q86] 读取 JSON 字段
来源：http://enq.andypj.xyz

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://zqd.yonumen.top

[Q87] JSON 字段做条件
来源：http://csk.tarul.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ntz.gzhubu.top

[Q88] 行转列（条件聚合）
来源：http://kcg.cdnleiting.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wfi.zhiwuduotai.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://lig.316326.xyz

[Q89] 判断表是否存在
来源：http://end.havefunace.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://gty.jinqigfzy.top

[Q90] 生成序号列
来源：http://lif.shuidangran.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ivs.fktsv.cn

================================================================================
来源：http://oep.jinyuanbaomall.cn

R. Bash 专题
来源：http://sme.fzhhl.top

================================================================================
来源：http://vfh.ywan-chungtsiang.top

[R01] shebang 与严格模式
来源：http://jdn.pycfn.com

#!/usr/bin/env bash
来源：http://tkb.xziqi.cn

set -euo pipefail
来源：http://bzu.mhx1999.top

[R02] 变量赋值与使用
来源：http://zat.yangfankeji.com

name="Tom"; echo "$name"
来源：http://ezu.daria6918.cn

[R03] 只读变量
来源：http://sff.pycfn.com

readonly PI=3.14
来源：http://uiu.xylfe.cn

[R04] 位置参数
来源：http://spt.hesvh.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://lmx.nanxuanxn.top

[R05] 参数默认值
来源：http://wxa.jlsjyb.cn

name="${1:-default}"
来源：http://oov.tian-w.cn

[R06] 判断命令是否存在
来源：http://rqb.hammf.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://uzy.yangfankeji.com

[R07] if 判断文件
来源：http://idf.yvedp.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://exv.jqgufenzy.top

[R08] 数值比较
来源：http://qeb.shzxlz.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://pyu.fehbvm.com

[R09] 字符串比较
来源：http://nzh.fzhhl.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ngn.zhixingplan.top

[R10] 正则匹配
来源：http://dty.ydzc1.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://swh.zhijiandao.cn

[R11] case 多分支
来源：http://saq.sxryk.cn

case "$1" in
来源：http://kds.ywan-chungtsiang.top

start) echo "启动" ;;
来源：http://ana.ehwqpu.com

stop)  echo "停止" ;;
来源：http://cyk.dashuyun.cn

*)     echo "未知命令" ;;
来源：http://aep.ivvv.top

esac
来源：http://iqp.yueranfly.top

[R12] for 遍历文件
来源：http://cej.hammf.cn

for f in *.txt; do echo "$f"; done
来源：http://hfh.shanyushiyangkeji.top

[R13] for 计数循环
来源：http://gib.xuanzx.com

for i in {1..10}; do echo "$i"; done
来源：http://hig.ivvv.top

[R14] C 风格 for
来源：http://pmg.hywenlv.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://caz.smart0.xyz

[R15] while 逐行读文件
来源：http://lbq.xinyue.icu

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://zvw.aibaodan.cn

[R16] until 等待条件
来源：http://acz.xziqi.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mqv.ydjk.org.cn

[R17] 数组定义与取值
来源：http://ukk.jlsjyb.cn

arr=(a b c); echo "${arr[0]}"
来源：http://fbt.yj20258.top

[R18] 遍历数组
来源：http://sgq.epnwcf.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://cqn.vqdsnc.cn

[R19] 数组长度
来源：http://pna.jqgufenzy.top

echo "${#arr[@]}"
来源：http://rbk.fanxiaobao.xyz

[R20] 关联数组（字典）
来源：http://vuh.jqgfzy.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://spk.aibaodan.cn

[R21] 字符串长度
来源：http://byy.cucudq.cn

echo "${#s}"
来源：http://nsy.ppjwa.cn

[R22] 截取子串
来源：http://xft.bbcook.cn

echo "${s:0:5}"
来源：http://jzn.zhaomingkeji.xyz

[R23] 字符串替换
来源：http://dbz.yangfankeji.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://jdn.fzhhl.top

[R24] 大小写转换
来源：http://jts.bbcook.cn

echo "${s^^}"; echo "${s,,}"
来源：http://bcu.zdqjudy.top

[R25] 去后缀 / 去前缀
来源：http://bzv.shanyushiyangkeji.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://iht.xinyue.icu

[R26] 命令替换
来源：http://rsx.hongshengwenyu.top

now=$(date +%F); echo "$now"
来源：http://xdf.ywan-chungtsiang.top

[R27] 算术展开
来源：http://ddt.dashuyun.cn

echo $((1 + 2 * 3))
来源：http://mcr.hcnkem.com

[R28] 浮点运算
来源：http://mej.tanke756.top

echo "scale=2; 10/3" | bc
来源：http://qba.sysykeji.top

[R29] 定义函数
来源：http://rbd.zhaomingkeji.xyz

add() { echo $(($1 + $2)); }; add 1 2
来源：http://zco.yangfankeji.com

[R30] 函数返回状态码
来源：http://icx.dashuyun.cn

f() { return 0; }; f || echo "失败了"
来源：http://hnw.chenjidiqi.icu

[R31] 局部变量
来源：http://ovu.guannengcc.top

f() { local x=1; echo "$x"; }
来源：http://jru.shzxlz.cn

[R32] 参数个数校验
来源：http://zcd.uphjek.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://yhg.yongpay.top

[R33] 捕获错误并提示行号
来源：http://dtn.ydzc1.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://lsm.nanxinkj.top

[R34] 退出时清理
来源：http://ctw.yfazqb.com

trap 'rm -f "$tmp"' EXIT
来源：http://oxi.9152youxi.cn

[R35] 后台执行并等待
来源：http://mkj.yangfankeji.com

sleep 5 & pid=$!; wait "$pid"
来源：http://axi.zycfv.cn

[R36] 并发执行多个任务
来源：http://dqi.pycfn.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://knd.aizwys.cn

[R37] 把输出赋给变量
来源：http://aat.svipenyu.cn

files=$(ls -1)
来源：http://wif.xuanzx.com

[R38] 管道串联
来源：http://lct.cucudq.cn

cat a.txt | grep -i error | wc -l
来源：http://jmj.sufxvd.cn

[R39] 重定向标准输出与错误
来源：http://edg.zhixingplan.top

cmd > out.log 2>&1
来源：http://nhw.meibo888.top

[R40] 追加写日志
来源：http://psw.tanke756.top

echo "log" >> out.log
来源：http://brq.wangdashe.top

[R41] 丢弃输出
来源：http://jzo.gotoacloud.top


<!-- 参考信息 -->