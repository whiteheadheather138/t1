代发 wailian999

================================================================================
来源：http://nqj.yj202588.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baa.aibaodan.cn

================================================================================
来源：http://ide.sxryk.cn

[Q01] 创建表
来源：http://agy.shanyushiyangkeji.top

CREATE TABLE users (
来源：http://nqo.shzxlz.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://iyz.bjfxy.top

name VARCHAR(50) NOT NULL,
来源：http://nvw.smart0.xyz

email VARCHAR(100) UNIQUE,
来源：http://dlc.sufxvd.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://vry.nanxuanxn.top

);
来源：http://dri.sweek.top

[Q02] 创建带外键的表
来源：http://dax.9152youxi.cn

CREATE TABLE orders (
来源：http://tlz.daxiang520.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ewx.feifeiyinyue.top

user_id INT NOT NULL,
来源：http://kin.ppjwa.cn

amount DECIMAL(10, 2),
来源：http://hqg.guowangkeji.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://omb.shzxlz.cn

);
来源：http://nym.jinyuanbaomall.cn

[Q03] 增加列
来源：http://zzi.aizwys.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://aoq.kuanghao11.cn

[Q04] 修改列类型
来源：http://aza.xinyue.icu

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://utf.xziqi.cn

[Q05] 重命名列
来源：http://mch.feifeiyinyue.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://pda.yanxiufei.cn

[Q06] 删除列
来源：http://koh.zdqjudy.top

ALTER TABLE users DROP COLUMN age;
来源：http://uad.sysykeji.top

[Q07] 删除表
来源：http://yso.pengpengdd.cyou

DROP TABLE IF EXISTS orders;
来源：http://ult.jianghu66.top

[Q08] 创建普通索引
来源：http://cbr.meibo888.top

CREATE INDEX idx_users_email ON users(email);
来源：http://wkb.uphjek.com

[Q09] 创建唯一索引
来源：http://brm.bbcook.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://zmk.tian-w.cn

[Q10] 插入单行
来源：http://hoj.fengsongda.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://jxa.xingfuxueyuan.xyz

[Q11] 一次插入多行
来源：http://uwn.jqgfzy.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ezh.shangyingyoupin.top

[Q12] 插入后取自增 ID
来源：http://yjm.xinyue.icu

INSERT INTO users (name) VALUES ('C');
来源：http://thf.redwolf501.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://lir.zhijiandao.cn

[Q13] 忽略重复插入
来源：http://wnn.redwolf501.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://gsq.bjfxy.top

[Q14] 存在则更新（upsert）
来源：http://jax.bjfxy.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://msh.gaohongyu789.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://gns.sweek.top

[Q15] 查询全部
来源：http://tuh.zdqjudy.top

SELECT * FROM users;
来源：http://azx.yj202588.top

[Q16] 查询指定列
来源：http://auc.fengsongda.top

SELECT id, name FROM users;
来源：http://ukp.snrcjt.cn

[Q17] 条件查询
来源：http://tvn.aibaodan.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://zpz.jinyuanbaomall.cn

[Q18] 模糊匹配
来源：http://dfu.daria6918.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://lwo.yongpay.top

[Q19] 范围查询
来源：http://edh.yvedp.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ebz.fzhhl.top

[Q20] IN 列表
来源：http://vpi.haohaochexian.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://gwl.ivvv.top

[Q21] 空值判断
来源：http://oce.wangshuangyany.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://fmc.epnwcf.com

[Q22] 排序
来源：http://bkm.52xcode.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://pem.aizwys.cn

[Q23] 分页
来源：http://wed.zhixingplan.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://oht.ybcxt.top

[Q24] 去重
来源：http://kqp.guannengcc.top

SELECT DISTINCT city FROM users;
来源：http://kbx.wangshuangyany.cn

[Q25] 只取前 N 条
来源：http://wyd.chenlongwang.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://gnz.fanxiaobao.xyz

[Q26] 计数
来源：http://zmw.ivvv.top

SELECT COUNT(*) FROM users;
来源：http://llg.ybcxt.top

[Q27] 条件计数
来源：http://opt.sxryk.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hum.hesvh.cn

[Q28] 求和与平均
来源：http://wgh.fehbvm.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://xjp.smart0.xyz

[Q29] 最大最小值
来源：http://vva.pengpengdd.cyou

SELECT MAX(age), MIN(age) FROM users;
来源：http://gyy.yfazqb.com

[Q30] 分组统计
来源：http://ota.c1oappe.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://qps.yueranfly.top

[Q31] 分组后过滤
来源：http://tdv.fanxiaobao.xyz

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://jqo.smart0.xyz

[Q32] 分组拼接字符串
来源：http://xee.nwbrower.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://uyt.mhx1999.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://zsd.gzhubu.top

[Q33] 多列分组
来源：http://fnz.yonumen.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://iri.pycfn.com

[Q34] 每组取第一条
来源：http://mtu.chenzaomai.com

SELECT * FROM (
来源：http://qmi.gzhubu.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://qzw.snrcjt.cn

) t WHERE rn = 1;
来源：http://zfy.0kj1m.cn

[Q35] 内连接
来源：http://eai.haohaochexian.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://zyd.fehbvm.com

[Q36] 左连接
来源：http://syu.haohaochexian.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://uzf.yuanzhike.top

[Q37] 右连接
来源：http://ype.meibo888.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mfr.9152youxi.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ntb.vehdjk.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://jfd.gaohongyu789.top

[Q39] 自连接（查上下级）
来源：http://vcx.shanyushiyangkeji.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://ibe.iojbl.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://vgu.gogol.net.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ufm.chenzaomai.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://tri.feifeiyinyue.top

[Q41] 多表连接
来源：http://klz.cashguo.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://smm.uphjek.com

JOIN users u ON u.id = o.user_id
来源：http://uul.gogol.net.cn

JOIN products p ON p.id = o.product_id;
来源：http://ikq.yj202588.top

[Q42] 连接条件附加过滤
来源：http://cdb.ivvv.top

SELECT u.name, o.amount FROM users u
来源：http://aox.kuanghao11.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://gca.zhijiandao.cn

[Q43] 标量子查询
来源：http://ntz.daria6918.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://vac.aibaodan.cn

[Q44] IN 子查询
来源：http://pof.hnxiangtu.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://weq.hongshengwenyu.top

[Q45] EXISTS 判断存在
来源：http://vlb.gogol.net.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://onk.snrcjt.cn

[Q46] NOT EXISTS 判断不存在
来源：http://grv.pengpengdd.cyou

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://sxy.shangyingyoupin.top

[Q47] 与平均值比较
来源：http://opa.wangdashe.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://iga.ydjk.org.cn

[Q48] CTE 公用表表达式
来源：http://pbj.vehdjk.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://dmv.tanke756.top

SELECT * FROM t WHERE c > 5;
来源：http://tuh.c1oappe.top

[Q49] 更新单行
来源：http://owq.wangdashe.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://nbw.pycfn.com

[Q50] 批量更新
来源：http://cqp.hywenlv.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://jpf.sjlbkw.cn

[Q51] 用子查询更新
来源：http://yiz.shanyushiyangkeji.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://lds.smart0.xyz

[Q52] 删除指定行
来源：http://sin.hnxiangtu.top

DELETE FROM users WHERE id = 10;
来源：http://nfl.ydzc1.top

[Q53] 按条件删除
来源：http://uke.haohaochexian.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ghp.zhixingplan.top

[Q54] 清空表
来源：http://iep.cashguo.top

TRUNCATE TABLE logs;
来源：http://bso.jqgfzy.top

[Q55] 排名（并列占位）
来源：http://ogj.chenjidiqi.icu

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://nly.hcnkem.com

[Q56] 密集排名（并列不占位）
来源：http://mou.shzxlz.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://lqf.nanxuanxn.top

[Q57] 行号
来源：http://nma.yj20258888.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://rgf.hammf.cn

[Q58] 累计求和
来源：http://tyw.zdbjq.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hzn.guannengcc.top

[Q59] 分组内累计
来源：http://hvc.redwolf501.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://tfk.guannengcc.top

[Q60] 取上一行 / 下一行
来源：http://cly.zhoulong.xyz

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://pdb.nwbrower.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://dhn.zhoulong.xyz

[Q61] 移动平均
来源：http://hok.fehbvm.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ych.vehdjk.com

[Q62] 分组占比
来源：http://ogq.chenzaomai.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://pza.andypj.xyz

[Q63] 开启事务
来源：http://czt.shanyushiyangtech.top

START TRANSACTION;                -- 或 BEGIN
来源：http://zsv.fanxiaobao.xyz

[Q64] 提交事务
来源：http://mnl.jinqigufen.top

COMMIT;
来源：http://zzy.guannengcc.top

[Q65] 回滚事务
来源：http://fgx.aizwys.cn

ROLLBACK;
来源：http://bdr.guowangkeji.top

[Q66] 行锁查询
来源：http://wvc.zhongyouzk.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wdn.fengsongda.top

[Q67] 设置隔离级别
来源：http://nxl.smart0.xyz

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://qyr.uphjek.com

[Q68] 保存点
来源：http://xeo.shanyushiyangtech.top

SAVEPOINT sp1;
来源：http://sny.haohaochexian.top

ROLLBACK TO sp1;
来源：http://hnh.sxryk.cn

[Q69] 查看执行计划
来源：http://mzu.shangyingyoupin.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wfa.fehbvm.com

[Q70] 更新统计信息
来源：http://hvw.hysaishi.cn

ANALYZE TABLE users;
来源：http://lzw.tianlin.xyz

[Q71] 查看建表语句
来源：http://abl.chenzaomai.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://kgg.tian-w.cn

[Q72] 查看索引
来源：http://jts.shanyushiyangkeji.top

SHOW INDEX FROM users;
来源：http://cct.yfazqb.com

[Q73] 查看表状态
来源：http://yif.fzhhl.top

SHOW TABLE STATUS LIKE 'users';
来源：http://pee.yuxming.cn

[Q74] 强制使用索引
来源：http://hob.jianghu66.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://woi.yuanzhike.top

[Q75] 日期格式化
来源：http://wny.redwolf501.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://fja.fengsongda.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://syw.xuetiantiany.cn

[Q76] 按天统计
来源：http://uht.sjlbkw.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://cpq.yj202588.top

[Q77] 时间加减
来源：http://gpc.tian-w.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://qci.iojbl.cn

[Q78] 当前时间
来源：http://mgh.yueranfly.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ypi.9152youxi.cn

[Q79] 字符串拼接
来源：http://opj.uphjek.com

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ahw.guannengcc.top

[Q80] 字符串截取
来源：http://qxy.316326.xyz

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://pgc.smart0.xyz

[Q81] 字符串替换
来源：http://bap.zhaomingkeji.xyz

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://cfk.daria6918.cn

[Q82] 字符长度与字节长度
来源：http://gaj.chenzaomai.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://asc.cqqwz.cn

[Q83] 大小写转换
来源：http://vqh.ppjwa.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://yyn.mhx1999.top

[Q84] 去除首尾空格
来源：http://mpv.guowangkeji.top

SELECT TRIM(name) FROM users;
来源：http://oqo.9152youxi.cn

[Q85] 数值取整
来源：http://kcb.fanxiaobao.xyz

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://jei.sweek.top

[Q86] 读取 JSON 字段
来源：http://wxy.zhengqikj.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ubo.zhiwuduotai.top

[Q87] JSON 字段做条件
来源：http://sgn.yj20258888.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://qtr.tianlin.xyz

[Q88] 行转列（条件聚合）
来源：http://skt.yueranfly.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ygi.fengsongda.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://afa.fanxiaobao.xyz

[Q89] 判断表是否存在
来源：http://hjv.jinyuanbaomall.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://nnq.mhx1999.top

[Q90] 生成序号列
来源：http://frv.xylfe.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://nqu.birdmap.top

================================================================================
来源：http://cie.yj202588.top

R. Bash 专题
来源：http://iuo.daxiang520.top

================================================================================
来源：http://jxm.yongpay.top

[R01] shebang 与严格模式
来源：http://qlh.yangfankeji.com

#!/usr/bin/env bash
来源：http://xip.gogol.net.cn

set -euo pipefail
来源：http://ehd.jinqigfzy.top

[R02] 变量赋值与使用
来源：http://ezq.gaohongyu789.top

name="Tom"; echo "$name"
来源：http://obm.hongshengwenyu.top

[R03] 只读变量
来源：http://krg.daxiang520.top

readonly PI=3.14
来源：http://mum.fengsongda.top

[R04] 位置参数
来源：http://jkg.tanke756.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://yvk.zhixingplan.top

[R05] 参数默认值
来源：http://spf.xinyue.icu

name="${1:-default}"
来源：http://zdc.gogol.net.cn

[R06] 判断命令是否存在
来源：http://bfw.zhijiandao.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ccn.jinqigufen.top

[R07] if 判断文件
来源：http://oav.jinqigfzy.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://tca.tarul.cn

[R08] 数值比较
来源：http://tlr.ppjwa.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ydg.xingfuxueyuan.xyz

[R09] 字符串比较
来源：http://rok.sufxvd.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://cxn.hysaishi.cn

[R10] 正则匹配
来源：http://oql.pycfn.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ysq.birdmap.top

[R11] case 多分支
来源：http://ecb.epnwcf.com

case "$1" in
来源：http://ebq.epnwcf.com

start) echo "启动" ;;
来源：http://tml.tanke756.top

stop)  echo "停止" ;;
来源：http://mkk.xuetiantiany.cn

*)     echo "未知命令" ;;
来源：http://bgb.sufxvd.cn

esac
来源：http://pxg.yongpay.top

[R12] for 遍历文件
来源：http://xpc.jqgfzy.top

for f in *.txt; do echo "$f"; done
来源：http://dem.nanxinkj.top

[R13] for 计数循环
来源：http://edm.ehwqpu.com

for i in {1..10}; do echo "$i"; done
来源：http://tvr.guannengcc.top

[R14] C 风格 for
来源：http://vny.birdmap.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://uya.guowangkeji.top

[R15] while 逐行读文件
来源：http://puu.vehdjk.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://xwv.cucudq.cn

[R16] until 等待条件
来源：http://dgz.sxryk.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://kqq.fzhhl.top

[R17] 数组定义与取值
来源：http://nug.yuanzhike.top

arr=(a b c); echo "${arr[0]}"
来源：http://quk.yj202588.top

[R18] 遍历数组
来源：http://dwb.birdmap.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://qhv.jianghu66.top

[R19] 数组长度
来源：http://tod.shzxlz.cn

echo "${#arr[@]}"
来源：http://fqs.yuxming.cn

[R20] 关联数组（字典）
来源：http://hfp.zhaomingkeji.xyz

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://anl.guowangkeji.top

[R21] 字符串长度
来源：http://pwy.aibaodan.cn

echo "${#s}"
来源：http://omg.fanxiaobao.xyz

[R22] 截取子串
来源：http://eej.smart0.xyz

echo "${s:0:5}"
来源：http://ixq.ivvv.top

[R23] 字符串替换
来源：http://rfy.chenzaomai.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://tuc.svipenyu.cn

[R24] 大小写转换
来源：http://fai.jyoumei.cn

echo "${s^^}"; echo "${s,,}"
来源：http://idi.bbcook.cn

[R25] 去后缀 / 去前缀
来源：http://gsd.svipenyu.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://wvz.andypj.xyz

[R26] 命令替换
来源：http://tqy.chenzaomai.com

now=$(date +%F); echo "$now"
来源：http://aoy.jinghuilouyu.cn

[R27] 算术展开
来源：http://tal.havefunace.top

echo $((1 + 2 * 3))
来源：http://khp.sysykeji.top

[R28] 浮点运算
来源：http://mnb.zhiwuduotai.top

echo "scale=2; 10/3" | bc
来源：http://idb.ivvv.top

[R29] 定义函数
来源：http://gwa.ydzc1.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://xox.chenjidiqi.icu

[R30] 函数返回状态码
来源：http://ral.jinghuilouyu.cn

f() { return 0; }; f || echo "失败了"
来源：http://ywu.mhx1999.top

[R31] 局部变量
来源：http://gkv.feifeiyinyue.top

f() { local x=1; echo "$x"; }
来源：http://bzi.xuanzx.com

[R32] 参数个数校验
来源：http://dmo.jiagoushi.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://fys.ybcxt.top

[R33] 捕获错误并提示行号
来源：http://khm.bbcook.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://gxt.yvedp.cn

[R34] 退出时清理
来源：http://pbe.dianchejie.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ifo.birdmap.top

[R35] 后台执行并等待
来源：http://psd.zycfv.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://kvh.yongpay.top

[R36] 并发执行多个任务
来源：http://iif.tianlin.xyz

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://xmo.xuanzx.com

[R37] 把输出赋给变量
来源：http://zri.daria6918.cn

files=$(ls -1)
来源：http://tao.hnqzz.top

[R38] 管道串联
来源：http://ske.haohaochexian.top

cat a.txt | grep -i error | wc -l
来源：http://whz.shangyingyoupin.top

[R39] 重定向标准输出与错误
来源：http://cta.pengpengdd.cyou

cmd > out.log 2>&1
来源：http://bhr.havefunace.top

[R40] 追加写日志
来源：http://mwv.yj202588.top

echo "log" >> out.log
来源：http://xaj.zhoulong.xyz

[R41] 丢弃输出
来源：http://icd.cashguo.top

cmd >/dev/null 2>&1
来源：http://tte.pycfn.com

[R42] 输入重定向
来源：http://hut.bjfxy.top

wc -l < a.txt
来源：http://ogu.xziqi.cn

[R43] 按名字查找文件
来源：http://ukx.pycfn.com


<!-- 参考信息 -->