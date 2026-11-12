代发 wailian999

================================================================================
来源：http://wyc.sxryk.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://eri.dashuyun.cn

================================================================================
来源：http://fqr.jqgfzy.top

[Q01] 创建表
来源：http://bxc.ywan-chungtsiang.top

CREATE TABLE users (
来源：http://ezo.hywenlv.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://qqd.aibaodan.cn

name VARCHAR(50) NOT NULL,
来源：http://gfe.nanxinkj.top

email VARCHAR(100) UNIQUE,
来源：http://cdw.pengpengdd.cyou

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://fab.ivvv.top

);
来源：http://ast.tianlin.xyz

[Q02] 创建带外键的表
来源：http://vfd.wangdashe.top

CREATE TABLE orders (
来源：http://oai.hongshengwenyu.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hgk.ydzc1.top

user_id INT NOT NULL,
来源：http://bfh.jinqigufen.top

amount DECIMAL(10, 2),
来源：http://vks.dashuyun.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://qib.316326.xyz

);
来源：http://hot.feifeiyinyue.top

[Q03] 增加列
来源：http://hfy.tanke756.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://usi.zhaomingkeji.xyz

[Q04] 修改列类型
来源：http://uym.hongshengwenyu.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mep.zhiwuduotai.top

[Q05] 重命名列
来源：http://mqq.guannengcc.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://rws.yuanzhike.top

[Q06] 删除列
来源：http://ves.zhixingplan.top

ALTER TABLE users DROP COLUMN age;
来源：http://sod.aibaodan.cn

[Q07] 删除表
来源：http://upm.cqqwz.cn

DROP TABLE IF EXISTS orders;
来源：http://qjk.zdbjq.cn

[Q08] 创建普通索引
来源：http://mgh.andypj.xyz

CREATE INDEX idx_users_email ON users(email);
来源：http://tol.svipenyu.cn

[Q09] 创建唯一索引
来源：http://hbv.hongshengwenyu.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://exz.zhengqikj.top

[Q10] 插入单行
来源：http://idr.hnxiangtu.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://itr.kuanghao11.cn

[Q11] 一次插入多行
来源：http://gos.fengsongda.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://lqy.shangyingyoupin.top

[Q12] 插入后取自增 ID
来源：http://dan.yvedp.cn

INSERT INTO users (name) VALUES ('C');
来源：http://tit.tarul.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://keq.xuetiantiany.cn

[Q13] 忽略重复插入
来源：http://wpu.sjlbkw.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://imm.svipenyu.cn

[Q14] 存在则更新（upsert）
来源：http://run.mhx1999.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://gzy.hnxiangtu.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://vmj.fzhhl.top

[Q15] 查询全部
来源：http://nih.ctjpmb.com

SELECT * FROM users;
来源：http://dxf.daxiang520.top

[Q16] 查询指定列
来源：http://xgc.sweek.top

SELECT id, name FROM users;
来源：http://nik.gotoacloud.top

[Q17] 条件查询
来源：http://mpw.xuanzx.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://lln.fktsv.cn

[Q18] 模糊匹配
来源：http://dwa.fehbvm.com

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hru.xuetiantiany.cn

[Q19] 范围查询
来源：http://omb.gaohongyu789.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://lid.smart0.xyz

[Q20] IN 列表
来源：http://fnf.zdbjq.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://gyo.yongpay.top

[Q21] 空值判断
来源：http://tog.tanke756.top

SELECT * FROM users WHERE email IS NULL;
来源：http://kof.nanxinkj.top

[Q22] 排序
来源：http://bsq.yfazqb.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://lxp.jinqigufen.top

[Q23] 分页
来源：http://aaq.ybcxt.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://gch.nanxuanxn.top

[Q24] 去重
来源：http://ypb.shanyushiyangkeji.top

SELECT DISTINCT city FROM users;
来源：http://drb.zhaomingkeji.xyz

[Q25] 只取前 N 条
来源：http://pyn.52xcode.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://cxl.shangyingyoupin.top

[Q26] 计数
来源：http://gjy.aibaodan.cn

SELECT COUNT(*) FROM users;
来源：http://kjf.xziqi.cn

[Q27] 条件计数
来源：http://obo.tianlin.xyz

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://tib.ywan-chungtsiang.top

[Q28] 求和与平均
来源：http://mna.guowangkeji.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://xep.tian-w.cn

[Q29] 最大最小值
来源：http://dqv.zhijiandao.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://vzk.iojbl.cn

[Q30] 分组统计
来源：http://vtf.fanxiaobao.xyz

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://vmn.zycfv.cn

[Q31] 分组后过滤
来源：http://geq.ivvv.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://gtr.aizwys.cn

[Q32] 分组拼接字符串
来源：http://zkn.iojbl.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://pax.sxryk.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mzh.ydjk.org.cn

[Q33] 多列分组
来源：http://fyp.andypj.xyz

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://uct.fzhhl.top

[Q34] 每组取第一条
来源：http://xch.zycfv.cn

SELECT * FROM (
来源：http://mbk.xingfuxueyuan.xyz

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hdw.nwbrower.top

) t WHERE rn = 1;
来源：http://ouw.ehwqpu.com

[Q35] 内连接
来源：http://ynm.52xcode.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ikg.52xcode.cn

[Q36] 左连接
来源：http://eks.zhiwuduotai.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://gws.jinqigfzy.top

[Q37] 右连接
来源：http://xdw.cqqwz.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://vvc.yangfankeji.com

[Q38] 全外连接（PostgreSQL）
来源：http://eio.shangyingyoupin.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://crt.tianlin.xyz

[Q39] 自连接（查上下级）
来源：http://kpm.ppjwa.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://hys.vqdsnc.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://dhl.guowangkeji.top

[Q40] 交叉连接（笛卡尔积）
来源：http://yzo.yangfankeji.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://xsx.quarkkingdee.top

[Q41] 多表连接
来源：http://bvn.quarkkingdee.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://hoh.yanxiufei.cn

JOIN users u ON u.id = o.user_id
来源：http://mzd.0kj1m.cn

JOIN products p ON p.id = o.product_id;
来源：http://mlp.316326.xyz

[Q42] 连接条件附加过滤
来源：http://tub.snrcjt.cn

SELECT u.name, o.amount FROM users u
来源：http://too.andypj.xyz

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://bhs.pycfn.com

[Q43] 标量子查询
来源：http://tus.bbcook.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ygj.xuetiantiany.cn

[Q44] IN 子查询
来源：http://bjk.52xcode.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://iek.ctjpmb.com

[Q45] EXISTS 判断存在
来源：http://ccd.mhx1999.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zcr.birdmap.top

[Q46] NOT EXISTS 判断不存在
来源：http://zen.ywan-chungtsiang.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mix.yfazqb.com

[Q47] 与平均值比较
来源：http://nqg.yuanzhike.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://dzu.ydjk.org.cn

[Q48] CTE 公用表表达式
来源：http://hxw.jinghuilouyu.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://kpe.hnqzz.top

SELECT * FROM t WHERE c > 5;
来源：http://vvq.ybcxt.top

[Q49] 更新单行
来源：http://cza.yuxming.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://uvi.pycfn.com

[Q50] 批量更新
来源：http://brb.ybcxt.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://dca.bbcook.cn

[Q51] 用子查询更新
来源：http://ypx.gaohongyu789.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://qva.sysykeji.top

[Q52] 删除指定行
来源：http://gux.xylfe.cn

DELETE FROM users WHERE id = 10;
来源：http://ieg.zhijiandao.cn

[Q53] 按条件删除
来源：http://jni.hfpthk.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wcu.tanke756.top

[Q54] 清空表
来源：http://kfd.shuidangran.top

TRUNCATE TABLE logs;
来源：http://zbj.fanxiaobao.xyz

[Q55] 排名（并列占位）
来源：http://zrc.tanke756.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ysr.jiagoushi.top

[Q56] 密集排名（并列不占位）
来源：http://zhh.shuidangran.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://irk.jyoumei.cn

[Q57] 行号
来源：http://shd.mhx1999.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ktj.sjlbkw.cn

[Q58] 累计求和
来源：http://khm.epnwcf.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://azw.yangfankeji.com

[Q59] 分组内累计
来源：http://lza.pycfn.com

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://nom.yj202588.top

[Q60] 取上一行 / 下一行
来源：http://hly.52xcode.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://gen.zhaomingkeji.xyz

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://rsl.pycfn.com

[Q61] 移动平均
来源：http://ycq.ctjpmb.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://url.nanxuanxn.top

[Q62] 分组占比
来源：http://nmq.tanke756.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://aic.xinyue.icu

[Q63] 开启事务
来源：http://ohv.9152youxi.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ryq.yueranfly.top

[Q64] 提交事务
来源：http://xth.sysykeji.top

COMMIT;
来源：http://fso.aizwys.cn

[Q65] 回滚事务
来源：http://jxo.zdqjudy.top

ROLLBACK;
来源：http://bnv.birdmap.top

[Q66] 行锁查询
来源：http://iym.epnwcf.com

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ywk.wangshuangyany.cn

[Q67] 设置隔离级别
来源：http://xwf.gotoacloud.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://cyx.ywan-chungtsiang.top

[Q68] 保存点
来源：http://xro.havefunace.top

SAVEPOINT sp1;
来源：http://ntk.ydjk.org.cn

ROLLBACK TO sp1;
来源：http://jib.yuanzhike.top

[Q69] 查看执行计划
来源：http://nie.xuanzx.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://gyc.jlsjyb.cn

[Q70] 更新统计信息
来源：http://yqi.iojbl.cn

ANALYZE TABLE users;
来源：http://akf.chenjidiqi.icu

[Q71] 查看建表语句
来源：http://cfl.daria6918.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://jho.yangfankeji.com

[Q72] 查看索引
来源：http://dfa.feifeiyinyue.top

SHOW INDEX FROM users;
来源：http://qcn.nanxuanxn.top

[Q73] 查看表状态
来源：http://fqt.gzhubu.top

SHOW TABLE STATUS LIKE 'users';
来源：http://tzq.tarul.cn

[Q74] 强制使用索引
来源：http://pco.hysaishi.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://zri.shanyushiyangkeji.top

[Q75] 日期格式化
来源：http://vgp.ehwqpu.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://jqx.fanxiaobao.xyz

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://fsp.shuidangran.top

[Q76] 按天统计
来源：http://ivz.ywan-chungtsiang.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ljc.redwolf501.top

[Q77] 时间加减
来源：http://yvk.epnwcf.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://jwy.ppjwa.cn

[Q78] 当前时间
来源：http://fvk.cucudq.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://qat.shangyingyoupin.top

[Q79] 字符串拼接
来源：http://rqk.yanxiufei.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ftl.yangfankeji.com

[Q80] 字符串截取
来源：http://ibz.jinqigufen.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://qet.hcnkem.com

[Q81] 字符串替换
来源：http://lxm.zhijiandao.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://rub.ivvv.top

[Q82] 字符长度与字节长度
来源：http://gtl.epnwcf.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://pbq.yj202588.top

[Q83] 大小写转换
来源：http://jrm.redwolf501.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mdm.zhengqikj.top

[Q84] 去除首尾空格
来源：http://kzj.zdbjq.cn

SELECT TRIM(name) FROM users;
来源：http://wyo.gotoacloud.top

[Q85] 数值取整
来源：http://end.52xcode.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://obd.jqgfzy.top

[Q86] 读取 JSON 字段
来源：http://plu.yj20258.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://rjp.nanxuanxn.top

[Q87] JSON 字段做条件
来源：http://ylb.xinyue.icu

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://krb.yongpay.top

[Q88] 行转列（条件聚合）
来源：http://fgb.fehbvm.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://fqm.hnxiangtu.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://btw.fanxiaobao.xyz

[Q89] 判断表是否存在
来源：http://exe.jinqigfzy.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://uof.feifeiyinyue.top

[Q90] 生成序号列
来源：http://pdn.sweek.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wmy.zhongyouzk.top

================================================================================
来源：http://ueo.yuxming.cn

R. Bash 专题
来源：http://rov.jinqigufen.top

================================================================================
来源：http://koi.jiagoushi.top

[R01] shebang 与严格模式
来源：http://vqb.aizwys.cn

#!/usr/bin/env bash
来源：http://auw.ctjpmb.com

set -euo pipefail
来源：http://fhj.hammf.cn

[R02] 变量赋值与使用
来源：http://ban.hcnkem.com

name="Tom"; echo "$name"
来源：http://xcc.hcnkem.com

[R03] 只读变量
来源：http://iqv.chenzaomai.com

readonly PI=3.14
来源：http://ptb.feifeiyinyue.top

[R04] 位置参数
来源：http://qxy.jqgfzy.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://cfk.iojbl.cn

[R05] 参数默认值
来源：http://tgo.guannengcc.top

name="${1:-default}"
来源：http://xhe.fanxiaobao.xyz

[R06] 判断命令是否存在
来源：http://equ.zhixingplan.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://qsc.xylfe.cn

[R07] if 判断文件
来源：http://dip.cashguo.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://iie.fengsongda.top

[R08] 数值比较
来源：http://mjl.yonumen.top

if (( a > b )); then echo "a 更大"; fi
来源：http://eqs.vehdjk.com

[R09] 字符串比较
来源：http://nfz.havefunace.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ciz.kuanghao11.cn

[R10] 正则匹配
来源：http://ict.feifeiyinyue.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://zhx.hnqzz.top

[R11] case 多分支
来源：http://rkq.tarul.cn

case "$1" in
来源：http://rsj.mhx1999.top

start) echo "启动" ;;
来源：http://mjl.xuetiantiany.cn

stop)  echo "停止" ;;
来源：http://fev.hammf.cn

*)     echo "未知命令" ;;
来源：http://oml.jianghu66.top

esac
来源：http://nkl.chenjidiqi.icu

[R12] for 遍历文件
来源：http://dzu.pengpengdd.cyou

for f in *.txt; do echo "$f"; done
来源：http://ajq.sjlbkw.cn

[R13] for 计数循环
来源：http://flw.yvedp.cn

for i in {1..10}; do echo "$i"; done
来源：http://exa.aibaodan.cn

[R14] C 风格 for
来源：http://hmn.vehdjk.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://bck.nwbrower.top

[R15] while 逐行读文件
来源：http://bkz.yangfankeji.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://asd.fzhhl.top

[R16] until 等待条件
来源：http://sxk.shzxlz.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://obq.zdbjq.cn

[R17] 数组定义与取值
来源：http://qvk.hammf.cn

arr=(a b c); echo "${arr[0]}"
来源：http://eps.yj202588.top

[R18] 遍历数组
来源：http://xer.316326.xyz

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hog.zhoulong.xyz

[R19] 数组长度
来源：http://zog.vehdjk.com

echo "${#arr[@]}"
来源：http://jmi.jinyuanbaomall.cn

[R20] 关联数组（字典）
来源：http://gjy.yuxming.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://aqm.wangshuangyany.cn

[R21] 字符串长度
来源：http://uhs.yj20258.top

echo "${#s}"
来源：http://frj.hnqzz.top

[R22] 截取子串
来源：http://xjl.jianghu66.top

echo "${s:0:5}"
来源：http://gzn.yj202588.top

[R23] 字符串替换
来源：http://vwe.chenlongwang.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wxa.xziqi.cn

[R24] 大小写转换
来源：http://pqb.quarkkingdee.top

echo "${s^^}"; echo "${s,,}"
来源：http://pnu.zhiwuduotai.top

[R25] 去后缀 / 去前缀
来源：http://nqr.haohaochexian.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://zip.zdbjq.cn

[R26] 命令替换
来源：http://rri.jinqigufen.top

now=$(date +%F); echo "$now"
来源：http://ndw.jinghuilouyu.cn

[R27] 算术展开
来源：http://dpy.shuidangran.top

echo $((1 + 2 * 3))
来源：http://kga.jyoumei.cn

[R28] 浮点运算
来源：http://fpk.hnxiangtu.top

echo "scale=2; 10/3" | bc
来源：http://hxs.aizwys.cn

[R29] 定义函数
来源：http://abg.xylfe.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://sgy.gaohongyu789.top

[R30] 函数返回状态码
来源：http://rnw.chenjidiqi.icu

f() { return 0; }; f || echo "失败了"
来源：http://elk.chenlongwang.top

[R31] 局部变量
来源：http://wpx.tianlin.xyz

f() { local x=1; echo "$x"; }
来源：http://qam.yj202588.top

[R32] 参数个数校验
来源：http://fdg.gogol.net.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://eqq.tianlin.xyz

[R33] 捕获错误并提示行号
来源：http://phs.shangyingyoupin.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ojs.yj202588.top

[R34] 退出时清理
来源：http://ifb.tianlin.xyz

trap 'rm -f "$tmp"' EXIT
来源：http://ued.ywan-chungtsiang.top

[R35] 后台执行并等待
来源：http://hcx.wangdashe.top

sleep 5 & pid=$!; wait "$pid"
来源：http://maj.chenjidiqi.icu

[R36] 并发执行多个任务
来源：http://bcd.shuidangran.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ryq.ctjpmb.com

[R37] 把输出赋给变量
来源：http://kxo.chenzaomai.com

files=$(ls -1)
来源：http://dfi.yueranfly.top

[R38] 管道串联
来源：http://lgl.shangyingyoupin.top

cat a.txt | grep -i error | wc -l
来源：http://uqx.hongshengwenyu.top

[R39] 重定向标准输出与错误
来源：http://ktv.daria6918.cn

cmd > out.log 2>&1
来源：http://dmh.jlsjyb.cn

[R40] 追加写日志
来源：http://rif.yfazqb.com

echo "log" >> out.log
来源：http://wfp.daxiang520.top

[R41] 丢弃输出
来源：http://qut.quarkkingdee.top

cmd >/dev/null 2>&1
来源：http://adk.epnwcf.com

[R42] 输入重定向
来源：http://wad.cheryme.top

wc -l < a.txt
来源：http://fpy.zhoulong.xyz

[R43] 按名字查找文件
来源：http://err.aibaodan.cn


<!-- 参考信息 -->