代发 wailian999

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://iup.nwbrower.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://dha.quarkkingdee.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ofn.nanxinkj.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wlo.yuxming.cn

================================================================================
来源：http://ypg.nanxuanxn.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://rps.jqgfzy.top

================================================================================
来源：http://yta.sufxvd.cn

[Q01] 创建表
来源：http://lir.fengsongda.top

CREATE TABLE users (
来源：http://cfg.xingfuxueyuan.xyz

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://sic.fzhhl.top

name VARCHAR(50) NOT NULL,
来源：http://oax.cheryme.top

email VARCHAR(100) UNIQUE,
来源：http://sbi.yanxiufei.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://yxm.xinyue.icu

);
来源：http://gop.sysykeji.top

[Q02] 创建带外键的表
来源：http://kal.cheryme.top

CREATE TABLE orders (
来源：http://jto.yueranfly.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://dti.ydjk.org.cn

user_id INT NOT NULL,
来源：http://shh.jinyuanbaomall.cn

amount DECIMAL(10, 2),
来源：http://hsj.pengpengdd.cyou

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://gyt.yangfankeji.com

);
来源：http://muj.316326.xyz

[Q03] 增加列
来源：http://syz.aizwys.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ioa.hysaishi.cn

[Q04] 修改列类型
来源：http://pei.c1oappe.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://egd.iojbl.cn

[Q05] 重命名列
来源：http://lth.redwolf501.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://eoh.fanxiaobao.xyz

[Q06] 删除列
来源：http://ooj.zhongyouzk.top

ALTER TABLE users DROP COLUMN age;
来源：http://bhx.xingfuxueyuan.xyz

[Q07] 删除表
来源：http://tqe.zhengqikj.top

DROP TABLE IF EXISTS orders;
来源：http://hal.cqqwz.cn

[Q08] 创建普通索引
来源：http://rai.dashuyun.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://bbk.uphjek.com

[Q09] 创建唯一索引
来源：http://znz.fanxiaobao.xyz

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://eyd.shangyingyoupin.top

[Q10] 插入单行
来源：http://plz.redwolf501.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://gdo.shanyushiyangkeji.top

[Q11] 一次插入多行
来源：http://xre.pycfn.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://oio.hcnkem.com

[Q12] 插入后取自增 ID
来源：http://bnm.svipenyu.cn

INSERT INTO users (name) VALUES ('C');
来源：http://bmh.hysaishi.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://dzk.vehdjk.com

[Q13] 忽略重复插入
来源：http://jql.fengsongda.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://xjg.vqdsnc.cn

[Q14] 存在则更新（upsert）
来源：http://jis.hesvh.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://vpy.0kj1m.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://pye.xingfuxueyuan.xyz

[Q15] 查询全部
来源：http://qpt.0kj1m.cn

SELECT * FROM users;
来源：http://rjt.hongshengwenyu.top

[Q16] 查询指定列
来源：http://ffy.jyoumei.cn

SELECT id, name FROM users;
来源：http://kbw.zhijiandao.cn

[Q17] 条件查询
来源：http://zvo.sysykeji.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://tji.zhijiandao.cn

[Q18] 模糊匹配
来源：http://mus.sxryk.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mam.redwolf501.top

[Q19] 范围查询
来源：http://hyf.ywan-chungtsiang.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://rrm.nanxuanxn.top

[Q20] IN 列表
来源：http://pkj.jiagoushi.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://jtu.hongshengwenyu.top

[Q21] 空值判断
来源：http://kdn.guannengcc.top

SELECT * FROM users WHERE email IS NULL;
来源：http://xnj.chenlongwang.top

[Q22] 排序
来源：http://ail.9152youxi.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://abq.havefunace.top

[Q23] 分页
来源：http://vkt.smart0.xyz

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hcz.tian-w.cn

[Q24] 去重
来源：http://sps.zhiwuduotai.top

SELECT DISTINCT city FROM users;
来源：http://xqr.uphjek.com

[Q25] 只取前 N 条
来源：http://oon.zhijiandao.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ioh.316326.xyz

[Q26] 计数
来源：http://hwa.pycfn.com

SELECT COUNT(*) FROM users;
来源：http://hge.xingfuxueyuan.xyz

[Q27] 条件计数
来源：http://sba.sxryk.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://npl.cucudq.cn

[Q28] 求和与平均
来源：http://ipf.shzxlz.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://pod.pycfn.com

[Q29] 最大最小值
来源：http://ggb.iojbl.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://hwg.jianghu66.top

[Q30] 分组统计
来源：http://anv.dianchejie.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ovk.pycfn.com

[Q31] 分组后过滤
来源：http://vih.fzhhl.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://eve.chenzaomai.com

[Q32] 分组拼接字符串
来源：http://knn.shangyingyoupin.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://vyr.tianlin.xyz

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://rrp.jqgufenzy.top

[Q33] 多列分组
来源：http://vaf.epnwcf.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://zrf.chenjidiqi.icu

[Q34] 每组取第一条
来源：http://oru.jianghu66.top

SELECT * FROM (
来源：http://qtb.meibo888.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://lvj.yj20258888.top

) t WHERE rn = 1;
来源：http://vtb.nanxinkj.top

[Q35] 内连接
来源：http://vwq.52xcode.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://kma.chenlongwang.top

[Q36] 左连接
来源：http://xyg.redwolf501.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://avx.tian-w.cn

[Q37] 右连接
来源：http://uxe.c1oappe.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://yil.hfpthk.cn

[Q38] 全外连接（PostgreSQL）
来源：http://rwc.hnxiangtu.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://kap.hammf.cn

[Q39] 自连接（查上下级）
来源：http://yyq.fanxiaobao.xyz

SELECT e.name, m.name AS manager FROM employees e
来源：http://raz.shangyingyoupin.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://uep.hammf.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://sfu.jinyuanbaomall.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ese.snrcjt.cn

[Q41] 多表连接
来源：http://arr.jqgfzy.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://awa.cqqwz.cn

JOIN users u ON u.id = o.user_id
来源：http://tla.cdnleiting.top

JOIN products p ON p.id = o.product_id;
来源：http://omn.havefunace.top

[Q42] 连接条件附加过滤
来源：http://lnd.ybcxt.top

SELECT u.name, o.amount FROM users u
来源：http://lbv.hysaishi.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://qpu.nanxuanxn.top

[Q43] 标量子查询
来源：http://jxf.fktsv.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://iez.hongshengwenyu.top

[Q44] IN 子查询
来源：http://fjk.ehwqpu.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://vex.guowangkeji.top

[Q45] EXISTS 判断存在
来源：http://trx.yuxming.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wjw.vqdsnc.cn

[Q46] NOT EXISTS 判断不存在
来源：http://apg.snrcjt.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://osa.hysaishi.cn

[Q47] 与平均值比较
来源：http://nfn.shangyingyoupin.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://nbg.yj20258888.top

[Q48] CTE 公用表表达式
来源：http://rfi.xylfe.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wip.nanxinkj.top

SELECT * FROM t WHERE c > 5;
来源：http://oyv.yuanzhike.top

[Q49] 更新单行
来源：http://fyg.sxryk.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://zlt.jyoumei.cn

[Q50] 批量更新
来源：http://kng.shuidangran.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://iin.hesvh.cn

[Q51] 用子查询更新
来源：http://ojn.birdmap.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://adp.zhongyouzk.top

[Q52] 删除指定行
来源：http://pyq.andypj.xyz

DELETE FROM users WHERE id = 10;
来源：http://ihe.cheryme.top

[Q53] 按条件删除
来源：http://umo.chenlongwang.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://oeu.aizwys.cn

[Q54] 清空表
来源：http://ecc.zhengqikj.top

TRUNCATE TABLE logs;
来源：http://rqj.feifeiyinyue.top

[Q55] 排名（并列占位）
来源：http://ctt.fengsongda.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wmq.yj20258888.top

[Q56] 密集排名（并列不占位）
来源：http://kij.svipenyu.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://dgd.ctjpmb.com

[Q57] 行号
来源：http://ivy.sweek.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://btm.jqgfzy.top

[Q58] 累计求和
来源：http://ejo.fehbvm.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://bih.smart0.xyz

[Q59] 分组内累计
来源：http://zro.guannengcc.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://snq.zhaomingkeji.xyz

[Q60] 取上一行 / 下一行
来源：http://miz.xuetiantiany.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://dlf.zhixingplan.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://xtd.gotoacloud.top

[Q61] 移动平均
来源：http://non.gaohongyu789.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://vzf.hongshengwenyu.top

[Q62] 分组占比
来源：http://hhc.zhijiandao.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mms.xingfuxueyuan.xyz

[Q63] 开启事务
来源：http://ept.yfazqb.com

START TRANSACTION;                -- 或 BEGIN
来源：http://dax.yanxiufei.cn

[Q64] 提交事务
来源：http://xcu.0kj1m.cn

COMMIT;
来源：http://trz.xuanzx.com

[Q65] 回滚事务
来源：http://wmy.wangshuangyany.cn

ROLLBACK;
来源：http://tqv.yvedp.cn

[Q66] 行锁查询
来源：http://jga.ybcxt.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://cuo.ppjwa.cn

[Q67] 设置隔离级别
来源：http://nzj.redwolf501.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://jcl.vehdjk.com

[Q68] 保存点
来源：http://qlv.zdqjudy.top

SAVEPOINT sp1;
来源：http://kes.cdnleiting.top

ROLLBACK TO sp1;
来源：http://dvx.andypj.xyz

[Q69] 查看执行计划
来源：http://xog.yuanzhike.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://gjm.9152youxi.cn

[Q70] 更新统计信息
来源：http://gik.guannengcc.top

ANALYZE TABLE users;
来源：http://ylk.redwolf501.top

[Q71] 查看建表语句
来源：http://lzv.gaohongyu789.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://kvq.redwolf501.top

[Q72] 查看索引
来源：http://nhj.cucudq.cn

SHOW INDEX FROM users;
来源：http://vlo.uphjek.com

[Q73] 查看表状态
来源：http://cfp.ydjk.org.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://fvj.xuanzx.com

[Q74] 强制使用索引
来源：http://fge.chenlongwang.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://szr.ctjpmb.com

[Q75] 日期格式化
来源：http://ewe.0kj1m.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://jmm.yj20258888.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://tux.xylfe.cn

[Q76] 按天统计
来源：http://tio.sjlbkw.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://sen.daria6918.cn

[Q77] 时间加减
来源：http://dcd.yuxming.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://tyl.yangfankeji.com

[Q78] 当前时间
来源：http://ddi.tianlin.xyz

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://dyk.dianchejie.cn

[Q79] 字符串拼接
来源：http://rac.yj20258.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hlt.zycfv.cn

[Q80] 字符串截取
来源：http://lig.mhx1999.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://sgy.yueranfly.top

[Q81] 字符串替换
来源：http://ron.zycfv.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ohr.xuetiantiany.cn

[Q82] 字符长度与字节长度
来源：http://mrx.ivvv.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://apa.jqgufenzy.top

[Q83] 大小写转换
来源：http://vub.ivvv.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hth.tianlin.xyz

[Q84] 去除首尾空格
来源：http://kup.zhaomingkeji.xyz

SELECT TRIM(name) FROM users;
来源：http://lsj.pycfn.com

[Q85] 数值取整
来源：http://ckg.hammf.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://oml.yj202588.top

[Q86] 读取 JSON 字段
来源：http://qbw.fktsv.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://nkw.daxiang520.top

[Q87] JSON 字段做条件
来源：http://uvs.daxiang520.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://djl.hcnkem.com

[Q88] 行转列（条件聚合）
来源：http://axf.shuidangran.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://acb.nanxinkj.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ctk.yonumen.top

[Q89] 判断表是否存在
来源：http://unm.yanxiufei.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://bth.9152youxi.cn

[Q90] 生成序号列
来源：http://bmt.redwolf501.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://jcv.ppjwa.cn

================================================================================
来源：http://rfc.svipenyu.cn

R. Bash 专题
来源：http://wab.jqgfzy.top

================================================================================
来源：http://frs.guannengcc.top

[R01] shebang 与严格模式
来源：http://cvn.bjfxy.top

#!/usr/bin/env bash
来源：http://awt.yonumen.top

set -euo pipefail
来源：http://uza.nwbrower.top

[R02] 变量赋值与使用
来源：http://jvx.shangyingyoupin.top

name="Tom"; echo "$name"
来源：http://lyw.fehbvm.com

[R03] 只读变量
来源：http://zcn.zhaomingkeji.xyz

readonly PI=3.14
来源：http://xxx.daria6918.cn

[R04] 位置参数
来源：http://smm.zhengqikj.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://rsh.epnwcf.com

[R05] 参数默认值
来源：http://xhl.aizwys.cn

name="${1:-default}"
来源：http://gts.guowangkeji.top

[R06] 判断命令是否存在
来源：http://tia.9152youxi.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ihk.zhaomingkeji.xyz

[R07] if 判断文件
来源：http://yxq.mhx1999.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://swi.shangyingyoupin.top

[R08] 数值比较
来源：http://yvr.fanxiaobao.xyz

if (( a > b )); then echo "a 更大"; fi
来源：http://ajo.sysykeji.top

[R09] 字符串比较
来源：http://gdd.zhongyouzk.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://xap.wangshuangyany.cn

[R10] 正则匹配
来源：http://vmf.ivvv.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://xtk.zhijiandao.cn

[R11] case 多分支
来源：http://wqx.smart0.xyz

case "$1" in
来源：http://rdx.shangyingyoupin.top

start) echo "启动" ;;
来源：http://ghn.feifeiyinyue.top

stop)  echo "停止" ;;
来源：http://nqv.sjlbkw.cn

*)     echo "未知命令" ;;
来源：http://geu.ydjk.org.cn

esac
来源：http://mca.ehwqpu.com

[R12] for 遍历文件
来源：http://qzy.zdqjudy.top

for f in *.txt; do echo "$f"; done
来源：http://toj.yonumen.top

[R13] for 计数循环
来源：http://nkw.jianghu66.top

for i in {1..10}; do echo "$i"; done
来源：http://wcy.jinghuilouyu.cn

[R14] C 风格 for
来源：http://rbc.jinqigfzy.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://udy.chenlongwang.top

[R15] while 逐行读文件
来源：http://qfg.zhixingplan.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://nvo.feifeiyinyue.top

[R16] until 等待条件
来源：http://isi.hywenlv.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://pex.nwbrower.top

[R17] 数组定义与取值
来源：http://ouc.fzhhl.top

arr=(a b c); echo "${arr[0]}"
来源：http://fcd.hnqzz.top

[R18] 遍历数组
来源：http://apc.hongshengwenyu.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://oho.yueranfly.top

[R19] 数组长度
来源：http://tuf.yj202588.top

echo "${#arr[@]}"
来源：http://xbs.cqqwz.cn

[R20] 关联数组（字典）
来源：http://kjb.quarkkingdee.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://erk.jiagoushi.top

[R21] 字符串长度
来源：http://wtx.vqdsnc.cn

echo "${#s}"
来源：http://wko.zdqjudy.top

[R22] 截取子串
来源：http://eac.jyoumei.cn

echo "${s:0:5}"
来源：http://wew.ehwqpu.com

[R23] 字符串替换
来源：http://myl.gogol.net.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://jqc.c1oappe.top

[R24] 大小写转换
来源：http://hou.bbcook.cn

echo "${s^^}"; echo "${s,,}"
来源：http://pfp.dashuyun.cn

[R25] 去后缀 / 去前缀
来源：http://khv.xylfe.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://wbr.zhiwuduotai.top

[R26] 命令替换
来源：http://dbp.ywan-chungtsiang.top

now=$(date +%F); echo "$now"
来源：http://fgz.yj20258888.top

[R27] 算术展开
来源：http://qre.0kj1m.cn

echo $((1 + 2 * 3))
来源：http://lwu.sufxvd.cn

[R28] 浮点运算
来源：http://twg.sjlbkw.cn

echo "scale=2; 10/3" | bc
来源：http://vxu.aibaodan.cn

[R29] 定义函数
来源：http://stg.tianlin.xyz

add() { echo $(($1 + $2)); }; add 1 2
来源：http://afw.dianchejie.cn

[R30] 函数返回状态码
来源：http://aya.jianghu66.top

f() { return 0; }; f || echo "失败了"
来源：http://mru.yangfankeji.com

[R31] 局部变量
来源：http://eny.yfazqb.com

f() { local x=1; echo "$x"; }
来源：http://jay.yanxiufei.cn

[R32] 参数个数校验
来源：http://vwd.yj202588.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://rlc.smart0.xyz

[R33] 捕获错误并提示行号
来源：http://xpf.sweek.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://agf.zhixingplan.top

[R34] 退出时清理
来源：http://gko.sysykeji.top

trap 'rm -f "$tmp"' EXIT
来源：http://qfp.xuetiantiany.cn

[R35] 后台执行并等待
来源：http://tgm.jyoumei.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://nkf.shanyushiyangtech.top

[R36] 并发执行多个任务
来源：http://fxc.nanxuanxn.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://dhs.zhixingplan.top

[R37] 把输出赋给变量
来源：http://xki.hnqzz.top

files=$(ls -1)
来源：http://aki.fktsv.cn

[R38] 管道串联
来源：http://joo.zhengqikj.top

cat a.txt | grep -i error | wc -l
来源：http://bhb.zhiwuduotai.top

[R39] 重定向标准输出与错误
来源：http://hvk.ywan-chungtsiang.top

cmd > out.log 2>&1
来源：http://ujv.bbcook.cn

[R40] 追加写日志
来源：http://ddg.xingfuxueyuan.xyz

echo "log" >> out.log
来源：http://wqe.hammf.cn

[R41] 丢弃输出
来源：http://yor.bjfxy.top


<!-- 参考信息 -->