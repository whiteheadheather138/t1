代发 wailian999

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://fwu.hnqzz.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://qmu.hysaishi.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ktp.sufxvd.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://slz.chenzaomai.com

================================================================================
来源：http://xau.yangfankeji.com

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://sav.yongpay.top

================================================================================
来源：http://tfo.zhaomingkeji.xyz

[Q01] 创建表
来源：http://nsw.xuetiantiany.cn

CREATE TABLE users (
来源：http://xnr.fehbvm.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://xox.hesvh.cn

name VARCHAR(50) NOT NULL,
来源：http://azq.redwolf501.top

email VARCHAR(100) UNIQUE,
来源：http://pfv.yuanzhike.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://zna.ydzc1.top

);
来源：http://rwv.tanke756.top

[Q02] 创建带外键的表
来源：http://jzc.jinyuanbaomall.cn

CREATE TABLE orders (
来源：http://pzf.chenzaomai.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ypl.yuanzhike.top

user_id INT NOT NULL,
来源：http://zty.aibaodan.cn

amount DECIMAL(10, 2),
来源：http://zio.svipenyu.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://teg.jinyuanbaomall.cn

);
来源：http://hvb.hnxiangtu.top

[Q03] 增加列
来源：http://olu.hammf.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://zdu.zhijiandao.cn

[Q04] 修改列类型
来源：http://zwq.shuidangran.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://dwo.jlsjyb.cn

[Q05] 重命名列
来源：http://giu.yuxming.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://xii.ywan-chungtsiang.top

[Q06] 删除列
来源：http://ggn.quarkkingdee.top

ALTER TABLE users DROP COLUMN age;
来源：http://yxs.sjlbkw.cn

[Q07] 删除表
来源：http://nkp.jinqigufen.top

DROP TABLE IF EXISTS orders;
来源：http://vll.316326.xyz

[Q08] 创建普通索引
来源：http://cmc.chenzaomai.com

CREATE INDEX idx_users_email ON users(email);
来源：http://xgn.sweek.top

[Q09] 创建唯一索引
来源：http://tai.shanyushiyangkeji.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mdb.fengsongda.top

[Q10] 插入单行
来源：http://zha.nwbrower.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://czx.meibo888.top

[Q11] 一次插入多行
来源：http://xps.epnwcf.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://beg.pycfn.com

[Q12] 插入后取自增 ID
来源：http://eeo.daria6918.cn

INSERT INTO users (name) VALUES ('C');
来源：http://lra.yj202588.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://sok.ydzc1.top

[Q13] 忽略重复插入
来源：http://hxx.nanxinkj.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wss.zdqjudy.top

[Q14] 存在则更新（upsert）
来源：http://ryq.cheryme.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://lkc.gotoacloud.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ckr.jyoumei.cn

[Q15] 查询全部
来源：http://saz.quarkkingdee.top

SELECT * FROM users;
来源：http://wbz.birdmap.top

[Q16] 查询指定列
来源：http://pdf.vqdsnc.cn

SELECT id, name FROM users;
来源：http://rgo.cheryme.top

[Q17] 条件查询
来源：http://rbi.aizwys.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://iyc.tian-w.cn

[Q18] 模糊匹配
来源：http://frg.tanke756.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://djh.xziqi.cn

[Q19] 范围查询
来源：http://gru.wangshuangyany.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ezq.dashuyun.cn

[Q20] IN 列表
来源：http://ejp.uphjek.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ugq.nanxinkj.top

[Q21] 空值判断
来源：http://rgp.jinqigfzy.top

SELECT * FROM users WHERE email IS NULL;
来源：http://usr.jinqigufen.top

[Q22] 排序
来源：http://mrv.yj202588.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://utd.hongshengwenyu.top

[Q23] 分页
来源：http://hhl.jinqigfzy.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://jhd.shanyushiyangkeji.top

[Q24] 去重
来源：http://luz.tanke756.top

SELECT DISTINCT city FROM users;
来源：http://tua.0kj1m.cn

[Q25] 只取前 N 条
来源：http://sfv.wangdashe.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://chk.hammf.cn

[Q26] 计数
来源：http://fvu.jqgufenzy.top

SELECT COUNT(*) FROM users;
来源：http://znw.ppjwa.cn

[Q27] 条件计数
来源：http://ghw.yuanzhike.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://zyn.jinqigufen.top

[Q28] 求和与平均
来源：http://jmk.fehbvm.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://jci.tanke756.top

[Q29] 最大最小值
来源：http://yqs.hysaishi.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://bhf.uphjek.com

[Q30] 分组统计
来源：http://klj.zhaomingkeji.xyz

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://dah.ivvv.top

[Q31] 分组后过滤
来源：http://ojj.xingfuxueyuan.xyz

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ugo.hnxiangtu.top

[Q32] 分组拼接字符串
来源：http://qrb.jinyuanbaomall.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://yqu.vqdsnc.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://gsm.snrcjt.cn

[Q33] 多列分组
来源：http://jzq.guannengcc.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mcx.redwolf501.top

[Q34] 每组取第一条
来源：http://xzd.zhengqikj.top

SELECT * FROM (
来源：http://gex.hammf.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://gwo.jyoumei.cn

) t WHERE rn = 1;
来源：http://dbp.zhixingplan.top

[Q35] 内连接
来源：http://spb.jiagoushi.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://vbd.chenlongwang.top

[Q36] 左连接
来源：http://qib.hysaishi.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://itz.ybcxt.top

[Q37] 右连接
来源：http://nli.zhiwuduotai.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://agk.jinqigufen.top

[Q38] 全外连接（PostgreSQL）
来源：http://agl.meibo888.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://zrd.xinyue.icu

[Q39] 自连接（查上下级）
来源：http://hmv.zhengqikj.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://bzn.zhiwuduotai.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://msn.ybcxt.top

[Q40] 交叉连接（笛卡尔积）
来源：http://xsz.pycfn.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://xyy.cheryme.top

[Q41] 多表连接
来源：http://oto.epnwcf.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://hhv.shuidangran.top

JOIN users u ON u.id = o.user_id
来源：http://vre.0kj1m.cn

JOIN products p ON p.id = o.product_id;
来源：http://isg.yfazqb.com

[Q42] 连接条件附加过滤
来源：http://ees.cheryme.top

SELECT u.name, o.amount FROM users u
来源：http://sxl.aizwys.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://abu.jqgfzy.top

[Q43] 标量子查询
来源：http://nhe.hfpthk.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://tku.52xcode.cn

[Q44] IN 子查询
来源：http://nqu.wangshuangyany.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://iwv.ppjwa.cn

[Q45] EXISTS 判断存在
来源：http://ylw.jianghu66.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vja.yueranfly.top

[Q46] NOT EXISTS 判断不存在
来源：http://jwq.chenlongwang.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://oyc.gaohongyu789.top

[Q47] 与平均值比较
来源：http://hre.sjlbkw.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://jrw.mhx1999.top

[Q48] CTE 公用表表达式
来源：http://urk.c1oappe.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://emv.xuanzx.com

SELECT * FROM t WHERE c > 5;
来源：http://www.yuxming.cn

[Q49] 更新单行
来源：http://ebt.shanyushiyangtech.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://vuh.shuidangran.top

[Q50] 批量更新
来源：http://hhz.tianlin.xyz

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://iuc.cqqwz.cn

[Q51] 用子查询更新
来源：http://nmw.ehwqpu.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://eeg.ctjpmb.com

[Q52] 删除指定行
来源：http://dkl.mhx1999.top

DELETE FROM users WHERE id = 10;
来源：http://clm.jqgufenzy.top

[Q53] 按条件删除
来源：http://irm.cheryme.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://pnd.xuetiantiany.cn

[Q54] 清空表
来源：http://psu.jianghu66.top

TRUNCATE TABLE logs;
来源：http://szh.ehwqpu.com

[Q55] 排名（并列占位）
来源：http://lpc.0kj1m.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://bjd.jqgfzy.top

[Q56] 密集排名（并列不占位）
来源：http://mbg.tianlin.xyz

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://kod.jianghu66.top

[Q57] 行号
来源：http://lwa.yuxming.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://jkd.birdmap.top

[Q58] 累计求和
来源：http://ewf.gogol.net.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ixe.ywan-chungtsiang.top

[Q59] 分组内累计
来源：http://djl.fktsv.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mir.wangshuangyany.cn

[Q60] 取上一行 / 下一行
来源：http://vts.chenzaomai.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://zod.wangdashe.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://taz.hfpthk.cn

[Q61] 移动平均
来源：http://jed.yuxming.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mkc.yangfankeji.com

[Q62] 分组占比
来源：http://nwv.hfpthk.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://duc.sjlbkw.cn

[Q63] 开启事务
来源：http://mqm.vehdjk.com

START TRANSACTION;                -- 或 BEGIN
来源：http://wfd.zhijiandao.cn

[Q64] 提交事务
来源：http://alr.dianchejie.cn

COMMIT;
来源：http://tsi.shanyushiyangtech.top

[Q65] 回滚事务
来源：http://sqo.gaohongyu789.top

ROLLBACK;
来源：http://rtr.cashguo.top

[Q66] 行锁查询
来源：http://acz.gogol.net.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hzv.xingfuxueyuan.xyz

[Q67] 设置隔离级别
来源：http://gli.xuanzx.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://btq.redwolf501.top

[Q68] 保存点
来源：http://lxd.jianghu66.top

SAVEPOINT sp1;
来源：http://mms.nanxuanxn.top

ROLLBACK TO sp1;
来源：http://zct.yongpay.top

[Q69] 查看执行计划
来源：http://qlm.sweek.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://qey.fktsv.cn

[Q70] 更新统计信息
来源：http://luw.zhijiandao.cn

ANALYZE TABLE users;
来源：http://ajz.hywenlv.cn

[Q71] 查看建表语句
来源：http://imz.zhoulong.xyz

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://niz.pengpengdd.cyou

[Q72] 查看索引
来源：http://ffy.sjlbkw.cn

SHOW INDEX FROM users;
来源：http://sxf.yj20258888.top

[Q73] 查看表状态
来源：http://ywr.pycfn.com

SHOW TABLE STATUS LIKE 'users';
来源：http://svs.yj202588.top

[Q74] 强制使用索引
来源：http://gqz.zhijiandao.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://rcm.mhx1999.top

[Q75] 日期格式化
来源：http://vkw.yongpay.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://nzy.zdqjudy.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://yjc.tarul.cn

[Q76] 按天统计
来源：http://mzk.zhaomingkeji.xyz

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://doj.nwbrower.top

[Q77] 时间加减
来源：http://gic.zdqjudy.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://qcv.wangshuangyany.cn

[Q78] 当前时间
来源：http://ibc.tian-w.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://aez.gzhubu.top

[Q79] 字符串拼接
来源：http://irn.zhengqikj.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://duv.hammf.cn

[Q80] 字符串截取
来源：http://pic.haohaochexian.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://key.sufxvd.cn

[Q81] 字符串替换
来源：http://qof.jiagoushi.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://khr.guannengcc.top

[Q82] 字符长度与字节长度
来源：http://wue.zhixingplan.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ipo.xingfuxueyuan.xyz

[Q83] 大小写转换
来源：http://moe.52xcode.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://gtg.shanyushiyangkeji.top

[Q84] 去除首尾空格
来源：http://mua.andypj.xyz

SELECT TRIM(name) FROM users;
来源：http://pht.jiagoushi.top

[Q85] 数值取整
来源：http://gzu.cucudq.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://sek.iojbl.cn

[Q86] 读取 JSON 字段
来源：http://ejn.vehdjk.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ast.feifeiyinyue.top

[Q87] JSON 字段做条件
来源：http://yjt.gzhubu.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://vew.cdnleiting.top

[Q88] 行转列（条件聚合）
来源：http://qyj.svipenyu.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://zhr.jqgfzy.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://grv.cqqwz.cn

[Q89] 判断表是否存在
来源：http://wmj.nanxuanxn.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://dwy.vqdsnc.cn

[Q90] 生成序号列
来源：http://nyc.guannengcc.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://glf.aizwys.cn

================================================================================
来源：http://ocj.hesvh.cn

R. Bash 专题
来源：http://wti.jinqigufen.top

================================================================================
来源：http://cnu.9152youxi.cn

[R01] shebang 与严格模式
来源：http://yqi.fzhhl.top

#!/usr/bin/env bash
来源：http://svd.quarkkingdee.top

set -euo pipefail
来源：http://gut.zhaomingkeji.xyz

[R02] 变量赋值与使用
来源：http://lol.cdnleiting.top

name="Tom"; echo "$name"
来源：http://nlu.jqgufenzy.top

[R03] 只读变量
来源：http://poe.xinyue.icu

readonly PI=3.14
来源：http://tgr.cqqwz.cn

[R04] 位置参数
来源：http://fit.shangyingyoupin.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ndr.ppjwa.cn

[R05] 参数默认值
来源：http://hvt.shangyingyoupin.top

name="${1:-default}"
来源：http://ilr.ywan-chungtsiang.top

[R06] 判断命令是否存在
来源：http://gdn.aibaodan.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://dcs.zhoulong.xyz

[R07] if 判断文件
来源：http://eax.jinqigfzy.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://qix.fehbvm.com

[R08] 数值比较
来源：http://ipf.zdbjq.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ela.fzhhl.top

[R09] 字符串比较
来源：http://nyb.yanxiufei.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ssd.gotoacloud.top

[R10] 正则匹配
来源：http://cpm.xuetiantiany.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://lib.yfazqb.com

[R11] case 多分支
来源：http://kxg.yuanzhike.top

case "$1" in
来源：http://jxy.zdqjudy.top

start) echo "启动" ;;
来源：http://tye.smart0.xyz

stop)  echo "停止" ;;
来源：http://rya.svipenyu.cn

*)     echo "未知命令" ;;
来源：http://rmd.ydjk.org.cn

esac
来源：http://fyf.quarkkingdee.top

[R12] for 遍历文件
来源：http://vlc.sufxvd.cn

for f in *.txt; do echo "$f"; done
来源：http://bsz.ydzc1.top

[R13] for 计数循环
来源：http://nas.xinyue.icu

for i in {1..10}; do echo "$i"; done
来源：http://pqk.jinqigfzy.top

[R14] C 风格 for
来源：http://cil.shanyushiyangkeji.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ghd.chenzaomai.com

[R15] while 逐行读文件
来源：http://xxi.jyoumei.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mol.zhiwuduotai.top

[R16] until 等待条件
来源：http://mdz.hcnkem.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://lty.xuanzx.com

[R17] 数组定义与取值
来源：http://mbc.hnxiangtu.top

arr=(a b c); echo "${arr[0]}"
来源：http://txr.jinghuilouyu.cn

[R18] 遍历数组
来源：http://mjr.gotoacloud.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://snt.ctjpmb.com

[R19] 数组长度
来源：http://oni.zdqjudy.top

echo "${#arr[@]}"
来源：http://cmk.hongshengwenyu.top

[R20] 关联数组（字典）
来源：http://ewq.aizwys.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://cft.cashguo.top

[R21] 字符串长度
来源：http://sja.zhijiandao.cn

echo "${#s}"
来源：http://owb.zhaomingkeji.xyz

[R22] 截取子串
来源：http://czk.ydjk.org.cn

echo "${s:0:5}"
来源：http://fsu.hnqzz.top

[R23] 字符串替换
来源：http://ojx.zdbjq.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://eso.gzhubu.top

[R24] 大小写转换
来源：http://pqq.meibo888.top

echo "${s^^}"; echo "${s,,}"
来源：http://dcf.c1oappe.top

[R25] 去后缀 / 去前缀
来源：http://unw.sweek.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://zqs.chenlongwang.top

[R26] 命令替换
来源：http://kca.jlsjyb.cn

now=$(date +%F); echo "$now"
来源：http://mug.bjfxy.top

[R27] 算术展开
来源：http://mkw.sufxvd.cn

echo $((1 + 2 * 3))
来源：http://dnd.xingfuxueyuan.xyz

[R28] 浮点运算
来源：http://qty.yongpay.top

echo "scale=2; 10/3" | bc
来源：http://gic.gaohongyu789.top

[R29] 定义函数
来源：http://owt.sjlbkw.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ido.sjlbkw.cn

[R30] 函数返回状态码
来源：http://plr.hesvh.cn

f() { return 0; }; f || echo "失败了"
来源：http://nsx.fehbvm.com

[R31] 局部变量
来源：http://ytz.cqqwz.cn

f() { local x=1; echo "$x"; }
来源：http://luo.hnqzz.top

[R32] 参数个数校验
来源：http://hlc.chenzaomai.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ngw.c1oappe.top

[R33] 捕获错误并提示行号
来源：http://eoo.fanxiaobao.xyz

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ooh.jiagoushi.top

[R34] 退出时清理
来源：http://wvq.haohaochexian.top

trap 'rm -f "$tmp"' EXIT
来源：http://aue.cqqwz.cn

[R35] 后台执行并等待
来源：http://sqp.9152youxi.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://hsb.vehdjk.com

[R36] 并发执行多个任务
来源：http://mxg.9152youxi.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://gjo.daria6918.cn

[R37] 把输出赋给变量
来源：http://ftv.chenlongwang.top

files=$(ls -1)
来源：http://vec.shangyingyoupin.top

[R38] 管道串联
来源：http://fxe.ehwqpu.com

cat a.txt | grep -i error | wc -l
来源：http://tti.havefunace.top

[R39] 重定向标准输出与错误
来源：http://nyw.ybcxt.top

cmd > out.log 2>&1
来源：http://jei.bjfxy.top

[R40] 追加写日志
来源：http://fvo.sxryk.cn

echo "log" >> out.log
来源：http://hub.feifeiyinyue.top

[R41] 丢弃输出
来源：http://gcu.fzhhl.top


<!-- 参考信息 -->