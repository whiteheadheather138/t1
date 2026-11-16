代发 wailian999

CREATE TABLE users (
来源：http://ili.zhoulong.xyz

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://jwe.fengsongda.top

name VARCHAR(50) NOT NULL,
来源：http://hhm.gaohongyu789.top

email VARCHAR(100) UNIQUE,
来源：http://obu.hammf.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mnt.ydjk.org.cn

);
来源：http://jgm.fengsongda.top

[Q02] 创建带外键的表
来源：http://fev.cqqwz.cn

CREATE TABLE orders (
来源：http://fhw.gaohongyu789.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://afx.daria6918.cn

user_id INT NOT NULL,
来源：http://ijz.hammf.cn

amount DECIMAL(10, 2),
来源：http://pxf.yueranfly.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ewo.yonumen.top

);
来源：http://udr.zhiwuduotai.top

[Q03] 增加列
来源：http://ehq.yongpay.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mnd.bjfxy.top

[Q04] 修改列类型
来源：http://kpm.fzhhl.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://bdw.aibaodan.cn

[Q05] 重命名列
来源：http://nuc.316326.xyz

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://xnc.nanxuanxn.top

[Q06] 删除列
来源：http://fcg.ivvv.top

ALTER TABLE users DROP COLUMN age;
来源：http://dbt.yangfankeji.com

[Q07] 删除表
来源：http://zww.hcnkem.com

DROP TABLE IF EXISTS orders;
来源：http://fbt.zycfv.cn

[Q08] 创建普通索引
来源：http://rlz.aizwys.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://wro.zdqjudy.top

[Q09] 创建唯一索引
来源：http://nne.shanyushiyangkeji.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://tju.yanxiufei.cn

[Q10] 插入单行
来源：http://phb.nwbrower.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://pqf.ehwqpu.com

[Q11] 一次插入多行
来源：http://xzh.feifeiyinyue.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://qes.sweek.top

[Q12] 插入后取自增 ID
来源：http://ewu.cucudq.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ojz.fktsv.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ogk.shangyingyoupin.top

[Q13] 忽略重复插入
来源：http://uko.yfazqb.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ejp.ivvv.top

[Q14] 存在则更新（upsert）
来源：http://hqt.chenjidiqi.icu

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://iux.havefunace.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://nzr.gaohongyu789.top

[Q15] 查询全部
来源：http://qrw.kuanghao11.cn

SELECT * FROM users;
来源：http://ksn.yongpay.top

[Q16] 查询指定列
来源：http://hpx.uphjek.com

SELECT id, name FROM users;
来源：http://ial.yj202588.top

[Q17] 条件查询
来源：http://fqx.hammf.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://umi.gzhubu.top

[Q18] 模糊匹配
来源：http://okv.gaohongyu789.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ttw.feifeiyinyue.top

[Q19] 范围查询
来源：http://obd.guannengcc.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ggy.bbcook.cn

[Q20] IN 列表
来源：http://wim.fehbvm.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wqw.hywenlv.cn

[Q21] 空值判断
来源：http://yne.zhiwuduotai.top

SELECT * FROM users WHERE email IS NULL;
来源：http://imr.jinyuanbaomall.cn

[Q22] 排序
来源：http://rjq.pycfn.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://zhz.chenjidiqi.icu

[Q23] 分页
来源：http://oid.zdqjudy.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://fqc.dashuyun.cn

[Q24] 去重
来源：http://bry.cucudq.cn

SELECT DISTINCT city FROM users;
来源：http://oek.zhoulong.xyz

[Q25] 只取前 N 条
来源：http://nbd.xinyue.icu

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://fpd.vehdjk.com

[Q26] 计数
来源：http://dcf.yongpay.top

SELECT COUNT(*) FROM users;
来源：http://gns.yuxming.cn

[Q27] 条件计数
来源：http://roh.tanke756.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://egd.xylfe.cn

[Q28] 求和与平均
来源：http://ixp.yanxiufei.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://lii.ehwqpu.com

[Q29] 最大最小值
来源：http://kvk.xylfe.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ylh.hongshengwenyu.top

[Q30] 分组统计
来源：http://ojf.smart0.xyz

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://uzx.chenlongwang.top

[Q31] 分组后过滤
来源：http://mcr.guowangkeji.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ktv.iojbl.cn

[Q32] 分组拼接字符串
来源：http://bha.chenlongwang.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://zjn.jinghuilouyu.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://jsz.kuanghao11.cn

[Q33] 多列分组
来源：http://fzs.c1oappe.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://dvh.nanxuanxn.top

[Q34] 每组取第一条
来源：http://tse.bjfxy.top

SELECT * FROM (
来源：http://npo.redwolf501.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://gqj.shzxlz.cn

) t WHERE rn = 1;
来源：http://eko.meibo888.top

[Q35] 内连接
来源：http://dys.nanxinkj.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ern.tian-w.cn

[Q36] 左连接
来源：http://alt.chenlongwang.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://idx.tianlin.xyz

[Q37] 右连接
来源：http://yxr.gaohongyu789.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://qoc.sjlbkw.cn

[Q38] 全外连接（PostgreSQL）
来源：http://vns.ppjwa.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://xel.epnwcf.com

[Q39] 自连接（查上下级）
来源：http://axn.52xcode.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://mxi.0kj1m.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://eik.shangyingyoupin.top

[Q40] 交叉连接（笛卡尔积）
来源：http://ggs.gzhubu.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://vxo.gotoacloud.top

[Q41] 多表连接
来源：http://ozy.vehdjk.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://nrt.kuanghao11.cn

JOIN users u ON u.id = o.user_id
来源：http://rgk.yfazqb.com

JOIN products p ON p.id = o.product_id;
来源：http://oak.shuidangran.top

[Q42] 连接条件附加过滤
来源：http://njn.redwolf501.top

SELECT u.name, o.amount FROM users u
来源：http://pcb.316326.xyz

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://eeb.pycfn.com

[Q43] 标量子查询
来源：http://qya.sysykeji.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://bsf.chenlongwang.top

[Q44] IN 子查询
来源：http://wwd.kuanghao11.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://rke.yangfankeji.com

[Q45] EXISTS 判断存在
来源：http://jrg.sjlbkw.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xns.zycfv.cn

[Q46] NOT EXISTS 判断不存在
来源：http://abg.pengpengdd.cyou

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://klb.jlsjyb.cn

[Q47] 与平均值比较
来源：http://nzq.xinyue.icu

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://owq.tanke756.top

[Q48] CTE 公用表表达式
来源：http://klh.yuanzhike.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://pxo.aizwys.cn

SELECT * FROM t WHERE c > 5;
来源：http://brs.ydjk.org.cn

[Q49] 更新单行
来源：http://pho.chenlongwang.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://rgb.iojbl.cn

[Q50] 批量更新
来源：http://lxq.316326.xyz

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://cgt.hcnkem.com

[Q51] 用子查询更新
来源：http://fwu.0kj1m.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://jwg.aizwys.cn

[Q52] 删除指定行
来源：http://bcj.nwbrower.top

DELETE FROM users WHERE id = 10;
来源：http://tyw.feifeiyinyue.top

[Q53] 按条件删除
来源：http://gkx.zhixingplan.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://rdw.feifeiyinyue.top

[Q54] 清空表
来源：http://ksz.sweek.top

TRUNCATE TABLE logs;
来源：http://kip.sweek.top

[Q55] 排名（并列占位）
来源：http://zrg.andypj.xyz

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://lpz.fanxiaobao.xyz

[Q56] 密集排名（并列不占位）
来源：http://ebo.nanxinkj.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://fva.gaohongyu789.top

[Q57] 行号
来源：http://bte.nwbrower.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://zxa.bjfxy.top

[Q58] 累计求和
来源：http://qao.xinyue.icu

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://skv.zdbjq.cn

[Q59] 分组内累计
来源：http://opl.0kj1m.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://pza.zdbjq.cn

[Q60] 取上一行 / 下一行
来源：http://eoi.quarkkingdee.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://dlc.0kj1m.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://aot.xylfe.cn

[Q61] 移动平均
来源：http://qbu.cucudq.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://aso.andypj.xyz

[Q62] 分组占比
来源：http://rzb.ybcxt.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ijf.xziqi.cn

[Q63] 开启事务
来源：http://dqz.sjlbkw.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://kzr.xziqi.cn

[Q64] 提交事务
来源：http://tvf.mhx1999.top

COMMIT;
来源：http://oen.xingfuxueyuan.xyz

[Q65] 回滚事务
来源：http://iqq.cheryme.top

ROLLBACK;
来源：http://unu.ehwqpu.com

[Q66] 行锁查询
来源：http://avn.zhaomingkeji.xyz

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://cnw.feifeiyinyue.top

[Q67] 设置隔离级别
来源：http://dhg.xylfe.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://gow.xylfe.cn

[Q68] 保存点
来源：http://hpt.ivvv.top

SAVEPOINT sp1;
来源：http://uwi.yj20258888.top

ROLLBACK TO sp1;
来源：http://sst.snrcjt.cn

[Q69] 查看执行计划
来源：http://ytf.ehwqpu.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://tnr.jinqigfzy.top

[Q70] 更新统计信息
来源：http://glb.chenzaomai.com

ANALYZE TABLE users;
来源：http://vkr.zhaomingkeji.xyz

[Q71] 查看建表语句
来源：http://vzi.hywenlv.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://jaq.jinqigfzy.top

[Q72] 查看索引
来源：http://bju.shangyingyoupin.top

SHOW INDEX FROM users;
来源：http://etw.ctjpmb.com

[Q73] 查看表状态
来源：http://jdi.0kj1m.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://vla.pengpengdd.cyou

[Q74] 强制使用索引
来源：http://zmj.shanyushiyangkeji.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://yiu.meibo888.top

[Q75] 日期格式化
来源：http://npv.sjlbkw.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://znt.zhixingplan.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ncy.gzhubu.top

[Q76] 按天统计
来源：http://nxs.yangfankeji.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://xkz.shangyingyoupin.top

[Q77] 时间加减
来源：http://uqe.shanyushiyangkeji.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ppa.dashuyun.cn

[Q78] 当前时间
来源：http://rjq.epnwcf.com

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://jdz.ywan-chungtsiang.top

[Q79] 字符串拼接
来源：http://eka.mhx1999.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ico.tianlin.xyz

[Q80] 字符串截取
来源：http://bzn.bjfxy.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mkd.vqdsnc.cn

[Q81] 字符串替换
来源：http://azq.mhx1999.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ynv.ydzc1.top

[Q82] 字符长度与字节长度
来源：http://dga.ybcxt.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://tav.jinghuilouyu.cn

[Q83] 大小写转换
来源：http://gni.yangfankeji.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://jzw.dianchejie.cn

[Q84] 去除首尾空格
来源：http://efh.quarkkingdee.top

SELECT TRIM(name) FROM users;
来源：http://owo.ivvv.top

[Q85] 数值取整
来源：http://bum.chenjidiqi.icu

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://pax.yj20258888.top

[Q86] 读取 JSON 字段
来源：http://ygs.ivvv.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://psl.cqqwz.cn

[Q87] JSON 字段做条件
来源：http://wnq.hongshengwenyu.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://xkz.shangyingyoupin.top

[Q88] 行转列（条件聚合）
来源：http://wvr.yuanzhike.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://upp.shangyingyoupin.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://qwg.hnqzz.top

[Q89] 判断表是否存在
来源：http://spl.uphjek.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://nvb.zdbjq.cn

[Q90] 生成序号列
来源：http://qyi.guannengcc.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://sjr.tanke756.top

================================================================================
来源：http://bgn.cheryme.top

R. Bash 专题
来源：http://etw.yanxiufei.cn

================================================================================
来源：http://pxi.chenlongwang.top

[R01] shebang 与严格模式
来源：http://wcj.wangdashe.top

#!/usr/bin/env bash
来源：http://mnk.aizwys.cn

set -euo pipefail
来源：http://oze.jqgfzy.top

[R02] 变量赋值与使用
来源：http://xfb.wangshuangyany.cn

name="Tom"; echo "$name"
来源：http://wox.cucudq.cn

[R03] 只读变量
来源：http://tmn.chenzaomai.com

readonly PI=3.14
来源：http://ckd.meibo888.top

[R04] 位置参数
来源：http://lkx.tian-w.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://gqb.c1oappe.top

[R05] 参数默认值
来源：http://cwr.shzxlz.cn

name="${1:-default}"
来源：http://rxs.xuetiantiany.cn

[R06] 判断命令是否存在
来源：http://fkf.zhijiandao.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://dbh.zdqjudy.top

[R07] if 判断文件
来源：http://oly.birdmap.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ayd.yueranfly.top

[R08] 数值比较
来源：http://ytd.52xcode.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://xhc.yangfankeji.com

[R09] 字符串比较
来源：http://ylb.cdnleiting.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://trm.c1oappe.top

[R10] 正则匹配
来源：http://xsd.gzhubu.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://sey.yvedp.cn

[R11] case 多分支
来源：http://ytb.zhixingplan.top

case "$1" in
来源：http://etq.zhaomingkeji.xyz

start) echo "启动" ;;
来源：http://ttf.dianchejie.cn

stop)  echo "停止" ;;
来源：http://gqc.jinghuilouyu.cn

*)     echo "未知命令" ;;
来源：http://knt.zhiwuduotai.top

esac
来源：http://tru.jianghu66.top

[R12] for 遍历文件
来源：http://rbh.meibo888.top

for f in *.txt; do echo "$f"; done
来源：http://iig.jqgufenzy.top

[R13] for 计数循环
来源：http://mpz.sjlbkw.cn

for i in {1..10}; do echo "$i"; done
来源：http://nny.bjfxy.top

[R14] C 风格 for
来源：http://zwj.sysykeji.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://duc.zhongyouzk.top

[R15] while 逐行读文件
来源：http://xgy.9152youxi.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://yqb.zhiwuduotai.top

[R16] until 等待条件
来源：http://jcl.feifeiyinyue.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://whb.0kj1m.cn

[R17] 数组定义与取值
来源：http://mik.gaohongyu789.top

arr=(a b c); echo "${arr[0]}"
来源：http://ydo.gzhubu.top

[R18] 遍历数组
来源：http://rya.hysaishi.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://uot.svipenyu.cn

[R19] 数组长度
来源：http://wen.sweek.top

echo "${#arr[@]}"
来源：http://lrc.shangyingyoupin.top

[R20] 关联数组（字典）
来源：http://uzd.fzhhl.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://cpu.jlsjyb.cn

[R21] 字符串长度
来源：http://cad.xuanzx.com

echo "${#s}"
来源：http://edc.chenjidiqi.icu

[R22] 截取子串
来源：http://tci.jyoumei.cn

echo "${s:0:5}"
来源：http://cwa.smart0.xyz

[R23] 字符串替换
来源：http://oyr.gogol.net.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://tya.hnxiangtu.top

[R24] 大小写转换
来源：http://feq.fehbvm.com

echo "${s^^}"; echo "${s,,}"
来源：http://gia.yuanzhike.top

[R25] 去后缀 / 去前缀
来源：http://dgy.hysaishi.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://xbl.cheryme.top

[R26] 命令替换
来源：http://ggp.fktsv.cn

now=$(date +%F); echo "$now"
来源：http://lxk.pengpengdd.cyou

[R27] 算术展开
来源：http://cdp.pengpengdd.cyou

echo $((1 + 2 * 3))
来源：http://xzu.hfpthk.cn

[R28] 浮点运算
来源：http://chj.wangdashe.top

echo "scale=2; 10/3" | bc
来源：http://bvw.xingfuxueyuan.xyz

[R29] 定义函数
来源：http://xmn.52xcode.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://lnx.havefunace.top

[R30] 函数返回状态码
来源：http://fgm.zhixingplan.top

f() { return 0; }; f || echo "失败了"
来源：http://ile.fehbvm.com

[R31] 局部变量
来源：http://rkz.quarkkingdee.top

f() { local x=1; echo "$x"; }
来源：http://wxw.chenjidiqi.icu

[R32] 参数个数校验
来源：http://bpe.shangyingyoupin.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://chz.hammf.cn

[R33] 捕获错误并提示行号
来源：http://dvu.uphjek.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://eot.zhiwuduotai.top

[R34] 退出时清理
来源：http://rmg.chenzaomai.com

trap 'rm -f "$tmp"' EXIT
来源：http://nou.iojbl.cn

[R35] 后台执行并等待
来源：http://xyv.tian-w.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://luk.fehbvm.com

[R36] 并发执行多个任务
来源：http://yll.yj202588.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://zxt.zdqjudy.top

[R37] 把输出赋给变量
来源：http://sgl.0kj1m.cn

files=$(ls -1)
来源：http://nvr.sufxvd.cn

[R38] 管道串联
来源：http://ofs.sxryk.cn

cat a.txt | grep -i error | wc -l
来源：http://wdr.xinyue.icu

[R39] 重定向标准输出与错误
来源：http://vsg.yanxiufei.cn

cmd > out.log 2>&1
来源：http://aif.chenlongwang.top

[R40] 追加写日志
来源：http://ywn.jlsjyb.cn

echo "log" >> out.log
来源：http://wci.epnwcf.com

[R41] 丢弃输出
来源：http://klb.nwbrower.top

cmd >/dev/null 2>&1
来源：http://ixb.bjfxy.top

[R42] 输入重定向
来源：http://azc.daxiang520.top

wc -l < a.txt
来源：http://vpb.cashguo.top

[R43] 按名字查找文件
来源：http://lta.ywan-chungtsiang.top

find . -name "*.log" -type f
来源：http://jnr.fanxiaobao.xyz

[R44] 按修改时间查找
来源：http://dyl.0kj1m.cn

find . -mtime -7 -type f
来源：http://cqg.ivvv.top

[R45] 批量删除
来源：http://qyp.jqgfzy.top


<!-- 参考信息 -->