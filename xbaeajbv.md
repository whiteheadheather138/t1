代发 wailian999

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wwk.shangyingyoupin.top

);
来源：http://yxl.jqgufenzy.top

[Q02] 创建带外键的表
来源：http://fnt.pycfn.com

CREATE TABLE orders (
来源：http://kiu.feifeiyinyue.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://brw.jinyuanbaomall.cn

user_id INT NOT NULL,
来源：http://ibo.xuetiantiany.cn

amount DECIMAL(10, 2),
来源：http://afy.shanyushiyangtech.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://grb.ivvv.top

);
来源：http://bsu.jinghuilouyu.cn

[Q03] 增加列
来源：http://zde.jlsjyb.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://msu.9152youxi.cn

[Q04] 修改列类型
来源：http://eqg.fehbvm.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wmo.andypj.xyz

[Q05] 重命名列
来源：http://xzz.kuanghao11.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://oxp.nanxinkj.top

[Q06] 删除列
来源：http://wkf.zycfv.cn

ALTER TABLE users DROP COLUMN age;
来源：http://qhh.guowangkeji.top

[Q07] 删除表
来源：http://gxt.yfazqb.com

DROP TABLE IF EXISTS orders;
来源：http://kqr.cdnleiting.top

[Q08] 创建普通索引
来源：http://rvx.hysaishi.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://gec.svipenyu.cn

[Q09] 创建唯一索引
来源：http://pqs.jiagoushi.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://cbg.yueranfly.top

[Q10] 插入单行
来源：http://iof.yonumen.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://lfg.guannengcc.top

[Q11] 一次插入多行
来源：http://qjj.gzhubu.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ybi.feifeiyinyue.top

[Q12] 插入后取自增 ID
来源：http://lwn.jyoumei.cn

INSERT INTO users (name) VALUES ('C');
来源：http://dnk.redwolf501.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://dpl.jinqigufen.top

[Q13] 忽略重复插入
来源：http://rtc.feifeiyinyue.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://bha.zhoulong.xyz

[Q14] 存在则更新（upsert）
来源：http://loo.yueranfly.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hzk.shzxlz.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://apl.wangshuangyany.cn

[Q15] 查询全部
来源：http://lnw.hnxiangtu.top

SELECT * FROM users;
来源：http://anc.yj202588.top

[Q16] 查询指定列
来源：http://ynq.9152youxi.cn

SELECT id, name FROM users;
来源：http://ezs.52xcode.cn

[Q17] 条件查询
来源：http://fou.wangshuangyany.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://szl.gaohongyu789.top

[Q18] 模糊匹配
来源：http://ghc.0kj1m.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://kpv.guowangkeji.top

[Q19] 范围查询
来源：http://kss.zhongyouzk.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://yel.hammf.cn

[Q20] IN 列表
来源：http://xma.vehdjk.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://rdh.nwbrower.top

[Q21] 空值判断
来源：http://csx.aibaodan.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://xzf.yj20258888.top

[Q22] 排序
来源：http://otr.andypj.xyz

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ugs.epnwcf.com

[Q23] 分页
来源：http://csy.zycfv.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://rss.yj20258888.top

[Q24] 去重
来源：http://lay.yuxming.cn

SELECT DISTINCT city FROM users;
来源：http://tgq.gzhubu.top

[Q25] 只取前 N 条
来源：http://gcn.jiagoushi.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://yjq.ctjpmb.com

[Q26] 计数
来源：http://bab.xylfe.cn

SELECT COUNT(*) FROM users;
来源：http://zdd.hcnkem.com

[Q27] 条件计数
来源：http://osk.xylfe.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ayh.ydjk.org.cn

[Q28] 求和与平均
来源：http://qaw.zhixingplan.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hqy.zhijiandao.cn

[Q29] 最大最小值
来源：http://zjb.daria6918.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://zty.chenlongwang.top

[Q30] 分组统计
来源：http://dvj.jinghuilouyu.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://brq.ydjk.org.cn

[Q31] 分组后过滤
来源：http://mat.sysykeji.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ehe.zhoulong.xyz

[Q32] 分组拼接字符串
来源：http://clc.tian-w.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://vsn.snrcjt.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ljb.sufxvd.cn

[Q33] 多列分组
来源：http://cvb.shanyushiyangkeji.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://tky.ivvv.top

[Q34] 每组取第一条
来源：http://vjr.jinghuilouyu.cn

SELECT * FROM (
来源：http://ujy.jinyuanbaomall.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wux.xylfe.cn

) t WHERE rn = 1;
来源：http://vhl.cqqwz.cn

[Q35] 内连接
来源：http://ffy.gaohongyu789.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ulk.xingfuxueyuan.xyz

[Q36] 左连接
来源：http://jir.gzhubu.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ops.zhongyouzk.top

[Q37] 右连接
来源：http://flz.dianchejie.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://qdn.cucudq.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ttc.cheryme.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://jwv.epnwcf.com

[Q39] 自连接（查上下级）
来源：http://urr.jlsjyb.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://hmc.dashuyun.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://fsq.vqdsnc.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://mia.svipenyu.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hpw.pycfn.com

[Q41] 多表连接
来源：http://wyg.yj202588.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://izc.cdnleiting.top

JOIN users u ON u.id = o.user_id
来源：http://yyg.xingfuxueyuan.xyz

JOIN products p ON p.id = o.product_id;
来源：http://jqg.yuxming.cn

[Q42] 连接条件附加过滤
来源：http://yyz.vehdjk.com

SELECT u.name, o.amount FROM users u
来源：http://sbg.jiagoushi.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ibm.hongshengwenyu.top

[Q43] 标量子查询
来源：http://tdv.hongshengwenyu.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://iox.vehdjk.com

[Q44] IN 子查询
来源：http://zuk.zycfv.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://czd.zhaomingkeji.xyz

[Q45] EXISTS 判断存在
来源：http://yds.hongshengwenyu.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://sth.pycfn.com

[Q46] NOT EXISTS 判断不存在
来源：http://ejh.jqgfzy.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kac.redwolf501.top

[Q47] 与平均值比较
来源：http://tuh.xingfuxueyuan.xyz

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ftn.hcnkem.com

[Q48] CTE 公用表表达式
来源：http://ogl.wangshuangyany.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://kuq.aibaodan.cn

SELECT * FROM t WHERE c > 5;
来源：http://vfs.52xcode.cn

[Q49] 更新单行
来源：http://sod.yangfankeji.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://pwg.smart0.xyz

[Q50] 批量更新
来源：http://veu.aizwys.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wct.wangshuangyany.cn

[Q51] 用子查询更新
来源：http://acb.haohaochexian.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ayz.vqdsnc.cn

[Q52] 删除指定行
来源：http://diu.bjfxy.top

DELETE FROM users WHERE id = 10;
来源：http://lxu.nanxinkj.top

[Q53] 按条件删除
来源：http://uwk.cheryme.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ftv.sysykeji.top

[Q54] 清空表
来源：http://flp.yuxming.cn

TRUNCATE TABLE logs;
来源：http://xur.fktsv.cn

[Q55] 排名（并列占位）
来源：http://kzz.shuidangran.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ysx.fktsv.cn

[Q56] 密集排名（并列不占位）
来源：http://uxh.fehbvm.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://riz.jlsjyb.cn

[Q57] 行号
来源：http://ton.feifeiyinyue.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://yfh.ctjpmb.com

[Q58] 累计求和
来源：http://vfx.hammf.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://uwu.zhaomingkeji.xyz

[Q59] 分组内累计
来源：http://swc.hywenlv.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://jaj.ivvv.top

[Q60] 取上一行 / 下一行
来源：http://hmi.tanke756.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://vxi.ywan-chungtsiang.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://sfk.jinyuanbaomall.cn

[Q61] 移动平均
来源：http://xtf.fengsongda.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://lxu.zhixingplan.top

[Q62] 分组占比
来源：http://egr.gotoacloud.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://qbj.yueranfly.top

[Q63] 开启事务
来源：http://xqd.redwolf501.top

START TRANSACTION;                -- 或 BEGIN
来源：http://cpz.cheryme.top

[Q64] 提交事务
来源：http://gdp.yj202588.top

COMMIT;
来源：http://mwt.mhx1999.top

[Q65] 回滚事务
来源：http://aji.guannengcc.top

ROLLBACK;
来源：http://qel.hfpthk.cn

[Q66] 行锁查询
来源：http://stq.ctjpmb.com

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://uld.zdbjq.cn

[Q67] 设置隔离级别
来源：http://jvp.yueranfly.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://evf.dianchejie.cn

[Q68] 保存点
来源：http://uqk.dianchejie.cn

SAVEPOINT sp1;
来源：http://ukb.svipenyu.cn

ROLLBACK TO sp1;
来源：http://wvc.zhengqikj.top

[Q69] 查看执行计划
来源：http://kzz.tarul.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://bxo.yj20258.top

[Q70] 更新统计信息
来源：http://opg.nanxinkj.top

ANALYZE TABLE users;
来源：http://ezq.havefunace.top

[Q71] 查看建表语句
来源：http://ypc.fzhhl.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://bno.meibo888.top

[Q72] 查看索引
来源：http://myd.yonumen.top

SHOW INDEX FROM users;
来源：http://mpk.daria6918.cn

[Q73] 查看表状态
来源：http://rur.yfazqb.com

SHOW TABLE STATUS LIKE 'users';
来源：http://cpu.yj20258888.top

[Q74] 强制使用索引
来源：http://wid.zhijiandao.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://lhq.havefunace.top

[Q75] 日期格式化
来源：http://rcw.hfpthk.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://iwy.yongpay.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://nnb.fehbvm.com

[Q76] 按天统计
来源：http://qdh.zdbjq.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hvr.sjlbkw.cn

[Q77] 时间加减
来源：http://bwq.hywenlv.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://iit.ctjpmb.com

[Q78] 当前时间
来源：http://ouw.nwbrower.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://gnt.havefunace.top

[Q79] 字符串拼接
来源：http://aky.hcnkem.com

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ujn.shzxlz.cn

[Q80] 字符串截取
来源：http://kyn.zhaomingkeji.xyz

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://vbd.vqdsnc.cn

[Q81] 字符串替换
来源：http://yrj.wangshuangyany.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://dpt.mhx1999.top

[Q82] 字符长度与字节长度
来源：http://wzw.feifeiyinyue.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://isn.zhaomingkeji.xyz

[Q83] 大小写转换
来源：http://ayy.pengpengdd.cyou

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hmg.nanxinkj.top

[Q84] 去除首尾空格
来源：http://slr.guannengcc.top

SELECT TRIM(name) FROM users;
来源：http://jjs.snrcjt.cn

[Q85] 数值取整
来源：http://etd.gaohongyu789.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://jkz.yuxming.cn

[Q86] 读取 JSON 字段
来源：http://guf.zhoulong.xyz

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mjd.shanyushiyangkeji.top

[Q87] JSON 字段做条件
来源：http://anj.jinghuilouyu.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://xdj.hywenlv.cn

[Q88] 行转列（条件聚合）
来源：http://lyl.c1oappe.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://bbr.svipenyu.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://xzm.sjlbkw.cn

[Q89] 判断表是否存在
来源：http://ppn.tanke756.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://rok.jyoumei.cn

[Q90] 生成序号列
来源：http://tht.zhiwuduotai.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mhp.hammf.cn

================================================================================
来源：http://rmo.pycfn.com

R. Bash 专题
来源：http://qwd.yj202588.top

================================================================================
来源：http://ytr.fktsv.cn

[R01] shebang 与严格模式
来源：http://log.0kj1m.cn

#!/usr/bin/env bash
来源：http://pcf.quarkkingdee.top

set -euo pipefail
来源：http://vtw.chenzaomai.com

[R02] 变量赋值与使用
来源：http://kig.daria6918.cn

name="Tom"; echo "$name"
来源：http://hsj.hnxiangtu.top

[R03] 只读变量
来源：http://tqv.yj20258888.top

readonly PI=3.14
来源：http://jfr.haohaochexian.top

[R04] 位置参数
来源：http://zwd.yj20258.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://bcq.fengsongda.top

[R05] 参数默认值
来源：http://sib.xingfuxueyuan.xyz

name="${1:-default}"
来源：http://ktp.gaohongyu789.top

[R06] 判断命令是否存在
来源：http://azr.sjlbkw.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://tsd.shzxlz.cn

[R07] if 判断文件
来源：http://dtg.uphjek.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ohp.kuanghao11.cn

[R08] 数值比较
来源：http://wty.yongpay.top

if (( a > b )); then echo "a 更大"; fi
来源：http://bhq.wangshuangyany.cn

[R09] 字符串比较
来源：http://kew.zhoulong.xyz

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ikv.jlsjyb.cn

[R10] 正则匹配
来源：http://ypi.bbcook.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://gaq.fengsongda.top

[R11] case 多分支
来源：http://uyy.tanke756.top

case "$1" in
来源：http://yjx.shanyushiyangkeji.top

start) echo "启动" ;;
来源：http://dej.sjlbkw.cn

stop)  echo "停止" ;;
来源：http://ydz.shzxlz.cn

*)     echo "未知命令" ;;
来源：http://bay.jlsjyb.cn

esac
来源：http://ubj.hysaishi.cn

[R12] for 遍历文件
来源：http://kpq.iojbl.cn

for f in *.txt; do echo "$f"; done
来源：http://rzq.uphjek.com

[R13] for 计数循环
来源：http://acq.shzxlz.cn

for i in {1..10}; do echo "$i"; done
来源：http://epd.ivvv.top

[R14] C 风格 for
来源：http://jqz.ppjwa.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ulw.iojbl.cn

[R15] while 逐行读文件
来源：http://ssn.iojbl.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://btt.xinyue.icu

[R16] until 等待条件
来源：http://lyj.ehwqpu.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://dfu.0kj1m.cn

[R17] 数组定义与取值
来源：http://fju.shanyushiyangtech.top

arr=(a b c); echo "${arr[0]}"
来源：http://mzx.cqqwz.cn

[R18] 遍历数组
来源：http://kck.ydjk.org.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://eaa.jiagoushi.top

[R19] 数组长度
来源：http://jkw.ivvv.top

echo "${#arr[@]}"
来源：http://owy.aizwys.cn

[R20] 关联数组（字典）
来源：http://qah.ybcxt.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://sww.ehwqpu.com

[R21] 字符串长度
来源：http://oqa.hongshengwenyu.top

echo "${#s}"
来源：http://kel.zycfv.cn

[R22] 截取子串
来源：http://jwv.yonumen.top

echo "${s:0:5}"
来源：http://zpz.aizwys.cn

[R23] 字符串替换
来源：http://zrb.zhixingplan.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://yvi.kuanghao11.cn

[R24] 大小写转换
来源：http://ksx.cheryme.top

echo "${s^^}"; echo "${s,,}"
来源：http://qgl.chenzaomai.com

[R25] 去后缀 / 去前缀
来源：http://oaj.aizwys.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://nab.hcnkem.com

[R26] 命令替换
来源：http://otw.xingfuxueyuan.xyz

now=$(date +%F); echo "$now"
来源：http://dhf.yuanzhike.top

[R27] 算术展开
来源：http://nrc.shangyingyoupin.top

echo $((1 + 2 * 3))
来源：http://uoa.aizwys.cn

[R28] 浮点运算
来源：http://roj.zhoulong.xyz

echo "scale=2; 10/3" | bc
来源：http://mtn.wangshuangyany.cn

[R29] 定义函数
来源：http://cky.shangyingyoupin.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://vzn.xziqi.cn

[R30] 函数返回状态码
来源：http://aog.mhx1999.top

f() { return 0; }; f || echo "失败了"
来源：http://jvh.xziqi.cn

[R31] 局部变量
来源：http://osy.jyoumei.cn

f() { local x=1; echo "$x"; }
来源：http://nsh.daxiang520.top

[R32] 参数个数校验
来源：http://zqa.yonumen.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://pym.havefunace.top

[R33] 捕获错误并提示行号
来源：http://veo.quarkkingdee.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ckg.meibo888.top

[R34] 退出时清理
来源：http://ibv.c1oappe.top

trap 'rm -f "$tmp"' EXIT
来源：http://ghp.yonumen.top

[R35] 后台执行并等待
来源：http://neu.sweek.top

sleep 5 & pid=$!; wait "$pid"
来源：http://spi.hcnkem.com

[R36] 并发执行多个任务
来源：http://bbk.hcnkem.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hxp.cheryme.top

[R37] 把输出赋给变量
来源：http://nnl.zhoulong.xyz

files=$(ls -1)
来源：http://tks.cucudq.cn

[R38] 管道串联
来源：http://twg.havefunace.top

cat a.txt | grep -i error | wc -l
来源：http://lec.svipenyu.cn

[R39] 重定向标准输出与错误
来源：http://apv.hfpthk.cn

cmd > out.log 2>&1
来源：http://nst.yangfankeji.com

[R40] 追加写日志
来源：http://jxh.haohaochexian.top

echo "log" >> out.log
来源：http://vux.mhx1999.top

[R41] 丢弃输出
来源：http://zzf.yfazqb.com

cmd >/dev/null 2>&1
来源：http://tio.shangyingyoupin.top

[R42] 输入重定向
来源：http://gvy.xylfe.cn

wc -l < a.txt
来源：http://waw.yangfankeji.com

[R43] 按名字查找文件
来源：http://gmm.zhoulong.xyz

find . -name "*.log" -type f
来源：http://emv.zhiwuduotai.top

[R44] 按修改时间查找
来源：http://che.gotoacloud.top

find . -mtime -7 -type f
来源：http://plq.tian-w.cn

[R45] 批量删除
来源：http://qlz.316326.xyz

find . -name "*.tmp" -delete
来源：http://jqf.zhengqikj.top

[R46] 递归替换文件内容
来源：http://ggv.ehwqpu.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://nhc.jinyuanbaomall.cn

[R47] sed 单行替换
来源：http://vkw.aibaodan.cn


<!-- 参考信息 -->