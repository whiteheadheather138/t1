代发 wailian999

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://eqn.hnqzz.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://zgg.nanxinkj.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://glm.jqgfzy.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ezz.cashguo.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://znq.xziqi.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://gxr.yj20258888.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://qkv.ybcxt.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://zwg.fktsv.cn

================================================================================
来源：http://qrb.52xcode.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://qxz.vehdjk.com

================================================================================
来源：http://inv.sufxvd.cn

[Q01] 创建表
来源：http://gdq.gzhubu.top

CREATE TABLE users (
来源：http://kkz.shanyushiyangtech.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ubf.havefunace.top

name VARCHAR(50) NOT NULL,
来源：http://efa.316326.xyz

email VARCHAR(100) UNIQUE,
来源：http://cza.wangshuangyany.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://zte.tarul.cn

);
来源：http://fod.svipenyu.cn

[Q02] 创建带外键的表
来源：http://ksp.zdbjq.cn

CREATE TABLE orders (
来源：http://puv.xuanzx.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ghs.yj20258888.top

user_id INT NOT NULL,
来源：http://rws.c1oappe.top

amount DECIMAL(10, 2),
来源：http://nzk.aizwys.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://qid.c1oappe.top

);
来源：http://bok.yanxiufei.cn

[Q03] 增加列
来源：http://akg.zhiwuduotai.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://lro.guannengcc.top

[Q04] 修改列类型
来源：http://nur.vqdsnc.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://kxq.yvedp.cn

[Q05] 重命名列
来源：http://yxr.daxiang520.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://poc.feifeiyinyue.top

[Q06] 删除列
来源：http://few.gzhubu.top

ALTER TABLE users DROP COLUMN age;
来源：http://csx.guowangkeji.top

[Q07] 删除表
来源：http://cqh.yfazqb.com

DROP TABLE IF EXISTS orders;
来源：http://vki.xylfe.cn

[Q08] 创建普通索引
来源：http://vlq.jinyuanbaomall.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://axn.tian-w.cn

[Q09] 创建唯一索引
来源：http://fze.gogol.net.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://nnn.xylfe.cn

[Q10] 插入单行
来源：http://jbm.hesvh.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://emh.jinqigfzy.top

[Q11] 一次插入多行
来源：http://jvz.gogol.net.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://otw.tian-w.cn

[Q12] 插入后取自增 ID
来源：http://jwu.ivvv.top

INSERT INTO users (name) VALUES ('C');
来源：http://twv.cucudq.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ncm.nwbrower.top

[Q13] 忽略重复插入
来源：http://tbx.epnwcf.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://nlx.ydjk.org.cn

[Q14] 存在则更新（upsert）
来源：http://vmq.hcnkem.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://zwr.sjlbkw.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://zsg.smart0.xyz

[Q15] 查询全部
来源：http://tym.wangdashe.top

SELECT * FROM users;
来源：http://kdt.epnwcf.com

[Q16] 查询指定列
来源：http://osf.zycfv.cn

SELECT id, name FROM users;
来源：http://fqv.tian-w.cn

[Q17] 条件查询
来源：http://mcs.yangfankeji.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://lhy.pengpengdd.cyou

[Q18] 模糊匹配
来源：http://htn.nwbrower.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://xrj.hysaishi.cn

[Q19] 范围查询
来源：http://cfl.shanyushiyangtech.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://qgf.uphjek.com

[Q20] IN 列表
来源：http://hie.chenjidiqi.icu

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://bra.vehdjk.com

[Q21] 空值判断
来源：http://eho.ywan-chungtsiang.top

SELECT * FROM users WHERE email IS NULL;
来源：http://iwu.hcnkem.com

[Q22] 排序
来源：http://jrm.gzhubu.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://nym.tianlin.xyz

[Q23] 分页
来源：http://nmi.sweek.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://lbm.andypj.xyz

[Q24] 去重
来源：http://cvw.zycfv.cn

SELECT DISTINCT city FROM users;
来源：http://ajh.wangdashe.top

[Q25] 只取前 N 条
来源：http://kqj.shzxlz.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://pwk.andypj.xyz

[Q26] 计数
来源：http://mws.cashguo.top

SELECT COUNT(*) FROM users;
来源：http://bzu.xuanzx.com

[Q27] 条件计数
来源：http://sos.vqdsnc.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mny.jyoumei.cn

[Q28] 求和与平均
来源：http://aqo.hnqzz.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://zaj.ydjk.org.cn

[Q29] 最大最小值
来源：http://drm.0kj1m.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://hun.yfazqb.com

[Q30] 分组统计
来源：http://vza.xziqi.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://opb.ydzc1.top

[Q31] 分组后过滤
来源：http://wwf.zhixingplan.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hmx.yongpay.top

[Q32] 分组拼接字符串
来源：http://ebx.jiagoushi.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://xay.sufxvd.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://vih.vehdjk.com

[Q33] 多列分组
来源：http://ueg.pengpengdd.cyou

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://pbe.yuxming.cn

[Q34] 每组取第一条
来源：http://zsu.jinghuilouyu.cn

SELECT * FROM (
来源：http://xvh.zhaomingkeji.xyz

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://kno.nwbrower.top

) t WHERE rn = 1;
来源：http://smp.nanxinkj.top

[Q35] 内连接
来源：http://nbn.aibaodan.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://erj.c1oappe.top

[Q36] 左连接
来源：http://tnk.ybcxt.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://tdp.fengsongda.top

[Q37] 右连接
来源：http://seu.haohaochexian.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://kux.chenzaomai.com

[Q38] 全外连接（PostgreSQL）
来源：http://zgg.jiagoushi.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wtc.zhengqikj.top

[Q39] 自连接（查上下级）
来源：http://juf.xuetiantiany.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://amb.xziqi.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ude.yj20258888.top

[Q40] 交叉连接（笛卡尔积）
来源：http://lvy.zhixingplan.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://jul.ctjpmb.com

[Q41] 多表连接
来源：http://dxs.yuanzhike.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://nas.birdmap.top

JOIN users u ON u.id = o.user_id
来源：http://bxx.epnwcf.com

JOIN products p ON p.id = o.product_id;
来源：http://dxx.andypj.xyz

[Q42] 连接条件附加过滤
来源：http://zha.epnwcf.com

SELECT u.name, o.amount FROM users u
来源：http://lqa.feifeiyinyue.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ofb.andypj.xyz

[Q43] 标量子查询
来源：http://sbp.jqgfzy.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://fhp.bjfxy.top

[Q44] IN 子查询
来源：http://vxu.fengsongda.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://obr.guannengcc.top

[Q45] EXISTS 判断存在
来源：http://uzw.xziqi.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://pjw.gogol.net.cn

[Q46] NOT EXISTS 判断不存在
来源：http://wet.zhijiandao.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://dgi.epnwcf.com

[Q47] 与平均值比较
来源：http://lvs.snrcjt.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://yqs.bjfxy.top

[Q48] CTE 公用表表达式
来源：http://foz.pengpengdd.cyou

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://dwm.gogol.net.cn

SELECT * FROM t WHERE c > 5;
来源：http://fvl.hongshengwenyu.top

[Q49] 更新单行
来源：http://dsa.shanyushiyangkeji.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://cdp.zhoulong.xyz

[Q50] 批量更新
来源：http://ght.hcnkem.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://dzd.zdbjq.cn

[Q51] 用子查询更新
来源：http://pdi.jinyuanbaomall.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://tow.haohaochexian.top

[Q52] 删除指定行
来源：http://imi.tian-w.cn

DELETE FROM users WHERE id = 10;
来源：http://uge.ivvv.top

[Q53] 按条件删除
来源：http://aqa.chenlongwang.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://pha.feifeiyinyue.top

[Q54] 清空表
来源：http://vdp.feifeiyinyue.top

TRUNCATE TABLE logs;
来源：http://zyi.ppjwa.cn

[Q55] 排名（并列占位）
来源：http://zda.ctjpmb.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ukp.hywenlv.cn

[Q56] 密集排名（并列不占位）
来源：http://qke.daxiang520.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ijb.xziqi.cn

[Q57] 行号
来源：http://heq.uphjek.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mbu.gogol.net.cn

[Q58] 累计求和
来源：http://dvw.yj202588.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://jhr.zhengqikj.top

[Q59] 分组内累计
来源：http://wgd.nwbrower.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://jjy.yueranfly.top

[Q60] 取上一行 / 下一行
来源：http://ifs.ybcxt.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://avk.gzhubu.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ayy.9152youxi.cn

[Q61] 移动平均
来源：http://iul.yj202588.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://jdf.zhengqikj.top

[Q62] 分组占比
来源：http://zyu.snrcjt.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://sfy.shanyushiyangkeji.top

[Q63] 开启事务
来源：http://two.daxiang520.top

START TRANSACTION;                -- 或 BEGIN
来源：http://hvl.havefunace.top

[Q64] 提交事务
来源：http://ogd.yj20258888.top

COMMIT;
来源：http://uox.cashguo.top

[Q65] 回滚事务
来源：http://zbw.zhengqikj.top

ROLLBACK;
来源：http://oef.feifeiyinyue.top

[Q66] 行锁查询
来源：http://vaf.yj20258888.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://aca.tarul.cn

[Q67] 设置隔离级别
来源：http://wvq.jinyuanbaomall.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://lhs.meibo888.top

[Q68] 保存点
来源：http://rci.yj20258888.top

SAVEPOINT sp1;
来源：http://zqg.cheryme.top

ROLLBACK TO sp1;
来源：http://aas.jiagoushi.top

[Q69] 查看执行计划
来源：http://itp.zhiwuduotai.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://apv.uphjek.com

[Q70] 更新统计信息
来源：http://vjm.hesvh.cn

ANALYZE TABLE users;
来源：http://bwj.havefunace.top

[Q71] 查看建表语句
来源：http://qtg.52xcode.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ukf.zhijiandao.cn

[Q72] 查看索引
来源：http://ckl.kuanghao11.cn

SHOW INDEX FROM users;
来源：http://gdq.jianghu66.top

[Q73] 查看表状态
来源：http://pub.aibaodan.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://jnu.bbcook.cn

[Q74] 强制使用索引
来源：http://kan.aibaodan.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://swa.pengpengdd.cyou

[Q75] 日期格式化
来源：http://egx.shangyingyoupin.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wfa.nanxuanxn.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://toa.chenzaomai.com

[Q76] 按天统计
来源：http://xqz.shanyushiyangtech.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hnh.guannengcc.top

[Q77] 时间加减
来源：http://hvu.yj202588.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://sju.9152youxi.cn

[Q78] 当前时间
来源：http://gph.bbcook.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://aur.9152youxi.cn

[Q79] 字符串拼接
来源：http://npl.vehdjk.com

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://yal.sufxvd.cn

[Q80] 字符串截取
来源：http://nht.xinyue.icu

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://cgr.gzhubu.top

[Q81] 字符串替换
来源：http://ygf.jinghuilouyu.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://lte.chenzaomai.com

[Q82] 字符长度与字节长度
来源：http://eja.svipenyu.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ouo.nanxinkj.top

[Q83] 大小写转换
来源：http://tbh.cashguo.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://skh.bjfxy.top

[Q84] 去除首尾空格
来源：http://qga.cqqwz.cn

SELECT TRIM(name) FROM users;
来源：http://byt.gogol.net.cn

[Q85] 数值取整
来源：http://kex.zycfv.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://brk.wangshuangyany.cn

[Q86] 读取 JSON 字段
来源：http://edx.52xcode.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ast.fanxiaobao.xyz

[Q87] JSON 字段做条件
来源：http://irr.zdbjq.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://kfs.fehbvm.com

[Q88] 行转列（条件聚合）
来源：http://jlq.smart0.xyz

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://uiw.chenlongwang.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://pav.dashuyun.cn

[Q89] 判断表是否存在
来源：http://uaw.pengpengdd.cyou

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://drl.yueranfly.top

[Q90] 生成序号列
来源：http://mmd.xuetiantiany.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ovy.ywan-chungtsiang.top

================================================================================
来源：http://cpz.shzxlz.cn

R. Bash 专题
来源：http://jvx.haohaochexian.top

================================================================================
来源：http://ulw.sysykeji.top

[R01] shebang 与严格模式
来源：http://rtg.wangdashe.top

#!/usr/bin/env bash
来源：http://klq.52xcode.cn

set -euo pipefail
来源：http://jju.bbcook.cn

[R02] 变量赋值与使用
来源：http://eey.xingfuxueyuan.xyz

name="Tom"; echo "$name"
来源：http://tys.ywan-chungtsiang.top

[R03] 只读变量
来源：http://jcd.tanke756.top

readonly PI=3.14
来源：http://tna.bjfxy.top

[R04] 位置参数
来源：http://xhl.ywan-chungtsiang.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://uqi.daxiang520.top

[R05] 参数默认值
来源：http://qls.shuidangran.top

name="${1:-default}"
来源：http://uxr.uphjek.com

[R06] 判断命令是否存在
来源：http://usr.feifeiyinyue.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wbi.yueranfly.top

[R07] if 判断文件
来源：http://wno.meibo888.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hvw.nwbrower.top

[R08] 数值比较
来源：http://pvt.meibo888.top

if (( a > b )); then echo "a 更大"; fi
来源：http://ljc.c1oappe.top

[R09] 字符串比较
来源：http://cyy.andypj.xyz

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://tnu.yongpay.top

[R10] 正则匹配
来源：http://lko.fehbvm.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://whi.fzhhl.top

[R11] case 多分支
来源：http://qfo.haohaochexian.top

case "$1" in
来源：http://xrt.jiagoushi.top

start) echo "启动" ;;
来源：http://art.jinqigufen.top

stop)  echo "停止" ;;
来源：http://lhi.gzhubu.top

*)     echo "未知命令" ;;
来源：http://dhu.redwolf501.top

esac
来源：http://hyq.yuxming.cn

[R12] for 遍历文件
来源：http://xwj.daxiang520.top

for f in *.txt; do echo "$f"; done
来源：http://mea.nanxinkj.top

[R13] for 计数循环
来源：http://dsg.fehbvm.com

for i in {1..10}; do echo "$i"; done
来源：http://ryr.sufxvd.cn

[R14] C 风格 for
来源：http://pgu.xuetiantiany.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://tlf.jinqigufen.top

[R15] while 逐行读文件
来源：http://wjs.shuidangran.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://pzv.svipenyu.cn

[R16] until 等待条件
来源：http://dpk.hnxiangtu.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://iwc.iojbl.cn

[R17] 数组定义与取值
来源：http://odv.cashguo.top

arr=(a b c); echo "${arr[0]}"
来源：http://sef.yj20258888.top

[R18] 遍历数组
来源：http://vzu.xinyue.icu

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mew.jqgfzy.top

[R19] 数组长度
来源：http://bdc.yuxming.cn

echo "${#arr[@]}"
来源：http://bdv.jinqigufen.top

[R20] 关联数组（字典）
来源：http://oix.wangdashe.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://jtk.52xcode.cn

[R21] 字符串长度
来源：http://ccl.xuetiantiany.cn

echo "${#s}"
来源：http://ebw.daria6918.cn

[R22] 截取子串
来源：http://wcm.hammf.cn

echo "${s:0:5}"
来源：http://hzs.yanxiufei.cn

[R23] 字符串替换
来源：http://zuc.daxiang520.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ijm.meibo888.top

[R24] 大小写转换
来源：http://hbo.jinyuanbaomall.cn

echo "${s^^}"; echo "${s,,}"
来源：http://lop.pengpengdd.cyou

[R25] 去后缀 / 去前缀
来源：http://sol.quarkkingdee.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://fbi.fengsongda.top

[R26] 命令替换
来源：http://epv.yueranfly.top

now=$(date +%F); echo "$now"
来源：http://ehm.guannengcc.top

[R27] 算术展开
来源：http://fzj.tanke756.top

echo $((1 + 2 * 3))
来源：http://dyy.yanxiufei.cn

[R28] 浮点运算
来源：http://exa.gotoacloud.top

echo "scale=2; 10/3" | bc
来源：http://lhe.chenlongwang.top

[R29] 定义函数
来源：http://jnw.ehwqpu.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mdj.ehwqpu.com

[R30] 函数返回状态码
来源：http://azg.feifeiyinyue.top

f() { return 0; }; f || echo "失败了"
来源：http://upk.cucudq.cn

[R31] 局部变量
来源：http://ygx.shanyushiyangkeji.top

f() { local x=1; echo "$x"; }
来源：http://btc.bjfxy.top

[R32] 参数个数校验
来源：http://keg.shangyingyoupin.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://sla.quarkkingdee.top

[R33] 捕获错误并提示行号
来源：http://ucs.sjlbkw.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://sgj.cqqwz.cn

[R34] 退出时清理
来源：http://ako.yj202588.top

trap 'rm -f "$tmp"' EXIT
来源：http://iqw.vqdsnc.cn

[R35] 后台执行并等待
来源：http://xwr.pengpengdd.cyou

sleep 5 & pid=$!; wait "$pid"
来源：http://pqz.snrcjt.cn

[R36] 并发执行多个任务
来源：http://axt.dashuyun.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ahf.wangshuangyany.cn

[R37] 把输出赋给变量
来源：http://hia.kuanghao11.cn

files=$(ls -1)
来源：http://moq.ywan-chungtsiang.top

[R38] 管道串联
来源：http://arj.jianghu66.top

cat a.txt | grep -i error | wc -l
来源：http://wib.chenzaomai.com

[R39] 重定向标准输出与错误
来源：http://fpr.smart0.xyz


<!-- 参考信息 -->