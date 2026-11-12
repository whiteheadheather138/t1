代发 wailian999

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://psc.daxiang520.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://kzs.xingfuxueyuan.xyz

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://vcj.zycfv.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://qno.fehbvm.com

================================================================================
来源：http://snj.meibo888.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://bua.yvedp.cn

================================================================================
来源：http://roy.sxryk.cn

[Q01] 创建表
来源：http://kby.uphjek.com

CREATE TABLE users (
来源：http://zrp.xinyue.icu

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://noa.c1oappe.top

name VARCHAR(50) NOT NULL,
来源：http://hhn.fanxiaobao.xyz

email VARCHAR(100) UNIQUE,
来源：http://jek.redwolf501.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ucs.zhongyouzk.top

);
来源：http://lji.hcnkem.com

[Q02] 创建带外键的表
来源：http://jua.xuetiantiany.cn

CREATE TABLE orders (
来源：http://oyw.shzxlz.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://dfn.zhoulong.xyz

user_id INT NOT NULL,
来源：http://sxk.nanxuanxn.top

amount DECIMAL(10, 2),
来源：http://thx.zdqjudy.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://tvq.shangyingyoupin.top

);
来源：http://ngh.chenzaomai.com

[Q03] 增加列
来源：http://jdp.gaohongyu789.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hdp.nwbrower.top

[Q04] 修改列类型
来源：http://dxq.haohaochexian.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://vkr.hfpthk.cn

[Q05] 重命名列
来源：http://jtu.pycfn.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://xxq.hcnkem.com

[Q06] 删除列
来源：http://wmk.fzhhl.top

ALTER TABLE users DROP COLUMN age;
来源：http://bzp.smart0.xyz

[Q07] 删除表
来源：http://rtc.fengsongda.top

DROP TABLE IF EXISTS orders;
来源：http://bkb.hcnkem.com

[Q08] 创建普通索引
来源：http://paw.hnqzz.top

CREATE INDEX idx_users_email ON users(email);
来源：http://tve.gogol.net.cn

[Q09] 创建唯一索引
来源：http://leq.fktsv.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://jcl.jinqigufen.top

[Q10] 插入单行
来源：http://fyr.nanxinkj.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://nkg.guowangkeji.top

[Q11] 一次插入多行
来源：http://buc.zhongyouzk.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://igg.fktsv.cn

[Q12] 插入后取自增 ID
来源：http://zfx.feifeiyinyue.top

INSERT INTO users (name) VALUES ('C');
来源：http://nti.jiagoushi.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wwu.zhoulong.xyz

[Q13] 忽略重复插入
来源：http://uox.nanxuanxn.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mnm.cheryme.top

[Q14] 存在则更新（upsert）
来源：http://aoo.nanxinkj.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ije.shangyingyoupin.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mvt.gotoacloud.top

[Q15] 查询全部
来源：http://ynk.ywan-chungtsiang.top

SELECT * FROM users;
来源：http://lyy.yuxming.cn

[Q16] 查询指定列
来源：http://yuq.zdqjudy.top

SELECT id, name FROM users;
来源：http://zsy.yonumen.top

[Q17] 条件查询
来源：http://vds.shzxlz.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://iti.jlsjyb.cn

[Q18] 模糊匹配
来源：http://lql.yueranfly.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://fvh.zhijiandao.cn

[Q19] 范围查询
来源：http://gzd.hesvh.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://oab.zdqjudy.top

[Q20] IN 列表
来源：http://che.gaohongyu789.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://xxg.daxiang520.top

[Q21] 空值判断
来源：http://yvy.jinyuanbaomall.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://dzv.zhixingplan.top

[Q22] 排序
来源：http://gza.yj202588.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://jjj.zhengqikj.top

[Q23] 分页
来源：http://ccr.zhengqikj.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://tox.ywan-chungtsiang.top

[Q24] 去重
来源：http://nld.hesvh.cn

SELECT DISTINCT city FROM users;
来源：http://adm.jlsjyb.cn

[Q25] 只取前 N 条
来源：http://wse.fengsongda.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ddo.meibo888.top

[Q26] 计数
来源：http://lpo.daria6918.cn

SELECT COUNT(*) FROM users;
来源：http://wtu.yongpay.top

[Q27] 条件计数
来源：http://vrn.jqgfzy.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://gny.guowangkeji.top

[Q28] 求和与平均
来源：http://bal.shanyushiyangtech.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wsy.wangdashe.top

[Q29] 最大最小值
来源：http://ooc.tianlin.xyz

SELECT MAX(age), MIN(age) FROM users;
来源：http://trx.0kj1m.cn

[Q30] 分组统计
来源：http://kul.zhongyouzk.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ief.hammf.cn

[Q31] 分组后过滤
来源：http://knp.tian-w.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://rxx.zhiwuduotai.top

[Q32] 分组拼接字符串
来源：http://kix.bbcook.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://nhc.shanyushiyangkeji.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://fps.ctjpmb.com

[Q33] 多列分组
来源：http://djl.yanxiufei.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://pzd.ppjwa.cn

[Q34] 每组取第一条
来源：http://bvg.tarul.cn

SELECT * FROM (
来源：http://fma.zhixingplan.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://faa.ivvv.top

) t WHERE rn = 1;
来源：http://pkr.shzxlz.cn

[Q35] 内连接
来源：http://lrt.hammf.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://xhk.zhaomingkeji.xyz

[Q36] 左连接
来源：http://bwm.xziqi.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ttp.52xcode.cn

[Q37] 右连接
来源：http://ino.fktsv.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://day.jqgfzy.top

[Q38] 全外连接（PostgreSQL）
来源：http://blo.yuanzhike.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://bzq.havefunace.top

[Q39] 自连接（查上下级）
来源：http://cfp.iojbl.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://gls.pycfn.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ree.jinqigufen.top

[Q40] 交叉连接（笛卡尔积）
来源：http://blh.yuanzhike.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://yuf.zhaomingkeji.xyz

[Q41] 多表连接
来源：http://tgj.yueranfly.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://yli.daria6918.cn

JOIN users u ON u.id = o.user_id
来源：http://rpx.9152youxi.cn

JOIN products p ON p.id = o.product_id;
来源：http://dpq.jinyuanbaomall.cn

[Q42] 连接条件附加过滤
来源：http://kyu.zhongyouzk.top

SELECT u.name, o.amount FROM users u
来源：http://wor.c1oappe.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://vfz.iojbl.cn

[Q43] 标量子查询
来源：http://kzh.yueranfly.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://rlu.nwbrower.top

[Q44] IN 子查询
来源：http://nsd.fengsongda.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://tix.jianghu66.top

[Q45] EXISTS 判断存在
来源：http://wak.shanyushiyangtech.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://lhb.xziqi.cn

[Q46] NOT EXISTS 判断不存在
来源：http://nhg.dianchejie.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bct.shanyushiyangtech.top

[Q47] 与平均值比较
来源：http://qrb.sjlbkw.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://nlw.0kj1m.cn

[Q48] CTE 公用表表达式
来源：http://wjd.yongpay.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://oqu.xinyue.icu

SELECT * FROM t WHERE c > 5;
来源：http://yih.snrcjt.cn

[Q49] 更新单行
来源：http://lga.xuanzx.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ddn.daria6918.cn

[Q50] 批量更新
来源：http://yel.mhx1999.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://yjw.nanxinkj.top

[Q51] 用子查询更新
来源：http://wax.hcnkem.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://sbe.jinqigfzy.top

[Q52] 删除指定行
来源：http://sgj.hysaishi.cn

DELETE FROM users WHERE id = 10;
来源：http://iuy.zhixingplan.top

[Q53] 按条件删除
来源：http://pgy.shanyushiyangtech.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://lee.ehwqpu.com

[Q54] 清空表
来源：http://sbg.kuanghao11.cn

TRUNCATE TABLE logs;
来源：http://sco.cashguo.top

[Q55] 排名（并列占位）
来源：http://ojm.fzhhl.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://jzm.tian-w.cn

[Q56] 密集排名（并列不占位）
来源：http://hzx.hfpthk.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://syk.zhijiandao.cn

[Q57] 行号
来源：http://uzl.chenlongwang.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://vls.ivvv.top

[Q58] 累计求和
来源：http://jde.uphjek.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://xss.yuxming.cn

[Q59] 分组内累计
来源：http://aql.9152youxi.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://jcd.cdnleiting.top

[Q60] 取上一行 / 下一行
来源：http://poy.bjfxy.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://qwn.zdqjudy.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ijq.bjfxy.top

[Q61] 移动平均
来源：http://dvn.guannengcc.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://vwe.hongshengwenyu.top

[Q62] 分组占比
来源：http://tta.cheryme.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://pom.hywenlv.cn

[Q63] 开启事务
来源：http://eiy.daxiang520.top

START TRANSACTION;                -- 或 BEGIN
来源：http://ovz.guannengcc.top

[Q64] 提交事务
来源：http://rqc.tian-w.cn

COMMIT;
来源：http://pck.meibo888.top

[Q65] 回滚事务
来源：http://upt.hnqzz.top

ROLLBACK;
来源：http://wyz.hongshengwenyu.top

[Q66] 行锁查询
来源：http://lzo.yueranfly.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mfx.ctjpmb.com

[Q67] 设置隔离级别
来源：http://jxd.shangyingyoupin.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mzr.xuanzx.com

[Q68] 保存点
来源：http://xjy.zhixingplan.top

SAVEPOINT sp1;
来源：http://hvp.cashguo.top

ROLLBACK TO sp1;
来源：http://oni.yangfankeji.com

[Q69] 查看执行计划
来源：http://ssi.tian-w.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://vcr.ywan-chungtsiang.top

[Q70] 更新统计信息
来源：http://xzq.hongshengwenyu.top

ANALYZE TABLE users;
来源：http://hmp.xylfe.cn

[Q71] 查看建表语句
来源：http://agd.kuanghao11.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://tuc.zhongyouzk.top

[Q72] 查看索引
来源：http://fec.shanyushiyangtech.top

SHOW INDEX FROM users;
来源：http://eol.xinyue.icu

[Q73] 查看表状态
来源：http://kac.jinqigufen.top

SHOW TABLE STATUS LIKE 'users';
来源：http://pof.yj20258888.top

[Q74] 强制使用索引
来源：http://toc.sjlbkw.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ngl.birdmap.top

[Q75] 日期格式化
来源：http://ljo.fanxiaobao.xyz

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mop.shangyingyoupin.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://lzl.tianlin.xyz

[Q76] 按天统计
来源：http://tbd.sweek.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://zxb.mhx1999.top

[Q77] 时间加减
来源：http://fmh.bbcook.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ilk.shuidangran.top

[Q78] 当前时间
来源：http://fby.jqgfzy.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://rdy.meibo888.top

[Q79] 字符串拼接
来源：http://gem.epnwcf.com

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://xey.pengpengdd.cyou

[Q80] 字符串截取
来源：http://mhf.wangdashe.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ydd.xingfuxueyuan.xyz

[Q81] 字符串替换
来源：http://iyn.jinyuanbaomall.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mdt.yj202588.top

[Q82] 字符长度与字节长度
来源：http://cfz.ehwqpu.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://qwz.quarkkingdee.top

[Q83] 大小写转换
来源：http://iwj.wangdashe.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://qlb.jianghu66.top

[Q84] 去除首尾空格
来源：http://yvp.jqgfzy.top

SELECT TRIM(name) FROM users;
来源：http://cyy.jianghu66.top

[Q85] 数值取整
来源：http://pmp.zhoulong.xyz

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://qve.wangshuangyany.cn

[Q86] 读取 JSON 字段
来源：http://jxb.tarul.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://bmv.zhaomingkeji.xyz

[Q87] JSON 字段做条件
来源：http://oko.zhaomingkeji.xyz

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://grl.svipenyu.cn

[Q88] 行转列（条件聚合）
来源：http://dlo.hnqzz.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://clu.aibaodan.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://gyz.smart0.xyz

[Q89] 判断表是否存在
来源：http://dfe.zhijiandao.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://fzo.xinyue.icu

[Q90] 生成序号列
来源：http://pre.zhijiandao.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://edp.shanyushiyangkeji.top

================================================================================
来源：http://gly.ydzc1.top

R. Bash 专题
来源：http://ith.yuanzhike.top

================================================================================
来源：http://epz.0kj1m.cn

[R01] shebang 与严格模式
来源：http://zcq.yangfankeji.com

#!/usr/bin/env bash
来源：http://ddy.jinghuilouyu.cn

set -euo pipefail
来源：http://onr.shanyushiyangkeji.top

[R02] 变量赋值与使用
来源：http://npt.yj20258.top

name="Tom"; echo "$name"
来源：http://crk.svipenyu.cn

[R03] 只读变量
来源：http://lcw.shanyushiyangtech.top

readonly PI=3.14
来源：http://vex.jyoumei.cn

[R04] 位置参数
来源：http://pqf.tianlin.xyz

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://aev.ctjpmb.com

[R05] 参数默认值
来源：http://uck.cqqwz.cn

name="${1:-default}"
来源：http://cko.sjlbkw.cn

[R06] 判断命令是否存在
来源：http://fvc.yangfankeji.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://urw.xylfe.cn

[R07] if 判断文件
来源：http://oab.jiagoushi.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://bme.epnwcf.com

[R08] 数值比较
来源：http://qxg.havefunace.top

if (( a > b )); then echo "a 更大"; fi
来源：http://klb.jiagoushi.top

[R09] 字符串比较
来源：http://icr.fehbvm.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://bpg.zhoulong.xyz

[R10] 正则匹配
来源：http://xst.kuanghao11.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://asl.shzxlz.cn

[R11] case 多分支
来源：http://idk.yj20258888.top

case "$1" in
来源：http://eqs.ywan-chungtsiang.top

start) echo "启动" ;;
来源：http://moc.hfpthk.cn

stop)  echo "停止" ;;
来源：http://oyi.zhaomingkeji.xyz

*)     echo "未知命令" ;;
来源：http://cpk.jianghu66.top

esac
来源：http://inl.xuetiantiany.cn

[R12] for 遍历文件
来源：http://ffg.nanxuanxn.top

for f in *.txt; do echo "$f"; done
来源：http://jns.redwolf501.top

[R13] for 计数循环
来源：http://bkq.ivvv.top

for i in {1..10}; do echo "$i"; done
来源：http://bnd.hesvh.cn

[R14] C 风格 for
来源：http://qng.yanxiufei.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://gvt.gogol.net.cn

[R15] while 逐行读文件
来源：http://ofv.quarkkingdee.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ezr.wangdashe.top

[R16] until 等待条件
来源：http://rvy.nanxinkj.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hmj.chenzaomai.com

[R17] 数组定义与取值
来源：http://feb.zhaomingkeji.xyz

arr=(a b c); echo "${arr[0]}"
来源：http://fty.zdqjudy.top

[R18] 遍历数组
来源：http://pyj.kuanghao11.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://esh.hywenlv.cn

[R19] 数组长度
来源：http://okw.jqgfzy.top

echo "${#arr[@]}"
来源：http://bdu.yonumen.top

[R20] 关联数组（字典）
来源：http://ukw.ppjwa.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://trf.fktsv.cn

[R21] 字符串长度
来源：http://uea.pengpengdd.cyou

echo "${#s}"
来源：http://eha.shzxlz.cn

[R22] 截取子串
来源：http://kfk.0kj1m.cn

echo "${s:0:5}"
来源：http://iua.sufxvd.cn

[R23] 字符串替换
来源：http://fjs.jinqigfzy.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hke.nanxinkj.top

[R24] 大小写转换
来源：http://acf.9152youxi.cn

echo "${s^^}"; echo "${s,,}"
来源：http://iet.epnwcf.com

[R25] 去后缀 / 去前缀
来源：http://hlf.yfazqb.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://vfx.pengpengdd.cyou

[R26] 命令替换
来源：http://jhs.uphjek.com

now=$(date +%F); echo "$now"
来源：http://mty.nanxinkj.top

[R27] 算术展开
来源：http://agq.epnwcf.com

echo $((1 + 2 * 3))
来源：http://szl.yueranfly.top

[R28] 浮点运算
来源：http://npq.yonumen.top

echo "scale=2; 10/3" | bc
来源：http://sba.jyoumei.cn

[R29] 定义函数
来源：http://abi.svipenyu.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://vtl.wangshuangyany.cn

[R30] 函数返回状态码
来源：http://viq.zhongyouzk.top

f() { return 0; }; f || echo "失败了"
来源：http://wnn.yj202588.top

[R31] 局部变量
来源：http://oku.pengpengdd.cyou

f() { local x=1; echo "$x"; }
来源：http://igp.sxryk.cn

[R32] 参数个数校验
来源：http://jwg.hesvh.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://bbi.nanxinkj.top

[R33] 捕获错误并提示行号
来源：http://ldu.ydzc1.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://slo.nanxuanxn.top

[R34] 退出时清理
来源：http://olk.epnwcf.com

trap 'rm -f "$tmp"' EXIT
来源：http://vja.yj20258.top

[R35] 后台执行并等待
来源：http://szu.jinghuilouyu.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://uja.cdnleiting.top

[R36] 并发执行多个任务
来源：http://eny.shzxlz.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://eus.yvedp.cn

[R37] 把输出赋给变量
来源：http://rpw.epnwcf.com

files=$(ls -1)
来源：http://cgj.dashuyun.cn

[R38] 管道串联
来源：http://ixu.sweek.top

cat a.txt | grep -i error | wc -l
来源：http://gnh.yj202588.top

[R39] 重定向标准输出与错误
来源：http://lkx.quarkkingdee.top

cmd > out.log 2>&1
来源：http://isp.nanxuanxn.top

[R40] 追加写日志
来源：http://mdb.tian-w.cn

echo "log" >> out.log
来源：http://tym.sysykeji.top

[R41] 丢弃输出
来源：http://xvb.yj202588.top


<!-- 参考信息 -->