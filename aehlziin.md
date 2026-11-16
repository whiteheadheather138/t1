代发 wailian999

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://giy.shuidangran.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://fji.pengpengdd.cyou

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://gsj.aizwys.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://zsl.316326.xyz

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://sik.cucudq.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mwp.ydzc1.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://lts.yj20258888.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://abz.yj20258.top

================================================================================
来源：http://fla.hywenlv.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ufn.c1oappe.top

================================================================================
来源：http://vts.shuidangran.top

[Q01] 创建表
来源：http://bls.yangfankeji.com

CREATE TABLE users (
来源：http://aqs.tanke756.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://gnj.wangdashe.top

name VARCHAR(50) NOT NULL,
来源：http://xve.xziqi.cn

email VARCHAR(100) UNIQUE,
来源：http://zyv.tianlin.xyz

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://myf.shuidangran.top

);
来源：http://nbf.shuidangran.top

[Q02] 创建带外键的表
来源：http://mrw.316326.xyz

CREATE TABLE orders (
来源：http://mdu.shuidangran.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://yha.ehwqpu.com

user_id INT NOT NULL,
来源：http://psk.zhijiandao.cn

amount DECIMAL(10, 2),
来源：http://lcz.shanyushiyangtech.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://qca.fanxiaobao.xyz

);
来源：http://fsp.yuxming.cn

[Q03] 增加列
来源：http://nvc.hfpthk.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wqg.yonumen.top

[Q04] 修改列类型
来源：http://pdf.yfazqb.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://xmb.havefunace.top

[Q05] 重命名列
来源：http://ekc.zhixingplan.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://bwc.daria6918.cn

[Q06] 删除列
来源：http://pzm.ehwqpu.com

ALTER TABLE users DROP COLUMN age;
来源：http://vtg.yvedp.cn

[Q07] 删除表
来源：http://hou.andypj.xyz

DROP TABLE IF EXISTS orders;
来源：http://hru.xingfuxueyuan.xyz

[Q08] 创建普通索引
来源：http://rtm.hesvh.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://pgd.hywenlv.cn

[Q09] 创建唯一索引
来源：http://oob.wangdashe.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://vfm.yangfankeji.com

[Q10] 插入单行
来源：http://txg.jlsjyb.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://zqe.nwbrower.top

[Q11] 一次插入多行
来源：http://ijl.cashguo.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://xcm.c1oappe.top

[Q12] 插入后取自增 ID
来源：http://ona.fanxiaobao.xyz

INSERT INTO users (name) VALUES ('C');
来源：http://mqi.zhongyouzk.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://daz.daria6918.cn

[Q13] 忽略重复插入
来源：http://exh.shanyushiyangkeji.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://eua.ydzc1.top

[Q14] 存在则更新（upsert）
来源：http://cys.sysykeji.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://lgu.fehbvm.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://oie.316326.xyz

[Q15] 查询全部
来源：http://urv.xuanzx.com

SELECT * FROM users;
来源：http://gzm.zhengqikj.top

[Q16] 查询指定列
来源：http://iej.zycfv.cn

SELECT id, name FROM users;
来源：http://fsz.guowangkeji.top

[Q17] 条件查询
来源：http://zcd.zhengqikj.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://znr.yj20258888.top

[Q18] 模糊匹配
来源：http://fgj.fehbvm.com

SELECT * FROM users WHERE name LIKE '张%';
来源：http://xjc.bbcook.cn

[Q19] 范围查询
来源：http://kvm.hfpthk.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://fhc.zycfv.cn

[Q20] IN 列表
来源：http://yzi.zhengqikj.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://oap.shzxlz.cn

[Q21] 空值判断
来源：http://hlx.fzhhl.top

SELECT * FROM users WHERE email IS NULL;
来源：http://onh.ybcxt.top

[Q22] 排序
来源：http://fpq.xylfe.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://vbm.xylfe.cn

[Q23] 分页
来源：http://yxa.xuanzx.com

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://dtu.nanxinkj.top

[Q24] 去重
来源：http://bgz.gotoacloud.top

SELECT DISTINCT city FROM users;
来源：http://bns.shuidangran.top

[Q25] 只取前 N 条
来源：http://uot.tianlin.xyz

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ezt.cdnleiting.top

[Q26] 计数
来源：http://upt.xingfuxueyuan.xyz

SELECT COUNT(*) FROM users;
来源：http://cny.ybcxt.top

[Q27] 条件计数
来源：http://zjf.ybcxt.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://zkj.birdmap.top

[Q28] 求和与平均
来源：http://sus.wangdashe.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://rkd.shuidangran.top

[Q29] 最大最小值
来源：http://cyh.zdbjq.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://lkz.jianghu66.top

[Q30] 分组统计
来源：http://jyb.hywenlv.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ntf.shuidangran.top

[Q31] 分组后过滤
来源：http://qwa.aibaodan.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://nlo.chenlongwang.top

[Q32] 分组拼接字符串
来源：http://spm.yj20258.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://nwq.hongshengwenyu.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://xhi.zhengqikj.top

[Q33] 多列分组
来源：http://diy.xuanzx.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mrz.haohaochexian.top

[Q34] 每组取第一条
来源：http://vwu.havefunace.top

SELECT * FROM (
来源：http://abu.svipenyu.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://qjo.bjfxy.top

) t WHERE rn = 1;
来源：http://jfn.daria6918.cn

[Q35] 内连接
来源：http://itd.hcnkem.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://vvm.fehbvm.com

[Q36] 左连接
来源：http://hbp.zhengqikj.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://alf.ydjk.org.cn

[Q37] 右连接
来源：http://hcq.jinqigufen.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://qcy.ivvv.top

[Q38] 全外连接（PostgreSQL）
来源：http://eww.pengpengdd.cyou

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://idh.quarkkingdee.top

[Q39] 自连接（查上下级）
来源：http://cno.zhiwuduotai.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://onw.ctjpmb.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://fdc.nwbrower.top

[Q40] 交叉连接（笛卡尔积）
来源：http://rlk.sysykeji.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ysn.yangfankeji.com

[Q41] 多表连接
来源：http://gtj.bjfxy.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://nwk.wangshuangyany.cn

JOIN users u ON u.id = o.user_id
来源：http://rrl.yj20258.top

JOIN products p ON p.id = o.product_id;
来源：http://fvw.guannengcc.top

[Q42] 连接条件附加过滤
来源：http://jay.hammf.cn

SELECT u.name, o.amount FROM users u
来源：http://rfu.snrcjt.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://pzk.chenzaomai.com

[Q43] 标量子查询
来源：http://sqt.yanxiufei.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://jbm.zhixingplan.top

[Q44] IN 子查询
来源：http://knw.ywan-chungtsiang.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://vuh.fengsongda.top

[Q45] EXISTS 判断存在
来源：http://def.ydjk.org.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://yqk.nanxuanxn.top

[Q46] NOT EXISTS 判断不存在
来源：http://pkh.dianchejie.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://iza.ctjpmb.com

[Q47] 与平均值比较
来源：http://aml.yj20258.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://sln.feifeiyinyue.top

[Q48] CTE 公用表表达式
来源：http://ryh.yueranfly.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://aon.zhixingplan.top

SELECT * FROM t WHERE c > 5;
来源：http://jkz.pengpengdd.cyou

[Q49] 更新单行
来源：http://tmd.shuidangran.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mky.chenzaomai.com

[Q50] 批量更新
来源：http://rtx.jiagoushi.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://jvd.cdnleiting.top

[Q51] 用子查询更新
来源：http://kkr.tanke756.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://fab.quarkkingdee.top

[Q52] 删除指定行
来源：http://ony.yueranfly.top

DELETE FROM users WHERE id = 10;
来源：http://cdi.uphjek.com

[Q53] 按条件删除
来源：http://hoe.hnqzz.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://vwn.fanxiaobao.xyz

[Q54] 清空表
来源：http://fil.fengsongda.top

TRUNCATE TABLE logs;
来源：http://wiq.wangdashe.top

[Q55] 排名（并列占位）
来源：http://njy.mhx1999.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://xfe.nanxuanxn.top

[Q56] 密集排名（并列不占位）
来源：http://emx.tianlin.xyz

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://iam.hesvh.cn

[Q57] 行号
来源：http://yqg.bbcook.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://edj.jinqigufen.top

[Q58] 累计求和
来源：http://mwy.yanxiufei.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://yjw.yangfankeji.com

[Q59] 分组内累计
来源：http://pma.svipenyu.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ajk.mhx1999.top

[Q60] 取上一行 / 下一行
来源：http://bhy.sjlbkw.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://cwc.nanxinkj.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://bzq.jinyuanbaomall.cn

[Q61] 移动平均
来源：http://eru.xingfuxueyuan.xyz

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ocj.fktsv.cn

[Q62] 分组占比
来源：http://dvu.yangfankeji.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://oco.hongshengwenyu.top

[Q63] 开启事务
来源：http://efw.wangshuangyany.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://qah.hongshengwenyu.top

[Q64] 提交事务
来源：http://xts.c1oappe.top

COMMIT;
来源：http://rwa.jinyuanbaomall.cn

[Q65] 回滚事务
来源：http://rqz.hysaishi.cn

ROLLBACK;
来源：http://aes.yonumen.top

[Q66] 行锁查询
来源：http://fiu.nwbrower.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://vfk.smart0.xyz

[Q67] 设置隔离级别
来源：http://pjk.birdmap.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://oiu.cdnleiting.top

[Q68] 保存点
来源：http://akq.zhengqikj.top

SAVEPOINT sp1;
来源：http://oze.cucudq.cn

ROLLBACK TO sp1;
来源：http://jqq.yfazqb.com

[Q69] 查看执行计划
来源：http://qsf.zycfv.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ktx.meibo888.top

[Q70] 更新统计信息
来源：http://esj.iojbl.cn

ANALYZE TABLE users;
来源：http://gcy.yangfankeji.com

[Q71] 查看建表语句
来源：http://zxl.sufxvd.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://bgk.jinqigfzy.top

[Q72] 查看索引
来源：http://erk.jinghuilouyu.cn

SHOW INDEX FROM users;
来源：http://mye.hesvh.cn

[Q73] 查看表状态
来源：http://yzh.shanyushiyangkeji.top

SHOW TABLE STATUS LIKE 'users';
来源：http://nbj.nanxinkj.top

[Q74] 强制使用索引
来源：http://qmf.ybcxt.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://njx.nanxinkj.top

[Q75] 日期格式化
来源：http://dzg.cdnleiting.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ppx.tanke756.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://kzw.jinyuanbaomall.cn

[Q76] 按天统计
来源：http://fad.zhijiandao.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://tfg.xuanzx.com

[Q77] 时间加减
来源：http://cfv.hammf.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://czc.hnqzz.top

[Q78] 当前时间
来源：http://utm.ydjk.org.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://pnq.tanke756.top

[Q79] 字符串拼接
来源：http://fpt.wangdashe.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://gto.cheryme.top

[Q80] 字符串截取
来源：http://shp.hysaishi.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://yif.tianlin.xyz

[Q81] 字符串替换
来源：http://jtb.chenjidiqi.icu

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://xkt.daria6918.cn

[Q82] 字符长度与字节长度
来源：http://wlj.yj20258888.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://xgr.316326.xyz

[Q83] 大小写转换
来源：http://cle.zhixingplan.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://lfj.hfpthk.cn

[Q84] 去除首尾空格
来源：http://wtj.ivvv.top

SELECT TRIM(name) FROM users;
来源：http://gnn.mhx1999.top

[Q85] 数值取整
来源：http://ndx.snrcjt.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://cxa.jinqigfzy.top

[Q86] 读取 JSON 字段
来源：http://eym.yvedp.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://lvs.jinghuilouyu.cn

[Q87] JSON 字段做条件
来源：http://mnw.yuanzhike.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mle.epnwcf.com

[Q88] 行转列（条件聚合）
来源：http://jjr.jlsjyb.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://uci.ywan-chungtsiang.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://dma.zycfv.cn

[Q89] 判断表是否存在
来源：http://arr.yj202588.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://gqw.svipenyu.cn

[Q90] 生成序号列
来源：http://ybs.aizwys.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://uss.zhongyouzk.top

================================================================================
来源：http://yhd.xuetiantiany.cn

R. Bash 专题
来源：http://dmj.pycfn.com

================================================================================
来源：http://jvd.yuanzhike.top

[R01] shebang 与严格模式
来源：http://wmd.xingfuxueyuan.xyz

#!/usr/bin/env bash
来源：http://duz.aizwys.cn

set -euo pipefail
来源：http://aan.yfazqb.com

[R02] 变量赋值与使用
来源：http://ijf.zhongyouzk.top

name="Tom"; echo "$name"
来源：http://edf.hesvh.cn

[R03] 只读变量
来源：http://vkp.yj202588.top

readonly PI=3.14
来源：http://sms.sysykeji.top

[R04] 位置参数
来源：http://xdz.feifeiyinyue.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://joo.xinyue.icu

[R05] 参数默认值
来源：http://keb.xingfuxueyuan.xyz

name="${1:-default}"
来源：http://jdc.fktsv.cn

[R06] 判断命令是否存在
来源：http://ihr.zhongyouzk.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://vyz.bjfxy.top

[R07] if 判断文件
来源：http://mcj.cdnleiting.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://khl.mhx1999.top

[R08] 数值比较
来源：http://pel.cdnleiting.top

if (( a > b )); then echo "a 更大"; fi
来源：http://zof.yvedp.cn

[R09] 字符串比较
来源：http://enz.shanyushiyangkeji.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://iyy.hnqzz.top

[R10] 正则匹配
来源：http://stm.ivvv.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://zsa.cashguo.top

[R11] case 多分支
来源：http://hst.andypj.xyz

case "$1" in
来源：http://wxv.chenjidiqi.icu

start) echo "启动" ;;
来源：http://uoc.fanxiaobao.xyz

stop)  echo "停止" ;;
来源：http://cvj.yvedp.cn

*)     echo "未知命令" ;;
来源：http://grj.tarul.cn

esac
来源：http://fdf.yvedp.cn

[R12] for 遍历文件
来源：http://bql.pycfn.com

for f in *.txt; do echo "$f"; done
来源：http://fdp.wangshuangyany.cn

[R13] for 计数循环
来源：http://arc.shzxlz.cn

for i in {1..10}; do echo "$i"; done
来源：http://mls.dashuyun.cn

[R14] C 风格 for
来源：http://xvy.meibo888.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ltq.xziqi.cn

[R15] while 逐行读文件
来源：http://ogv.hcnkem.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://yut.wangdashe.top

[R16] until 等待条件
来源：http://ttx.ydzc1.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://uwz.tianlin.xyz

[R17] 数组定义与取值
来源：http://gpo.guannengcc.top

arr=(a b c); echo "${arr[0]}"
来源：http://ced.dianchejie.cn

[R18] 遍历数组
来源：http://ius.zhaomingkeji.xyz

for x in "${arr[@]}"; do echo "$x"; done
来源：http://lxf.xingfuxueyuan.xyz

[R19] 数组长度
来源：http://fjg.guannengcc.top

echo "${#arr[@]}"
来源：http://dit.jinghuilouyu.cn

[R20] 关联数组（字典）
来源：http://rjk.aizwys.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://uem.yueranfly.top

[R21] 字符串长度
来源：http://dgb.pengpengdd.cyou

echo "${#s}"
来源：http://efb.jinyuanbaomall.cn

[R22] 截取子串
来源：http://iax.gogol.net.cn

echo "${s:0:5}"
来源：http://llk.chenzaomai.com

[R23] 字符串替换
来源：http://jxv.xinyue.icu

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://pbu.xuetiantiany.cn

[R24] 大小写转换
来源：http://qvj.shzxlz.cn

echo "${s^^}"; echo "${s,,}"
来源：http://job.nanxinkj.top

[R25] 去后缀 / 去前缀
来源：http://rbx.yfazqb.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://cba.cdnleiting.top

[R26] 命令替换
来源：http://riw.cashguo.top

now=$(date +%F); echo "$now"
来源：http://jkx.hesvh.cn

[R27] 算术展开
来源：http://udp.zhixingplan.top

echo $((1 + 2 * 3))
来源：http://ygg.zhiwuduotai.top

[R28] 浮点运算
来源：http://tpn.jinqigufen.top

echo "scale=2; 10/3" | bc
来源：http://qtt.tian-w.cn

[R29] 定义函数
来源：http://lcb.yj20258.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://axr.cdnleiting.top

[R30] 函数返回状态码
来源：http://lsa.fktsv.cn

f() { return 0; }; f || echo "失败了"
来源：http://mxg.hywenlv.cn

[R31] 局部变量
来源：http://nzy.jinghuilouyu.cn

f() { local x=1; echo "$x"; }
来源：http://zoj.hnqzz.top

[R32] 参数个数校验
来源：http://wgz.yj20258888.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ozx.aizwys.cn

[R33] 捕获错误并提示行号
来源：http://uet.daxiang520.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://lll.yj20258.top

[R34] 退出时清理
来源：http://shd.ctjpmb.com

trap 'rm -f "$tmp"' EXIT
来源：http://qvv.yuanzhike.top

[R35] 后台执行并等待
来源：http://vlh.jianghu66.top

sleep 5 & pid=$!; wait "$pid"
来源：http://htm.ydjk.org.cn

[R36] 并发执行多个任务
来源：http://euv.birdmap.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://duh.gaohongyu789.top

[R37] 把输出赋给变量
来源：http://deg.yfazqb.com

files=$(ls -1)
来源：http://yxm.xziqi.cn

[R38] 管道串联
来源：http://lka.gaohongyu789.top

cat a.txt | grep -i error | wc -l
来源：http://mti.yangfankeji.com

[R39] 重定向标准输出与错误
来源：http://sat.nanxuanxn.top


<!-- 参考信息 -->