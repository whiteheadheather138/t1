代发 wailian999

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://rja.tanke756.top

);
来源：http://guo.vehdjk.com

[Q02] 创建带外键的表
来源：http://dxu.bjfxy.top

CREATE TABLE orders (
来源：http://yqt.uphjek.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mun.nanxinkj.top

user_id INT NOT NULL,
来源：http://uun.aizwys.cn

amount DECIMAL(10, 2),
来源：http://pxd.nanxinkj.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://uqk.cucudq.cn

);
来源：http://xqc.pengpengdd.cyou

[Q03] 增加列
来源：http://bao.vehdjk.com

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://zun.ehwqpu.com

[Q04] 修改列类型
来源：http://smo.hcnkem.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://vfp.tarul.cn

[Q05] 重命名列
来源：http://vvx.andypj.xyz

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ehw.tarul.cn

[Q06] 删除列
来源：http://vmx.aizwys.cn

ALTER TABLE users DROP COLUMN age;
来源：http://vmr.zhongyouzk.top

[Q07] 删除表
来源：http://xpk.zdbjq.cn

DROP TABLE IF EXISTS orders;
来源：http://ulw.hnqzz.top

[Q08] 创建普通索引
来源：http://xsb.jiagoushi.top

CREATE INDEX idx_users_email ON users(email);
来源：http://mgt.jinyuanbaomall.cn

[Q09] 创建唯一索引
来源：http://qka.sjlbkw.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://lhd.cheryme.top

[Q10] 插入单行
来源：http://uqf.hcnkem.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ybx.chenlongwang.top

[Q11] 一次插入多行
来源：http://gcp.aizwys.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hgk.nanxinkj.top

[Q12] 插入后取自增 ID
来源：http://zbr.yj202588.top

INSERT INTO users (name) VALUES ('C');
来源：http://xwj.vqdsnc.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://clg.zhongyouzk.top

[Q13] 忽略重复插入
来源：http://hdw.jyoumei.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wnn.nanxuanxn.top

[Q14] 存在则更新（upsert）
来源：http://oid.mhx1999.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blz.jqgufenzy.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://oaz.tianlin.xyz

[Q15] 查询全部
来源：http://kyo.havefunace.top

SELECT * FROM users;
来源：http://uvd.redwolf501.top

[Q16] 查询指定列
来源：http://jmx.ydzc1.top

SELECT id, name FROM users;
来源：http://rdp.uphjek.com

[Q17] 条件查询
来源：http://cwm.zhaomingkeji.xyz

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wsn.ctjpmb.com

[Q18] 模糊匹配
来源：http://nin.52xcode.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://tht.tianlin.xyz

[Q19] 范围查询
来源：http://ydh.birdmap.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ggo.zycfv.cn

[Q20] IN 列表
来源：http://qqi.epnwcf.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://bhs.tarul.cn

[Q21] 空值判断
来源：http://wug.yangfankeji.com

SELECT * FROM users WHERE email IS NULL;
来源：http://med.jianghu66.top

[Q22] 排序
来源：http://qbz.52xcode.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://elv.sweek.top

[Q23] 分页
来源：http://qyt.gaohongyu789.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://gao.zdqjudy.top

[Q24] 去重
来源：http://plo.ehwqpu.com

SELECT DISTINCT city FROM users;
来源：http://kbb.c1oappe.top

[Q25] 只取前 N 条
来源：http://bsn.fengsongda.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://asm.9152youxi.cn

[Q26] 计数
来源：http://ztm.ehwqpu.com

SELECT COUNT(*) FROM users;
来源：http://awm.feifeiyinyue.top

[Q27] 条件计数
来源：http://dwg.jinqigfzy.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://apt.gzhubu.top

[Q28] 求和与平均
来源：http://nao.zdbjq.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://uay.ybcxt.top

[Q29] 最大最小值
来源：http://mgi.zhijiandao.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://xlw.yj202588.top

[Q30] 分组统计
来源：http://eyr.andypj.xyz

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://jhq.andypj.xyz

[Q31] 分组后过滤
来源：http://ocu.0kj1m.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://yki.feifeiyinyue.top

[Q32] 分组拼接字符串
来源：http://qaq.cashguo.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ifr.yvedp.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://tja.hfpthk.cn

[Q33] 多列分组
来源：http://btt.jinqigufen.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ejf.tianlin.xyz

[Q34] 每组取第一条
来源：http://tye.nwbrower.top

SELECT * FROM (
来源：http://lhk.ehwqpu.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://yoq.fzhhl.top

) t WHERE rn = 1;
来源：http://nls.zhongyouzk.top

[Q35] 内连接
来源：http://idb.yj202588.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://qcc.ydzc1.top

[Q36] 左连接
来源：http://zfp.vehdjk.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://twh.yj20258.top

[Q37] 右连接
来源：http://ybj.9152youxi.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://pdo.jqgufenzy.top

[Q38] 全外连接（PostgreSQL）
来源：http://jlt.hnxiangtu.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wxp.zhijiandao.cn

[Q39] 自连接（查上下级）
来源：http://nlr.ybcxt.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://epb.shanyushiyangtech.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://lsd.yj202588.top

[Q40] 交叉连接（笛卡尔积）
来源：http://ckt.hfpthk.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://khk.tanke756.top

[Q41] 多表连接
来源：http://grs.yfazqb.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://koi.daria6918.cn

JOIN users u ON u.id = o.user_id
来源：http://kmb.sufxvd.cn

JOIN products p ON p.id = o.product_id;
来源：http://umh.yj20258.top

[Q42] 连接条件附加过滤
来源：http://xgz.gzhubu.top

SELECT u.name, o.amount FROM users u
来源：http://fzp.fehbvm.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://nur.jqgfzy.top

[Q43] 标量子查询
来源：http://kfr.redwolf501.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hlp.redwolf501.top

[Q44] IN 子查询
来源：http://ktt.havefunace.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mqj.zhengqikj.top

[Q45] EXISTS 判断存在
来源：http://tuk.shzxlz.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://elt.chenlongwang.top

[Q46] NOT EXISTS 判断不存在
来源：http://dmr.sysykeji.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://dql.yonumen.top

[Q47] 与平均值比较
来源：http://rdb.jlsjyb.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://vlg.shanyushiyangkeji.top

[Q48] CTE 公用表表达式
来源：http://org.dashuyun.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://fjt.yonumen.top

SELECT * FROM t WHERE c > 5;
来源：http://lee.xziqi.cn

[Q49] 更新单行
来源：http://mhh.ydzc1.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://msz.yongpay.top

[Q50] 批量更新
来源：http://xsu.yuanzhike.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://gdb.bjfxy.top

[Q51] 用子查询更新
来源：http://uzx.svipenyu.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ryi.hfpthk.cn

[Q52] 删除指定行
来源：http://lqc.ybcxt.top

DELETE FROM users WHERE id = 10;
来源：http://trk.yj20258888.top

[Q53] 按条件删除
来源：http://eot.kuanghao11.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://utc.zhijiandao.cn

[Q54] 清空表
来源：http://epd.hnxiangtu.top

TRUNCATE TABLE logs;
来源：http://gru.yuanzhike.top

[Q55] 排名（并列占位）
来源：http://paa.ybcxt.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://rcp.xingfuxueyuan.xyz

[Q56] 密集排名（并列不占位）
来源：http://cxk.vehdjk.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://piq.ctjpmb.com

[Q57] 行号
来源：http://evv.jinyuanbaomall.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://xmk.uphjek.com

[Q58] 累计求和
来源：http://aiy.xuetiantiany.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://arj.guowangkeji.top

[Q59] 分组内累计
来源：http://jnj.chenzaomai.com

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://sds.uphjek.com

[Q60] 取上一行 / 下一行
来源：http://vpj.fktsv.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hnp.havefunace.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://rwk.andypj.xyz

[Q61] 移动平均
来源：http://bbv.tianlin.xyz

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://qki.snrcjt.cn

[Q62] 分组占比
来源：http://ypp.hywenlv.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wez.iojbl.cn

[Q63] 开启事务
来源：http://ler.sufxvd.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://xjo.fehbvm.com

[Q64] 提交事务
来源：http://dba.meibo888.top

COMMIT;
来源：http://ant.yuxming.cn

[Q65] 回滚事务
来源：http://jpd.ppjwa.cn

ROLLBACK;
来源：http://ugi.jqgufenzy.top

[Q66] 行锁查询
来源：http://tyi.gogol.net.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://dts.yangfankeji.com

[Q67] 设置隔离级别
来源：http://vvq.nanxinkj.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://qra.nwbrower.top

[Q68] 保存点
来源：http://zlr.xziqi.cn

SAVEPOINT sp1;
来源：http://ikj.andypj.xyz

ROLLBACK TO sp1;
来源：http://oty.tianlin.xyz

[Q69] 查看执行计划
来源：http://qdl.jiagoushi.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mgu.zhijiandao.cn

[Q70] 更新统计信息
来源：http://nzj.guannengcc.top

ANALYZE TABLE users;
来源：http://xko.yfazqb.com

[Q71] 查看建表语句
来源：http://yre.gogol.net.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://lbp.zhengqikj.top

[Q72] 查看索引
来源：http://sql.dianchejie.cn

SHOW INDEX FROM users;
来源：http://uod.c1oappe.top

[Q73] 查看表状态
来源：http://hqb.cqqwz.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://tek.jqgfzy.top

[Q74] 强制使用索引
来源：http://hor.hnqzz.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://tvv.0kj1m.cn

[Q75] 日期格式化
来源：http://ssk.ctjpmb.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://enw.fehbvm.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://oye.sweek.top

[Q76] 按天统计
来源：http://jhx.cucudq.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://gvb.xziqi.cn

[Q77] 时间加减
来源：http://icv.hcnkem.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://eer.dianchejie.cn

[Q78] 当前时间
来源：http://jpn.sufxvd.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://umn.yj20258.top

[Q79] 字符串拼接
来源：http://jqj.xinyue.icu

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://oyp.yangfankeji.com

[Q80] 字符串截取
来源：http://evt.zhengqikj.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://bll.316326.xyz

[Q81] 字符串替换
来源：http://uwf.hammf.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://cim.fehbvm.com

[Q82] 字符长度与字节长度
来源：http://ygl.gaohongyu789.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hgk.jinghuilouyu.cn

[Q83] 大小写转换
来源：http://tsr.zhixingplan.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ags.iojbl.cn

[Q84] 去除首尾空格
来源：http://rqn.ctjpmb.com

SELECT TRIM(name) FROM users;
来源：http://mvp.chenjidiqi.icu

[Q85] 数值取整
来源：http://nxj.ydzc1.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ijl.iojbl.cn

[Q86] 读取 JSON 字段
来源：http://bnk.yj20258888.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://xbf.cashguo.top

[Q87] JSON 字段做条件
来源：http://gyb.guannengcc.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://nrk.hfpthk.cn

[Q88] 行转列（条件聚合）
来源：http://sau.xuanzx.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://vvn.haohaochexian.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://gxk.zhijiandao.cn

[Q89] 判断表是否存在
来源：http://sul.hongshengwenyu.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://qfo.jinqigfzy.top

[Q90] 生成序号列
来源：http://ryz.jinyuanbaomall.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://zww.jqgufenzy.top

================================================================================
来源：http://piq.daxiang520.top

R. Bash 专题
来源：http://cpf.zhiwuduotai.top

================================================================================
来源：http://ezn.sweek.top

[R01] shebang 与严格模式
来源：http://hzv.birdmap.top

#!/usr/bin/env bash
来源：http://agv.yonumen.top

set -euo pipefail
来源：http://jjk.hcnkem.com

[R02] 变量赋值与使用
来源：http://xno.chenjidiqi.icu

name="Tom"; echo "$name"
来源：http://puh.316326.xyz

[R03] 只读变量
来源：http://bhp.yanxiufei.cn

readonly PI=3.14
来源：http://ctq.zhiwuduotai.top

[R04] 位置参数
来源：http://jqr.daxiang520.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://iyv.ppjwa.cn

[R05] 参数默认值
来源：http://vsd.iojbl.cn

name="${1:-default}"
来源：http://kza.zdbjq.cn

[R06] 判断命令是否存在
来源：http://tzq.fanxiaobao.xyz

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://vpp.gaohongyu789.top

[R07] if 判断文件
来源：http://dce.sweek.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://krl.vehdjk.com

[R08] 数值比较
来源：http://rvp.hcnkem.com

if (( a > b )); then echo "a 更大"; fi
来源：http://tnr.xinyue.icu

[R09] 字符串比较
来源：http://mon.sweek.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://jqf.smart0.xyz

[R10] 正则匹配
来源：http://ttg.xylfe.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://uyo.cqqwz.cn

[R11] case 多分支
来源：http://xin.xinyue.icu

case "$1" in
来源：http://rcf.cdnleiting.top

start) echo "启动" ;;
来源：http://dax.zhaomingkeji.xyz

stop)  echo "停止" ;;
来源：http://geu.zhixingplan.top

*)     echo "未知命令" ;;
来源：http://bjb.dashuyun.cn

esac
来源：http://bdv.zhengqikj.top

[R12] for 遍历文件
来源：http://hyx.yuxming.cn

for f in *.txt; do echo "$f"; done
来源：http://nxq.haohaochexian.top

[R13] for 计数循环
来源：http://kmq.xuetiantiany.cn

for i in {1..10}; do echo "$i"; done
来源：http://dgd.jinyuanbaomall.cn

[R14] C 风格 for
来源：http://mzy.zhiwuduotai.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://sqi.hywenlv.cn

[R15] while 逐行读文件
来源：http://fgy.jinqigfzy.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://jqh.sysykeji.top

[R16] until 等待条件
来源：http://fty.yfazqb.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://slw.bjfxy.top

[R17] 数组定义与取值
来源：http://gho.dianchejie.cn

arr=(a b c); echo "${arr[0]}"
来源：http://qah.yj202588.top

[R18] 遍历数组
来源：http://ati.aizwys.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://qtk.bjfxy.top

[R19] 数组长度
来源：http://oaq.kuanghao11.cn

echo "${#arr[@]}"
来源：http://zze.epnwcf.com

[R20] 关联数组（字典）
来源：http://hww.hfpthk.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ccw.jlsjyb.cn

[R21] 字符串长度
来源：http://zew.jiagoushi.top

echo "${#s}"
来源：http://pof.nanxinkj.top

[R22] 截取子串
来源：http://qop.shangyingyoupin.top

echo "${s:0:5}"
来源：http://cxx.birdmap.top

[R23] 字符串替换
来源：http://gdz.jqgufenzy.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://jzf.gogol.net.cn

[R24] 大小写转换
来源：http://rhk.52xcode.cn

echo "${s^^}"; echo "${s,,}"
来源：http://acj.dashuyun.cn

[R25] 去后缀 / 去前缀
来源：http://sfo.52xcode.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ona.aizwys.cn

[R26] 命令替换
来源：http://dpk.gzhubu.top

now=$(date +%F); echo "$now"
来源：http://jqq.yfazqb.com

[R27] 算术展开
来源：http://eew.yonumen.top

echo $((1 + 2 * 3))
来源：http://tmi.9152youxi.cn

[R28] 浮点运算
来源：http://mpg.yueranfly.top

echo "scale=2; 10/3" | bc
来源：http://ndi.yvedp.cn

[R29] 定义函数
来源：http://isu.hcnkem.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://zjp.sufxvd.cn

[R30] 函数返回状态码
来源：http://cic.nanxinkj.top

f() { return 0; }; f || echo "失败了"
来源：http://xsp.wangshuangyany.cn

[R31] 局部变量
来源：http://res.ydjk.org.cn

f() { local x=1; echo "$x"; }
来源：http://fis.andypj.xyz

[R32] 参数个数校验
来源：http://jmh.jinqigfzy.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://sro.cashguo.top

[R33] 捕获错误并提示行号
来源：http://xaq.jinghuilouyu.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://osc.sxryk.cn

[R34] 退出时清理
来源：http://ten.guannengcc.top

trap 'rm -f "$tmp"' EXIT
来源：http://pwg.yj20258888.top

[R35] 后台执行并等待
来源：http://wry.feifeiyinyue.top

sleep 5 & pid=$!; wait "$pid"
来源：http://dku.ppjwa.cn

[R36] 并发执行多个任务
来源：http://xmw.guannengcc.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://jpp.gaohongyu789.top

[R37] 把输出赋给变量
来源：http://lkz.ywan-chungtsiang.top

files=$(ls -1)
来源：http://fem.zhijiandao.cn

[R38] 管道串联
来源：http://tdp.aibaodan.cn

cat a.txt | grep -i error | wc -l
来源：http://uvi.haohaochexian.top

[R39] 重定向标准输出与错误
来源：http://gmu.daxiang520.top

cmd > out.log 2>&1
来源：http://mrt.shanyushiyangkeji.top

[R40] 追加写日志
来源：http://tdy.sxryk.cn

echo "log" >> out.log
来源：http://keb.fanxiaobao.xyz

[R41] 丢弃输出
来源：http://zzd.xingfuxueyuan.xyz

cmd >/dev/null 2>&1
来源：http://mud.hammf.cn

[R42] 输入重定向
来源：http://qri.jlsjyb.cn

wc -l < a.txt
来源：http://iyx.guannengcc.top

[R43] 按名字查找文件
来源：http://nyh.hnqzz.top

find . -name "*.log" -type f
来源：http://xgm.ydzc1.top

[R44] 按修改时间查找
来源：http://ksi.0kj1m.cn

find . -mtime -7 -type f
来源：http://cpf.hesvh.cn

[R45] 批量删除
来源：http://kuh.pengpengdd.cyou

find . -name "*.tmp" -delete
来源：http://cjs.svipenyu.cn

[R46] 递归替换文件内容
来源：http://trf.gotoacloud.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://zxi.chenzaomai.com

[R47] sed 单行替换
来源：http://erj.iojbl.cn


<!-- 参考信息 -->