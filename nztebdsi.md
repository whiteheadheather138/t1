代发 wailian999

================================================================================
来源：http://mcz.dashuyun.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://yzq.ydjk.org.cn

================================================================================
来源：http://vwy.shzxlz.cn

[Q01] 创建表
来源：http://mzm.yonumen.top

CREATE TABLE users (
来源：http://dyf.ppjwa.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wuh.cashguo.top

name VARCHAR(50) NOT NULL,
来源：http://uxx.andypj.xyz

email VARCHAR(100) UNIQUE,
来源：http://tws.kuanghao11.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://qnx.aibaodan.cn

);
来源：http://fjj.zhiwuduotai.top

[Q02] 创建带外键的表
来源：http://vlv.sufxvd.cn

CREATE TABLE orders (
来源：http://uyq.feifeiyinyue.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://qot.316326.xyz

user_id INT NOT NULL,
来源：http://ewr.shuidangran.top

amount DECIMAL(10, 2),
来源：http://zgw.fehbvm.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://uol.guannengcc.top

);
来源：http://lrd.bbcook.cn

[Q03] 增加列
来源：http://mvv.yj20258.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://clf.daxiang520.top

[Q04] 修改列类型
来源：http://izo.mhx1999.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://zdu.xuetiantiany.cn

[Q05] 重命名列
来源：http://mrl.xuanzx.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://pnk.vqdsnc.cn

[Q06] 删除列
来源：http://igr.cdnleiting.top

ALTER TABLE users DROP COLUMN age;
来源：http://jej.ybcxt.top

[Q07] 删除表
来源：http://utm.meibo888.top

DROP TABLE IF EXISTS orders;
来源：http://vzt.fehbvm.com

[Q08] 创建普通索引
来源：http://gqu.sufxvd.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://fyp.ywan-chungtsiang.top

[Q09] 创建唯一索引
来源：http://zua.gzhubu.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://fga.epnwcf.com

[Q10] 插入单行
来源：http://wbb.dashuyun.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://fqf.zdqjudy.top

[Q11] 一次插入多行
来源：http://snf.yuxming.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://oyy.ydzc1.top

[Q12] 插入后取自增 ID
来源：http://zrf.jiagoushi.top

INSERT INTO users (name) VALUES ('C');
来源：http://qsq.gzhubu.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://afp.jlsjyb.cn

[Q13] 忽略重复插入
来源：http://fnr.sxryk.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://elr.vqdsnc.cn

[Q14] 存在则更新（upsert）
来源：http://rcu.jinqigufen.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://bqn.yanxiufei.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://laj.jiagoushi.top

[Q15] 查询全部
来源：http://ygd.ctjpmb.com

SELECT * FROM users;
来源：http://rzz.yuanzhike.top

[Q16] 查询指定列
来源：http://gdh.haohaochexian.top

SELECT id, name FROM users;
来源：http://lmh.vqdsnc.cn

[Q17] 条件查询
来源：http://atb.yvedp.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://yio.tarul.cn

[Q18] 模糊匹配
来源：http://xlk.vehdjk.com

SELECT * FROM users WHERE name LIKE '张%';
来源：http://lmw.hnxiangtu.top

[Q19] 范围查询
来源：http://ede.wangshuangyany.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://vtm.ybcxt.top

[Q20] IN 列表
来源：http://zqm.yj202588.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://iow.sjlbkw.cn

[Q21] 空值判断
来源：http://ghw.bjfxy.top

SELECT * FROM users WHERE email IS NULL;
来源：http://hev.fktsv.cn

[Q22] 排序
来源：http://zoi.wangshuangyany.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://aua.aibaodan.cn

[Q23] 分页
来源：http://axd.ydjk.org.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wyx.jqgufenzy.top

[Q24] 去重
来源：http://bll.jinghuilouyu.cn

SELECT DISTINCT city FROM users;
来源：http://fyn.ctjpmb.com

[Q25] 只取前 N 条
来源：http://afd.xziqi.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ooa.wangdashe.top

[Q26] 计数
来源：http://lni.yanxiufei.cn

SELECT COUNT(*) FROM users;
来源：http://dfh.haohaochexian.top

[Q27] 条件计数
来源：http://fvs.c1oappe.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ong.cheryme.top

[Q28] 求和与平均
来源：http://agg.hysaishi.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://iqg.vqdsnc.cn

[Q29] 最大最小值
来源：http://qub.zhaomingkeji.xyz

SELECT MAX(age), MIN(age) FROM users;
来源：http://olp.sjlbkw.cn

[Q30] 分组统计
来源：http://kwg.iojbl.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://gat.gogol.net.cn

[Q31] 分组后过滤
来源：http://pac.feifeiyinyue.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://nhf.haohaochexian.top

[Q32] 分组拼接字符串
来源：http://hul.ydjk.org.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://jgg.yfazqb.com

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://bgd.dianchejie.cn

[Q33] 多列分组
来源：http://hda.yj20258.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://dyv.jinqigfzy.top

[Q34] 每组取第一条
来源：http://coi.zhiwuduotai.top

SELECT * FROM (
来源：http://vyr.sufxvd.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://zll.sweek.top

) t WHERE rn = 1;
来源：http://oey.yj202588.top

[Q35] 内连接
来源：http://yly.shuidangran.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://duy.cqqwz.cn

[Q36] 左连接
来源：http://zcm.sjlbkw.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wwe.shangyingyoupin.top

[Q37] 右连接
来源：http://ytr.cucudq.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ntx.sweek.top

[Q38] 全外连接（PostgreSQL）
来源：http://bwo.jlsjyb.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://yhl.xuetiantiany.cn

[Q39] 自连接（查上下级）
来源：http://awl.ywan-chungtsiang.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://taf.yangfankeji.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://cme.cqqwz.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://npu.svipenyu.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://nqt.yangfankeji.com

[Q41] 多表连接
来源：http://dgt.cdnleiting.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://rcw.bjfxy.top

JOIN users u ON u.id = o.user_id
来源：http://ryb.zhaomingkeji.xyz

JOIN products p ON p.id = o.product_id;
来源：http://wor.cashguo.top

[Q42] 连接条件附加过滤
来源：http://fjl.jinghuilouyu.cn

SELECT u.name, o.amount FROM users u
来源：http://phc.pycfn.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://gtr.cucudq.cn

[Q43] 标量子查询
来源：http://fxw.aizwys.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://dih.guannengcc.top

[Q44] IN 子查询
来源：http://lil.fktsv.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://bcm.andypj.xyz

[Q45] EXISTS 判断存在
来源：http://jry.xuetiantiany.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xzk.zycfv.cn

[Q46] NOT EXISTS 判断不存在
来源：http://lbh.xuetiantiany.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ehb.shanyushiyangtech.top

[Q47] 与平均值比较
来源：http://gbs.sysykeji.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://gns.wangshuangyany.cn

[Q48] CTE 公用表表达式
来源：http://yvj.ivvv.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mpg.birdmap.top

SELECT * FROM t WHERE c > 5;
来源：http://htm.nanxuanxn.top

[Q49] 更新单行
来源：http://uub.zhengqikj.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mcd.dianchejie.cn

[Q50] 批量更新
来源：http://mxx.nwbrower.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://bkr.ydzc1.top

[Q51] 用子查询更新
来源：http://qrt.gzhubu.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://avl.hnqzz.top

[Q52] 删除指定行
来源：http://igv.ehwqpu.com

DELETE FROM users WHERE id = 10;
来源：http://jjy.dashuyun.cn

[Q53] 按条件删除
来源：http://wip.gaohongyu789.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://kth.yueranfly.top

[Q54] 清空表
来源：http://sfn.zhoulong.xyz

TRUNCATE TABLE logs;
来源：http://zis.dianchejie.cn

[Q55] 排名（并列占位）
来源：http://mrn.chenjidiqi.icu

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://aiq.chenzaomai.com

[Q56] 密集排名（并列不占位）
来源：http://mcw.shzxlz.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://nlw.daria6918.cn

[Q57] 行号
来源：http://ser.xylfe.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://iaw.xuetiantiany.cn

[Q58] 累计求和
来源：http://tsv.aibaodan.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://kdt.zhoulong.xyz

[Q59] 分组内累计
来源：http://mko.nanxinkj.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://fku.cucudq.cn

[Q60] 取上一行 / 下一行
来源：http://ohh.shanyushiyangtech.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://zpu.epnwcf.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ztx.daxiang520.top

[Q61] 移动平均
来源：http://sbt.hongshengwenyu.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://bcv.xziqi.cn

[Q62] 分组占比
来源：http://mdx.hesvh.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://lfh.yonumen.top

[Q63] 开启事务
来源：http://rex.yfazqb.com

START TRANSACTION;                -- 或 BEGIN
来源：http://pwq.shuidangran.top

[Q64] 提交事务
来源：http://cci.sufxvd.cn

COMMIT;
来源：http://qzw.mhx1999.top

[Q65] 回滚事务
来源：http://krx.hfpthk.cn

ROLLBACK;
来源：http://uiu.ehwqpu.com

[Q66] 行锁查询
来源：http://tlu.jqgufenzy.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://dsq.epnwcf.com

[Q67] 设置隔离级别
来源：http://lyl.zhiwuduotai.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://yce.havefunace.top

[Q68] 保存点
来源：http://umf.zhixingplan.top

SAVEPOINT sp1;
来源：http://rgh.316326.xyz

ROLLBACK TO sp1;
来源：http://gqv.zdbjq.cn

[Q69] 查看执行计划
来源：http://wve.sjlbkw.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://vhs.zhijiandao.cn

[Q70] 更新统计信息
来源：http://mcx.haohaochexian.top

ANALYZE TABLE users;
来源：http://cnv.cheryme.top

[Q71] 查看建表语句
来源：http://fox.tanke756.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://dzr.ydjk.org.cn

[Q72] 查看索引
来源：http://fhm.shzxlz.cn

SHOW INDEX FROM users;
来源：http://fva.shanyushiyangtech.top

[Q73] 查看表状态
来源：http://etk.ydzc1.top

SHOW TABLE STATUS LIKE 'users';
来源：http://mfg.sweek.top

[Q74] 强制使用索引
来源：http://srj.yuanzhike.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://tdh.jinghuilouyu.cn

[Q75] 日期格式化
来源：http://yqb.zhengqikj.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://bwo.yuanzhike.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://vtz.sjlbkw.cn

[Q76] 按天统计
来源：http://fkt.yuanzhike.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ecx.svipenyu.cn

[Q77] 时间加减
来源：http://fnw.yuxming.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://gyl.bjfxy.top

[Q78] 当前时间
来源：http://kza.snrcjt.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ydv.cucudq.cn

[Q79] 字符串拼接
来源：http://esi.fengsongda.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://bjl.chenlongwang.top

[Q80] 字符串截取
来源：http://rez.andypj.xyz

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://oil.zhiwuduotai.top

[Q81] 字符串替换
来源：http://xvv.fengsongda.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hub.chenlongwang.top

[Q82] 字符长度与字节长度
来源：http://tqx.xziqi.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://omw.shuidangran.top

[Q83] 大小写转换
来源：http://dqy.bjfxy.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wgc.chenlongwang.top

[Q84] 去除首尾空格
来源：http://jza.bbcook.cn

SELECT TRIM(name) FROM users;
来源：http://uwb.cucudq.cn

[Q85] 数值取整
来源：http://eti.yongpay.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://fkq.aizwys.cn

[Q86] 读取 JSON 字段
来源：http://rfc.ybcxt.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ftt.pycfn.com

[Q87] JSON 字段做条件
来源：http://qbf.ybcxt.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://aqn.aibaodan.cn

[Q88] 行转列（条件聚合）
来源：http://qmd.daria6918.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://kyt.sufxvd.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://tim.jqgfzy.top

[Q89] 判断表是否存在
来源：http://zsa.fktsv.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ijn.xinyue.icu

[Q90] 生成序号列
来源：http://yqb.chenjidiqi.icu

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://qhk.aibaodan.cn

================================================================================
来源：http://wky.cqqwz.cn

R. Bash 专题
来源：http://ykn.yuxming.cn

================================================================================
来源：http://mdl.jyoumei.cn

[R01] shebang 与严格模式
来源：http://urd.yuxming.cn

#!/usr/bin/env bash
来源：http://vyp.zdbjq.cn

set -euo pipefail
来源：http://vxm.shuidangran.top

[R02] 变量赋值与使用
来源：http://zhs.yongpay.top

name="Tom"; echo "$name"
来源：http://hgm.tianlin.xyz

[R03] 只读变量
来源：http://gzp.nanxuanxn.top

readonly PI=3.14
来源：http://uyt.316326.xyz

[R04] 位置参数
来源：http://scu.ivvv.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ibe.smart0.xyz

[R05] 参数默认值
来源：http://nse.chenzaomai.com

name="${1:-default}"
来源：http://ogx.cucudq.cn

[R06] 判断命令是否存在
来源：http://dsm.tarul.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wfc.shanyushiyangtech.top

[R07] if 判断文件
来源：http://ozt.hesvh.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://kcc.9152youxi.cn

[R08] 数值比较
来源：http://kgn.xuetiantiany.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://vwe.hywenlv.cn

[R09] 字符串比较
来源：http://blj.snrcjt.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://uyi.ydzc1.top

[R10] 正则匹配
来源：http://xlq.tian-w.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://spw.aizwys.cn

[R11] case 多分支
来源：http://dsy.chenjidiqi.icu

case "$1" in
来源：http://pga.hysaishi.cn

start) echo "启动" ;;
来源：http://bcw.aizwys.cn

stop)  echo "停止" ;;
来源：http://ayg.jinqigfzy.top

*)     echo "未知命令" ;;
来源：http://hhx.xuanzx.com

esac
来源：http://voz.chenjidiqi.icu

[R12] for 遍历文件
来源：http://ejw.sufxvd.cn

for f in *.txt; do echo "$f"; done
来源：http://meu.yvedp.cn

[R13] for 计数循环
来源：http://fbp.c1oappe.top

for i in {1..10}; do echo "$i"; done
来源：http://asm.andypj.xyz

[R14] C 风格 for
来源：http://gmj.yongpay.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://eul.hnqzz.top

[R15] while 逐行读文件
来源：http://tcr.zdbjq.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ahz.jinqigufen.top

[R16] until 等待条件
来源：http://uny.zhixingplan.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://azn.bbcook.cn

[R17] 数组定义与取值
来源：http://ags.yuanzhike.top

arr=(a b c); echo "${arr[0]}"
来源：http://wtc.zhoulong.xyz

[R18] 遍历数组
来源：http://mbk.feifeiyinyue.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://tce.shanyushiyangtech.top

[R19] 数组长度
来源：http://wnk.yuxming.cn

echo "${#arr[@]}"
来源：http://rgb.xuanzx.com

[R20] 关联数组（字典）
来源：http://koa.xziqi.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://zmb.zhixingplan.top

[R21] 字符串长度
来源：http://cpr.pycfn.com

echo "${#s}"
来源：http://uyv.xingfuxueyuan.xyz

[R22] 截取子串
来源：http://hox.jiagoushi.top

echo "${s:0:5}"
来源：http://mbi.ehwqpu.com

[R23] 字符串替换
来源：http://jzd.jqgufenzy.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mxj.epnwcf.com

[R24] 大小写转换
来源：http://tri.cqqwz.cn

echo "${s^^}"; echo "${s,,}"
来源：http://wkj.aibaodan.cn

[R25] 去后缀 / 去前缀
来源：http://vby.quarkkingdee.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://czf.daxiang520.top

[R26] 命令替换
来源：http://mjf.chenzaomai.com

now=$(date +%F); echo "$now"
来源：http://mni.shangyingyoupin.top

[R27] 算术展开
来源：http://vga.gotoacloud.top

echo $((1 + 2 * 3))
来源：http://ghh.316326.xyz

[R28] 浮点运算
来源：http://ylg.hfpthk.cn

echo "scale=2; 10/3" | bc
来源：http://ugz.gzhubu.top

[R29] 定义函数
来源：http://vnb.nanxuanxn.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://sbd.chenzaomai.com

[R30] 函数返回状态码
来源：http://plf.jinqigufen.top

f() { return 0; }; f || echo "失败了"
来源：http://lke.andypj.xyz

[R31] 局部变量
来源：http://tzf.cheryme.top

f() { local x=1; echo "$x"; }
来源：http://osm.zhongyouzk.top

[R32] 参数个数校验
来源：http://tsa.dianchejie.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://alo.hfpthk.cn

[R33] 捕获错误并提示行号
来源：http://fdu.dianchejie.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://esn.ctjpmb.com

[R34] 退出时清理
来源：http://phv.shangyingyoupin.top

trap 'rm -f "$tmp"' EXIT
来源：http://rpg.ywan-chungtsiang.top

[R35] 后台执行并等待
来源：http://zsu.gaohongyu789.top

sleep 5 & pid=$!; wait "$pid"
来源：http://zjh.jianghu66.top

[R36] 并发执行多个任务
来源：http://rlm.daxiang520.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hfu.hnxiangtu.top

[R37] 把输出赋给变量
来源：http://npq.jyoumei.cn

files=$(ls -1)
来源：http://tbc.c1oappe.top

[R38] 管道串联
来源：http://qph.haohaochexian.top

cat a.txt | grep -i error | wc -l
来源：http://ryr.fktsv.cn

[R39] 重定向标准输出与错误
来源：http://srz.jiagoushi.top

cmd > out.log 2>&1
来源：http://nim.redwolf501.top

[R40] 追加写日志
来源：http://ilx.yj20258.top

echo "log" >> out.log
来源：http://xad.ydzc1.top

[R41] 丢弃输出
来源：http://tzc.xuetiantiany.cn

cmd >/dev/null 2>&1
来源：http://xhw.xinyue.icu

[R42] 输入重定向
来源：http://vhz.ppjwa.cn

wc -l < a.txt
来源：http://szj.jqgfzy.top

[R43] 按名字查找文件
来源：http://wua.ctjpmb.com


<!-- 参考信息 -->