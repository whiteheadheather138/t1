代发 wailian999

================================================================================
来源：http://bpe.fengsongda.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://fwz.wangshuangyany.cn

================================================================================
来源：http://gik.havefunace.top

[Q01] 创建表
来源：http://wds.iojbl.cn

CREATE TABLE users (
来源：http://ewr.gogol.net.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wec.fanxiaobao.xyz

name VARCHAR(50) NOT NULL,
来源：http://ecq.hesvh.cn

email VARCHAR(100) UNIQUE,
来源：http://uvg.cashguo.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://kgu.yueranfly.top

);
来源：http://gzy.daria6918.cn

[Q02] 创建带外键的表
来源：http://epb.shzxlz.cn

CREATE TABLE orders (
来源：http://qqn.smart0.xyz

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://yba.quarkkingdee.top

user_id INT NOT NULL,
来源：http://mhi.xuanzx.com

amount DECIMAL(10, 2),
来源：http://ofs.uphjek.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ywq.fanxiaobao.xyz

);
来源：http://jwo.gogol.net.cn

[Q03] 增加列
来源：http://zru.zdqjudy.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://kgu.yangfankeji.com

[Q04] 修改列类型
来源：http://hsc.kuanghao11.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://bid.cucudq.cn

[Q05] 重命名列
来源：http://bjd.yueranfly.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ttd.316326.xyz

[Q06] 删除列
来源：http://bqr.yongpay.top

ALTER TABLE users DROP COLUMN age;
来源：http://wyp.shuidangran.top

[Q07] 删除表
来源：http://ndh.yangfankeji.com

DROP TABLE IF EXISTS orders;
来源：http://rrp.yangfankeji.com

[Q08] 创建普通索引
来源：http://xcn.mhx1999.top

CREATE INDEX idx_users_email ON users(email);
来源：http://sxl.ppjwa.cn

[Q09] 创建唯一索引
来源：http://sad.ppjwa.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://jge.yvedp.cn

[Q10] 插入单行
来源：http://frv.yueranfly.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://cbj.tarul.cn

[Q11] 一次插入多行
来源：http://ytf.guowangkeji.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ohq.ybcxt.top

[Q12] 插入后取自增 ID
来源：http://aus.hywenlv.cn

INSERT INTO users (name) VALUES ('C');
来源：http://nef.hcnkem.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://dtv.yonumen.top

[Q13] 忽略重复插入
来源：http://wxr.zdqjudy.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://knq.feifeiyinyue.top

[Q14] 存在则更新（upsert）
来源：http://osu.feifeiyinyue.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://prl.vqdsnc.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://nkl.gotoacloud.top

[Q15] 查询全部
来源：http://qpq.dianchejie.cn

SELECT * FROM users;
来源：http://gpv.9152youxi.cn

[Q16] 查询指定列
来源：http://ogw.fengsongda.top

SELECT id, name FROM users;
来源：http://tye.svipenyu.cn

[Q17] 条件查询
来源：http://bgi.shanyushiyangtech.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://qhj.jianghu66.top

[Q18] 模糊匹配
来源：http://plm.hammf.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://lzq.xziqi.cn

[Q19] 范围查询
来源：http://fxs.yj20258888.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wxs.redwolf501.top

[Q20] IN 列表
来源：http://xlk.9152youxi.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://akm.xziqi.cn

[Q21] 空值判断
来源：http://vke.yj20258888.top

SELECT * FROM users WHERE email IS NULL;
来源：http://hlq.cucudq.cn

[Q22] 排序
来源：http://cmi.mhx1999.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hvu.jianghu66.top

[Q23] 分页
来源：http://pnn.yvedp.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://fjx.hammf.cn

[Q24] 去重
来源：http://ccn.tianlin.xyz

SELECT DISTINCT city FROM users;
来源：http://ptp.fehbvm.com

[Q25] 只取前 N 条
来源：http://zix.xylfe.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://yex.tianlin.xyz

[Q26] 计数
来源：http://rdw.pengpengdd.cyou

SELECT COUNT(*) FROM users;
来源：http://vch.sysykeji.top

[Q27] 条件计数
来源：http://lda.tarul.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://jcx.zhongyouzk.top

[Q28] 求和与平均
来源：http://jov.jinqigufen.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://rsw.xingfuxueyuan.xyz

[Q29] 最大最小值
来源：http://zbi.316326.xyz

SELECT MAX(age), MIN(age) FROM users;
来源：http://cgb.jqgufenzy.top

[Q30] 分组统计
来源：http://dij.hammf.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://doy.jinghuilouyu.cn

[Q31] 分组后过滤
来源：http://uzu.yj20258.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ubj.xuetiantiany.cn

[Q32] 分组拼接字符串
来源：http://kkh.vehdjk.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hqu.gaohongyu789.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://lzn.ppjwa.cn

[Q33] 多列分组
来源：http://vhj.dianchejie.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hws.yangfankeji.com

[Q34] 每组取第一条
来源：http://sfs.yvedp.cn

SELECT * FROM (
来源：http://ndi.c1oappe.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ovz.xuetiantiany.cn

) t WHERE rn = 1;
来源：http://czh.yj20258.top

[Q35] 内连接
来源：http://qao.jqgufenzy.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://iuq.quarkkingdee.top

[Q36] 左连接
来源：http://civ.ydjk.org.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://rdb.birdmap.top

[Q37] 右连接
来源：http://fpg.feifeiyinyue.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://kob.redwolf501.top

[Q38] 全外连接（PostgreSQL）
来源：http://wrr.daria6918.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://dap.chenlongwang.top

[Q39] 自连接（查上下级）
来源：http://oqz.vehdjk.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://tht.nanxuanxn.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://iog.svipenyu.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://euj.haohaochexian.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://sby.daxiang520.top

[Q41] 多表连接
来源：http://tol.redwolf501.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://svn.pengpengdd.cyou

JOIN users u ON u.id = o.user_id
来源：http://hnx.xziqi.cn

JOIN products p ON p.id = o.product_id;
来源：http://gsg.nanxinkj.top

[Q42] 连接条件附加过滤
来源：http://vao.aibaodan.cn

SELECT u.name, o.amount FROM users u
来源：http://czs.xylfe.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ngu.jianghu66.top

[Q43] 标量子查询
来源：http://syd.zhongyouzk.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hgp.yangfankeji.com

[Q44] IN 子查询
来源：http://jtr.aizwys.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://suh.yvedp.cn

[Q45] EXISTS 判断存在
来源：http://pyf.yonumen.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://nne.jyoumei.cn

[Q46] NOT EXISTS 判断不存在
来源：http://tnh.zdqjudy.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://piy.shanyushiyangkeji.top

[Q47] 与平均值比较
来源：http://rlq.zdbjq.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://pdv.shzxlz.cn

[Q48] CTE 公用表表达式
来源：http://gwa.andypj.xyz

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://pga.ydjk.org.cn

SELECT * FROM t WHERE c > 5;
来源：http://jxd.hysaishi.cn

[Q49] 更新单行
来源：http://mdw.ywan-chungtsiang.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://zol.zhengqikj.top

[Q50] 批量更新
来源：http://znj.yuanzhike.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wnr.cqqwz.cn

[Q51] 用子查询更新
来源：http://mjt.guowangkeji.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blr.meibo888.top

[Q52] 删除指定行
来源：http://ycu.smart0.xyz

DELETE FROM users WHERE id = 10;
来源：http://dtn.xuetiantiany.cn

[Q53] 按条件删除
来源：http://kvn.xingfuxueyuan.xyz

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://obf.tarul.cn

[Q54] 清空表
来源：http://bxq.xziqi.cn

TRUNCATE TABLE logs;
来源：http://djq.nwbrower.top

[Q55] 排名（并列占位）
来源：http://jsy.hongshengwenyu.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://itl.aibaodan.cn

[Q56] 密集排名（并列不占位）
来源：http://brb.yuxming.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://kiz.zhiwuduotai.top

[Q57] 行号
来源：http://qat.sxryk.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://zgk.yj202588.top

[Q58] 累计求和
来源：http://koq.wangdashe.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mbm.mhx1999.top

[Q59] 分组内累计
来源：http://hek.cashguo.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wtg.tian-w.cn

[Q60] 取上一行 / 下一行
来源：http://hsc.yueranfly.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://vpv.jqgufenzy.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://nfe.feifeiyinyue.top

[Q61] 移动平均
来源：http://clk.snrcjt.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://zvi.hysaishi.cn

[Q62] 分组占比
来源：http://ydu.shzxlz.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://gox.hnxiangtu.top

[Q63] 开启事务
来源：http://wbw.shangyingyoupin.top

START TRANSACTION;                -- 或 BEGIN
来源：http://lew.jiagoushi.top

[Q64] 提交事务
来源：http://alk.zdqjudy.top

COMMIT;
来源：http://kir.smart0.xyz

[Q65] 回滚事务
来源：http://knn.hysaishi.cn

ROLLBACK;
来源：http://yiz.zhiwuduotai.top

[Q66] 行锁查询
来源：http://pqh.cashguo.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://cps.yuanzhike.top

[Q67] 设置隔离级别
来源：http://men.kuanghao11.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ytx.zdbjq.cn

[Q68] 保存点
来源：http://hjd.shzxlz.cn

SAVEPOINT sp1;
来源：http://nnj.pengpengdd.cyou

ROLLBACK TO sp1;
来源：http://xlu.jinghuilouyu.cn

[Q69] 查看执行计划
来源：http://rqw.cucudq.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wjf.xinyue.icu

[Q70] 更新统计信息
来源：http://eja.hammf.cn

ANALYZE TABLE users;
来源：http://avg.hcnkem.com

[Q71] 查看建表语句
来源：http://hwz.redwolf501.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://rlx.wangdashe.top

[Q72] 查看索引
来源：http://vcc.jinghuilouyu.cn

SHOW INDEX FROM users;
来源：http://ohg.shanyushiyangtech.top

[Q73] 查看表状态
来源：http://mtc.epnwcf.com

SHOW TABLE STATUS LIKE 'users';
来源：http://kvt.quarkkingdee.top

[Q74] 强制使用索引
来源：http://nhh.shzxlz.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://gia.vqdsnc.cn

[Q75] 日期格式化
来源：http://wdk.xziqi.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://rbj.xuanzx.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://jcp.gogol.net.cn

[Q76] 按天统计
来源：http://urz.hesvh.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://xhr.ehwqpu.com

[Q77] 时间加减
来源：http://vxo.gogol.net.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://fwy.dianchejie.cn

[Q78] 当前时间
来源：http://hif.jqgfzy.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://lti.redwolf501.top

[Q79] 字符串拼接
来源：http://zef.9152youxi.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://sbh.ehwqpu.com

[Q80] 字符串截取
来源：http://xsu.dianchejie.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://unj.yj202588.top

[Q81] 字符串替换
来源：http://cbh.ctjpmb.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://tqg.sjlbkw.cn

[Q82] 字符长度与字节长度
来源：http://eas.andypj.xyz

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ptr.xuanzx.com

[Q83] 大小写转换
来源：http://gpk.wangshuangyany.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://jyl.tarul.cn

[Q84] 去除首尾空格
来源：http://vkb.316326.xyz

SELECT TRIM(name) FROM users;
来源：http://zzk.chenjidiqi.icu

[Q85] 数值取整
来源：http://lei.wangshuangyany.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://bnu.c1oappe.top

[Q86] 读取 JSON 字段
来源：http://uhq.fehbvm.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://uic.feifeiyinyue.top

[Q87] JSON 字段做条件
来源：http://vhw.bbcook.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://inr.aibaodan.cn

[Q88] 行转列（条件聚合）
来源：http://fht.zhijiandao.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://tjx.fengsongda.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ugd.havefunace.top

[Q89] 判断表是否存在
来源：http://acy.snrcjt.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://jid.52xcode.cn

[Q90] 生成序号列
来源：http://scc.daxiang520.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://uiq.zycfv.cn

================================================================================
来源：http://std.zycfv.cn

R. Bash 专题
来源：http://fug.jqgfzy.top

================================================================================
来源：http://jdv.9152youxi.cn

[R01] shebang 与严格模式
来源：http://zvf.wangshuangyany.cn

#!/usr/bin/env bash
来源：http://zif.hongshengwenyu.top

set -euo pipefail
来源：http://bmx.nanxinkj.top

[R02] 变量赋值与使用
来源：http://wxw.nanxinkj.top

name="Tom"; echo "$name"
来源：http://rar.zhijiandao.cn

[R03] 只读变量
来源：http://pxz.sufxvd.cn

readonly PI=3.14
来源：http://dsi.nwbrower.top

[R04] 位置参数
来源：http://vll.yuanzhike.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://vcl.jinqigufen.top

[R05] 参数默认值
来源：http://htn.xingfuxueyuan.xyz

name="${1:-default}"
来源：http://nzq.guannengcc.top

[R06] 判断命令是否存在
来源：http://ziy.cashguo.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://udf.zhijiandao.cn

[R07] if 判断文件
来源：http://nkf.shuidangran.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mlv.ppjwa.cn

[R08] 数值比较
来源：http://and.ppjwa.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://hmd.hywenlv.cn

[R09] 字符串比较
来源：http://doo.dianchejie.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://fzq.tarul.cn

[R10] 正则匹配
来源：http://wmz.fanxiaobao.xyz

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://har.zhijiandao.cn

[R11] case 多分支
来源：http://yfd.yuanzhike.top

case "$1" in
来源：http://sxb.shangyingyoupin.top

start) echo "启动" ;;
来源：http://pfv.guannengcc.top

stop)  echo "停止" ;;
来源：http://kdf.feifeiyinyue.top

*)     echo "未知命令" ;;
来源：http://tdg.cdnleiting.top

esac
来源：http://goh.tarul.cn

[R12] for 遍历文件
来源：http://rvw.meibo888.top

for f in *.txt; do echo "$f"; done
来源：http://eqx.jinqigufen.top

[R13] for 计数循环
来源：http://hit.fzhhl.top

for i in {1..10}; do echo "$i"; done
来源：http://fdj.iojbl.cn

[R14] C 风格 for
来源：http://lhy.fktsv.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://xri.pycfn.com

[R15] while 逐行读文件
来源：http://scb.shangyingyoupin.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://dta.dashuyun.cn

[R16] until 等待条件
来源：http://mjm.9152youxi.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://gdl.hnqzz.top

[R17] 数组定义与取值
来源：http://zoh.xuetiantiany.cn

arr=(a b c); echo "${arr[0]}"
来源：http://qmv.cheryme.top

[R18] 遍历数组
来源：http://wmq.aibaodan.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://aks.jinqigfzy.top

[R19] 数组长度
来源：http://miu.fzhhl.top

echo "${#arr[@]}"
来源：http://wwd.hcnkem.com

[R20] 关联数组（字典）
来源：http://pgj.zdqjudy.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://viw.yueranfly.top

[R21] 字符串长度
来源：http://tit.vehdjk.com

echo "${#s}"
来源：http://sef.tian-w.cn

[R22] 截取子串
来源：http://dhn.daxiang520.top

echo "${s:0:5}"
来源：http://uff.yj20258.top

[R23] 字符串替换
来源：http://ixs.shuidangran.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wpm.gaohongyu789.top

[R24] 大小写转换
来源：http://ioy.vehdjk.com

echo "${s^^}"; echo "${s,,}"
来源：http://iko.yangfankeji.com

[R25] 去后缀 / 去前缀
来源：http://sqs.jianghu66.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://ejr.yuxming.cn

[R26] 命令替换
来源：http://igx.yj20258888.top

now=$(date +%F); echo "$now"
来源：http://wge.ywan-chungtsiang.top

[R27] 算术展开
来源：http://jzc.cqqwz.cn

echo $((1 + 2 * 3))
来源：http://jtb.bjfxy.top

[R28] 浮点运算
来源：http://sri.wangdashe.top

echo "scale=2; 10/3" | bc
来源：http://slv.ydzc1.top

[R29] 定义函数
来源：http://yzp.xinyue.icu

add() { echo $(($1 + $2)); }; add 1 2
来源：http://arj.haohaochexian.top

[R30] 函数返回状态码
来源：http://jjg.zdqjudy.top

f() { return 0; }; f || echo "失败了"
来源：http://iut.gotoacloud.top

[R31] 局部变量
来源：http://ast.zdbjq.cn

f() { local x=1; echo "$x"; }
来源：http://ehd.quarkkingdee.top

[R32] 参数个数校验
来源：http://xki.pycfn.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://nix.hywenlv.cn

[R33] 捕获错误并提示行号
来源：http://bkp.xingfuxueyuan.xyz

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://rqg.sjlbkw.cn

[R34] 退出时清理
来源：http://gwx.hywenlv.cn

trap 'rm -f "$tmp"' EXIT
来源：http://mvm.guowangkeji.top

[R35] 后台执行并等待
来源：http://svx.shangyingyoupin.top

sleep 5 & pid=$!; wait "$pid"
来源：http://faq.316326.xyz

[R36] 并发执行多个任务
来源：http://bzr.smart0.xyz

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://xid.fengsongda.top

[R37] 把输出赋给变量
来源：http://wex.yuanzhike.top

files=$(ls -1)
来源：http://xje.dianchejie.cn

[R38] 管道串联
来源：http://zix.havefunace.top

cat a.txt | grep -i error | wc -l
来源：http://kcr.52xcode.cn

[R39] 重定向标准输出与错误
来源：http://osu.shuidangran.top

cmd > out.log 2>&1
来源：http://qfs.zdqjudy.top

[R40] 追加写日志
来源：http://byg.ehwqpu.com

echo "log" >> out.log
来源：http://biv.nwbrower.top

[R41] 丢弃输出
来源：http://dcp.yanxiufei.cn

cmd >/dev/null 2>&1
来源：http://saf.meibo888.top

[R42] 输入重定向
来源：http://ujj.pengpengdd.cyou

wc -l < a.txt
来源：http://ple.hfpthk.cn

[R43] 按名字查找文件
来源：http://rbr.ppjwa.cn


<!-- 参考信息 -->