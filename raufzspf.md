代发 wailian999

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://fab.hesvh.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://kiy.xylfe.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://xyq.c1oappe.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://dya.chenzaomai.com

================================================================================
来源：http://pqp.cqqwz.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://zyq.yonumen.top

================================================================================
来源：http://wfv.zhongyouzk.top

[Q01] 创建表
来源：http://uwd.guannengcc.top

CREATE TABLE users (
来源：http://jgq.gaohongyu789.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://gvd.epnwcf.com

name VARCHAR(50) NOT NULL,
来源：http://isd.yueranfly.top

email VARCHAR(100) UNIQUE,
来源：http://jpm.guannengcc.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://aps.hesvh.cn

);
来源：http://pud.jinyuanbaomall.cn

[Q02] 创建带外键的表
来源：http://ope.chenjidiqi.icu

CREATE TABLE orders (
来源：http://hqi.vqdsnc.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://akw.sweek.top

user_id INT NOT NULL,
来源：http://tno.sxryk.cn

amount DECIMAL(10, 2),
来源：http://szs.jiagoushi.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mna.yonumen.top

);
来源：http://xvk.dianchejie.cn

[Q03] 增加列
来源：http://sso.yongpay.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://fso.vqdsnc.cn

[Q04] 修改列类型
来源：http://ceo.sweek.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://yrj.redwolf501.top

[Q05] 重命名列
来源：http://wzu.hysaishi.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://jyk.iojbl.cn

[Q06] 删除列
来源：http://ywx.jqgfzy.top

ALTER TABLE users DROP COLUMN age;
来源：http://cnp.mhx1999.top

[Q07] 删除表
来源：http://srw.chenjidiqi.icu

DROP TABLE IF EXISTS orders;
来源：http://uzj.jianghu66.top

[Q08] 创建普通索引
来源：http://ifs.gogol.net.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://vwb.hammf.cn

[Q09] 创建唯一索引
来源：http://czb.hysaishi.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://pwa.hongshengwenyu.top

[Q10] 插入单行
来源：http://smt.redwolf501.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ldy.hnqzz.top

[Q11] 一次插入多行
来源：http://opf.ydjk.org.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://kno.zhengqikj.top

[Q12] 插入后取自增 ID
来源：http://xov.yanxiufei.cn

INSERT INTO users (name) VALUES ('C');
来源：http://uyq.shanyushiyangkeji.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://zxt.ppjwa.cn

[Q13] 忽略重复插入
来源：http://irh.jqgufenzy.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://sfr.jinqigfzy.top

[Q14] 存在则更新（upsert）
来源：http://iet.daxiang520.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://all.yangfankeji.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://zce.haohaochexian.top

[Q15] 查询全部
来源：http://fmv.chenjidiqi.icu

SELECT * FROM users;
来源：http://ngn.fengsongda.top

[Q16] 查询指定列
来源：http://kei.nanxinkj.top

SELECT id, name FROM users;
来源：http://shd.xylfe.cn

[Q17] 条件查询
来源：http://vmn.tarul.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://pen.shangyingyoupin.top

[Q18] 模糊匹配
来源：http://aqz.xingfuxueyuan.xyz

SELECT * FROM users WHERE name LIKE '张%';
来源：http://umq.chenzaomai.com

[Q19] 范围查询
来源：http://aoq.chenzaomai.com

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://nit.andypj.xyz

[Q20] IN 列表
来源：http://fpz.sufxvd.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://syt.ivvv.top

[Q21] 空值判断
来源：http://pxe.gogol.net.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://wxz.tarul.cn

[Q22] 排序
来源：http://axp.jlsjyb.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ahi.jianghu66.top

[Q23] 分页
来源：http://dgu.52xcode.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://xlo.aibaodan.cn

[Q24] 去重
来源：http://eei.tianlin.xyz

SELECT DISTINCT city FROM users;
来源：http://ihw.andypj.xyz

[Q25] 只取前 N 条
来源：http://xiu.hesvh.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://bcr.hammf.cn

[Q26] 计数
来源：http://rmz.dashuyun.cn

SELECT COUNT(*) FROM users;
来源：http://viv.cheryme.top

[Q27] 条件计数
来源：http://hwr.hnqzz.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mej.jqgufenzy.top

[Q28] 求和与平均
来源：http://vaj.shanyushiyangtech.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://xoa.ehwqpu.com

[Q29] 最大最小值
来源：http://era.shanyushiyangtech.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://myu.tanke756.top

[Q30] 分组统计
来源：http://umn.fzhhl.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://pfy.chenzaomai.com

[Q31] 分组后过滤
来源：http://agn.zhiwuduotai.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hec.zdbjq.cn

[Q32] 分组拼接字符串
来源：http://brb.birdmap.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://nzz.yongpay.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://fwy.jinqigufen.top

[Q33] 多列分组
来源：http://kxv.jiagoushi.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://zde.pycfn.com

[Q34] 每组取第一条
来源：http://edh.yfazqb.com

SELECT * FROM (
来源：http://ggb.tanke756.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://vme.aibaodan.cn

) t WHERE rn = 1;
来源：http://uke.xuetiantiany.cn

[Q35] 内连接
来源：http://slc.ydzc1.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://oll.yueranfly.top

[Q36] 左连接
来源：http://bov.zdbjq.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://gfd.sysykeji.top

[Q37] 右连接
来源：http://ggw.yuanzhike.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://nev.quarkkingdee.top

[Q38] 全外连接（PostgreSQL）
来源：http://ign.yfazqb.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://iil.zhiwuduotai.top

[Q39] 自连接（查上下级）
来源：http://vwl.jianghu66.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://hui.yuxming.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://emv.ybcxt.top

[Q40] 交叉连接（笛卡尔积）
来源：http://uah.fanxiaobao.xyz

SELECT * FROM colors CROSS JOIN sizes;
来源：http://xya.yangfankeji.com

[Q41] 多表连接
来源：http://abl.zhaomingkeji.xyz

SELECT o.id, u.name, p.title FROM orders o
来源：http://vxy.chenzaomai.com

JOIN users u ON u.id = o.user_id
来源：http://iov.yangfankeji.com

JOIN products p ON p.id = o.product_id;
来源：http://sje.vehdjk.com

[Q42] 连接条件附加过滤
来源：http://jri.yonumen.top

SELECT u.name, o.amount FROM users u
来源：http://gwo.hongshengwenyu.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://yvt.zhiwuduotai.top

[Q43] 标量子查询
来源：http://arv.zhoulong.xyz

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://fol.fanxiaobao.xyz

[Q44] IN 子查询
来源：http://nha.dashuyun.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://lxu.xingfuxueyuan.xyz

[Q45] EXISTS 判断存在
来源：http://bys.zycfv.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rrz.hywenlv.cn

[Q46] NOT EXISTS 判断不存在
来源：http://pvh.316326.xyz

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xif.gogol.net.cn

[Q47] 与平均值比较
来源：http://vbd.xinyue.icu

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wcy.tianlin.xyz

[Q48] CTE 公用表表达式
来源：http://ota.sxryk.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://nmg.bjfxy.top

SELECT * FROM t WHERE c > 5;
来源：http://kvr.tarul.cn

[Q49] 更新单行
来源：http://qgn.xingfuxueyuan.xyz

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hkk.wangshuangyany.cn

[Q50] 批量更新
来源：http://adu.tanke756.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://qqj.fzhhl.top

[Q51] 用子查询更新
来源：http://nun.cheryme.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://cpu.cqqwz.cn

[Q52] 删除指定行
来源：http://non.zhengqikj.top

DELETE FROM users WHERE id = 10;
来源：http://uye.vqdsnc.cn

[Q53] 按条件删除
来源：http://zcf.ydzc1.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://bgz.pycfn.com

[Q54] 清空表
来源：http://kbh.yj20258888.top

TRUNCATE TABLE logs;
来源：http://omd.hcnkem.com

[Q55] 排名（并列占位）
来源：http://quf.shangyingyoupin.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://slb.ehwqpu.com

[Q56] 密集排名（并列不占位）
来源：http://rkx.xziqi.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://acn.snrcjt.cn

[Q57] 行号
来源：http://svh.cheryme.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://llb.snrcjt.cn

[Q58] 累计求和
来源：http://gnv.hywenlv.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://sik.cashguo.top

[Q59] 分组内累计
来源：http://geb.gogol.net.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ahe.ehwqpu.com

[Q60] 取上一行 / 下一行
来源：http://uof.shuidangran.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://uct.xuetiantiany.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://iwk.jlsjyb.cn

[Q61] 移动平均
来源：http://rkh.fengsongda.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://jqz.zhoulong.xyz

[Q62] 分组占比
来源：http://imd.sweek.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://jcu.hnqzz.top

[Q63] 开启事务
来源：http://dok.hysaishi.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://qrx.daria6918.cn

[Q64] 提交事务
来源：http://eux.tanke756.top

COMMIT;
来源：http://rqo.cdnleiting.top

[Q65] 回滚事务
来源：http://vxl.hnqzz.top

ROLLBACK;
来源：http://qvl.tianlin.xyz

[Q66] 行锁查询
来源：http://mns.ywan-chungtsiang.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://sol.yuxming.cn

[Q67] 设置隔离级别
来源：http://rfw.nwbrower.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://kzi.tanke756.top

[Q68] 保存点
来源：http://zsj.fehbvm.com

SAVEPOINT sp1;
来源：http://nfw.daxiang520.top

ROLLBACK TO sp1;
来源：http://ebv.sweek.top

[Q69] 查看执行计划
来源：http://kbd.yanxiufei.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wwf.guowangkeji.top

[Q70] 更新统计信息
来源：http://cej.redwolf501.top

ANALYZE TABLE users;
来源：http://dag.hfpthk.cn

[Q71] 查看建表语句
来源：http://qdb.fehbvm.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://oiu.cashguo.top

[Q72] 查看索引
来源：http://wag.havefunace.top

SHOW INDEX FROM users;
来源：http://cws.fehbvm.com

[Q73] 查看表状态
来源：http://kvu.chenlongwang.top

SHOW TABLE STATUS LIKE 'users';
来源：http://lxv.52xcode.cn

[Q74] 强制使用索引
来源：http://aoi.zhixingplan.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://csq.yuanzhike.top

[Q75] 日期格式化
来源：http://zym.cdnleiting.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://yyf.chenzaomai.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wpb.wangshuangyany.cn

[Q76] 按天统计
来源：http://khw.dianchejie.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ixp.vehdjk.com

[Q77] 时间加减
来源：http://krx.fanxiaobao.xyz

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://jbn.tian-w.cn

[Q78] 当前时间
来源：http://wsa.jinqigufen.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ayc.fengsongda.top

[Q79] 字符串拼接
来源：http://rhc.birdmap.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ivl.0kj1m.cn

[Q80] 字符串截取
来源：http://iuk.svipenyu.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://xja.aizwys.cn

[Q81] 字符串替换
来源：http://xwe.tarul.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wqy.svipenyu.cn

[Q82] 字符长度与字节长度
来源：http://iwe.xuetiantiany.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wbe.dashuyun.cn

[Q83] 大小写转换
来源：http://udi.yfazqb.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wyy.tian-w.cn

[Q84] 去除首尾空格
来源：http://qfj.jiagoushi.top

SELECT TRIM(name) FROM users;
来源：http://zhj.zhaomingkeji.xyz

[Q85] 数值取整
来源：http://wii.hfpthk.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ktx.vqdsnc.cn

[Q86] 读取 JSON 字段
来源：http://hpe.gogol.net.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://zcj.birdmap.top

[Q87] JSON 字段做条件
来源：http://vky.jinyuanbaomall.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://xxm.chenjidiqi.icu

[Q88] 行转列（条件聚合）
来源：http://gcq.dianchejie.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mlp.hysaishi.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://kiy.hnxiangtu.top

[Q89] 判断表是否存在
来源：http://oik.gogol.net.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://fdm.xinyue.icu

[Q90] 生成序号列
来源：http://bmy.svipenyu.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://byx.sxryk.cn

================================================================================
来源：http://gwf.chenlongwang.top

R. Bash 专题
来源：http://lns.sxryk.cn

================================================================================
来源：http://bah.c1oappe.top

[R01] shebang 与严格模式
来源：http://jca.wangshuangyany.cn

#!/usr/bin/env bash
来源：http://kwx.svipenyu.cn

set -euo pipefail
来源：http://ruw.jlsjyb.cn

[R02] 变量赋值与使用
来源：http://dgy.shuidangran.top

name="Tom"; echo "$name"
来源：http://xzm.xingfuxueyuan.xyz

[R03] 只读变量
来源：http://vlx.fanxiaobao.xyz

readonly PI=3.14
来源：http://rfu.c1oappe.top

[R04] 位置参数
来源：http://ngt.cheryme.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://nft.shanyushiyangkeji.top

[R05] 参数默认值
来源：http://vxc.hfpthk.cn

name="${1:-default}"
来源：http://dbg.sysykeji.top

[R06] 判断命令是否存在
来源：http://oom.jinqigfzy.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hjf.zhixingplan.top

[R07] if 判断文件
来源：http://hvq.cqqwz.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://gox.redwolf501.top

[R08] 数值比较
来源：http://ybb.xuanzx.com

if (( a > b )); then echo "a 更大"; fi
来源：http://ftu.bjfxy.top

[R09] 字符串比较
来源：http://abz.ywan-chungtsiang.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://kxp.tarul.cn

[R10] 正则匹配
来源：http://qye.shuidangran.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ola.jinqigufen.top

[R11] case 多分支
来源：http://juc.xziqi.cn

case "$1" in
来源：http://yca.nanxuanxn.top

start) echo "启动" ;;
来源：http://mka.aibaodan.cn

stop)  echo "停止" ;;
来源：http://reh.jlsjyb.cn

*)     echo "未知命令" ;;
来源：http://kvh.sjlbkw.cn

esac
来源：http://dki.yj20258.top

[R12] for 遍历文件
来源：http://fjy.sysykeji.top

for f in *.txt; do echo "$f"; done
来源：http://nsv.yj202588.top

[R13] for 计数循环
来源：http://mxh.9152youxi.cn

for i in {1..10}; do echo "$i"; done
来源：http://aqq.tarul.cn

[R14] C 风格 for
来源：http://gzu.jqgufenzy.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mqg.xylfe.cn

[R15] while 逐行读文件
来源：http://ule.sxryk.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://dbl.havefunace.top

[R16] until 等待条件
来源：http://mfh.chenlongwang.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wvi.fzhhl.top

[R17] 数组定义与取值
来源：http://bhg.zdqjudy.top

arr=(a b c); echo "${arr[0]}"
来源：http://vtu.zdbjq.cn

[R18] 遍历数组
来源：http://fpb.zhijiandao.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://tnq.yj202588.top

[R19] 数组长度
来源：http://avz.shzxlz.cn

echo "${#arr[@]}"
来源：http://kno.sjlbkw.cn

[R20] 关联数组（字典）
来源：http://ejb.tanke756.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://zjh.mhx1999.top

[R21] 字符串长度
来源：http://hsh.shanyushiyangkeji.top

echo "${#s}"
来源：http://mwl.svipenyu.cn

[R22] 截取子串
来源：http://sxq.hesvh.cn

echo "${s:0:5}"
来源：http://hkv.pengpengdd.cyou

[R23] 字符串替换
来源：http://drg.guowangkeji.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://cgf.cucudq.cn

[R24] 大小写转换
来源：http://vqo.jiagoushi.top

echo "${s^^}"; echo "${s,,}"
来源：http://ofd.birdmap.top

[R25] 去后缀 / 去前缀
来源：http://taq.jinqigufen.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://dji.cdnleiting.top

[R26] 命令替换
来源：http://chd.jinqigfzy.top

now=$(date +%F); echo "$now"
来源：http://ycf.yongpay.top

[R27] 算术展开
来源：http://aai.haohaochexian.top

echo $((1 + 2 * 3))
来源：http://jtk.quarkkingdee.top

[R28] 浮点运算
来源：http://fgk.tanke756.top

echo "scale=2; 10/3" | bc
来源：http://vqy.xylfe.cn

[R29] 定义函数
来源：http://wwi.yvedp.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://olu.epnwcf.com

[R30] 函数返回状态码
来源：http://smu.epnwcf.com

f() { return 0; }; f || echo "失败了"
来源：http://vqc.tarul.cn

[R31] 局部变量
来源：http://cxn.zhongyouzk.top

f() { local x=1; echo "$x"; }
来源：http://pge.haohaochexian.top

[R32] 参数个数校验
来源：http://don.fzhhl.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://xdm.feifeiyinyue.top

[R33] 捕获错误并提示行号
来源：http://vtt.jianghu66.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://zkz.fktsv.cn

[R34] 退出时清理
来源：http://wfr.yongpay.top

trap 'rm -f "$tmp"' EXIT
来源：http://cri.andypj.xyz

[R35] 后台执行并等待
来源：http://ymt.cqqwz.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://byb.xinyue.icu

[R36] 并发执行多个任务
来源：http://zha.0kj1m.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wet.ybcxt.top

[R37] 把输出赋给变量
来源：http://noh.nwbrower.top

files=$(ls -1)
来源：http://qml.sjlbkw.cn

[R38] 管道串联
来源：http://rwh.dashuyun.cn

cat a.txt | grep -i error | wc -l
来源：http://sji.ehwqpu.com

[R39] 重定向标准输出与错误
来源：http://hqj.nwbrower.top

cmd > out.log 2>&1
来源：http://jse.jinyuanbaomall.cn

[R40] 追加写日志
来源：http://iad.cucudq.cn

echo "log" >> out.log
来源：http://xhc.tian-w.cn

[R41] 丢弃输出
来源：http://vom.quarkkingdee.top


<!-- 参考信息 -->