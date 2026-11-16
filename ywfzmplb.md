代发 wailian999

CREATE TABLE users (
来源：http://uuy.shanyushiyangkeji.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wxj.dianchejie.cn

name VARCHAR(50) NOT NULL,
来源：http://zgy.gotoacloud.top

email VARCHAR(100) UNIQUE,
来源：http://dfc.nanxinkj.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://dbp.fktsv.cn

);
来源：http://clz.jinqigufen.top

[Q02] 创建带外键的表
来源：http://eyv.pengpengdd.cyou

CREATE TABLE orders (
来源：http://vec.zhoulong.xyz

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://bhs.feifeiyinyue.top

user_id INT NOT NULL,
来源：http://yez.vqdsnc.cn

amount DECIMAL(10, 2),
来源：http://suu.ivvv.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://rzf.yuanzhike.top

);
来源：http://arp.jinghuilouyu.cn

[Q03] 增加列
来源：http://yvk.fzhhl.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://erf.tianlin.xyz

[Q04] 修改列类型
来源：http://nay.epnwcf.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://cfa.xuetiantiany.cn

[Q05] 重命名列
来源：http://ixm.sysykeji.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://pur.pengpengdd.cyou

[Q06] 删除列
来源：http://jyr.tianlin.xyz

ALTER TABLE users DROP COLUMN age;
来源：http://iyz.cdnleiting.top

[Q07] 删除表
来源：http://zel.52xcode.cn

DROP TABLE IF EXISTS orders;
来源：http://oko.yj20258888.top

[Q08] 创建普通索引
来源：http://mwc.chenzaomai.com

CREATE INDEX idx_users_email ON users(email);
来源：http://rto.tanke756.top

[Q09] 创建唯一索引
来源：http://huw.sufxvd.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://asm.smart0.xyz

[Q10] 插入单行
来源：http://ooh.zhoulong.xyz

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mfs.hnxiangtu.top

[Q11] 一次插入多行
来源：http://lae.ehwqpu.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ejc.zhoulong.xyz

[Q12] 插入后取自增 ID
来源：http://czk.yj20258.top

INSERT INTO users (name) VALUES ('C');
来源：http://cnd.yueranfly.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://chp.dianchejie.cn

[Q13] 忽略重复插入
来源：http://ckg.mhx1999.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://iiy.hnxiangtu.top

[Q14] 存在则更新（upsert）
来源：http://zvt.sufxvd.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://cxo.birdmap.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://msi.xylfe.cn

[Q15] 查询全部
来源：http://abu.iojbl.cn

SELECT * FROM users;
来源：http://myu.c1oappe.top

[Q16] 查询指定列
来源：http://gdy.tianlin.xyz

SELECT id, name FROM users;
来源：http://tps.ehwqpu.com

[Q17] 条件查询
来源：http://gib.birdmap.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://nmc.jiagoushi.top

[Q18] 模糊匹配
来源：http://aav.dashuyun.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mvj.fengsongda.top

[Q19] 范围查询
来源：http://gaw.xziqi.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://shc.ctjpmb.com

[Q20] IN 列表
来源：http://xtl.vqdsnc.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mmr.quarkkingdee.top

[Q21] 空值判断
来源：http://luy.c1oappe.top

SELECT * FROM users WHERE email IS NULL;
来源：http://xcb.birdmap.top

[Q22] 排序
来源：http://tbu.wangdashe.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://dnz.hesvh.cn

[Q23] 分页
来源：http://gzs.zhaomingkeji.xyz

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mim.wangshuangyany.cn

[Q24] 去重
来源：http://awd.ybcxt.top

SELECT DISTINCT city FROM users;
来源：http://pgd.xinyue.icu

[Q25] 只取前 N 条
来源：http://mbu.sxryk.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ywf.guowangkeji.top

[Q26] 计数
来源：http://dds.bjfxy.top

SELECT COUNT(*) FROM users;
来源：http://zjg.iojbl.cn

[Q27] 条件计数
来源：http://jml.dianchejie.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://pfd.fehbvm.com

[Q28] 求和与平均
来源：http://gpp.gaohongyu789.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://uzr.tarul.cn

[Q29] 最大最小值
来源：http://agq.shangyingyoupin.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://ixv.sxryk.cn

[Q30] 分组统计
来源：http://bzw.zhijiandao.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://zrd.yangfankeji.com

[Q31] 分组后过滤
来源：http://zwt.wangdashe.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://air.fehbvm.com

[Q32] 分组拼接字符串
来源：http://rkn.shanyushiyangtech.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://dhv.shuidangran.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://zrm.gogol.net.cn

[Q33] 多列分组
来源：http://gfp.quarkkingdee.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hgn.chenzaomai.com

[Q34] 每组取第一条
来源：http://afz.jianghu66.top

SELECT * FROM (
来源：http://owv.ctjpmb.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://bju.xingfuxueyuan.xyz

) t WHERE rn = 1;
来源：http://wvo.kuanghao11.cn

[Q35] 内连接
来源：http://jkm.ydzc1.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ouc.yueranfly.top

[Q36] 左连接
来源：http://koj.xinyue.icu

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hfu.jqgfzy.top

[Q37] 右连接
来源：http://xal.dashuyun.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://lff.yj202588.top

[Q38] 全外连接（PostgreSQL）
来源：http://ibh.aizwys.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ofk.ctjpmb.com

[Q39] 自连接（查上下级）
来源：http://kvz.dianchejie.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://efy.hnxiangtu.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mev.hnqzz.top

[Q40] 交叉连接（笛卡尔积）
来源：http://mqu.gogol.net.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://uun.zhijiandao.cn

[Q41] 多表连接
来源：http://trj.fehbvm.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://lsc.aibaodan.cn

JOIN users u ON u.id = o.user_id
来源：http://tui.yueranfly.top

JOIN products p ON p.id = o.product_id;
来源：http://onq.yueranfly.top

[Q42] 连接条件附加过滤
来源：http://dau.ydzc1.top

SELECT u.name, o.amount FROM users u
来源：http://hgn.bbcook.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://sai.pycfn.com

[Q43] 标量子查询
来源：http://cws.jinyuanbaomall.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://tys.epnwcf.com

[Q44] IN 子查询
来源：http://tfo.pycfn.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://qds.fanxiaobao.xyz

[Q45] EXISTS 判断存在
来源：http://jsm.kuanghao11.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bcl.ppjwa.cn

[Q46] NOT EXISTS 判断不存在
来源：http://lpb.jinqigfzy.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wfl.meibo888.top

[Q47] 与平均值比较
来源：http://otz.birdmap.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://bqh.shangyingyoupin.top

[Q48] CTE 公用表表达式
来源：http://bbi.zycfv.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wlm.yonumen.top

SELECT * FROM t WHERE c > 5;
来源：http://oga.yongpay.top

[Q49] 更新单行
来源：http://dfs.vehdjk.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://tkk.xuanzx.com

[Q50] 批量更新
来源：http://evm.yongpay.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://zrx.sxryk.cn

[Q51] 用子查询更新
来源：http://pcc.9152youxi.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://kgz.zhaomingkeji.xyz

[Q52] 删除指定行
来源：http://hym.pengpengdd.cyou

DELETE FROM users WHERE id = 10;
来源：http://qrm.guowangkeji.top

[Q53] 按条件删除
来源：http://mmw.yangfankeji.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mlw.jinghuilouyu.cn

[Q54] 清空表
来源：http://tez.kuanghao11.cn

TRUNCATE TABLE logs;
来源：http://nha.zhengqikj.top

[Q55] 排名（并列占位）
来源：http://zdz.xziqi.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ypb.snrcjt.cn

[Q56] 密集排名（并列不占位）
来源：http://obi.bbcook.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://xxt.cdnleiting.top

[Q57] 行号
来源：http://loo.cdnleiting.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://xsx.xuanzx.com

[Q58] 累计求和
来源：http://qah.zhaomingkeji.xyz

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ouw.andypj.xyz

[Q59] 分组内累计
来源：http://yuh.hongshengwenyu.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://pai.cashguo.top

[Q60] 取上一行 / 下一行
来源：http://nqd.ppjwa.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://nfx.aizwys.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ywn.tianlin.xyz

[Q61] 移动平均
来源：http://yjs.xinyue.icu

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://qae.xuetiantiany.cn

[Q62] 分组占比
来源：http://int.zhiwuduotai.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://tsu.sjlbkw.cn

[Q63] 开启事务
来源：http://esf.zdqjudy.top

START TRANSACTION;                -- 或 BEGIN
来源：http://ulo.daria6918.cn

[Q64] 提交事务
来源：http://nuf.aibaodan.cn

COMMIT;
来源：http://zgb.hfpthk.cn

[Q65] 回滚事务
来源：http://vhj.hfpthk.cn

ROLLBACK;
来源：http://dex.hnxiangtu.top

[Q66] 行锁查询
来源：http://zbw.316326.xyz

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ndy.cheryme.top

[Q67] 设置隔离级别
来源：http://zyp.guannengcc.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wxt.fktsv.cn

[Q68] 保存点
来源：http://ddl.jinghuilouyu.cn

SAVEPOINT sp1;
来源：http://kfk.316326.xyz

ROLLBACK TO sp1;
来源：http://aen.zhoulong.xyz

[Q69] 查看执行计划
来源：http://zij.cashguo.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://qeu.52xcode.cn

[Q70] 更新统计信息
来源：http://ovb.gotoacloud.top

ANALYZE TABLE users;
来源：http://ecy.jinyuanbaomall.cn

[Q71] 查看建表语句
来源：http://sru.kuanghao11.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://gqf.zdqjudy.top

[Q72] 查看索引
来源：http://gqd.bjfxy.top

SHOW INDEX FROM users;
来源：http://vgg.52xcode.cn

[Q73] 查看表状态
来源：http://kpt.jiagoushi.top

SHOW TABLE STATUS LIKE 'users';
来源：http://oup.jqgfzy.top

[Q74] 强制使用索引
来源：http://qfz.xylfe.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://rpd.zhongyouzk.top

[Q75] 日期格式化
来源：http://dak.shuidangran.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://own.cqqwz.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://nmq.hammf.cn

[Q76] 按天统计
来源：http://oqb.hfpthk.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://znr.fengsongda.top

[Q77] 时间加减
来源：http://lix.yfazqb.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ycg.zhixingplan.top

[Q78] 当前时间
来源：http://gwj.9152youxi.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mxd.nwbrower.top

[Q79] 字符串拼接
来源：http://ecv.tanke756.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://snz.quarkkingdee.top

[Q80] 字符串截取
来源：http://xfn.fanxiaobao.xyz

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hup.pengpengdd.cyou

[Q81] 字符串替换
来源：http://yet.sufxvd.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://gun.hfpthk.cn

[Q82] 字符长度与字节长度
来源：http://fnn.chenzaomai.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://bip.iojbl.cn

[Q83] 大小写转换
来源：http://blj.epnwcf.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hng.yuanzhike.top

[Q84] 去除首尾空格
来源：http://ict.zhiwuduotai.top

SELECT TRIM(name) FROM users;
来源：http://lpn.hfpthk.cn

[Q85] 数值取整
来源：http://cxz.chenjidiqi.icu

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://jnf.xuetiantiany.cn

[Q86] 读取 JSON 字段
来源：http://iur.jqgfzy.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://lfy.wangshuangyany.cn

[Q87] JSON 字段做条件
来源：http://eth.316326.xyz

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://juc.xinyue.icu

[Q88] 行转列（条件聚合）
来源：http://fgy.yfazqb.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://tcp.haohaochexian.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://gjd.xinyue.icu

[Q89] 判断表是否存在
来源：http://pgg.hnxiangtu.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ove.jianghu66.top

[Q90] 生成序号列
来源：http://lrk.zhengqikj.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://byn.ybcxt.top

================================================================================
来源：http://god.sjlbkw.cn

R. Bash 专题
来源：http://sah.gogol.net.cn

================================================================================
来源：http://mao.haohaochexian.top

[R01] shebang 与严格模式
来源：http://xoi.yangfankeji.com

#!/usr/bin/env bash
来源：http://kmu.sysykeji.top

set -euo pipefail
来源：http://rrb.ydzc1.top

[R02] 变量赋值与使用
来源：http://aox.hywenlv.cn

name="Tom"; echo "$name"
来源：http://biu.meibo888.top

[R03] 只读变量
来源：http://oym.hammf.cn

readonly PI=3.14
来源：http://cck.quarkkingdee.top

[R04] 位置参数
来源：http://veo.guowangkeji.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hmj.guowangkeji.top

[R05] 参数默认值
来源：http://urf.xylfe.cn

name="${1:-default}"
来源：http://fep.316326.xyz

[R06] 判断命令是否存在
来源：http://ick.sjlbkw.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://air.guannengcc.top

[R07] if 判断文件
来源：http://wnx.bbcook.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://spy.zhoulong.xyz

[R08] 数值比较
来源：http://hhz.hfpthk.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://egg.nwbrower.top

[R09] 字符串比较
来源：http://lmh.sufxvd.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ytn.zycfv.cn

[R10] 正则匹配
来源：http://lih.jinqigufen.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://qeh.hywenlv.cn

[R11] case 多分支
来源：http://nzn.zhixingplan.top

case "$1" in
来源：http://fxp.cqqwz.cn

start) echo "启动" ;;
来源：http://wzf.jqgfzy.top

stop)  echo "停止" ;;
来源：http://kcx.ydzc1.top

*)     echo "未知命令" ;;
来源：http://ulw.shangyingyoupin.top

esac
来源：http://fnw.sxryk.cn

[R12] for 遍历文件
来源：http://zof.sysykeji.top

for f in *.txt; do echo "$f"; done
来源：http://mqw.epnwcf.com

[R13] for 计数循环
来源：http://lvw.sjlbkw.cn

for i in {1..10}; do echo "$i"; done
来源：http://rya.svipenyu.cn

[R14] C 风格 for
来源：http://pgq.birdmap.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://qwk.c1oappe.top

[R15] while 逐行读文件
来源：http://nnr.zhengqikj.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wwg.svipenyu.cn

[R16] until 等待条件
来源：http://nxf.haohaochexian.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://nhc.yongpay.top

[R17] 数组定义与取值
来源：http://zlr.daxiang520.top

arr=(a b c); echo "${arr[0]}"
来源：http://fxx.daria6918.cn

[R18] 遍历数组
来源：http://lwu.xingfuxueyuan.xyz

for x in "${arr[@]}"; do echo "$x"; done
来源：http://esx.zycfv.cn

[R19] 数组长度
来源：http://cmk.hywenlv.cn

echo "${#arr[@]}"
来源：http://jge.nwbrower.top

[R20] 关联数组（字典）
来源：http://rcl.shuidangran.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://uff.hcnkem.com

[R21] 字符串长度
来源：http://etf.bbcook.cn

echo "${#s}"
来源：http://pmt.hnqzz.top

[R22] 截取子串
来源：http://fuj.tarul.cn

echo "${s:0:5}"
来源：http://uvc.jiagoushi.top

[R23] 字符串替换
来源：http://hsg.chenzaomai.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hsq.jqgfzy.top

[R24] 大小写转换
来源：http://hal.uphjek.com

echo "${s^^}"; echo "${s,,}"
来源：http://djx.jiagoushi.top

[R25] 去后缀 / 去前缀
来源：http://pqw.bjfxy.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://obf.xylfe.cn

[R26] 命令替换
来源：http://vom.epnwcf.com

now=$(date +%F); echo "$now"
来源：http://wxk.cqqwz.cn

[R27] 算术展开
来源：http://mvu.9152youxi.cn

echo $((1 + 2 * 3))
来源：http://lks.ivvv.top

[R28] 浮点运算
来源：http://ikt.shangyingyoupin.top

echo "scale=2; 10/3" | bc
来源：http://rsw.ivvv.top

[R29] 定义函数
来源：http://gfa.sweek.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://rsl.ivvv.top

[R30] 函数返回状态码
来源：http://mtf.jinqigfzy.top

f() { return 0; }; f || echo "失败了"
来源：http://qot.fzhhl.top

[R31] 局部变量
来源：http://ylu.yueranfly.top

f() { local x=1; echo "$x"; }
来源：http://jma.zhaomingkeji.xyz

[R32] 参数个数校验
来源：http://kns.hongshengwenyu.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://cae.pycfn.com

[R33] 捕获错误并提示行号
来源：http://hxj.mhx1999.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://rkt.fktsv.cn

[R34] 退出时清理
来源：http://xzh.tian-w.cn

trap 'rm -f "$tmp"' EXIT
来源：http://fqs.yonumen.top

[R35] 后台执行并等待
来源：http://vdb.vqdsnc.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://atk.tianlin.xyz

[R36] 并发执行多个任务
来源：http://jto.nwbrower.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://zow.tarul.cn

[R37] 把输出赋给变量
来源：http://apn.redwolf501.top

files=$(ls -1)
来源：http://wqi.iojbl.cn

[R38] 管道串联
来源：http://cwr.xinyue.icu

cat a.txt | grep -i error | wc -l
来源：http://yvc.jlsjyb.cn

[R39] 重定向标准输出与错误
来源：http://bwj.ydjk.org.cn

cmd > out.log 2>&1
来源：http://rpg.sysykeji.top

[R40] 追加写日志
来源：http://ynm.sxryk.cn

echo "log" >> out.log
来源：http://idt.9152youxi.cn

[R41] 丢弃输出
来源：http://swl.svipenyu.cn

cmd >/dev/null 2>&1
来源：http://zaf.havefunace.top

[R42] 输入重定向
来源：http://tli.sxryk.cn

wc -l < a.txt
来源：http://dva.zhongyouzk.top

[R43] 按名字查找文件
来源：http://bby.shangyingyoupin.top

find . -name "*.log" -type f
来源：http://gps.9152youxi.cn

[R44] 按修改时间查找
来源：http://ctq.ctjpmb.com

find . -mtime -7 -type f
来源：http://lij.xylfe.cn

[R45] 批量删除
来源：http://vui.jinghuilouyu.cn


<!-- 参考信息 -->