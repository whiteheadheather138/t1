代发 wailian999

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://rky.fanxiaobao.xyz

user_id INT NOT NULL,
来源：http://cwg.316326.xyz

amount DECIMAL(10, 2),
来源：http://wnk.bjfxy.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://kog.zhoulong.xyz

);
来源：http://swm.jinyuanbaomall.cn

[Q03] 增加列
来源：http://hpc.hnxiangtu.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://eks.yanxiufei.cn

[Q04] 修改列类型
来源：http://lef.xylfe.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://nye.jinghuilouyu.cn

[Q05] 重命名列
来源：http://tif.tanke756.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://gdk.hywenlv.cn

[Q06] 删除列
来源：http://yus.gzhubu.top

ALTER TABLE users DROP COLUMN age;
来源：http://jiu.fanxiaobao.xyz

[Q07] 删除表
来源：http://ssb.shanyushiyangtech.top

DROP TABLE IF EXISTS orders;
来源：http://zbk.yvedp.cn

[Q08] 创建普通索引
来源：http://hcd.xingfuxueyuan.xyz

CREATE INDEX idx_users_email ON users(email);
来源：http://gqd.zhaomingkeji.xyz

[Q09] 创建唯一索引
来源：http://qqa.zhongyouzk.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hfe.jinyuanbaomall.cn

[Q10] 插入单行
来源：http://gqe.zhengqikj.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ted.nanxuanxn.top

[Q11] 一次插入多行
来源：http://ugc.uphjek.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://fvv.sweek.top

[Q12] 插入后取自增 ID
来源：http://lhs.hnxiangtu.top

INSERT INTO users (name) VALUES ('C');
来源：http://eag.dianchejie.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://opx.ctjpmb.com

[Q13] 忽略重复插入
来源：http://pya.hfpthk.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://vqv.aibaodan.cn

[Q14] 存在则更新（upsert）
来源：http://yff.yfazqb.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://gcj.aizwys.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://qkj.snrcjt.cn

[Q15] 查询全部
来源：http://qzn.nanxuanxn.top

SELECT * FROM users;
来源：http://ysj.vehdjk.com

[Q16] 查询指定列
来源：http://mzl.xuetiantiany.cn

SELECT id, name FROM users;
来源：http://vuk.yonumen.top

[Q17] 条件查询
来源：http://qok.ivvv.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://gww.jinqigufen.top

[Q18] 模糊匹配
来源：http://rkw.sjlbkw.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://lxd.tian-w.cn

[Q19] 范围查询
来源：http://mwj.quarkkingdee.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://bjq.fktsv.cn

[Q20] IN 列表
来源：http://nxi.jinqigfzy.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://nya.yueranfly.top

[Q21] 空值判断
来源：http://ipo.shanyushiyangtech.top

SELECT * FROM users WHERE email IS NULL;
来源：http://ned.jinqigufen.top

[Q22] 排序
来源：http://xfu.yonumen.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://jou.c1oappe.top

[Q23] 分页
来源：http://tss.yongpay.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://xgu.gotoacloud.top

[Q24] 去重
来源：http://rov.guowangkeji.top

SELECT DISTINCT city FROM users;
来源：http://ypd.vehdjk.com

[Q25] 只取前 N 条
来源：http://sgj.xinyue.icu

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://fqc.ybcxt.top

[Q26] 计数
来源：http://yzy.zhoulong.xyz

SELECT COUNT(*) FROM users;
来源：http://yar.gaohongyu789.top

[Q27] 条件计数
来源：http://ekx.ydjk.org.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mwn.tarul.cn

[Q28] 求和与平均
来源：http://gcf.ctjpmb.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://vpt.sysykeji.top

[Q29] 最大最小值
来源：http://ntn.ydzc1.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://lae.zhaomingkeji.xyz

[Q30] 分组统计
来源：http://qys.shanyushiyangkeji.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://cuu.havefunace.top

[Q31] 分组后过滤
来源：http://qzn.cqqwz.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://nha.jinyuanbaomall.cn

[Q32] 分组拼接字符串
来源：http://nrk.yvedp.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://bdn.hongshengwenyu.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://vax.zhijiandao.cn

[Q33] 多列分组
来源：http://chf.tanke756.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://quk.cdnleiting.top

[Q34] 每组取第一条
来源：http://zwx.shangyingyoupin.top

SELECT * FROM (
来源：http://whg.yueranfly.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://kfc.tanke756.top

) t WHERE rn = 1;
来源：http://fpc.9152youxi.cn

[Q35] 内连接
来源：http://mpm.gzhubu.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://bfz.vqdsnc.cn

[Q36] 左连接
来源：http://kim.fzhhl.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://nna.zhiwuduotai.top

[Q37] 右连接
来源：http://pwt.shangyingyoupin.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://kml.shzxlz.cn

[Q38] 全外连接（PostgreSQL）
来源：http://irp.hywenlv.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://icn.tarul.cn

[Q39] 自连接（查上下级）
来源：http://okj.nwbrower.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://rro.aibaodan.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://zjc.chenlongwang.top

[Q40] 交叉连接（笛卡尔积）
来源：http://jte.hesvh.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://omi.tarul.cn

[Q41] 多表连接
来源：http://xej.hcnkem.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://nyc.tianlin.xyz

JOIN users u ON u.id = o.user_id
来源：http://jda.tianlin.xyz

JOIN products p ON p.id = o.product_id;
来源：http://mba.shanyushiyangkeji.top

[Q42] 连接条件附加过滤
来源：http://mkg.chenlongwang.top

SELECT u.name, o.amount FROM users u
来源：http://gnp.ywan-chungtsiang.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hou.zhaomingkeji.xyz

[Q43] 标量子查询
来源：http://vli.xingfuxueyuan.xyz

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://apo.zhijiandao.cn

[Q44] IN 子查询
来源：http://yfo.chenlongwang.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://akj.chenlongwang.top

[Q45] EXISTS 判断存在
来源：http://ava.ydzc1.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://tmi.aizwys.cn

[Q46] NOT EXISTS 判断不存在
来源：http://wuf.snrcjt.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mvb.fehbvm.com

[Q47] 与平均值比较
来源：http://kuy.9152youxi.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://cbv.hnxiangtu.top

[Q48] CTE 公用表表达式
来源：http://yrb.iojbl.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://xlg.haohaochexian.top

SELECT * FROM t WHERE c > 5;
来源：http://hrp.hysaishi.cn

[Q49] 更新单行
来源：http://dux.dashuyun.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://utb.shanyushiyangkeji.top

[Q50] 批量更新
来源：http://dpw.snrcjt.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ctg.iojbl.cn

[Q51] 用子查询更新
来源：http://zgc.cqqwz.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://sqk.jqgufenzy.top

[Q52] 删除指定行
来源：http://sqz.yuanzhike.top

DELETE FROM users WHERE id = 10;
来源：http://deg.shuidangran.top

[Q53] 按条件删除
来源：http://mfi.zhengqikj.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://dsc.ehwqpu.com

[Q54] 清空表
来源：http://vld.chenjidiqi.icu

TRUNCATE TABLE logs;
来源：http://biv.hnxiangtu.top

[Q55] 排名（并列占位）
来源：http://gwy.52xcode.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ydv.andypj.xyz

[Q56] 密集排名（并列不占位）
来源：http://vuw.316326.xyz

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://zyk.c1oappe.top

[Q57] 行号
来源：http://xjg.jinqigfzy.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://pjc.cashguo.top

[Q58] 累计求和
来源：http://jke.tanke756.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://jqe.yueranfly.top

[Q59] 分组内累计
来源：http://dws.yongpay.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://sst.xinyue.icu

[Q60] 取上一行 / 下一行
来源：http://uqx.xuanzx.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://son.ydzc1.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://xtq.wangdashe.top

[Q61] 移动平均
来源：http://khs.hesvh.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://myz.fehbvm.com

[Q62] 分组占比
来源：http://scj.hywenlv.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://die.shuidangran.top

[Q63] 开启事务
来源：http://jzs.aibaodan.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://eep.shangyingyoupin.top

[Q64] 提交事务
来源：http://bxa.zhoulong.xyz

COMMIT;
来源：http://vek.yvedp.cn

[Q65] 回滚事务
来源：http://hlp.hywenlv.cn

ROLLBACK;
来源：http://fdd.jqgufenzy.top

[Q66] 行锁查询
来源：http://xpg.shanyushiyangtech.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hfp.ybcxt.top

[Q67] 设置隔离级别
来源：http://dls.xingfuxueyuan.xyz

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://spq.xuanzx.com

[Q68] 保存点
来源：http://srf.guowangkeji.top

SAVEPOINT sp1;
来源：http://jul.cashguo.top

ROLLBACK TO sp1;
来源：http://bsy.ybcxt.top

[Q69] 查看执行计划
来源：http://yzf.hnqzz.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://inx.52xcode.cn

[Q70] 更新统计信息
来源：http://xuo.zhengqikj.top

ANALYZE TABLE users;
来源：http://djl.kuanghao11.cn

[Q71] 查看建表语句
来源：http://lwn.sxryk.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://kly.zhoulong.xyz

[Q72] 查看索引
来源：http://euj.pengpengdd.cyou

SHOW INDEX FROM users;
来源：http://jfy.jianghu66.top

[Q73] 查看表状态
来源：http://bom.yfazqb.com

SHOW TABLE STATUS LIKE 'users';
来源：http://dqs.cqqwz.cn

[Q74] 强制使用索引
来源：http://xjp.dianchejie.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ebr.zhongyouzk.top

[Q75] 日期格式化
来源：http://axg.epnwcf.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://juj.hongshengwenyu.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hvq.wangdashe.top

[Q76] 按天统计
来源：http://zri.c1oappe.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://zrs.nanxinkj.top

[Q77] 时间加减
来源：http://xxc.ctjpmb.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://efd.cheryme.top

[Q78] 当前时间
来源：http://ohb.nanxinkj.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ifp.chenlongwang.top

[Q79] 字符串拼接
来源：http://mnv.tanke756.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://jks.tarul.cn

[Q80] 字符串截取
来源：http://suw.tarul.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://sci.kuanghao11.cn

[Q81] 字符串替换
来源：http://ppt.0kj1m.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://epw.guowangkeji.top

[Q82] 字符长度与字节长度
来源：http://lzq.snrcjt.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://lqn.daxiang520.top

[Q83] 大小写转换
来源：http://ndn.chenlongwang.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ism.fengsongda.top

[Q84] 去除首尾空格
来源：http://qhr.hesvh.cn

SELECT TRIM(name) FROM users;
来源：http://zdf.hnxiangtu.top

[Q85] 数值取整
来源：http://eil.guowangkeji.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://vnc.xuetiantiany.cn

[Q86] 读取 JSON 字段
来源：http://uvl.iojbl.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://tkl.pycfn.com

[Q87] JSON 字段做条件
来源：http://zoq.tarul.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://jcz.tian-w.cn

[Q88] 行转列（条件聚合）
来源：http://gwm.nanxuanxn.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://lsk.fktsv.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://fgi.hcnkem.com

[Q89] 判断表是否存在
来源：http://qrm.dianchejie.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://lpl.yuxming.cn

[Q90] 生成序号列
来源：http://dcm.birdmap.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://pbx.ybcxt.top

================================================================================
来源：http://qzn.xingfuxueyuan.xyz

R. Bash 专题
来源：http://kzu.yj202588.top

================================================================================
来源：http://hcx.gogol.net.cn

[R01] shebang 与严格模式
来源：http://baq.zycfv.cn

#!/usr/bin/env bash
来源：http://ixg.shangyingyoupin.top

set -euo pipefail
来源：http://mhf.gogol.net.cn

[R02] 变量赋值与使用
来源：http://rke.uphjek.com

name="Tom"; echo "$name"
来源：http://zkw.zhaomingkeji.xyz

[R03] 只读变量
来源：http://bco.jiagoushi.top

readonly PI=3.14
来源：http://auk.dianchejie.cn

[R04] 位置参数
来源：http://rrv.bbcook.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://xem.nanxuanxn.top

[R05] 参数默认值
来源：http://noh.smart0.xyz

name="${1:-default}"
来源：http://xyy.yj202588.top

[R06] 判断命令是否存在
来源：http://ehl.jinyuanbaomall.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://heb.hongshengwenyu.top

[R07] if 判断文件
来源：http://mbj.yanxiufei.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://fox.sysykeji.top

[R08] 数值比较
来源：http://ruh.fanxiaobao.xyz

if (( a > b )); then echo "a 更大"; fi
来源：http://ssg.sufxvd.cn

[R09] 字符串比较
来源：http://vtv.zhaomingkeji.xyz

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://vcy.pengpengdd.cyou

[R10] 正则匹配
来源：http://scz.smart0.xyz

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ohs.jlsjyb.cn

[R11] case 多分支
来源：http://laj.fanxiaobao.xyz

case "$1" in
来源：http://llc.jinqigufen.top

start) echo "启动" ;;
来源：http://nrx.jiagoushi.top

stop)  echo "停止" ;;
来源：http://ixa.yonumen.top

*)     echo "未知命令" ;;
来源：http://sgi.daxiang520.top

esac
来源：http://udl.shangyingyoupin.top

[R12] for 遍历文件
来源：http://ucu.hywenlv.cn

for f in *.txt; do echo "$f"; done
来源：http://cym.feifeiyinyue.top

[R13] for 计数循环
来源：http://yee.jinqigufen.top

for i in {1..10}; do echo "$i"; done
来源：http://pys.nwbrower.top

[R14] C 风格 for
来源：http://ulr.gogol.net.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wmi.yuanzhike.top

[R15] while 逐行读文件
来源：http://frz.daxiang520.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://lun.guowangkeji.top

[R16] until 等待条件
来源：http://ymr.guannengcc.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://sfo.havefunace.top

[R17] 数组定义与取值
来源：http://yho.havefunace.top

arr=(a b c); echo "${arr[0]}"
来源：http://uyt.yangfankeji.com

[R18] 遍历数组
来源：http://gcq.andypj.xyz

for x in "${arr[@]}"; do echo "$x"; done
来源：http://luq.vehdjk.com

[R19] 数组长度
来源：http://fhw.gaohongyu789.top

echo "${#arr[@]}"
来源：http://yyd.jinqigufen.top

[R20] 关联数组（字典）
来源：http://qaa.yueranfly.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://cud.hfpthk.cn

[R21] 字符串长度
来源：http://orc.kuanghao11.cn

echo "${#s}"
来源：http://lyk.jinyuanbaomall.cn

[R22] 截取子串
来源：http://ovf.zhixingplan.top

echo "${s:0:5}"
来源：http://nwz.ydjk.org.cn

[R23] 字符串替换
来源：http://pyz.jqgufenzy.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hso.sweek.top

[R24] 大小写转换
来源：http://flg.yuxming.cn

echo "${s^^}"; echo "${s,,}"
来源：http://jql.316326.xyz

[R25] 去后缀 / 去前缀
来源：http://iox.sufxvd.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ofl.ppjwa.cn

[R26] 命令替换
来源：http://yzk.jinqigufen.top

now=$(date +%F); echo "$now"
来源：http://ckh.yuanzhike.top

[R27] 算术展开
来源：http://pjc.ydzc1.top

echo $((1 + 2 * 3))
来源：http://mqs.cdnleiting.top

[R28] 浮点运算
来源：http://fvn.hcnkem.com

echo "scale=2; 10/3" | bc
来源：http://jqi.ydzc1.top

[R29] 定义函数
来源：http://ilg.wangdashe.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://idd.0kj1m.cn

[R30] 函数返回状态码
来源：http://vnh.fanxiaobao.xyz

f() { return 0; }; f || echo "失败了"
来源：http://mau.hfpthk.cn

[R31] 局部变量
来源：http://poe.bjfxy.top

f() { local x=1; echo "$x"; }
来源：http://kkx.yangfankeji.com

[R32] 参数个数校验
来源：http://mla.xuanzx.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://iik.shanyushiyangkeji.top

[R33] 捕获错误并提示行号
来源：http://ijp.yj202588.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://kos.zhongyouzk.top

[R34] 退出时清理
来源：http://skb.zhijiandao.cn

trap 'rm -f "$tmp"' EXIT
来源：http://wjn.shanyushiyangtech.top

[R35] 后台执行并等待
来源：http://dpl.zdbjq.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://oza.nwbrower.top

[R36] 并发执行多个任务
来源：http://zlz.dianchejie.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://yiv.zhoulong.xyz

[R37] 把输出赋给变量
来源：http://hjy.dashuyun.cn

files=$(ls -1)
来源：http://qbn.hywenlv.cn

[R38] 管道串联
来源：http://nig.hfpthk.cn

cat a.txt | grep -i error | wc -l
来源：http://usi.yanxiufei.cn

[R39] 重定向标准输出与错误
来源：http://kjm.yanxiufei.cn

cmd > out.log 2>&1
来源：http://jtb.daria6918.cn

[R40] 追加写日志
来源：http://gua.cheryme.top

echo "log" >> out.log
来源：http://zgz.hcnkem.com

[R41] 丢弃输出
来源：http://tna.dianchejie.cn

cmd >/dev/null 2>&1
来源：http://sxp.ybcxt.top

[R42] 输入重定向
来源：http://ese.sysykeji.top

wc -l < a.txt
来源：http://hzm.316326.xyz

[R43] 按名字查找文件
来源：http://bjc.hnqzz.top

find . -name "*.log" -type f
来源：http://rsr.vehdjk.com

[R44] 按修改时间查找
来源：http://cnm.pengpengdd.cyou

find . -mtime -7 -type f
来源：http://wda.jianghu66.top

[R45] 批量删除
来源：http://kqb.yueranfly.top

find . -name "*.tmp" -delete
来源：http://whf.ydzc1.top

[R46] 递归替换文件内容
来源：http://emx.sjlbkw.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://alr.xuanzx.com

[R47] sed 单行替换
来源：http://upr.zycfv.cn

sed -i 's/foo/bar/g' a.txt
来源：http://rms.cqqwz.cn

[R48] awk 取指定列
来源：http://bsg.andypj.xyz

awk '{print $1, $3}' a.txt
来源：http://uns.yj20258888.top

[R49] awk 带条件
来源：http://vtx.xuetiantiany.cn


<!-- 参考信息 -->