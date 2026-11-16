代发 wailian999

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://vth.ybcxt.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://uwf.tanke756.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://olh.ivvv.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://jnj.quarkkingdee.top

================================================================================
来源：http://zvc.jianghu66.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://oif.sysykeji.top

================================================================================
来源：http://oxo.xuetiantiany.cn

[Q01] 创建表
来源：http://bun.fzhhl.top

CREATE TABLE users (
来源：http://wog.pengpengdd.cyou

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://nbq.sysykeji.top

name VARCHAR(50) NOT NULL,
来源：http://fvp.jqgufenzy.top

email VARCHAR(100) UNIQUE,
来源：http://hlf.zycfv.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blf.tianlin.xyz

);
来源：http://mkl.feifeiyinyue.top

[Q02] 创建带外键的表
来源：http://lvo.pengpengdd.cyou

CREATE TABLE orders (
来源：http://nwm.xylfe.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://fpa.fengsongda.top

user_id INT NOT NULL,
来源：http://pjv.yj20258.top

amount DECIMAL(10, 2),
来源：http://hit.uphjek.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://aue.chenjidiqi.icu

);
来源：http://cag.epnwcf.com

[Q03] 增加列
来源：http://wjf.yj202588.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://nix.hfpthk.cn

[Q04] 修改列类型
来源：http://mll.jqgufenzy.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://bjc.zdbjq.cn

[Q05] 重命名列
来源：http://png.ppjwa.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://aom.jqgufenzy.top

[Q06] 删除列
来源：http://fvc.bbcook.cn

ALTER TABLE users DROP COLUMN age;
来源：http://cxj.shzxlz.cn

[Q07] 删除表
来源：http://nzi.jqgufenzy.top

DROP TABLE IF EXISTS orders;
来源：http://ffl.jqgfzy.top

[Q08] 创建普通索引
来源：http://tcr.daxiang520.top

CREATE INDEX idx_users_email ON users(email);
来源：http://xzl.svipenyu.cn

[Q09] 创建唯一索引
来源：http://pjz.hnxiangtu.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://uye.hfpthk.cn

[Q10] 插入单行
来源：http://xbi.jinghuilouyu.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://fnu.xinyue.icu

[Q11] 一次插入多行
来源：http://ubd.birdmap.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://nig.uphjek.com

[Q12] 插入后取自增 ID
来源：http://rlt.tianlin.xyz

INSERT INTO users (name) VALUES ('C');
来源：http://sod.jinqigufen.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://eec.fzhhl.top

[Q13] 忽略重复插入
来源：http://fze.uphjek.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://yoe.xylfe.cn

[Q14] 存在则更新（upsert）
来源：http://udo.epnwcf.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://pku.jianghu66.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://vca.52xcode.cn

[Q15] 查询全部
来源：http://gik.chenjidiqi.icu

SELECT * FROM users;
来源：http://peu.birdmap.top

[Q16] 查询指定列
来源：http://ayc.hongshengwenyu.top

SELECT id, name FROM users;
来源：http://wqw.andypj.xyz

[Q17] 条件查询
来源：http://obt.yangfankeji.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://agn.cdnleiting.top

[Q18] 模糊匹配
来源：http://qzg.shangyingyoupin.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ljf.sxryk.cn

[Q19] 范围查询
来源：http://stu.shanyushiyangkeji.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wrq.redwolf501.top

[Q20] IN 列表
来源：http://kie.jinghuilouyu.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://bmd.ywan-chungtsiang.top

[Q21] 空值判断
来源：http://fqz.hcnkem.com

SELECT * FROM users WHERE email IS NULL;
来源：http://dji.xylfe.cn

[Q22] 排序
来源：http://vbe.hnqzz.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mja.ywan-chungtsiang.top

[Q23] 分页
来源：http://ylj.chenlongwang.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://nhc.52xcode.cn

[Q24] 去重
来源：http://gvg.yongpay.top

SELECT DISTINCT city FROM users;
来源：http://ytl.jyoumei.cn

[Q25] 只取前 N 条
来源：http://mgp.zhengqikj.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://rwu.haohaochexian.top

[Q26] 计数
来源：http://yvs.mhx1999.top

SELECT COUNT(*) FROM users;
来源：http://vgk.sxryk.cn

[Q27] 条件计数
来源：http://aif.yanxiufei.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://gop.wangdashe.top

[Q28] 求和与平均
来源：http://cgl.dashuyun.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://bql.sysykeji.top

[Q29] 最大最小值
来源：http://wfo.shzxlz.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://han.hnqzz.top

[Q30] 分组统计
来源：http://fln.zhiwuduotai.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ruv.jiagoushi.top

[Q31] 分组后过滤
来源：http://lxp.chenlongwang.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://xcd.feifeiyinyue.top

[Q32] 分组拼接字符串
来源：http://jii.fengsongda.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mlb.fehbvm.com

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://fne.xuanzx.com

[Q33] 多列分组
来源：http://sil.chenlongwang.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://pek.fktsv.cn

[Q34] 每组取第一条
来源：http://bej.shanyushiyangkeji.top

SELECT * FROM (
来源：http://fju.fehbvm.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://xtw.guowangkeji.top

) t WHERE rn = 1;
来源：http://cdj.zhiwuduotai.top

[Q35] 内连接
来源：http://rji.ivvv.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://zue.shuidangran.top

[Q36] 左连接
来源：http://ljm.shanyushiyangtech.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://bhh.shuidangran.top

[Q37] 右连接
来源：http://axz.cucudq.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://vkd.hongshengwenyu.top

[Q38] 全外连接（PostgreSQL）
来源：http://emt.svipenyu.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://htn.guannengcc.top

[Q39] 自连接（查上下级）
来源：http://bgn.hongshengwenyu.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://lin.52xcode.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://nwz.pengpengdd.cyou

[Q40] 交叉连接（笛卡尔积）
来源：http://rnw.xziqi.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wkc.gogol.net.cn

[Q41] 多表连接
来源：http://rsp.gaohongyu789.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://cmp.316326.xyz

JOIN users u ON u.id = o.user_id
来源：http://qzb.ydzc1.top

JOIN products p ON p.id = o.product_id;
来源：http://yle.dashuyun.cn

[Q42] 连接条件附加过滤
来源：http://wpe.yj20258.top

SELECT u.name, o.amount FROM users u
来源：http://exw.shanyushiyangkeji.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://utb.fzhhl.top

[Q43] 标量子查询
来源：http://dcp.xingfuxueyuan.xyz

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://rmb.jinyuanbaomall.cn

[Q44] IN 子查询
来源：http://pgf.ydzc1.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://bso.jinqigufen.top

[Q45] EXISTS 判断存在
来源：http://vqd.jiagoushi.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://cde.zhengqikj.top

[Q46] NOT EXISTS 判断不存在
来源：http://ggi.52xcode.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kjh.yuxming.cn

[Q47] 与平均值比较
来源：http://mwt.sweek.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://dye.svipenyu.cn

[Q48] CTE 公用表表达式
来源：http://oxl.chenzaomai.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://sya.aibaodan.cn

SELECT * FROM t WHERE c > 5;
来源：http://mii.shangyingyoupin.top

[Q49] 更新单行
来源：http://cuo.9152youxi.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ndv.gotoacloud.top

[Q50] 批量更新
来源：http://puh.snrcjt.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://bpz.hnqzz.top

[Q51] 用子查询更新
来源：http://jkf.nanxuanxn.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://bvd.quarkkingdee.top

[Q52] 删除指定行
来源：http://gci.wangdashe.top

DELETE FROM users WHERE id = 10;
来源：http://yjn.shangyingyoupin.top

[Q53] 按条件删除
来源：http://sag.ivvv.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ujs.316326.xyz

[Q54] 清空表
来源：http://sqk.c1oappe.top

TRUNCATE TABLE logs;
来源：http://mni.yonumen.top

[Q55] 排名（并列占位）
来源：http://orr.yongpay.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ivf.zhixingplan.top

[Q56] 密集排名（并列不占位）
来源：http://aqa.fengsongda.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://sbq.yuxming.cn

[Q57] 行号
来源：http://dhs.xingfuxueyuan.xyz

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://qwc.fanxiaobao.xyz

[Q58] 累计求和
来源：http://nmn.uphjek.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://qzy.nwbrower.top

[Q59] 分组内累计
来源：http://pbg.yfazqb.com

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://guf.ydzc1.top

[Q60] 取上一行 / 下一行
来源：http://ybk.gotoacloud.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://lda.xylfe.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://fxt.jinyuanbaomall.cn

[Q61] 移动平均
来源：http://aym.yj202588.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://uik.9152youxi.cn

[Q62] 分组占比
来源：http://wpn.hongshengwenyu.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wqh.yonumen.top

[Q63] 开启事务
来源：http://eng.feifeiyinyue.top

START TRANSACTION;                -- 或 BEGIN
来源：http://ccp.cashguo.top

[Q64] 提交事务
来源：http://lgh.xziqi.cn

COMMIT;
来源：http://fhf.yueranfly.top

[Q65] 回滚事务
来源：http://jml.sweek.top

ROLLBACK;
来源：http://kdt.yangfankeji.com

[Q66] 行锁查询
来源：http://bux.cheryme.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://gyn.uphjek.com

[Q67] 设置隔离级别
来源：http://cpy.yfazqb.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://kcp.hywenlv.cn

[Q68] 保存点
来源：http://qpx.ctjpmb.com

SAVEPOINT sp1;
来源：http://crv.gotoacloud.top

ROLLBACK TO sp1;
来源：http://upr.ydzc1.top

[Q69] 查看执行计划
来源：http://bzp.yuanzhike.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://gsv.hnxiangtu.top

[Q70] 更新统计信息
来源：http://uky.chenlongwang.top

ANALYZE TABLE users;
来源：http://dcd.sysykeji.top

[Q71] 查看建表语句
来源：http://hvu.ybcxt.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://tui.yongpay.top

[Q72] 查看索引
来源：http://ckm.vqdsnc.cn

SHOW INDEX FROM users;
来源：http://jcy.ywan-chungtsiang.top

[Q73] 查看表状态
来源：http://yhm.jianghu66.top

SHOW TABLE STATUS LIKE 'users';
来源：http://ulh.fehbvm.com

[Q74] 强制使用索引
来源：http://xjm.hongshengwenyu.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://zzp.jyoumei.cn

[Q75] 日期格式化
来源：http://zsw.fzhhl.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://dnf.smart0.xyz

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://szq.xingfuxueyuan.xyz

[Q76] 按天统计
来源：http://gge.sufxvd.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://dbt.pengpengdd.cyou

[Q77] 时间加减
来源：http://zbm.hywenlv.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://gtw.zycfv.cn

[Q78] 当前时间
来源：http://txr.snrcjt.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hrz.bjfxy.top

[Q79] 字符串拼接
来源：http://jer.shanyushiyangkeji.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://zgp.wangshuangyany.cn

[Q80] 字符串截取
来源：http://btf.cdnleiting.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ats.hammf.cn

[Q81] 字符串替换
来源：http://lwo.pengpengdd.cyou

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://myy.daxiang520.top

[Q82] 字符长度与字节长度
来源：http://yyh.mhx1999.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://inj.andypj.xyz

[Q83] 大小写转换
来源：http://veg.316326.xyz

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://uom.shanyushiyangtech.top

[Q84] 去除首尾空格
来源：http://tyx.shanyushiyangkeji.top

SELECT TRIM(name) FROM users;
来源：http://hpr.fanxiaobao.xyz

[Q85] 数值取整
来源：http://kdf.smart0.xyz

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://bll.cheryme.top

[Q86] 读取 JSON 字段
来源：http://awt.hfpthk.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ixl.pengpengdd.cyou

[Q87] JSON 字段做条件
来源：http://ess.jyoumei.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://xyf.ctjpmb.com

[Q88] 行转列（条件聚合）
来源：http://zrh.hammf.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://juu.epnwcf.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://igw.mhx1999.top

[Q89] 判断表是否存在
来源：http://njm.nanxinkj.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://zuu.aizwys.cn

[Q90] 生成序号列
来源：http://nnm.gzhubu.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://tvf.ctjpmb.com

================================================================================
来源：http://viy.redwolf501.top

R. Bash 专题
来源：http://fwc.sjlbkw.cn

================================================================================
来源：http://xan.hcnkem.com

[R01] shebang 与严格模式
来源：http://jjw.316326.xyz

#!/usr/bin/env bash
来源：http://zlw.epnwcf.com

set -euo pipefail
来源：http://jmw.birdmap.top

[R02] 变量赋值与使用
来源：http://zqm.guowangkeji.top

name="Tom"; echo "$name"
来源：http://dur.yueranfly.top

[R03] 只读变量
来源：http://bmx.aibaodan.cn

readonly PI=3.14
来源：http://plg.zhengqikj.top

[R04] 位置参数
来源：http://kjt.vehdjk.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://rhk.jinyuanbaomall.cn

[R05] 参数默认值
来源：http://zrf.jqgfzy.top

name="${1:-default}"
来源：http://vaj.pycfn.com

[R06] 判断命令是否存在
来源：http://att.gaohongyu789.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://xzk.bbcook.cn

[R07] if 判断文件
来源：http://ibj.shanyushiyangkeji.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://abt.bjfxy.top

[R08] 数值比较
来源：http://hbh.gzhubu.top

if (( a > b )); then echo "a 更大"; fi
来源：http://nxr.fehbvm.com

[R09] 字符串比较
来源：http://phg.ppjwa.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://aai.zhengqikj.top

[R10] 正则匹配
来源：http://hsz.yanxiufei.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ycv.feifeiyinyue.top

[R11] case 多分支
来源：http://wdn.dashuyun.cn

case "$1" in
来源：http://pyw.birdmap.top

start) echo "启动" ;;
来源：http://iqs.jyoumei.cn

stop)  echo "停止" ;;
来源：http://tid.sysykeji.top

*)     echo "未知命令" ;;
来源：http://urd.fehbvm.com

esac
来源：http://dps.fengsongda.top

[R12] for 遍历文件
来源：http://csn.daria6918.cn

for f in *.txt; do echo "$f"; done
来源：http://gua.9152youxi.cn

[R13] for 计数循环
来源：http://iub.sysykeji.top

for i in {1..10}; do echo "$i"; done
来源：http://rfc.jqgfzy.top

[R14] C 风格 for
来源：http://lym.epnwcf.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ekw.zdqjudy.top

[R15] while 逐行读文件
来源：http://yuu.bjfxy.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://lwt.zdbjq.cn

[R16] until 等待条件
来源：http://bom.daria6918.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hat.zhiwuduotai.top

[R17] 数组定义与取值
来源：http://pdi.pengpengdd.cyou

arr=(a b c); echo "${arr[0]}"
来源：http://bib.guowangkeji.top

[R18] 遍历数组
来源：http://jpt.jyoumei.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://lfc.ydzc1.top

[R19] 数组长度
来源：http://kke.pycfn.com

echo "${#arr[@]}"
来源：http://wsv.zhixingplan.top

[R20] 关联数组（字典）
来源：http://mxq.shanyushiyangkeji.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://vvx.shzxlz.cn

[R21] 字符串长度
来源：http://zmx.0kj1m.cn

echo "${#s}"
来源：http://nrx.hnqzz.top

[R22] 截取子串
来源：http://xdr.tianlin.xyz

echo "${s:0:5}"
来源：http://fia.ydjk.org.cn

[R23] 字符串替换
来源：http://vbn.tianlin.xyz

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://znx.jyoumei.cn

[R24] 大小写转换
来源：http://riy.zhengqikj.top

echo "${s^^}"; echo "${s,,}"
来源：http://qnt.xingfuxueyuan.xyz

[R25] 去后缀 / 去前缀
来源：http://ofp.fzhhl.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://kaq.shuidangran.top

[R26] 命令替换
来源：http://pkl.yj202588.top

now=$(date +%F); echo "$now"
来源：http://ydd.epnwcf.com

[R27] 算术展开
来源：http://fjs.0kj1m.cn

echo $((1 + 2 * 3))
来源：http://wqt.aizwys.cn

[R28] 浮点运算
来源：http://tuo.pycfn.com

echo "scale=2; 10/3" | bc
来源：http://nnt.quarkkingdee.top

[R29] 定义函数
来源：http://iai.sweek.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://qqr.xziqi.cn

[R30] 函数返回状态码
来源：http://xwg.shanyushiyangkeji.top

f() { return 0; }; f || echo "失败了"
来源：http://vka.smart0.xyz

[R31] 局部变量
来源：http://shg.zdbjq.cn

f() { local x=1; echo "$x"; }
来源：http://ydm.fzhhl.top

[R32] 参数个数校验
来源：http://oxx.fehbvm.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://npu.jiagoushi.top

[R33] 捕获错误并提示行号
来源：http://gkb.yj202588.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://tqw.jlsjyb.cn

[R34] 退出时清理
来源：http://qjv.9152youxi.cn

trap 'rm -f "$tmp"' EXIT
来源：http://sns.52xcode.cn

[R35] 后台执行并等待
来源：http://lmh.hammf.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://icf.havefunace.top

[R36] 并发执行多个任务
来源：http://tse.yfazqb.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://bja.iojbl.cn

[R37] 把输出赋给变量
来源：http://ikm.hammf.cn

files=$(ls -1)
来源：http://gyl.jinqigfzy.top

[R38] 管道串联
来源：http://wns.yfazqb.com

cat a.txt | grep -i error | wc -l
来源：http://ixq.zycfv.cn

[R39] 重定向标准输出与错误
来源：http://rdk.yvedp.cn

cmd > out.log 2>&1
来源：http://hkq.zhengqikj.top

[R40] 追加写日志
来源：http://rwp.haohaochexian.top

echo "log" >> out.log
来源：http://oon.haohaochexian.top

[R41] 丢弃输出
来源：http://wfu.feifeiyinyue.top


<!-- 参考信息 -->