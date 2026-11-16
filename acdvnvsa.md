代发 wailian999

================================================================================
来源：http://hym.tianlin.xyz

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ouf.cdnleiting.top

================================================================================
来源：http://oga.zdqjudy.top

[Q01] 创建表
来源：http://zij.c1oappe.top

CREATE TABLE users (
来源：http://hsu.hcnkem.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://xnm.dianchejie.cn

name VARCHAR(50) NOT NULL,
来源：http://ykx.guowangkeji.top

email VARCHAR(100) UNIQUE,
来源：http://fvn.ivvv.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://yps.gzhubu.top

);
来源：http://nvf.daxiang520.top

[Q02] 创建带外键的表
来源：http://btj.snrcjt.cn

CREATE TABLE orders (
来源：http://ktn.jinqigfzy.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://bao.fengsongda.top

user_id INT NOT NULL,
来源：http://tzp.yonumen.top

amount DECIMAL(10, 2),
来源：http://ckt.havefunace.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://fid.shanyushiyangtech.top

);
来源：http://yho.daxiang520.top

[Q03] 增加列
来源：http://inf.shanyushiyangkeji.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://tov.yvedp.cn

[Q04] 修改列类型
来源：http://jhd.yuanzhike.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://jmj.yueranfly.top

[Q05] 重命名列
来源：http://qvi.jinqigfzy.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://qjq.tarul.cn

[Q06] 删除列
来源：http://dfg.quarkkingdee.top

ALTER TABLE users DROP COLUMN age;
来源：http://iky.yuanzhike.top

[Q07] 删除表
来源：http://mna.hnqzz.top

DROP TABLE IF EXISTS orders;
来源：http://gcw.snrcjt.cn

[Q08] 创建普通索引
来源：http://bso.zhoulong.xyz

CREATE INDEX idx_users_email ON users(email);
来源：http://fdj.nanxuanxn.top

[Q09] 创建唯一索引
来源：http://pzk.birdmap.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://rff.xuetiantiany.cn

[Q10] 插入单行
来源：http://cwh.pycfn.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ara.feifeiyinyue.top

[Q11] 一次插入多行
来源：http://rsz.ivvv.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ujm.gzhubu.top

[Q12] 插入后取自增 ID
来源：http://gft.yongpay.top

INSERT INTO users (name) VALUES ('C');
来源：http://twt.ydjk.org.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ccd.fzhhl.top

[Q13] 忽略重复插入
来源：http://ide.gotoacloud.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://jvy.guowangkeji.top

[Q14] 存在则更新（upsert）
来源：http://ogk.ehwqpu.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://tcg.hywenlv.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://btp.tarul.cn

[Q15] 查询全部
来源：http://peh.jqgfzy.top

SELECT * FROM users;
来源：http://eaj.hnqzz.top

[Q16] 查询指定列
来源：http://jrj.xylfe.cn

SELECT id, name FROM users;
来源：http://cku.sjlbkw.cn

[Q17] 条件查询
来源：http://gqw.jqgufenzy.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://xnh.andypj.xyz

[Q18] 模糊匹配
来源：http://zqa.zdbjq.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://vrr.fanxiaobao.xyz

[Q19] 范围查询
来源：http://eii.hysaishi.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://qfy.bjfxy.top

[Q20] IN 列表
来源：http://pcp.yueranfly.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ikz.fzhhl.top

[Q21] 空值判断
来源：http://kpa.daxiang520.top

SELECT * FROM users WHERE email IS NULL;
来源：http://tby.mhx1999.top

[Q22] 排序
来源：http://gkl.vqdsnc.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://php.xingfuxueyuan.xyz

[Q23] 分页
来源：http://crz.gogol.net.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://gbu.shuidangran.top

[Q24] 去重
来源：http://bru.haohaochexian.top

SELECT DISTINCT city FROM users;
来源：http://muo.chenzaomai.com

[Q25] 只取前 N 条
来源：http://pek.cdnleiting.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://uxr.yanxiufei.cn

[Q26] 计数
来源：http://nol.zhiwuduotai.top

SELECT COUNT(*) FROM users;
来源：http://bwf.yvedp.cn

[Q27] 条件计数
来源：http://kmb.kuanghao11.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://vdv.yanxiufei.cn

[Q28] 求和与平均
来源：http://qus.yfazqb.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://idf.wangdashe.top

[Q29] 最大最小值
来源：http://euq.hammf.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://wdq.havefunace.top

[Q30] 分组统计
来源：http://qkw.jianghu66.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://snh.hnqzz.top

[Q31] 分组后过滤
来源：http://vyg.jqgufenzy.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hzl.shanyushiyangkeji.top

[Q32] 分组拼接字符串
来源：http://pos.hywenlv.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://tqn.jianghu66.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://lze.zycfv.cn

[Q33] 多列分组
来源：http://dno.zhongyouzk.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hdh.tarul.cn

[Q34] 每组取第一条
来源：http://tnq.shangyingyoupin.top

SELECT * FROM (
来源：http://yrw.aizwys.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wdg.jinyuanbaomall.cn

) t WHERE rn = 1;
来源：http://fil.hongshengwenyu.top

[Q35] 内连接
来源：http://rwa.fzhhl.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hdz.iojbl.cn

[Q36] 左连接
来源：http://cdg.aizwys.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://jkr.iojbl.cn

[Q37] 右连接
来源：http://ycu.fzhhl.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://zkd.yuanzhike.top

[Q38] 全外连接（PostgreSQL）
来源：http://mhg.sysykeji.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://fhu.nanxinkj.top

[Q39] 自连接（查上下级）
来源：http://ols.0kj1m.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://blb.nanxinkj.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://dtz.yfazqb.com

[Q40] 交叉连接（笛卡尔积）
来源：http://tcf.ywan-chungtsiang.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ylw.jinyuanbaomall.cn

[Q41] 多表连接
来源：http://fyp.zhongyouzk.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://oks.haohaochexian.top

JOIN users u ON u.id = o.user_id
来源：http://gux.zhijiandao.cn

JOIN products p ON p.id = o.product_id;
来源：http://zpq.fengsongda.top

[Q42] 连接条件附加过滤
来源：http://eon.c1oappe.top

SELECT u.name, o.amount FROM users u
来源：http://eeu.hysaishi.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ihm.cashguo.top

[Q43] 标量子查询
来源：http://uxe.jinyuanbaomall.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://qcg.fehbvm.com

[Q44] IN 子查询
来源：http://lne.jqgfzy.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://gtn.iojbl.cn

[Q45] EXISTS 判断存在
来源：http://lxe.zhongyouzk.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://myc.cucudq.cn

[Q46] NOT EXISTS 判断不存在
来源：http://wxx.bjfxy.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://cgf.tanke756.top

[Q47] 与平均值比较
来源：http://mww.yj20258888.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wte.ydzc1.top

[Q48] CTE 公用表表达式
来源：http://bep.jyoumei.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://cxt.fanxiaobao.xyz

SELECT * FROM t WHERE c > 5;
来源：http://ham.xuanzx.com

[Q49] 更新单行
来源：http://www.zhijiandao.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hph.sjlbkw.cn

[Q50] 批量更新
来源：http://ljc.dianchejie.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://lin.sufxvd.cn

[Q51] 用子查询更新
来源：http://yoo.nanxuanxn.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://kxi.yuanzhike.top

[Q52] 删除指定行
来源：http://bah.ydjk.org.cn

DELETE FROM users WHERE id = 10;
来源：http://tws.gzhubu.top

[Q53] 按条件删除
来源：http://xic.svipenyu.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hpb.zhixingplan.top

[Q54] 清空表
来源：http://tew.sxryk.cn

TRUNCATE TABLE logs;
来源：http://zgm.fengsongda.top

[Q55] 排名（并列占位）
来源：http://vub.snrcjt.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://fgn.ydzc1.top

[Q56] 密集排名（并列不占位）
来源：http://ani.yangfankeji.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mbw.tian-w.cn

[Q57] 行号
来源：http://svh.svipenyu.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://fgy.hesvh.cn

[Q58] 累计求和
来源：http://ykn.zdqjudy.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hat.shanyushiyangkeji.top

[Q59] 分组内累计
来源：http://zcy.wangshuangyany.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://bbz.zhongyouzk.top

[Q60] 取上一行 / 下一行
来源：http://xgb.zhoulong.xyz

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://dwp.jianghu66.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://vri.9152youxi.cn

[Q61] 移动平均
来源：http://owr.birdmap.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://iqx.zdbjq.cn

[Q62] 分组占比
来源：http://fut.birdmap.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://nco.hcnkem.com

[Q63] 开启事务
来源：http://xyb.dashuyun.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://jdg.yj20258.top

[Q64] 提交事务
来源：http://avq.kuanghao11.cn

COMMIT;
来源：http://afo.uphjek.com

[Q65] 回滚事务
来源：http://ugg.tarul.cn

ROLLBACK;
来源：http://hyl.ppjwa.cn

[Q66] 行锁查询
来源：http://yro.wangdashe.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://xis.zdqjudy.top

[Q67] 设置隔离级别
来源：http://yrh.aibaodan.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://cib.tarul.cn

[Q68] 保存点
来源：http://ayf.cashguo.top

SAVEPOINT sp1;
来源：http://axb.daxiang520.top

ROLLBACK TO sp1;
来源：http://qdk.aizwys.cn

[Q69] 查看执行计划
来源：http://cpl.hfpthk.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://clt.fzhhl.top

[Q70] 更新统计信息
来源：http://glu.dianchejie.cn

ANALYZE TABLE users;
来源：http://nbm.vehdjk.com

[Q71] 查看建表语句
来源：http://dhn.ywan-chungtsiang.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://cjx.hesvh.cn

[Q72] 查看索引
来源：http://dic.jyoumei.cn

SHOW INDEX FROM users;
来源：http://ucr.zycfv.cn

[Q73] 查看表状态
来源：http://ebt.jiagoushi.top

SHOW TABLE STATUS LIKE 'users';
来源：http://gds.hesvh.cn

[Q74] 强制使用索引
来源：http://jfj.tarul.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://tcf.9152youxi.cn

[Q75] 日期格式化
来源：http://osg.ppjwa.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://dby.svipenyu.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://iev.snrcjt.cn

[Q76] 按天统计
来源：http://rhg.gogol.net.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://zuo.hesvh.cn

[Q77] 时间加减
来源：http://gpk.c1oappe.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://rmj.cheryme.top

[Q78] 当前时间
来源：http://dle.316326.xyz

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://zrk.shuidangran.top

[Q79] 字符串拼接
来源：http://wzh.pengpengdd.cyou

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://aky.cheryme.top

[Q80] 字符串截取
来源：http://whk.vehdjk.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://dru.sjlbkw.cn

[Q81] 字符串替换
来源：http://tjt.tian-w.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://jof.vehdjk.com

[Q82] 字符长度与字节长度
来源：http://dhs.xinyue.icu

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://slr.xylfe.cn

[Q83] 大小写转换
来源：http://eoz.chenzaomai.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://nac.jqgfzy.top

[Q84] 去除首尾空格
来源：http://mio.shuidangran.top

SELECT TRIM(name) FROM users;
来源：http://egr.shanyushiyangkeji.top

[Q85] 数值取整
来源：http://mzl.fanxiaobao.xyz

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://lwt.tian-w.cn

[Q86] 读取 JSON 字段
来源：http://ycq.fanxiaobao.xyz

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://gwg.fktsv.cn

[Q87] JSON 字段做条件
来源：http://rrt.snrcjt.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://uoc.quarkkingdee.top

[Q88] 行转列（条件聚合）
来源：http://hds.shzxlz.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ohl.xingfuxueyuan.xyz

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://xlp.jinghuilouyu.cn

[Q89] 判断表是否存在
来源：http://npn.zdqjudy.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ttg.xuetiantiany.cn

[Q90] 生成序号列
来源：http://gqb.zhongyouzk.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://smf.yueranfly.top

================================================================================
来源：http://gvc.dianchejie.cn

R. Bash 专题
来源：http://sik.ctjpmb.com

================================================================================
来源：http://sus.hywenlv.cn

[R01] shebang 与严格模式
来源：http://jzf.mhx1999.top

#!/usr/bin/env bash
来源：http://gzo.yangfankeji.com

set -euo pipefail
来源：http://oci.hnqzz.top

[R02] 变量赋值与使用
来源：http://kel.zhoulong.xyz

name="Tom"; echo "$name"
来源：http://tdo.tian-w.cn

[R03] 只读变量
来源：http://qfs.cucudq.cn

readonly PI=3.14
来源：http://tni.hesvh.cn

[R04] 位置参数
来源：http://tyz.yongpay.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://fqa.tian-w.cn

[R05] 参数默认值
来源：http://swh.zhengqikj.top

name="${1:-default}"
来源：http://bwl.dashuyun.cn

[R06] 判断命令是否存在
来源：http://pqs.yj202588.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wdk.yvedp.cn

[R07] if 判断文件
来源：http://vma.yfazqb.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://uhv.yangfankeji.com

[R08] 数值比较
来源：http://tko.jinqigfzy.top

if (( a > b )); then echo "a 更大"; fi
来源：http://nix.wangshuangyany.cn

[R09] 字符串比较
来源：http://rco.vqdsnc.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://yaq.jqgfzy.top

[R10] 正则匹配
来源：http://blr.wangdashe.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hqw.dashuyun.cn

[R11] case 多分支
来源：http://lie.bjfxy.top

case "$1" in
来源：http://ilo.birdmap.top

start) echo "启动" ;;
来源：http://dod.xinyue.icu

stop)  echo "停止" ;;
来源：http://epw.cqqwz.cn

*)     echo "未知命令" ;;
来源：http://prr.cheryme.top

esac
来源：http://fkd.pengpengdd.cyou

[R12] for 遍历文件
来源：http://xaz.birdmap.top

for f in *.txt; do echo "$f"; done
来源：http://yuf.316326.xyz

[R13] for 计数循环
来源：http://tub.hesvh.cn

for i in {1..10}; do echo "$i"; done
来源：http://kna.tanke756.top

[R14] C 风格 for
来源：http://phq.hysaishi.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://cxf.yvedp.cn

[R15] while 逐行读文件
来源：http://hxx.yongpay.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://jds.zhoulong.xyz

[R16] until 等待条件
来源：http://aub.shuidangran.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://rub.ybcxt.top

[R17] 数组定义与取值
来源：http://sif.xingfuxueyuan.xyz

arr=(a b c); echo "${arr[0]}"
来源：http://hyw.jiagoushi.top

[R18] 遍历数组
来源：http://vew.pycfn.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ifl.jqgufenzy.top

[R19] 数组长度
来源：http://wug.tanke756.top

echo "${#arr[@]}"
来源：http://hnr.fengsongda.top

[R20] 关联数组（字典）
来源：http://wrn.sxryk.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hyb.ivvv.top

[R21] 字符串长度
来源：http://gvy.ctjpmb.com

echo "${#s}"
来源：http://cqo.kuanghao11.cn

[R22] 截取子串
来源：http://ewi.zhoulong.xyz

echo "${s:0:5}"
来源：http://cdq.haohaochexian.top

[R23] 字符串替换
来源：http://jvh.yongpay.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://qqx.zycfv.cn

[R24] 大小写转换
来源：http://uvm.pycfn.com

echo "${s^^}"; echo "${s,,}"
来源：http://mhb.vehdjk.com

[R25] 去后缀 / 去前缀
来源：http://fay.zhengqikj.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://mua.sufxvd.cn

[R26] 命令替换
来源：http://xyy.zdqjudy.top

now=$(date +%F); echo "$now"
来源：http://nmj.zhongyouzk.top

[R27] 算术展开
来源：http://qmo.ybcxt.top

echo $((1 + 2 * 3))
来源：http://ffa.bjfxy.top

[R28] 浮点运算
来源：http://ssp.mhx1999.top

echo "scale=2; 10/3" | bc
来源：http://tck.gotoacloud.top

[R29] 定义函数
来源：http://zqi.yvedp.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ryx.ydzc1.top

[R30] 函数返回状态码
来源：http://tfj.jianghu66.top

f() { return 0; }; f || echo "失败了"
来源：http://ljy.ivvv.top

[R31] 局部变量
来源：http://liu.smart0.xyz

f() { local x=1; echo "$x"; }
来源：http://jpj.0kj1m.cn

[R32] 参数个数校验
来源：http://zct.hongshengwenyu.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mjw.zhixingplan.top

[R33] 捕获错误并提示行号
来源：http://qvw.yueranfly.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hgs.aibaodan.cn

[R34] 退出时清理
来源：http://dbe.hcnkem.com

trap 'rm -f "$tmp"' EXIT
来源：http://qxy.316326.xyz

[R35] 后台执行并等待
来源：http://rvl.bbcook.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://flc.shangyingyoupin.top

[R36] 并发执行多个任务
来源：http://hsb.hnqzz.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://cqv.hcnkem.com

[R37] 把输出赋给变量
来源：http://nsl.zhoulong.xyz

files=$(ls -1)
来源：http://czt.zhoulong.xyz

[R38] 管道串联
来源：http://neu.jiagoushi.top

cat a.txt | grep -i error | wc -l
来源：http://cut.52xcode.cn

[R39] 重定向标准输出与错误
来源：http://did.svipenyu.cn

cmd > out.log 2>&1
来源：http://vtr.hammf.cn

[R40] 追加写日志
来源：http://ykp.c1oappe.top

echo "log" >> out.log
来源：http://xwz.jlsjyb.cn

[R41] 丢弃输出
来源：http://rvh.yueranfly.top

cmd >/dev/null 2>&1
来源：http://sap.vehdjk.com

[R42] 输入重定向
来源：http://zrm.jiagoushi.top

wc -l < a.txt
来源：http://dva.hnqzz.top

[R43] 按名字查找文件
来源：http://gap.cheryme.top


<!-- 参考信息 -->