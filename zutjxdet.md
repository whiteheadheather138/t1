代发 wailian999

CREATE TABLE users (
来源：http://hwq.meibo888.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wqp.pycfn.com

name VARCHAR(50) NOT NULL,
来源：http://nua.jlsjyb.cn

email VARCHAR(100) UNIQUE,
来源：http://xhi.epnwcf.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://muh.9152youxi.cn

);
来源：http://vsn.aizwys.cn

[Q02] 创建带外键的表
来源：http://efa.sweek.top

CREATE TABLE orders (
来源：http://eif.fanxiaobao.xyz

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hwj.yanxiufei.cn

user_id INT NOT NULL,
来源：http://zjd.smart0.xyz

amount DECIMAL(10, 2),
来源：http://kjt.daria6918.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://eoj.hcnkem.com

);
来源：http://jhq.yj20258888.top

[Q03] 增加列
来源：http://zfs.epnwcf.com

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ceu.xingfuxueyuan.xyz

[Q04] 修改列类型
来源：http://bwy.aizwys.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ehm.feifeiyinyue.top

[Q05] 重命名列
来源：http://cqh.redwolf501.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://nrb.chenjidiqi.icu

[Q06] 删除列
来源：http://zjg.daxiang520.top

ALTER TABLE users DROP COLUMN age;
来源：http://eln.jinyuanbaomall.cn

[Q07] 删除表
来源：http://tmv.yuanzhike.top

DROP TABLE IF EXISTS orders;
来源：http://hfo.316326.xyz

[Q08] 创建普通索引
来源：http://pqd.cucudq.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://xbk.hnqzz.top

[Q09] 创建唯一索引
来源：http://vkl.jianghu66.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://psx.aibaodan.cn

[Q10] 插入单行
来源：http://prv.hongshengwenyu.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://yzc.316326.xyz

[Q11] 一次插入多行
来源：http://yxm.cqqwz.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://xxk.gogol.net.cn

[Q12] 插入后取自增 ID
来源：http://acx.sufxvd.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ydi.mhx1999.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://upb.316326.xyz

[Q13] 忽略重复插入
来源：http://bjb.zycfv.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://pam.xylfe.cn

[Q14] 存在则更新（upsert）
来源：http://fkn.sufxvd.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://czy.zhixingplan.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://kyp.fengsongda.top

[Q15] 查询全部
来源：http://orp.yj20258.top

SELECT * FROM users;
来源：http://eie.dashuyun.cn

[Q16] 查询指定列
来源：http://taj.redwolf501.top

SELECT id, name FROM users;
来源：http://foa.yj20258.top

[Q17] 条件查询
来源：http://fyw.316326.xyz

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://lxd.shanyushiyangtech.top

[Q18] 模糊匹配
来源：http://frg.hesvh.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://psv.yueranfly.top

[Q19] 范围查询
来源：http://jdu.hfpthk.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://oww.gzhubu.top

[Q20] IN 列表
来源：http://ohp.tanke756.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://dsc.jianghu66.top

[Q21] 空值判断
来源：http://tut.hnqzz.top

SELECT * FROM users WHERE email IS NULL;
来源：http://zlq.hfpthk.cn

[Q22] 排序
来源：http://frf.jqgfzy.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hio.gotoacloud.top

[Q23] 分页
来源：http://rmn.jianghu66.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://auq.shanyushiyangtech.top

[Q24] 去重
来源：http://hwe.guowangkeji.top

SELECT DISTINCT city FROM users;
来源：http://tzp.ppjwa.cn

[Q25] 只取前 N 条
来源：http://fec.52xcode.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://uiw.fanxiaobao.xyz

[Q26] 计数
来源：http://jov.haohaochexian.top

SELECT COUNT(*) FROM users;
来源：http://rue.smart0.xyz

[Q27] 条件计数
来源：http://jps.jinqigufen.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://obf.nanxuanxn.top

[Q28] 求和与平均
来源：http://cke.vehdjk.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://tnv.jqgfzy.top

[Q29] 最大最小值
来源：http://pnw.ctjpmb.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://epf.hysaishi.cn

[Q30] 分组统计
来源：http://cqd.fengsongda.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://jnn.fzhhl.top

[Q31] 分组后过滤
来源：http://wwv.xinyue.icu

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://eoo.vqdsnc.cn

[Q32] 分组拼接字符串
来源：http://gpm.316326.xyz

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://rcp.jianghu66.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://pgu.xuetiantiany.cn

[Q33] 多列分组
来源：http://ptu.cashguo.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://dbq.dashuyun.cn

[Q34] 每组取第一条
来源：http://lnn.nwbrower.top

SELECT * FROM (
来源：http://sud.xuanzx.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ktr.shangyingyoupin.top

) t WHERE rn = 1;
来源：http://qcb.ehwqpu.com

[Q35] 内连接
来源：http://und.hesvh.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://xqp.yonumen.top

[Q36] 左连接
来源：http://xzd.haohaochexian.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mth.zdbjq.cn

[Q37] 右连接
来源：http://fup.quarkkingdee.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://kez.ivvv.top

[Q38] 全外连接（PostgreSQL）
来源：http://mdz.shuidangran.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ila.zhixingplan.top

[Q39] 自连接（查上下级）
来源：http://ouq.shzxlz.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://zqb.zhongyouzk.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://zpk.9152youxi.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://cfd.cucudq.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://fot.gzhubu.top

[Q41] 多表连接
来源：http://zoz.pengpengdd.cyou

SELECT o.id, u.name, p.title FROM orders o
来源：http://jux.xingfuxueyuan.xyz

JOIN users u ON u.id = o.user_id
来源：http://fof.cqqwz.cn

JOIN products p ON p.id = o.product_id;
来源：http://jkj.tianlin.xyz

[Q42] 连接条件附加过滤
来源：http://jwn.svipenyu.cn

SELECT u.name, o.amount FROM users u
来源：http://iia.quarkkingdee.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://fgh.fzhhl.top

[Q43] 标量子查询
来源：http://ldk.epnwcf.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://fzd.zhongyouzk.top

[Q44] IN 子查询
来源：http://dzq.ivvv.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://dxt.jianghu66.top

[Q45] EXISTS 判断存在
来源：http://lsb.snrcjt.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://owg.vehdjk.com

[Q46] NOT EXISTS 判断不存在
来源：http://zlu.ehwqpu.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://byg.nwbrower.top

[Q47] 与平均值比较
来源：http://fkz.wangdashe.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://kow.hammf.cn

[Q48] CTE 公用表表达式
来源：http://vpc.guannengcc.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://rii.sysykeji.top

SELECT * FROM t WHERE c > 5;
来源：http://zxb.sysykeji.top

[Q49] 更新单行
来源：http://ysr.0kj1m.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hny.jianghu66.top

[Q50] 批量更新
来源：http://duf.gzhubu.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://evr.uphjek.com

[Q51] 用子查询更新
来源：http://ozn.pengpengdd.cyou

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://lug.hnqzz.top

[Q52] 删除指定行
来源：http://orz.zhongyouzk.top

DELETE FROM users WHERE id = 10;
来源：http://smn.jlsjyb.cn

[Q53] 按条件删除
来源：http://zxh.sufxvd.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://qfj.xinyue.icu

[Q54] 清空表
来源：http://eml.ywan-chungtsiang.top

TRUNCATE TABLE logs;
来源：http://ivq.epnwcf.com

[Q55] 排名（并列占位）
来源：http://fag.tarul.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://xon.cucudq.cn

[Q56] 密集排名（并列不占位）
来源：http://szt.hywenlv.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://qsm.yj202588.top

[Q57] 行号
来源：http://tds.hesvh.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://bcv.jianghu66.top

[Q58] 累计求和
来源：http://wut.zdqjudy.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://vnk.hammf.cn

[Q59] 分组内累计
来源：http://dfg.xinyue.icu

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ssw.daria6918.cn

[Q60] 取上一行 / 下一行
来源：http://euy.ivvv.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://xoc.fktsv.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ghm.jqgufenzy.top

[Q61] 移动平均
来源：http://eku.hfpthk.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://cbr.yuxming.cn

[Q62] 分组占比
来源：http://nhx.nwbrower.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://xmg.sweek.top

[Q63] 开启事务
来源：http://gjw.uphjek.com

START TRANSACTION;                -- 或 BEGIN
来源：http://hui.andypj.xyz

[Q64] 提交事务
来源：http://wji.cdnleiting.top

COMMIT;
来源：http://ffa.hysaishi.cn

[Q65] 回滚事务
来源：http://wsj.zhaomingkeji.xyz

ROLLBACK;
来源：http://ruj.xylfe.cn

[Q66] 行锁查询
来源：http://isr.xuanzx.com

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://vex.jinghuilouyu.cn

[Q67] 设置隔离级别
来源：http://eue.iojbl.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://uwb.cucudq.cn

[Q68] 保存点
来源：http://fyq.shuidangran.top

SAVEPOINT sp1;
来源：http://jzh.nwbrower.top

ROLLBACK TO sp1;
来源：http://znr.yanxiufei.cn

[Q69] 查看执行计划
来源：http://lal.shanyushiyangtech.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hcp.shanyushiyangkeji.top

[Q70] 更新统计信息
来源：http://tzk.9152youxi.cn

ANALYZE TABLE users;
来源：http://xhh.xziqi.cn

[Q71] 查看建表语句
来源：http://hxc.xinyue.icu

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://vey.birdmap.top

[Q72] 查看索引
来源：http://sbl.wangdashe.top

SHOW INDEX FROM users;
来源：http://ini.redwolf501.top

[Q73] 查看表状态
来源：http://oxw.smart0.xyz

SHOW TABLE STATUS LIKE 'users';
来源：http://gxf.tanke756.top

[Q74] 强制使用索引
来源：http://ulk.dashuyun.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://orw.shanyushiyangkeji.top

[Q75] 日期格式化
来源：http://ybs.yangfankeji.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://zms.hysaishi.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://zqa.jyoumei.cn

[Q76] 按天统计
来源：http://mpj.sufxvd.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://myf.haohaochexian.top

[Q77] 时间加减
来源：http://vkm.aizwys.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://arj.xziqi.cn

[Q78] 当前时间
来源：http://ocl.kuanghao11.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mon.fktsv.cn

[Q79] 字符串拼接
来源：http://huk.yuxming.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://kuf.chenlongwang.top

[Q80] 字符串截取
来源：http://hyk.meibo888.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ioj.hywenlv.cn

[Q81] 字符串替换
来源：http://bej.cheryme.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://sja.yuanzhike.top

[Q82] 字符长度与字节长度
来源：http://vgf.nanxuanxn.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wow.tianlin.xyz

[Q83] 大小写转换
来源：http://guh.fengsongda.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://rou.hongshengwenyu.top

[Q84] 去除首尾空格
来源：http://eex.hfpthk.cn

SELECT TRIM(name) FROM users;
来源：http://wff.ivvv.top

[Q85] 数值取整
来源：http://cqy.fzhhl.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://jfj.hywenlv.cn

[Q86] 读取 JSON 字段
来源：http://mwz.shanyushiyangtech.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://pct.aizwys.cn

[Q87] JSON 字段做条件
来源：http://jol.yuanzhike.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://qfa.xziqi.cn

[Q88] 行转列（条件聚合）
来源：http://fij.gotoacloud.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://boo.xylfe.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://byx.redwolf501.top

[Q89] 判断表是否存在
来源：http://xvb.ivvv.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://uyv.yonumen.top

[Q90] 生成序号列
来源：http://uap.zhiwuduotai.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ehd.xylfe.cn

================================================================================
来源：http://sag.zhoulong.xyz

R. Bash 专题
来源：http://ifv.daria6918.cn

================================================================================
来源：http://dvs.sjlbkw.cn

[R01] shebang 与严格模式
来源：http://ndh.jinghuilouyu.cn

#!/usr/bin/env bash
来源：http://yjd.bbcook.cn

set -euo pipefail
来源：http://ppf.cheryme.top

[R02] 变量赋值与使用
来源：http://cth.svipenyu.cn

name="Tom"; echo "$name"
来源：http://fkc.wangdashe.top

[R03] 只读变量
来源：http://bpd.xziqi.cn

readonly PI=3.14
来源：http://xqb.yueranfly.top

[R04] 位置参数
来源：http://rhd.hongshengwenyu.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://err.hnqzz.top

[R05] 参数默认值
来源：http://bcb.jqgufenzy.top

name="${1:-default}"
来源：http://goq.nwbrower.top

[R06] 判断命令是否存在
来源：http://vuz.ybcxt.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://cox.dashuyun.cn

[R07] if 判断文件
来源：http://rpx.shuidangran.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://csv.zdqjudy.top

[R08] 数值比较
来源：http://qdw.xinyue.icu

if (( a > b )); then echo "a 更大"; fi
来源：http://why.zdqjudy.top

[R09] 字符串比较
来源：http://yre.quarkkingdee.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wkn.jlsjyb.cn

[R10] 正则匹配
来源：http://xmh.yj202588.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://omf.xziqi.cn

[R11] case 多分支
来源：http://kym.shanyushiyangkeji.top

case "$1" in
来源：http://wzg.hfpthk.cn

start) echo "启动" ;;
来源：http://fiw.smart0.xyz

stop)  echo "停止" ;;
来源：http://vuq.jqgufenzy.top

*)     echo "未知命令" ;;
来源：http://yah.bjfxy.top

esac
来源：http://nmw.hongshengwenyu.top

[R12] for 遍历文件
来源：http://xaw.zhaomingkeji.xyz

for f in *.txt; do echo "$f"; done
来源：http://bcv.ivvv.top

[R13] for 计数循环
来源：http://irx.chenjidiqi.icu

for i in {1..10}; do echo "$i"; done
来源：http://rpg.kuanghao11.cn

[R14] C 风格 for
来源：http://grc.zhiwuduotai.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://zta.yj20258888.top

[R15] while 逐行读文件
来源：http://ugv.jianghu66.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://sml.zhongyouzk.top

[R16] until 等待条件
来源：http://aga.jinyuanbaomall.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://czk.wangshuangyany.cn

[R17] 数组定义与取值
来源：http://pap.chenlongwang.top

arr=(a b c); echo "${arr[0]}"
来源：http://emv.gogol.net.cn

[R18] 遍历数组
来源：http://gdg.shanyushiyangkeji.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://orn.hammf.cn

[R19] 数组长度
来源：http://bzo.cdnleiting.top

echo "${#arr[@]}"
来源：http://stw.xziqi.cn

[R20] 关联数组（字典）
来源：http://lam.nanxuanxn.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://oyv.svipenyu.cn

[R21] 字符串长度
来源：http://trt.shzxlz.cn

echo "${#s}"
来源：http://ofj.tarul.cn

[R22] 截取子串
来源：http://agv.sjlbkw.cn

echo "${s:0:5}"
来源：http://kam.wangdashe.top

[R23] 字符串替换
来源：http://ihp.cheryme.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://yus.havefunace.top

[R24] 大小写转换
来源：http://cgv.0kj1m.cn

echo "${s^^}"; echo "${s,,}"
来源：http://mxj.cucudq.cn

[R25] 去后缀 / 去前缀
来源：http://zza.yvedp.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://sab.fanxiaobao.xyz

[R26] 命令替换
来源：http://ici.daxiang520.top

now=$(date +%F); echo "$now"
来源：http://zhb.vqdsnc.cn

[R27] 算术展开
来源：http://mxs.hywenlv.cn

echo $((1 + 2 * 3))
来源：http://qqs.vqdsnc.cn

[R28] 浮点运算
来源：http://zja.meibo888.top

echo "scale=2; 10/3" | bc
来源：http://dfv.shuidangran.top

[R29] 定义函数
来源：http://lmb.sufxvd.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://eoc.yuxming.cn

[R30] 函数返回状态码
来源：http://oor.jlsjyb.cn

f() { return 0; }; f || echo "失败了"
来源：http://nis.hysaishi.cn

[R31] 局部变量
来源：http://ymp.tarul.cn

f() { local x=1; echo "$x"; }
来源：http://qom.daxiang520.top

[R32] 参数个数校验
来源：http://rfi.fengsongda.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://dxl.jianghu66.top

[R33] 捕获错误并提示行号
来源：http://fvs.xziqi.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ltt.ydzc1.top

[R34] 退出时清理
来源：http://erd.vqdsnc.cn

trap 'rm -f "$tmp"' EXIT
来源：http://kfa.ivvv.top

[R35] 后台执行并等待
来源：http://rjo.xingfuxueyuan.xyz

sleep 5 & pid=$!; wait "$pid"
来源：http://ofd.zhixingplan.top

[R36] 并发执行多个任务
来源：http://kvk.shangyingyoupin.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://unv.yvedp.cn

[R37] 把输出赋给变量
来源：http://beo.yfazqb.com

files=$(ls -1)
来源：http://fqj.vqdsnc.cn

[R38] 管道串联
来源：http://brr.yonumen.top

cat a.txt | grep -i error | wc -l
来源：http://tvk.kuanghao11.cn

[R39] 重定向标准输出与错误
来源：http://ejw.xuetiantiany.cn

cmd > out.log 2>&1
来源：http://yya.zhijiandao.cn

[R40] 追加写日志
来源：http://dyq.zdqjudy.top

echo "log" >> out.log
来源：http://icz.yj202588.top

[R41] 丢弃输出
来源：http://kjf.iojbl.cn

cmd >/dev/null 2>&1
来源：http://uvm.xuetiantiany.cn

[R42] 输入重定向
来源：http://xle.andypj.xyz

wc -l < a.txt
来源：http://pvw.yueranfly.top

[R43] 按名字查找文件
来源：http://xjm.wangshuangyany.cn

find . -name "*.log" -type f
来源：http://fxq.guannengcc.top

[R44] 按修改时间查找
来源：http://yjl.jinghuilouyu.cn

find . -mtime -7 -type f
来源：http://ljm.zdqjudy.top

[R45] 批量删除
来源：http://gux.hywenlv.cn


<!-- 参考信息 -->