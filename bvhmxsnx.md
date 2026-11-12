代发 wailian999

CREATE TABLE users (
来源：http://cyn.316326.xyz

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://vpm.bjfxy.top

name VARCHAR(50) NOT NULL,
来源：http://ryo.jiagoushi.top

email VARCHAR(100) UNIQUE,
来源：http://axx.wangdashe.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://tjk.svipenyu.cn

);
来源：http://qmw.guowangkeji.top

[Q02] 创建带外键的表
来源：http://hdr.cqqwz.cn

CREATE TABLE orders (
来源：http://oew.nwbrower.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://tag.daria6918.cn

user_id INT NOT NULL,
来源：http://jtj.andypj.xyz

amount DECIMAL(10, 2),
来源：http://xkz.snrcjt.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://qsj.xuetiantiany.cn

);
来源：http://qfo.chenzaomai.com

[Q03] 增加列
来源：http://xft.xylfe.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://nyz.jqgufenzy.top

[Q04] 修改列类型
来源：http://jhy.aizwys.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mry.zdqjudy.top

[Q05] 重命名列
来源：http://pux.quarkkingdee.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hzr.hammf.cn

[Q06] 删除列
来源：http://fty.hammf.cn

ALTER TABLE users DROP COLUMN age;
来源：http://jvg.0kj1m.cn

[Q07] 删除表
来源：http://rtq.aibaodan.cn

DROP TABLE IF EXISTS orders;
来源：http://udh.mhx1999.top

[Q08] 创建普通索引
来源：http://uxi.ydzc1.top

CREATE INDEX idx_users_email ON users(email);
来源：http://aej.pengpengdd.cyou

[Q09] 创建唯一索引
来源：http://lqn.xylfe.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://avq.bbcook.cn

[Q10] 插入单行
来源：http://gnz.chenjidiqi.icu

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://bsr.fktsv.cn

[Q11] 一次插入多行
来源：http://fqg.316326.xyz

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://iqo.jinqigufen.top

[Q12] 插入后取自增 ID
来源：http://vmd.shangyingyoupin.top

INSERT INTO users (name) VALUES ('C');
来源：http://iaf.vehdjk.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mvz.fehbvm.com

[Q13] 忽略重复插入
来源：http://rqn.shuidangran.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://rnc.cheryme.top

[Q14] 存在则更新（upsert）
来源：http://pum.ivvv.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://nst.xinyue.icu

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://gwp.zhiwuduotai.top

[Q15] 查询全部
来源：http://gzo.dianchejie.cn

SELECT * FROM users;
来源：http://fgu.zhaomingkeji.xyz

[Q16] 查询指定列
来源：http://ugr.xuetiantiany.cn

SELECT id, name FROM users;
来源：http://xrt.yj20258.top

[Q17] 条件查询
来源：http://uss.gotoacloud.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://moh.dashuyun.cn

[Q18] 模糊匹配
来源：http://jom.cucudq.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://llp.meibo888.top

[Q19] 范围查询
来源：http://tao.cashguo.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://tme.haohaochexian.top

[Q20] IN 列表
来源：http://map.ydzc1.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://lzy.ivvv.top

[Q21] 空值判断
来源：http://zrd.epnwcf.com

SELECT * FROM users WHERE email IS NULL;
来源：http://bqr.hfpthk.cn

[Q22] 排序
来源：http://brg.cheryme.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://pyt.sxryk.cn

[Q23] 分页
来源：http://jdv.feifeiyinyue.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://npm.shangyingyoupin.top

[Q24] 去重
来源：http://tcd.fengsongda.top

SELECT DISTINCT city FROM users;
来源：http://mtq.dianchejie.cn

[Q25] 只取前 N 条
来源：http://chu.cheryme.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ixn.chenlongwang.top

[Q26] 计数
来源：http://vok.hywenlv.cn

SELECT COUNT(*) FROM users;
来源：http://rjt.tianlin.xyz

[Q27] 条件计数
来源：http://mhv.shanyushiyangkeji.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://jhv.yanxiufei.cn

[Q28] 求和与平均
来源：http://wpg.vqdsnc.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://doo.zhixingplan.top

[Q29] 最大最小值
来源：http://sql.guannengcc.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://okj.jinghuilouyu.cn

[Q30] 分组统计
来源：http://hew.kuanghao11.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://xyg.ctjpmb.com

[Q31] 分组后过滤
来源：http://vsv.yuxming.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ebp.aizwys.cn

[Q32] 分组拼接字符串
来源：http://wjh.yj202588.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://nfw.0kj1m.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://kwq.ywan-chungtsiang.top

[Q33] 多列分组
来源：http://lnz.hnxiangtu.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://cwl.hywenlv.cn

[Q34] 每组取第一条
来源：http://tjw.zhiwuduotai.top

SELECT * FROM (
来源：http://kmq.zhoulong.xyz

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://xgt.fktsv.cn

) t WHERE rn = 1;
来源：http://qqv.hammf.cn

[Q35] 内连接
来源：http://nhx.mhx1999.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://tmg.yj20258.top

[Q36] 左连接
来源：http://mpr.dashuyun.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://lck.yuanzhike.top

[Q37] 右连接
来源：http://gvx.uphjek.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://llt.9152youxi.cn

[Q38] 全外连接（PostgreSQL）
来源：http://gic.c1oappe.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://qcs.zhengqikj.top

[Q39] 自连接（查上下级）
来源：http://vqx.gzhubu.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://kbz.hnqzz.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://kom.hammf.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://qcr.chenzaomai.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://tia.0kj1m.cn

[Q41] 多表连接
来源：http://yjv.fzhhl.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://lty.chenlongwang.top

JOIN users u ON u.id = o.user_id
来源：http://chp.zhengqikj.top

JOIN products p ON p.id = o.product_id;
来源：http://ifx.gzhubu.top

[Q42] 连接条件附加过滤
来源：http://yqc.snrcjt.cn

SELECT u.name, o.amount FROM users u
来源：http://gvu.guowangkeji.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://iar.smart0.xyz

[Q43] 标量子查询
来源：http://hef.yuxming.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://que.hongshengwenyu.top

[Q44] IN 子查询
来源：http://cvp.shangyingyoupin.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://dct.feifeiyinyue.top

[Q45] EXISTS 判断存在
来源：http://xil.sxryk.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jxs.daria6918.cn

[Q46] NOT EXISTS 判断不存在
来源：http://tue.zhiwuduotai.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fxd.jinqigfzy.top

[Q47] 与平均值比较
来源：http://tuj.shanyushiyangkeji.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://agg.zhijiandao.cn

[Q48] CTE 公用表表达式
来源：http://dms.chenjidiqi.icu

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ofr.xingfuxueyuan.xyz

SELECT * FROM t WHERE c > 5;
来源：http://mbe.tianlin.xyz

[Q49] 更新单行
来源：http://lam.ywan-chungtsiang.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://rmb.gogol.net.cn

[Q50] 批量更新
来源：http://sif.cdnleiting.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ugy.jiagoushi.top

[Q51] 用子查询更新
来源：http://fcj.sxryk.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://nnw.fktsv.cn

[Q52] 删除指定行
来源：http://gat.fengsongda.top

DELETE FROM users WHERE id = 10;
来源：http://ucx.zycfv.cn

[Q53] 按条件删除
来源：http://lja.xuanzx.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://umm.yongpay.top

[Q54] 清空表
来源：http://xmx.fzhhl.top

TRUNCATE TABLE logs;
来源：http://dda.52xcode.cn

[Q55] 排名（并列占位）
来源：http://ydm.c1oappe.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://jbs.hysaishi.cn

[Q56] 密集排名（并列不占位）
来源：http://uyy.aizwys.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://eqq.ywan-chungtsiang.top

[Q57] 行号
来源：http://yxe.epnwcf.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://tio.fehbvm.com

[Q58] 累计求和
来源：http://ckt.jiagoushi.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://qra.aizwys.cn

[Q59] 分组内累计
来源：http://zkx.jinqigufen.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ipw.ivvv.top

[Q60] 取上一行 / 下一行
来源：http://bjq.fengsongda.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://unn.gogol.net.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://tlp.sysykeji.top

[Q61] 移动平均
来源：http://yxn.zhoulong.xyz

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://gnz.52xcode.cn

[Q62] 分组占比
来源：http://rnc.jianghu66.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://vha.ydjk.org.cn

[Q63] 开启事务
来源：http://bhy.yj20258.top

START TRANSACTION;                -- 或 BEGIN
来源：http://wnv.gogol.net.cn

[Q64] 提交事务
来源：http://qzh.bjfxy.top

COMMIT;
来源：http://gng.epnwcf.com

[Q65] 回滚事务
来源：http://ovs.haohaochexian.top

ROLLBACK;
来源：http://vjg.ydjk.org.cn

[Q66] 行锁查询
来源：http://bem.jlsjyb.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://sgq.wangdashe.top

[Q67] 设置隔离级别
来源：http://zyv.xinyue.icu

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ext.dianchejie.cn

[Q68] 保存点
来源：http://pnm.shzxlz.cn

SAVEPOINT sp1;
来源：http://nuu.zhijiandao.cn

ROLLBACK TO sp1;
来源：http://tma.ydjk.org.cn

[Q69] 查看执行计划
来源：http://kqx.pycfn.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ubi.aibaodan.cn

[Q70] 更新统计信息
来源：http://dup.nanxinkj.top

ANALYZE TABLE users;
来源：http://czn.hnqzz.top

[Q71] 查看建表语句
来源：http://whq.daxiang520.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ngu.cqqwz.cn

[Q72] 查看索引
来源：http://yof.xingfuxueyuan.xyz

SHOW INDEX FROM users;
来源：http://kcf.sweek.top

[Q73] 查看表状态
来源：http://pqe.cqqwz.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://hbl.fanxiaobao.xyz

[Q74] 强制使用索引
来源：http://nbn.andypj.xyz

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://dsr.daxiang520.top

[Q75] 日期格式化
来源：http://iaw.nwbrower.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://zdw.zhengqikj.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://gxw.dashuyun.cn

[Q76] 按天统计
来源：http://vta.feifeiyinyue.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://oex.yj20258888.top

[Q77] 时间加减
来源：http://idx.nwbrower.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://dli.zycfv.cn

[Q78] 当前时间
来源：http://vdb.yonumen.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://chj.hammf.cn

[Q79] 字符串拼接
来源：http://xqh.shuidangran.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://lfd.kuanghao11.cn

[Q80] 字符串截取
来源：http://pom.chenzaomai.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://zdq.yj20258.top

[Q81] 字符串替换
来源：http://rlt.redwolf501.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mvx.tanke756.top

[Q82] 字符长度与字节长度
来源：http://ant.yangfankeji.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://jfl.0kj1m.cn

[Q83] 大小写转换
来源：http://rwg.guowangkeji.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://kwh.yanxiufei.cn

[Q84] 去除首尾空格
来源：http://mey.xuanzx.com

SELECT TRIM(name) FROM users;
来源：http://zfj.tianlin.xyz

[Q85] 数值取整
来源：http://edf.ctjpmb.com

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hmi.shangyingyoupin.top

[Q86] 读取 JSON 字段
来源：http://ybz.wangdashe.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://tho.cqqwz.cn

[Q87] JSON 字段做条件
来源：http://ahg.nanxuanxn.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hnk.jqgufenzy.top

[Q88] 行转列（条件聚合）
来源：http://cch.vqdsnc.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://elv.wangshuangyany.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://dex.epnwcf.com

[Q89] 判断表是否存在
来源：http://cph.jlsjyb.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wlt.shuidangran.top

[Q90] 生成序号列
来源：http://yma.andypj.xyz

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://aez.zhoulong.xyz

================================================================================
来源：http://xab.dashuyun.cn

R. Bash 专题
来源：http://nfu.quarkkingdee.top

================================================================================
来源：http://jcp.hfpthk.cn

[R01] shebang 与严格模式
来源：http://nyt.yj202588.top

#!/usr/bin/env bash
来源：http://tmj.ppjwa.cn

set -euo pipefail
来源：http://ydn.nanxinkj.top

[R02] 变量赋值与使用
来源：http://azx.ivvv.top

name="Tom"; echo "$name"
来源：http://kgr.yuanzhike.top

[R03] 只读变量
来源：http://kjk.cashguo.top

readonly PI=3.14
来源：http://tzd.fzhhl.top

[R04] 位置参数
来源：http://hru.cqqwz.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://dde.zhoulong.xyz

[R05] 参数默认值
来源：http://mlq.fehbvm.com

name="${1:-default}"
来源：http://daz.daria6918.cn

[R06] 判断命令是否存在
来源：http://ntm.ivvv.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://evy.birdmap.top

[R07] if 判断文件
来源：http://pta.yj202588.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://aqc.hammf.cn

[R08] 数值比较
来源：http://uvl.pengpengdd.cyou

if (( a > b )); then echo "a 更大"; fi
来源：http://tpm.andypj.xyz

[R09] 字符串比较
来源：http://hkm.shuidangran.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://gza.mhx1999.top

[R10] 正则匹配
来源：http://ldp.chenzaomai.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://xgj.nwbrower.top

[R11] case 多分支
来源：http://hlz.fktsv.cn

case "$1" in
来源：http://zkb.feifeiyinyue.top

start) echo "启动" ;;
来源：http://efd.yfazqb.com

stop)  echo "停止" ;;
来源：http://kos.xuetiantiany.cn

*)     echo "未知命令" ;;
来源：http://iha.hfpthk.cn

esac
来源：http://abo.0kj1m.cn

[R12] for 遍历文件
来源：http://kay.uphjek.com

for f in *.txt; do echo "$f"; done
来源：http://mxi.yj202588.top

[R13] for 计数循环
来源：http://mld.ppjwa.cn

for i in {1..10}; do echo "$i"; done
来源：http://lcr.zycfv.cn

[R14] C 风格 for
来源：http://ymg.quarkkingdee.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://pph.nanxuanxn.top

[R15] while 逐行读文件
来源：http://rlt.haohaochexian.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mov.svipenyu.cn

[R16] until 等待条件
来源：http://wrm.gzhubu.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wll.hywenlv.cn

[R17] 数组定义与取值
来源：http://vpn.zdbjq.cn

arr=(a b c); echo "${arr[0]}"
来源：http://wek.kuanghao11.cn

[R18] 遍历数组
来源：http://bji.guannengcc.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://kds.tianlin.xyz

[R19] 数组长度
来源：http://zkj.yj20258888.top

echo "${#arr[@]}"
来源：http://wfv.hammf.cn

[R20] 关联数组（字典）
来源：http://yuv.jiagoushi.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://frx.zdbjq.cn

[R21] 字符串长度
来源：http://mqs.nwbrower.top

echo "${#s}"
来源：http://fts.xuanzx.com

[R22] 截取子串
来源：http://afb.fengsongda.top

echo "${s:0:5}"
来源：http://ndq.jyoumei.cn

[R23] 字符串替换
来源：http://pxm.yueranfly.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://eke.ydzc1.top

[R24] 大小写转换
来源：http://ctv.ivvv.top

echo "${s^^}"; echo "${s,,}"
来源：http://flb.aibaodan.cn

[R25] 去后缀 / 去前缀
来源：http://qtj.jqgfzy.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://duh.pengpengdd.cyou

[R26] 命令替换
来源：http://msf.tian-w.cn

now=$(date +%F); echo "$now"
来源：http://ntu.guannengcc.top

[R27] 算术展开
来源：http://hzs.vehdjk.com

echo $((1 + 2 * 3))
来源：http://ttm.vehdjk.com

[R28] 浮点运算
来源：http://cnr.chenjidiqi.icu

echo "scale=2; 10/3" | bc
来源：http://gub.zhaomingkeji.xyz

[R29] 定义函数
来源：http://vpq.uphjek.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://fhc.ydjk.org.cn

[R30] 函数返回状态码
来源：http://txq.feifeiyinyue.top

f() { return 0; }; f || echo "失败了"
来源：http://ngy.dianchejie.cn

[R31] 局部变量
来源：http://bdf.fanxiaobao.xyz

f() { local x=1; echo "$x"; }
来源：http://nsy.aibaodan.cn

[R32] 参数个数校验
来源：http://vtx.xingfuxueyuan.xyz

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://nwk.cdnleiting.top

[R33] 捕获错误并提示行号
来源：http://trz.guowangkeji.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://zwp.xziqi.cn

[R34] 退出时清理
来源：http://nos.cdnleiting.top

trap 'rm -f "$tmp"' EXIT
来源：http://ypm.meibo888.top

[R35] 后台执行并等待
来源：http://hkj.xinyue.icu

sleep 5 & pid=$!; wait "$pid"
来源：http://cbz.zhaomingkeji.xyz

[R36] 并发执行多个任务
来源：http://wjg.ppjwa.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://jhu.hfpthk.cn

[R37] 把输出赋给变量
来源：http://gxq.guowangkeji.top

files=$(ls -1)
来源：http://nzj.ctjpmb.com

[R38] 管道串联
来源：http://ylc.hnxiangtu.top

cat a.txt | grep -i error | wc -l
来源：http://pgv.zdbjq.cn

[R39] 重定向标准输出与错误
来源：http://fpt.quarkkingdee.top

cmd > out.log 2>&1
来源：http://ocv.guannengcc.top

[R40] 追加写日志
来源：http://hyd.jinyuanbaomall.cn

echo "log" >> out.log
来源：http://gkw.quarkkingdee.top

[R41] 丢弃输出
来源：http://hse.aizwys.cn

cmd >/dev/null 2>&1
来源：http://gci.hfpthk.cn

[R42] 输入重定向
来源：http://dno.jiagoushi.top

wc -l < a.txt
来源：http://yxf.sjlbkw.cn

[R43] 按名字查找文件
来源：http://dad.redwolf501.top

find . -name "*.log" -type f
来源：http://vpe.tianlin.xyz

[R44] 按修改时间查找
来源：http://xnf.chenlongwang.top

find . -mtime -7 -type f
来源：http://dbw.yj20258888.top

[R45] 批量删除
来源：http://uga.feifeiyinyue.top


<!-- 参考信息 -->