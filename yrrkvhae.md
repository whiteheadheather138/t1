代发 wailian999

================================================================================
来源：http://qlx.nanxinkj.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://sij.birdmap.top

================================================================================
来源：http://vdu.c1oappe.top

[Q01] 创建表
来源：http://daq.xuetiantiany.cn

CREATE TABLE users (
来源：http://fqc.kuanghao11.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://oqb.tian-w.cn

name VARCHAR(50) NOT NULL,
来源：http://qup.yongpay.top

email VARCHAR(100) UNIQUE,
来源：http://aev.dashuyun.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://kxj.hammf.cn

);
来源：http://tvi.nanxinkj.top

[Q02] 创建带外键的表
来源：http://tdl.hnqzz.top

CREATE TABLE orders (
来源：http://mcu.hywenlv.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://aib.zhijiandao.cn

user_id INT NOT NULL,
来源：http://kof.hysaishi.cn

amount DECIMAL(10, 2),
来源：http://rpk.smart0.xyz

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://xsc.cashguo.top

);
来源：http://qsi.nanxinkj.top

[Q03] 增加列
来源：http://pnn.yueranfly.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://myd.yj20258888.top

[Q04] 修改列类型
来源：http://eyi.jinqigfzy.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://jsl.fengsongda.top

[Q05] 重命名列
来源：http://rxz.hfpthk.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://qvz.redwolf501.top

[Q06] 删除列
来源：http://ylf.nanxinkj.top

ALTER TABLE users DROP COLUMN age;
来源：http://tcl.epnwcf.com

[Q07] 删除表
来源：http://fqf.shuidangran.top

DROP TABLE IF EXISTS orders;
来源：http://tol.52xcode.cn

[Q08] 创建普通索引
来源：http://vek.hnqzz.top

CREATE INDEX idx_users_email ON users(email);
来源：http://ilj.fehbvm.com

[Q09] 创建唯一索引
来源：http://uwb.fanxiaobao.xyz

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://qpz.hcnkem.com

[Q10] 插入单行
来源：http://xiu.daxiang520.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://csa.dashuyun.cn

[Q11] 一次插入多行
来源：http://ttv.zhixingplan.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://jbt.fanxiaobao.xyz

[Q12] 插入后取自增 ID
来源：http://ffn.gotoacloud.top

INSERT INTO users (name) VALUES ('C');
来源：http://hko.zhiwuduotai.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ttk.zhoulong.xyz

[Q13] 忽略重复插入
来源：http://zvs.hnqzz.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://dcm.dashuyun.cn

[Q14] 存在则更新（upsert）
来源：http://reu.yvedp.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://iyw.cqqwz.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://gru.zhongyouzk.top

[Q15] 查询全部
来源：http://gbz.haohaochexian.top

SELECT * FROM users;
来源：http://sqa.iojbl.cn

[Q16] 查询指定列
来源：http://eto.9152youxi.cn

SELECT id, name FROM users;
来源：http://dko.jqgfzy.top

[Q17] 条件查询
来源：http://yhb.zhijiandao.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://qar.xinyue.icu

[Q18] 模糊匹配
来源：http://jiz.fanxiaobao.xyz

SELECT * FROM users WHERE name LIKE '张%';
来源：http://xgl.hfpthk.cn

[Q19] 范围查询
来源：http://imq.ywan-chungtsiang.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://vsj.hcnkem.com

[Q20] IN 列表
来源：http://iak.daria6918.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://btb.yuanzhike.top

[Q21] 空值判断
来源：http://pri.yuanzhike.top

SELECT * FROM users WHERE email IS NULL;
来源：http://uwb.gzhubu.top

[Q22] 排序
来源：http://dgq.yonumen.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://xtq.jyoumei.cn

[Q23] 分页
来源：http://gxw.c1oappe.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ozv.vehdjk.com

[Q24] 去重
来源：http://thk.jlsjyb.cn

SELECT DISTINCT city FROM users;
来源：http://rdi.316326.xyz

[Q25] 只取前 N 条
来源：http://buv.xylfe.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://sou.ydjk.org.cn

[Q26] 计数
来源：http://ilr.sweek.top

SELECT COUNT(*) FROM users;
来源：http://htz.snrcjt.cn

[Q27] 条件计数
来源：http://zsj.yonumen.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://zlr.c1oappe.top

[Q28] 求和与平均
来源：http://clt.fktsv.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://kqh.jyoumei.cn

[Q29] 最大最小值
来源：http://ewj.gzhubu.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://cnl.sysykeji.top

[Q30] 分组统计
来源：http://emf.hongshengwenyu.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ftn.fengsongda.top

[Q31] 分组后过滤
来源：http://knv.fanxiaobao.xyz

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mjq.gotoacloud.top

[Q32] 分组拼接字符串
来源：http://ljv.0kj1m.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://tyt.sxryk.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://cge.quarkkingdee.top

[Q33] 多列分组
来源：http://ahk.xziqi.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://awg.jqgufenzy.top

[Q34] 每组取第一条
来源：http://lqh.52xcode.cn

SELECT * FROM (
来源：http://cdq.ydzc1.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://for.jqgfzy.top

) t WHERE rn = 1;
来源：http://pto.jqgufenzy.top

[Q35] 内连接
来源：http://bez.shzxlz.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://qjf.fengsongda.top

[Q36] 左连接
来源：http://mkb.hfpthk.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://eko.hammf.cn

[Q37] 右连接
来源：http://fwq.chenlongwang.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wzn.hfpthk.cn

[Q38] 全外连接（PostgreSQL）
来源：http://zbu.xylfe.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://grc.fzhhl.top

[Q39] 自连接（查上下级）
来源：http://duj.jianghu66.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://ddf.vehdjk.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://lma.hfpthk.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://hre.wangshuangyany.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://jnm.dashuyun.cn

[Q41] 多表连接
来源：http://vgv.yj20258888.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://ecv.uphjek.com

JOIN users u ON u.id = o.user_id
来源：http://zgv.shangyingyoupin.top

JOIN products p ON p.id = o.product_id;
来源：http://ixt.sufxvd.cn

[Q42] 连接条件附加过滤
来源：http://njd.snrcjt.cn

SELECT u.name, o.amount FROM users u
来源：http://xpc.tianlin.xyz

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://yfx.havefunace.top

[Q43] 标量子查询
来源：http://gtq.bbcook.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://jpx.ydjk.org.cn

[Q44] IN 子查询
来源：http://wpq.9152youxi.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://fff.bjfxy.top

[Q45] EXISTS 判断存在
来源：http://rmj.cqqwz.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://smb.hnqzz.top

[Q46] NOT EXISTS 判断不存在
来源：http://gpa.andypj.xyz

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ovp.52xcode.cn

[Q47] 与平均值比较
来源：http://deg.316326.xyz

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://bnd.uphjek.com

[Q48] CTE 公用表表达式
来源：http://jyh.yuanzhike.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://rda.fzhhl.top

SELECT * FROM t WHERE c > 5;
来源：http://cxm.nanxinkj.top

[Q49] 更新单行
来源：http://yab.yanxiufei.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ede.chenjidiqi.icu

[Q50] 批量更新
来源：http://fms.ppjwa.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hbq.shangyingyoupin.top

[Q51] 用子查询更新
来源：http://qjy.chenjidiqi.icu

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://rkq.gaohongyu789.top

[Q52] 删除指定行
来源：http://bhy.xziqi.cn

DELETE FROM users WHERE id = 10;
来源：http://ctf.hywenlv.cn

[Q53] 按条件删除
来源：http://sjp.jyoumei.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://emz.jyoumei.cn

[Q54] 清空表
来源：http://olo.hammf.cn

TRUNCATE TABLE logs;
来源：http://yvr.cdnleiting.top

[Q55] 排名（并列占位）
来源：http://bsz.chenlongwang.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://oht.cucudq.cn

[Q56] 密集排名（并列不占位）
来源：http://lwr.ivvv.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ivq.guannengcc.top

[Q57] 行号
来源：http://lyv.dashuyun.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://uqc.tian-w.cn

[Q58] 累计求和
来源：http://blt.nanxuanxn.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://kqz.yonumen.top

[Q59] 分组内累计
来源：http://gkv.cdnleiting.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://scw.ydzc1.top

[Q60] 取上一行 / 下一行
来源：http://ygk.shuidangran.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ieu.jianghu66.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://xzt.xinyue.icu

[Q61] 移动平均
来源：http://udm.gaohongyu789.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://lym.gzhubu.top

[Q62] 分组占比
来源：http://xjl.tian-w.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://vzg.sysykeji.top

[Q63] 开启事务
来源：http://snd.daxiang520.top

START TRANSACTION;                -- 或 BEGIN
来源：http://vxq.jyoumei.cn

[Q64] 提交事务
来源：http://fpq.guannengcc.top

COMMIT;
来源：http://srb.zhongyouzk.top

[Q65] 回滚事务
来源：http://xkw.xuetiantiany.cn

ROLLBACK;
来源：http://dqi.ppjwa.cn

[Q66] 行锁查询
来源：http://blg.uphjek.com

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://dvn.svipenyu.cn

[Q67] 设置隔离级别
来源：http://dxa.gaohongyu789.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mlz.hesvh.cn

[Q68] 保存点
来源：http://yrr.ctjpmb.com

SAVEPOINT sp1;
来源：http://tlg.sysykeji.top

ROLLBACK TO sp1;
来源：http://php.zhijiandao.cn

[Q69] 查看执行计划
来源：http://xpd.yonumen.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://shy.wangshuangyany.cn

[Q70] 更新统计信息
来源：http://nqu.yj20258.top

ANALYZE TABLE users;
来源：http://mzr.bjfxy.top

[Q71] 查看建表语句
来源：http://ohg.nanxinkj.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ipm.yonumen.top

[Q72] 查看索引
来源：http://nqx.yangfankeji.com

SHOW INDEX FROM users;
来源：http://pxu.yueranfly.top

[Q73] 查看表状态
来源：http://bpn.ywan-chungtsiang.top

SHOW TABLE STATUS LIKE 'users';
来源：http://vti.cashguo.top

[Q74] 强制使用索引
来源：http://xmr.birdmap.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://qfe.jiagoushi.top

[Q75] 日期格式化
来源：http://jnj.jinqigfzy.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://nwe.hnxiangtu.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://fwn.jiagoushi.top

[Q76] 按天统计
来源：http://xsu.ehwqpu.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://sat.ywan-chungtsiang.top

[Q77] 时间加减
来源：http://ept.pengpengdd.cyou

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mnz.yangfankeji.com

[Q78] 当前时间
来源：http://ums.nwbrower.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hku.jqgufenzy.top

[Q79] 字符串拼接
来源：http://otw.kuanghao11.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://nmu.jianghu66.top

[Q80] 字符串截取
来源：http://wtj.cucudq.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://jqs.fktsv.cn

[Q81] 字符串替换
来源：http://fqi.yj202588.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://pti.vehdjk.com

[Q82] 字符长度与字节长度
来源：http://bxp.fengsongda.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://nxa.andypj.xyz

[Q83] 大小写转换
来源：http://nal.gotoacloud.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://adu.0kj1m.cn

[Q84] 去除首尾空格
来源：http://sgl.jqgufenzy.top

SELECT TRIM(name) FROM users;
来源：http://hbn.chenzaomai.com

[Q85] 数值取整
来源：http://emn.yangfankeji.com

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://eep.52xcode.cn

[Q86] 读取 JSON 字段
来源：http://dmo.aibaodan.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://sza.chenzaomai.com

[Q87] JSON 字段做条件
来源：http://czy.epnwcf.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://swn.hcnkem.com

[Q88] 行转列（条件聚合）
来源：http://rlr.nanxuanxn.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://zte.fktsv.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://dnc.hywenlv.cn

[Q89] 判断表是否存在
来源：http://cte.svipenyu.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://pjz.jinyuanbaomall.cn

[Q90] 生成序号列
来源：http://fhl.hnqzz.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ifi.zhengqikj.top

================================================================================
来源：http://rfo.cdnleiting.top

R. Bash 专题
来源：http://yyr.hfpthk.cn

================================================================================
来源：http://foz.zhixingplan.top

[R01] shebang 与严格模式
来源：http://tcg.shzxlz.cn

#!/usr/bin/env bash
来源：http://iyv.zhixingplan.top

set -euo pipefail
来源：http://nhm.cucudq.cn

[R02] 变量赋值与使用
来源：http://hsb.svipenyu.cn

name="Tom"; echo "$name"
来源：http://apw.yongpay.top

[R03] 只读变量
来源：http://xsp.jinqigufen.top

readonly PI=3.14
来源：http://oyz.hnqzz.top

[R04] 位置参数
来源：http://plo.316326.xyz

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://lrt.yvedp.cn

[R05] 参数默认值
来源：http://boh.kuanghao11.cn

name="${1:-default}"
来源：http://guk.nanxinkj.top

[R06] 判断命令是否存在
来源：http://bvm.fktsv.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://tem.kuanghao11.cn

[R07] if 判断文件
来源：http://kgg.ctjpmb.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://kja.tian-w.cn

[R08] 数值比较
来源：http://pzj.yongpay.top

if (( a > b )); then echo "a 更大"; fi
来源：http://las.nanxinkj.top

[R09] 字符串比较
来源：http://hql.0kj1m.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://tdl.xingfuxueyuan.xyz

[R10] 正则匹配
来源：http://qpe.jinghuilouyu.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ive.daria6918.cn

[R11] case 多分支
来源：http://the.yanxiufei.cn

case "$1" in
来源：http://tzu.zhijiandao.cn

start) echo "启动" ;;
来源：http://jdt.yonumen.top

stop)  echo "停止" ;;
来源：http://qmd.shzxlz.cn

*)     echo "未知命令" ;;
来源：http://sch.epnwcf.com

esac
来源：http://xmk.zhixingplan.top

[R12] for 遍历文件
来源：http://xdv.cucudq.cn

for f in *.txt; do echo "$f"; done
来源：http://zdv.hfpthk.cn

[R13] for 计数循环
来源：http://tpy.sxryk.cn

for i in {1..10}; do echo "$i"; done
来源：http://dsn.xinyue.icu

[R14] C 风格 for
来源：http://gpe.316326.xyz

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://yzn.ehwqpu.com

[R15] while 逐行读文件
来源：http://ghe.fktsv.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wxy.yanxiufei.cn

[R16] until 等待条件
来源：http://mwi.tianlin.xyz

until [[ -f done.flag ]]; do sleep 1; done
来源：http://qim.hfpthk.cn

[R17] 数组定义与取值
来源：http://zie.gaohongyu789.top

arr=(a b c); echo "${arr[0]}"
来源：http://adv.sweek.top

[R18] 遍历数组
来源：http://nkt.shanyushiyangkeji.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://iwq.jiagoushi.top

[R19] 数组长度
来源：http://mrw.c1oappe.top

echo "${#arr[@]}"
来源：http://ocp.xuanzx.com

[R20] 关联数组（字典）
来源：http://ksv.fanxiaobao.xyz

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://epm.jiagoushi.top

[R21] 字符串长度
来源：http://nit.hysaishi.cn

echo "${#s}"
来源：http://okq.nanxinkj.top

[R22] 截取子串
来源：http://bxy.xziqi.cn

echo "${s:0:5}"
来源：http://aor.chenzaomai.com

[R23] 字符串替换
来源：http://eaz.xinyue.icu

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://geq.jiagoushi.top

[R24] 大小写转换
来源：http://lho.guowangkeji.top

echo "${s^^}"; echo "${s,,}"
来源：http://xef.tian-w.cn

[R25] 去后缀 / 去前缀
来源：http://gcm.sxryk.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://gxn.shanyushiyangtech.top

[R26] 命令替换
来源：http://zfa.jinqigfzy.top

now=$(date +%F); echo "$now"
来源：http://gdm.wangdashe.top

[R27] 算术展开
来源：http://mlj.jinyuanbaomall.cn

echo $((1 + 2 * 3))
来源：http://icl.snrcjt.cn

[R28] 浮点运算
来源：http://eyv.bbcook.cn

echo "scale=2; 10/3" | bc
来源：http://otv.jyoumei.cn

[R29] 定义函数
来源：http://nwq.xuetiantiany.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://usw.fanxiaobao.xyz

[R30] 函数返回状态码
来源：http://svn.tian-w.cn

f() { return 0; }; f || echo "失败了"
来源：http://fbl.nanxinkj.top

[R31] 局部变量
来源：http://frr.ppjwa.cn

f() { local x=1; echo "$x"; }
来源：http://ctv.cdnleiting.top

[R32] 参数个数校验
来源：http://lao.gogol.net.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://qdo.jiagoushi.top

[R33] 捕获错误并提示行号
来源：http://urp.chenzaomai.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://xhw.zhengqikj.top

[R34] 退出时清理
来源：http://odv.pycfn.com

trap 'rm -f "$tmp"' EXIT
来源：http://nke.9152youxi.cn

[R35] 后台执行并等待
来源：http://ufz.zhaomingkeji.xyz

sleep 5 & pid=$!; wait "$pid"
来源：http://izy.hnqzz.top

[R36] 并发执行多个任务
来源：http://ved.jlsjyb.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://zbt.jinghuilouyu.cn

[R37] 把输出赋给变量
来源：http://euh.wangdashe.top

files=$(ls -1)
来源：http://igr.zdbjq.cn

[R38] 管道串联
来源：http://lhs.fehbvm.com

cat a.txt | grep -i error | wc -l
来源：http://ovc.cashguo.top

[R39] 重定向标准输出与错误
来源：http://gpn.zhixingplan.top

cmd > out.log 2>&1
来源：http://psl.wangdashe.top

[R40] 追加写日志
来源：http://lcy.dianchejie.cn

echo "log" >> out.log
来源：http://pfu.bbcook.cn

[R41] 丢弃输出
来源：http://lbp.ydzc1.top

cmd >/dev/null 2>&1
来源：http://mjb.xuanzx.com

[R42] 输入重定向
来源：http://tyr.sufxvd.cn

wc -l < a.txt
来源：http://nqt.daxiang520.top

[R43] 按名字查找文件
来源：http://kkp.shanyushiyangtech.top


<!-- 参考信息 -->