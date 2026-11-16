代发 wailian999

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://bvh.chenzaomai.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://kuy.wangshuangyany.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://gft.jqgufenzy.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://qta.hywenlv.cn

================================================================================
来源：http://uwa.guowangkeji.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://rok.zhijiandao.cn

================================================================================
来源：http://par.gaohongyu789.top

[Q01] 创建表
来源：http://rkk.guannengcc.top

CREATE TABLE users (
来源：http://osu.zycfv.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://oak.shanyushiyangtech.top

name VARCHAR(50) NOT NULL,
来源：http://nmd.xinyue.icu

email VARCHAR(100) UNIQUE,
来源：http://dmm.bjfxy.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hql.xuanzx.com

);
来源：http://udc.svipenyu.cn

[Q02] 创建带外键的表
来源：http://qwp.yanxiufei.cn

CREATE TABLE orders (
来源：http://yoe.chenjidiqi.icu

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mje.cqqwz.cn

user_id INT NOT NULL,
来源：http://hur.hcnkem.com

amount DECIMAL(10, 2),
来源：http://rzd.zycfv.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://trl.ywan-chungtsiang.top

);
来源：http://vwu.jinghuilouyu.cn

[Q03] 增加列
来源：http://frc.jqgufenzy.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://vei.zhongyouzk.top

[Q04] 修改列类型
来源：http://rml.hywenlv.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://gry.ehwqpu.com

[Q05] 重命名列
来源：http://yfa.jyoumei.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hlv.0kj1m.cn

[Q06] 删除列
来源：http://zyr.kuanghao11.cn

ALTER TABLE users DROP COLUMN age;
来源：http://iaa.fzhhl.top

[Q07] 删除表
来源：http://ujv.ybcxt.top

DROP TABLE IF EXISTS orders;
来源：http://qbk.sxryk.cn

[Q08] 创建普通索引
来源：http://ubx.shzxlz.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://qsu.nwbrower.top

[Q09] 创建唯一索引
来源：http://ypu.meibo888.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hnm.fanxiaobao.xyz

[Q10] 插入单行
来源：http://ksv.redwolf501.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://zqj.yueranfly.top

[Q11] 一次插入多行
来源：http://grr.9152youxi.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://sxp.c1oappe.top

[Q12] 插入后取自增 ID
来源：http://hue.svipenyu.cn

INSERT INTO users (name) VALUES ('C');
来源：http://rnf.kuanghao11.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://rqd.nanxinkj.top

[Q13] 忽略重复插入
来源：http://rjd.xuetiantiany.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://pcd.yj202588.top

[Q14] 存在则更新（upsert）
来源：http://gfx.ppjwa.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://kme.yonumen.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://bgm.ydzc1.top

[Q15] 查询全部
来源：http://ntb.hfpthk.cn

SELECT * FROM users;
来源：http://afu.hcnkem.com

[Q16] 查询指定列
来源：http://ymj.hammf.cn

SELECT id, name FROM users;
来源：http://cjs.jinghuilouyu.cn

[Q17] 条件查询
来源：http://bqn.nanxinkj.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://zqz.hywenlv.cn

[Q18] 模糊匹配
来源：http://lcm.birdmap.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ifu.sufxvd.cn

[Q19] 范围查询
来源：http://nvy.uphjek.com

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://djm.daxiang520.top

[Q20] IN 列表
来源：http://xik.zdqjudy.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://uzf.bjfxy.top

[Q21] 空值判断
来源：http://djr.jlsjyb.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://lnu.yueranfly.top

[Q22] 排序
来源：http://bks.epnwcf.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ggs.epnwcf.com

[Q23] 分页
来源：http://qjc.cucudq.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://iqn.0kj1m.cn

[Q24] 去重
来源：http://git.wangshuangyany.cn

SELECT DISTINCT city FROM users;
来源：http://efu.sufxvd.cn

[Q25] 只取前 N 条
来源：http://ucr.fzhhl.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://lln.hnqzz.top

[Q26] 计数
来源：http://dkd.jyoumei.cn

SELECT COUNT(*) FROM users;
来源：http://yfm.nanxinkj.top

[Q27] 条件计数
来源：http://vvn.jiagoushi.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://rar.jinghuilouyu.cn

[Q28] 求和与平均
来源：http://jjb.ppjwa.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wun.xinyue.icu

[Q29] 最大最小值
来源：http://fnd.birdmap.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://uwz.gogol.net.cn

[Q30] 分组统计
来源：http://xij.sysykeji.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://vbk.fengsongda.top

[Q31] 分组后过滤
来源：http://mip.fanxiaobao.xyz

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://gqy.yuanzhike.top

[Q32] 分组拼接字符串
来源：http://ilb.yangfankeji.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://avk.9152youxi.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wpz.xylfe.cn

[Q33] 多列分组
来源：http://ovj.chenzaomai.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://vzo.nwbrower.top

[Q34] 每组取第一条
来源：http://rfh.zdqjudy.top

SELECT * FROM (
来源：http://goz.shanyushiyangtech.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://eip.0kj1m.cn

) t WHERE rn = 1;
来源：http://hzn.hywenlv.cn

[Q35] 内连接
来源：http://fsg.epnwcf.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://gwi.xinyue.icu

[Q36] 左连接
来源：http://auo.jinyuanbaomall.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://pnh.fehbvm.com

[Q37] 右连接
来源：http://wfb.jiagoushi.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://qsp.jqgfzy.top

[Q38] 全外连接（PostgreSQL）
来源：http://nzn.guowangkeji.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ccb.epnwcf.com

[Q39] 自连接（查上下级）
来源：http://hrm.gotoacloud.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://fdf.iojbl.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wfe.havefunace.top

[Q40] 交叉连接（笛卡尔积）
来源：http://awd.chenzaomai.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://syy.snrcjt.cn

[Q41] 多表连接
来源：http://fll.pengpengdd.cyou

SELECT o.id, u.name, p.title FROM orders o
来源：http://ysg.tianlin.xyz

JOIN users u ON u.id = o.user_id
来源：http://mnk.aibaodan.cn

JOIN products p ON p.id = o.product_id;
来源：http://fou.xylfe.cn

[Q42] 连接条件附加过滤
来源：http://azm.nanxinkj.top

SELECT u.name, o.amount FROM users u
来源：http://obu.iojbl.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://jdl.zhengqikj.top

[Q43] 标量子查询
来源：http://kwl.yangfankeji.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wcy.haohaochexian.top

[Q44] IN 子查询
来源：http://gps.fzhhl.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://xwd.bjfxy.top

[Q45] EXISTS 判断存在
来源：http://qxw.fktsv.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jcy.xinyue.icu

[Q46] NOT EXISTS 判断不存在
来源：http://zyc.9152youxi.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://clo.snrcjt.cn

[Q47] 与平均值比较
来源：http://stg.hysaishi.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://yai.zhoulong.xyz

[Q48] CTE 公用表表达式
来源：http://udn.aizwys.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://xck.xinyue.icu

SELECT * FROM t WHERE c > 5;
来源：http://pxr.feifeiyinyue.top

[Q49] 更新单行
来源：http://own.yuxming.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://nib.zhiwuduotai.top

[Q50] 批量更新
来源：http://hgq.mhx1999.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://nwk.sjlbkw.cn

[Q51] 用子查询更新
来源：http://chx.ivvv.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wrt.xziqi.cn

[Q52] 删除指定行
来源：http://vye.gzhubu.top

DELETE FROM users WHERE id = 10;
来源：http://dkt.birdmap.top

[Q53] 按条件删除
来源：http://mko.havefunace.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hpx.smart0.xyz

[Q54] 清空表
来源：http://bpu.ivvv.top

TRUNCATE TABLE logs;
来源：http://gmd.jqgufenzy.top

[Q55] 排名（并列占位）
来源：http://doc.hammf.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://kxl.yvedp.cn

[Q56] 密集排名（并列不占位）
来源：http://iwr.hammf.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://kar.tarul.cn

[Q57] 行号
来源：http://jtq.daxiang520.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://yof.yvedp.cn

[Q58] 累计求和
来源：http://qew.bjfxy.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://elg.cdnleiting.top

[Q59] 分组内累计
来源：http://ksk.ctjpmb.com

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://lld.havefunace.top

[Q60] 取上一行 / 下一行
来源：http://ogi.ehwqpu.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://drs.sweek.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hei.gogol.net.cn

[Q61] 移动平均
来源：http://ozc.xingfuxueyuan.xyz

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://srh.shangyingyoupin.top

[Q62] 分组占比
来源：http://nan.hesvh.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://fgh.xuanzx.com

[Q63] 开启事务
来源：http://cve.daria6918.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://vtq.yj20258.top

[Q64] 提交事务
来源：http://aef.hysaishi.cn

COMMIT;
来源：http://koi.shangyingyoupin.top

[Q65] 回滚事务
来源：http://pfo.jianghu66.top

ROLLBACK;
来源：http://smg.hesvh.cn

[Q66] 行锁查询
来源：http://duh.birdmap.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ffr.xinyue.icu

[Q67] 设置隔离级别
来源：http://anh.jinqigfzy.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://fsy.mhx1999.top

[Q68] 保存点
来源：http://nsf.pycfn.com

SAVEPOINT sp1;
来源：http://izf.ydjk.org.cn

ROLLBACK TO sp1;
来源：http://von.jinqigufen.top

[Q69] 查看执行计划
来源：http://znj.pengpengdd.cyou

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://dde.cheryme.top

[Q70] 更新统计信息
来源：http://lwb.dianchejie.cn

ANALYZE TABLE users;
来源：http://ykb.fanxiaobao.xyz

[Q71] 查看建表语句
来源：http://gsq.ybcxt.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://fmc.birdmap.top

[Q72] 查看索引
来源：http://yju.sweek.top

SHOW INDEX FROM users;
来源：http://tgn.vqdsnc.cn

[Q73] 查看表状态
来源：http://dmb.dashuyun.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://cdo.ivvv.top

[Q74] 强制使用索引
来源：http://wul.shanyushiyangtech.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://lfz.jinqigufen.top

[Q75] 日期格式化
来源：http://iie.jinqigfzy.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://oql.sxryk.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://frn.havefunace.top

[Q76] 按天统计
来源：http://eli.zdbjq.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://tet.jinqigufen.top

[Q77] 时间加减
来源：http://lrt.zhiwuduotai.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://kif.dashuyun.cn

[Q78] 当前时间
来源：http://hhf.vqdsnc.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://jiy.gotoacloud.top

[Q79] 字符串拼接
来源：http://ujj.wangshuangyany.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ock.hnqzz.top

[Q80] 字符串截取
来源：http://cpy.gzhubu.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wfp.andypj.xyz

[Q81] 字符串替换
来源：http://xcy.tian-w.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://lpf.uphjek.com

[Q82] 字符长度与字节长度
来源：http://opn.c1oappe.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://gdi.nwbrower.top

[Q83] 大小写转换
来源：http://uwd.tian-w.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://cdq.jinyuanbaomall.cn

[Q84] 去除首尾空格
来源：http://oxq.tianlin.xyz

SELECT TRIM(name) FROM users;
来源：http://klq.daxiang520.top

[Q85] 数值取整
来源：http://ekk.tianlin.xyz

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://stz.jianghu66.top

[Q86] 读取 JSON 字段
来源：http://cfl.iojbl.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://uhi.yongpay.top

[Q87] JSON 字段做条件
来源：http://olm.xuanzx.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mvj.yangfankeji.com

[Q88] 行转列（条件聚合）
来源：http://lbc.9152youxi.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://eoj.fktsv.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ecn.daria6918.cn

[Q89] 判断表是否存在
来源：http://kfs.shanyushiyangkeji.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://rlx.shuidangran.top

[Q90] 生成序号列
来源：http://wqr.xinyue.icu

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://iqg.yuanzhike.top

================================================================================
来源：http://jxj.uphjek.com

R. Bash 专题
来源：http://hsl.uphjek.com

================================================================================
来源：http://cgn.vehdjk.com

[R01] shebang 与严格模式
来源：http://urs.jinghuilouyu.cn

#!/usr/bin/env bash
来源：http://zan.aibaodan.cn

set -euo pipefail
来源：http://txv.uphjek.com

[R02] 变量赋值与使用
来源：http://zgl.ydzc1.top

name="Tom"; echo "$name"
来源：http://btx.xziqi.cn

[R03] 只读变量
来源：http://fbw.sufxvd.cn

readonly PI=3.14
来源：http://liy.shzxlz.cn

[R04] 位置参数
来源：http://xqs.hammf.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://jms.hcnkem.com

[R05] 参数默认值
来源：http://xre.gaohongyu789.top

name="${1:-default}"
来源：http://jkp.fehbvm.com

[R06] 判断命令是否存在
来源：http://lxl.epnwcf.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ooj.shanyushiyangkeji.top

[R07] if 判断文件
来源：http://ubd.xingfuxueyuan.xyz

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ixp.xylfe.cn

[R08] 数值比较
来源：http://sya.smart0.xyz

if (( a > b )); then echo "a 更大"; fi
来源：http://lij.fengsongda.top

[R09] 字符串比较
来源：http://spn.sufxvd.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://tpl.ehwqpu.com

[R10] 正则匹配
来源：http://qwc.wangshuangyany.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://cfn.smart0.xyz

[R11] case 多分支
来源：http://xwg.yuanzhike.top

case "$1" in
来源：http://jwp.daxiang520.top

start) echo "启动" ;;
来源：http://ckv.hcnkem.com

stop)  echo "停止" ;;
来源：http://lcn.nanxinkj.top

*)     echo "未知命令" ;;
来源：http://pni.smart0.xyz

esac
来源：http://ctn.ywan-chungtsiang.top

[R12] for 遍历文件
来源：http://eog.yj202588.top

for f in *.txt; do echo "$f"; done
来源：http://zny.shanyushiyangkeji.top

[R13] for 计数循环
来源：http://vct.gzhubu.top

for i in {1..10}; do echo "$i"; done
来源：http://bys.dashuyun.cn

[R14] C 风格 for
来源：http://upr.52xcode.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hkt.vehdjk.com

[R15] while 逐行读文件
来源：http://dub.hammf.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://nhl.hywenlv.cn

[R16] until 等待条件
来源：http://ovd.aizwys.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wtc.hammf.cn

[R17] 数组定义与取值
来源：http://aaa.aibaodan.cn

arr=(a b c); echo "${arr[0]}"
来源：http://iax.daxiang520.top

[R18] 遍历数组
来源：http://eon.fehbvm.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mwi.sufxvd.cn

[R19] 数组长度
来源：http://qws.xuetiantiany.cn

echo "${#arr[@]}"
来源：http://lzt.hysaishi.cn

[R20] 关联数组（字典）
来源：http://brr.tarul.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://nkd.gogol.net.cn

[R21] 字符串长度
来源：http://rut.c1oappe.top

echo "${#s}"
来源：http://mtk.dianchejie.cn

[R22] 截取子串
来源：http://ckr.zhengqikj.top

echo "${s:0:5}"
来源：http://hcs.havefunace.top

[R23] 字符串替换
来源：http://dvb.jianghu66.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://aau.cdnleiting.top

[R24] 大小写转换
来源：http://meh.fktsv.cn

echo "${s^^}"; echo "${s,,}"
来源：http://acn.fanxiaobao.xyz

[R25] 去后缀 / 去前缀
来源：http://phj.cucudq.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://haj.yuxming.cn

[R26] 命令替换
来源：http://ycb.zhaomingkeji.xyz

now=$(date +%F); echo "$now"
来源：http://enp.hfpthk.cn

[R27] 算术展开
来源：http://mjm.52xcode.cn

echo $((1 + 2 * 3))
来源：http://wtf.yanxiufei.cn

[R28] 浮点运算
来源：http://hqi.xinyue.icu

echo "scale=2; 10/3" | bc
来源：http://ese.yvedp.cn

[R29] 定义函数
来源：http://ipt.chenjidiqi.icu

add() { echo $(($1 + $2)); }; add 1 2
来源：http://imh.ppjwa.cn

[R30] 函数返回状态码
来源：http://bzj.shanyushiyangtech.top

f() { return 0; }; f || echo "失败了"
来源：http://ufb.jqgfzy.top

[R31] 局部变量
来源：http://zvd.yongpay.top

f() { local x=1; echo "$x"; }
来源：http://dof.yj20258.top

[R32] 参数个数校验
来源：http://xwl.jinqigufen.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://vjx.fengsongda.top

[R33] 捕获错误并提示行号
来源：http://gki.xuanzx.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://dsw.gaohongyu789.top

[R34] 退出时清理
来源：http://jma.feifeiyinyue.top

trap 'rm -f "$tmp"' EXIT
来源：http://oqo.gogol.net.cn

[R35] 后台执行并等待
来源：http://jti.xziqi.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ogz.bbcook.cn

[R36] 并发执行多个任务
来源：http://sxo.yonumen.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://kro.hesvh.cn

[R37] 把输出赋给变量
来源：http://ukk.tianlin.xyz

files=$(ls -1)
来源：http://yas.havefunace.top

[R38] 管道串联
来源：http://hms.shuidangran.top

cat a.txt | grep -i error | wc -l
来源：http://ttq.0kj1m.cn

[R39] 重定向标准输出与错误
来源：http://alv.gaohongyu789.top

cmd > out.log 2>&1
来源：http://awv.xinyue.icu

[R40] 追加写日志
来源：http://hea.sysykeji.top

echo "log" >> out.log
来源：http://yip.haohaochexian.top

[R41] 丢弃输出
来源：http://odl.epnwcf.com


<!-- 参考信息 -->