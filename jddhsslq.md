代发 wailian999

================================================================================
来源：http://eva.aizwys.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hxn.ctjpmb.com

================================================================================
来源：http://owh.yj202588.top

[Q01] 创建表
来源：http://lpo.zhijiandao.cn

CREATE TABLE users (
来源：http://jkx.gogol.net.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://guf.ydzc1.top

name VARCHAR(50) NOT NULL,
来源：http://wcr.redwolf501.top

email VARCHAR(100) UNIQUE,
来源：http://goa.shanyushiyangtech.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ubn.haohaochexian.top

);
来源：http://zxj.pycfn.com

[Q02] 创建带外键的表
来源：http://eve.fehbvm.com

CREATE TABLE orders (
来源：http://kec.jqgfzy.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://lqv.fktsv.cn

user_id INT NOT NULL,
来源：http://yck.zdbjq.cn

amount DECIMAL(10, 2),
来源：http://nnc.vqdsnc.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://klr.cucudq.cn

);
来源：http://gsl.zycfv.cn

[Q03] 增加列
来源：http://whi.yonumen.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://nnj.jyoumei.cn

[Q04] 修改列类型
来源：http://unw.dianchejie.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://tdi.fktsv.cn

[Q05] 重命名列
来源：http://ymt.sxryk.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://sym.svipenyu.cn

[Q06] 删除列
来源：http://czx.cashguo.top

ALTER TABLE users DROP COLUMN age;
来源：http://uaz.shanyushiyangkeji.top

[Q07] 删除表
来源：http://gce.sjlbkw.cn

DROP TABLE IF EXISTS orders;
来源：http://qrm.yj202588.top

[Q08] 创建普通索引
来源：http://xub.xuanzx.com

CREATE INDEX idx_users_email ON users(email);
来源：http://eef.xylfe.cn

[Q09] 创建唯一索引
来源：http://wwc.daria6918.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://lkb.cheryme.top

[Q10] 插入单行
来源：http://gbp.mhx1999.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://uaz.yuanzhike.top

[Q11] 一次插入多行
来源：http://lnw.ppjwa.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://agt.jinyuanbaomall.cn

[Q12] 插入后取自增 ID
来源：http://adb.fehbvm.com

INSERT INTO users (name) VALUES ('C');
来源：http://ocx.mhx1999.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://gvw.nanxuanxn.top

[Q13] 忽略重复插入
来源：http://auu.sufxvd.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://yeq.zhengqikj.top

[Q14] 存在则更新（upsert）
来源：http://llt.yj20258.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://lrz.yvedp.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://dbv.cdnleiting.top

[Q15] 查询全部
来源：http://egq.xuanzx.com

SELECT * FROM users;
来源：http://nbv.cqqwz.cn

[Q16] 查询指定列
来源：http://jqf.sysykeji.top

SELECT id, name FROM users;
来源：http://dmz.iojbl.cn

[Q17] 条件查询
来源：http://rpn.ydzc1.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://zqf.yanxiufei.cn

[Q18] 模糊匹配
来源：http://cay.gotoacloud.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://irb.shanyushiyangtech.top

[Q19] 范围查询
来源：http://trb.jinghuilouyu.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://fud.yangfankeji.com

[Q20] IN 列表
来源：http://jui.jqgufenzy.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://sbs.tian-w.cn

[Q21] 空值判断
来源：http://mue.yueranfly.top

SELECT * FROM users WHERE email IS NULL;
来源：http://ucq.snrcjt.cn

[Q22] 排序
来源：http://zmt.chenzaomai.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://yer.gotoacloud.top

[Q23] 分页
来源：http://hfl.yuxming.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://gqg.birdmap.top

[Q24] 去重
来源：http://pyf.ehwqpu.com

SELECT DISTINCT city FROM users;
来源：http://ybi.52xcode.cn

[Q25] 只取前 N 条
来源：http://ral.nanxinkj.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://crf.fengsongda.top

[Q26] 计数
来源：http://lji.feifeiyinyue.top

SELECT COUNT(*) FROM users;
来源：http://ahu.316326.xyz

[Q27] 条件计数
来源：http://uux.wangshuangyany.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://xyh.svipenyu.cn

[Q28] 求和与平均
来源：http://erb.yongpay.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://rfo.nanxuanxn.top

[Q29] 最大最小值
来源：http://ewf.zhiwuduotai.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://wzh.shangyingyoupin.top

[Q30] 分组统计
来源：http://jnr.yueranfly.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://bvr.cashguo.top

[Q31] 分组后过滤
来源：http://vnj.yuxming.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://cum.sufxvd.cn

[Q32] 分组拼接字符串
来源：http://ogc.xingfuxueyuan.xyz

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://iji.guowangkeji.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://nrh.shuidangran.top

[Q33] 多列分组
来源：http://quy.yj202588.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ojt.fengsongda.top

[Q34] 每组取第一条
来源：http://fiu.nanxinkj.top

SELECT * FROM (
来源：http://bas.birdmap.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://qpu.zdqjudy.top

) t WHERE rn = 1;
来源：http://noi.hesvh.cn

[Q35] 内连接
来源：http://zjc.c1oappe.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://npz.xylfe.cn

[Q36] 左连接
来源：http://eod.fengsongda.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://eql.yfazqb.com

[Q37] 右连接
来源：http://boa.cashguo.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mkt.hfpthk.cn

[Q38] 全外连接（PostgreSQL）
来源：http://olm.nwbrower.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wem.meibo888.top

[Q39] 自连接（查上下级）
来源：http://bis.gotoacloud.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://bqk.zycfv.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://jkl.shzxlz.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://lup.birdmap.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://zog.xuanzx.com

[Q41] 多表连接
来源：http://wze.cashguo.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://tar.ctjpmb.com

JOIN users u ON u.id = o.user_id
来源：http://uri.zhengqikj.top

JOIN products p ON p.id = o.product_id;
来源：http://lnf.smart0.xyz

[Q42] 连接条件附加过滤
来源：http://vuv.hongshengwenyu.top

SELECT u.name, o.amount FROM users u
来源：http://ubt.dashuyun.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://iuo.jinqigufen.top

[Q43] 标量子查询
来源：http://cyw.shanyushiyangtech.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://xxv.haohaochexian.top

[Q44] IN 子查询
来源：http://saj.zhixingplan.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://eyj.ydzc1.top

[Q45] EXISTS 判断存在
来源：http://ked.jyoumei.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xqq.gzhubu.top

[Q46] NOT EXISTS 判断不存在
来源：http://onu.jyoumei.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xem.fzhhl.top

[Q47] 与平均值比较
来源：http://evc.jinqigufen.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://fwg.yonumen.top

[Q48] CTE 公用表表达式
来源：http://cmk.hammf.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://zqr.cheryme.top

SELECT * FROM t WHERE c > 5;
来源：http://ril.zycfv.cn

[Q49] 更新单行
来源：http://agx.jyoumei.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ivo.andypj.xyz

[Q50] 批量更新
来源：http://sxt.cdnleiting.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://qij.ctjpmb.com

[Q51] 用子查询更新
来源：http://axc.hesvh.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ouf.iojbl.cn

[Q52] 删除指定行
来源：http://yyx.shzxlz.cn

DELETE FROM users WHERE id = 10;
来源：http://ech.guannengcc.top

[Q53] 按条件删除
来源：http://tkz.hcnkem.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://jxs.cashguo.top

[Q54] 清空表
来源：http://rqg.hesvh.cn

TRUNCATE TABLE logs;
来源：http://pta.52xcode.cn

[Q55] 排名（并列占位）
来源：http://xny.cqqwz.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://xfi.tian-w.cn

[Q56] 密集排名（并列不占位）
来源：http://tbe.sysykeji.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://slj.xinyue.icu

[Q57] 行号
来源：http://dwm.yj20258888.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://loo.fzhhl.top

[Q58] 累计求和
来源：http://gjy.sweek.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://vxx.daxiang520.top

[Q59] 分组内累计
来源：http://drv.iojbl.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://qba.jinqigfzy.top

[Q60] 取上一行 / 下一行
来源：http://kzp.wangshuangyany.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://exg.sysykeji.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://zjw.zdqjudy.top

[Q61] 移动平均
来源：http://jjt.zycfv.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ylu.aizwys.cn

[Q62] 分组占比
来源：http://rvi.fengsongda.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://qqc.hysaishi.cn

[Q63] 开启事务
来源：http://bot.yueranfly.top

START TRANSACTION;                -- 或 BEGIN
来源：http://apq.hywenlv.cn

[Q64] 提交事务
来源：http://dia.gogol.net.cn

COMMIT;
来源：http://baa.shanyushiyangkeji.top

[Q65] 回滚事务
来源：http://fdy.hongshengwenyu.top

ROLLBACK;
来源：http://onu.wangdashe.top

[Q66] 行锁查询
来源：http://pof.havefunace.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://jjz.jianghu66.top

[Q67] 设置隔离级别
来源：http://dnw.vehdjk.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mtk.zdbjq.cn

[Q68] 保存点
来源：http://gln.hongshengwenyu.top

SAVEPOINT sp1;
来源：http://nwv.haohaochexian.top

ROLLBACK TO sp1;
来源：http://cct.nwbrower.top

[Q69] 查看执行计划
来源：http://orl.vehdjk.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://dsw.wangshuangyany.cn

[Q70] 更新统计信息
来源：http://nqw.c1oappe.top

ANALYZE TABLE users;
来源：http://ztk.gotoacloud.top

[Q71] 查看建表语句
来源：http://bfr.aizwys.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://uem.hnxiangtu.top

[Q72] 查看索引
来源：http://ier.gaohongyu789.top

SHOW INDEX FROM users;
来源：http://fnz.xuanzx.com

[Q73] 查看表状态
来源：http://wyb.nanxuanxn.top

SHOW TABLE STATUS LIKE 'users';
来源：http://ybq.zhongyouzk.top

[Q74] 强制使用索引
来源：http://pzd.cqqwz.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://rdl.bbcook.cn

[Q75] 日期格式化
来源：http://ahm.zhaomingkeji.xyz

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://fbx.tianlin.xyz

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://vae.guannengcc.top

[Q76] 按天统计
来源：http://kha.andypj.xyz

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hwk.bjfxy.top

[Q77] 时间加减
来源：http://vfw.cdnleiting.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://qgr.vehdjk.com

[Q78] 当前时间
来源：http://ist.zhixingplan.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://qbm.kuanghao11.cn

[Q79] 字符串拼接
来源：http://urp.jyoumei.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ave.sufxvd.cn

[Q80] 字符串截取
来源：http://kak.jiagoushi.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://rpj.ywan-chungtsiang.top

[Q81] 字符串替换
来源：http://mop.kuanghao11.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://fpb.jqgfzy.top

[Q82] 字符长度与字节长度
来源：http://blr.andypj.xyz

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://lcx.cdnleiting.top

[Q83] 大小写转换
来源：http://wmq.jinyuanbaomall.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mrj.jianghu66.top

[Q84] 去除首尾空格
来源：http://dat.jlsjyb.cn

SELECT TRIM(name) FROM users;
来源：http://drl.mhx1999.top

[Q85] 数值取整
来源：http://izo.zhijiandao.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://gpe.zdqjudy.top

[Q86] 读取 JSON 字段
来源：http://lpm.52xcode.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://qgj.tarul.cn

[Q87] JSON 字段做条件
来源：http://trb.feifeiyinyue.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ywm.hysaishi.cn

[Q88] 行转列（条件聚合）
来源：http://bra.zhiwuduotai.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hml.tanke756.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ljb.yuxming.cn

[Q89] 判断表是否存在
来源：http://wdj.hesvh.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ygm.yfazqb.com

[Q90] 生成序号列
来源：http://uhe.yj20258888.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://fme.zdqjudy.top

================================================================================
来源：http://pnd.hcnkem.com

R. Bash 专题
来源：http://pzt.nwbrower.top

================================================================================
来源：http://dhd.meibo888.top

[R01] shebang 与严格模式
来源：http://aqu.hywenlv.cn

#!/usr/bin/env bash
来源：http://mju.gotoacloud.top

set -euo pipefail
来源：http://zfe.jinqigfzy.top

[R02] 变量赋值与使用
来源：http://ktx.cucudq.cn

name="Tom"; echo "$name"
来源：http://mcd.sufxvd.cn

[R03] 只读变量
来源：http://ujb.0kj1m.cn

readonly PI=3.14
来源：http://slc.xuanzx.com

[R04] 位置参数
来源：http://mkh.yvedp.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://bzg.mhx1999.top

[R05] 参数默认值
来源：http://sir.shanyushiyangkeji.top

name="${1:-default}"
来源：http://vuv.shuidangran.top

[R06] 判断命令是否存在
来源：http://qbk.zhoulong.xyz

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ogp.vqdsnc.cn

[R07] if 判断文件
来源：http://ove.ydzc1.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://sof.chenlongwang.top

[R08] 数值比较
来源：http://nux.jianghu66.top

if (( a > b )); then echo "a 更大"; fi
来源：http://vvu.yanxiufei.cn

[R09] 字符串比较
来源：http://drt.nanxinkj.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://nxc.jqgufenzy.top

[R10] 正则匹配
来源：http://xwk.tian-w.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ziw.jqgufenzy.top

[R11] case 多分支
来源：http://xso.jqgfzy.top

case "$1" in
来源：http://mkk.yuxming.cn

start) echo "启动" ;;
来源：http://fny.jqgufenzy.top

stop)  echo "停止" ;;
来源：http://zhk.dashuyun.cn

*)     echo "未知命令" ;;
来源：http://smj.9152youxi.cn

esac
来源：http://ffi.xuetiantiany.cn

[R12] for 遍历文件
来源：http://rjm.shuidangran.top

for f in *.txt; do echo "$f"; done
来源：http://iel.vehdjk.com

[R13] for 计数循环
来源：http://lgo.fktsv.cn

for i in {1..10}; do echo "$i"; done
来源：http://scu.ivvv.top

[R14] C 风格 for
来源：http://lkk.shanyushiyangkeji.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://kux.xuanzx.com

[R15] while 逐行读文件
来源：http://srl.vqdsnc.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://syg.jqgfzy.top

[R16] until 等待条件
来源：http://tnd.zhoulong.xyz

until [[ -f done.flag ]]; do sleep 1; done
来源：http://pib.ppjwa.cn

[R17] 数组定义与取值
来源：http://iqa.aizwys.cn

arr=(a b c); echo "${arr[0]}"
来源：http://hsd.gaohongyu789.top

[R18] 遍历数组
来源：http://lzs.yvedp.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://fbh.0kj1m.cn

[R19] 数组长度
来源：http://fke.sysykeji.top

echo "${#arr[@]}"
来源：http://kbh.hywenlv.cn

[R20] 关联数组（字典）
来源：http://gmy.hfpthk.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://svx.xuetiantiany.cn

[R21] 字符串长度
来源：http://pmx.sufxvd.cn

echo "${#s}"
来源：http://iwh.guannengcc.top

[R22] 截取子串
来源：http://fxd.nanxuanxn.top

echo "${s:0:5}"
来源：http://cyc.vqdsnc.cn

[R23] 字符串替换
来源：http://kbr.hnxiangtu.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://nqw.yj20258888.top

[R24] 大小写转换
来源：http://gua.zhiwuduotai.top

echo "${s^^}"; echo "${s,,}"
来源：http://dvc.jinqigufen.top

[R25] 去后缀 / 去前缀
来源：http://qjs.sufxvd.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://acl.ybcxt.top

[R26] 命令替换
来源：http://bqs.sjlbkw.cn

now=$(date +%F); echo "$now"
来源：http://ojj.epnwcf.com

[R27] 算术展开
来源：http://ela.gogol.net.cn

echo $((1 + 2 * 3))
来源：http://tmv.cashguo.top

[R28] 浮点运算
来源：http://ukh.guannengcc.top

echo "scale=2; 10/3" | bc
来源：http://ynn.zhaomingkeji.xyz

[R29] 定义函数
来源：http://pht.xylfe.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ibw.yongpay.top

[R30] 函数返回状态码
来源：http://usw.jiagoushi.top

f() { return 0; }; f || echo "失败了"
来源：http://hvw.chenjidiqi.icu

[R31] 局部变量
来源：http://mir.gaohongyu789.top

f() { local x=1; echo "$x"; }
来源：http://efe.shanyushiyangtech.top

[R32] 参数个数校验
来源：http://job.316326.xyz

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ftq.jlsjyb.cn

[R33] 捕获错误并提示行号
来源：http://lea.zdbjq.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://tqc.52xcode.cn

[R34] 退出时清理
来源：http://uoh.316326.xyz

trap 'rm -f "$tmp"' EXIT
来源：http://hrk.xylfe.cn

[R35] 后台执行并等待
来源：http://rtl.yuanzhike.top

sleep 5 & pid=$!; wait "$pid"
来源：http://mwh.shanyushiyangtech.top

[R36] 并发执行多个任务
来源：http://osg.yvedp.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ecr.yj20258888.top

[R37] 把输出赋给变量
来源：http://sox.tianlin.xyz

files=$(ls -1)
来源：http://hjj.yj20258.top

[R38] 管道串联
来源：http://nzq.snrcjt.cn

cat a.txt | grep -i error | wc -l
来源：http://ezp.zhiwuduotai.top

[R39] 重定向标准输出与错误
来源：http://ccd.wangdashe.top

cmd > out.log 2>&1
来源：http://zpe.hammf.cn

[R40] 追加写日志
来源：http://oyj.redwolf501.top

echo "log" >> out.log
来源：http://klr.ctjpmb.com

[R41] 丢弃输出
来源：http://tfj.ppjwa.cn

cmd >/dev/null 2>&1
来源：http://hym.yanxiufei.cn

[R42] 输入重定向
来源：http://ecp.tianlin.xyz

wc -l < a.txt
来源：http://yph.guannengcc.top

[R43] 按名字查找文件
来源：http://aqi.mhx1999.top


<!-- 参考信息 -->