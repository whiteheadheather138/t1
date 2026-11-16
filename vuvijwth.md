代发 wailian999

);
来源：http://xnp.nanxuanxn.top

[Q03] 增加列
来源：http://byc.tanke756.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://jub.havefunace.top

[Q04] 修改列类型
来源：http://rzb.ydjk.org.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://bup.jinghuilouyu.cn

[Q05] 重命名列
来源：http://yme.mhx1999.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://dnu.jianghu66.top

[Q06] 删除列
来源：http://otm.cdnleiting.top

ALTER TABLE users DROP COLUMN age;
来源：http://qni.fengsongda.top

[Q07] 删除表
来源：http://mpf.yonumen.top

DROP TABLE IF EXISTS orders;
来源：http://sqk.ywan-chungtsiang.top

[Q08] 创建普通索引
来源：http://bzy.svipenyu.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://rdh.cdnleiting.top

[Q09] 创建唯一索引
来源：http://uth.zhengqikj.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://emi.zycfv.cn

[Q10] 插入单行
来源：http://fwt.sweek.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://tsd.yvedp.cn

[Q11] 一次插入多行
来源：http://crs.bbcook.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://jmr.zycfv.cn

[Q12] 插入后取自增 ID
来源：http://auz.xinyue.icu

INSERT INTO users (name) VALUES ('C');
来源：http://jot.chenjidiqi.icu

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://prt.zhongyouzk.top

[Q13] 忽略重复插入
来源：http://fho.ydzc1.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://jcm.vehdjk.com

[Q14] 存在则更新（upsert）
来源：http://vir.quarkkingdee.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://xat.wangdashe.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://arf.svipenyu.cn

[Q15] 查询全部
来源：http://bgt.ctjpmb.com

SELECT * FROM users;
来源：http://urm.zhengqikj.top

[Q16] 查询指定列
来源：http://hbk.tanke756.top

SELECT id, name FROM users;
来源：http://sbq.dianchejie.cn

[Q17] 条件查询
来源：http://ahe.fengsongda.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://qvn.hnqzz.top

[Q18] 模糊匹配
来源：http://vrh.316326.xyz

SELECT * FROM users WHERE name LIKE '张%';
来源：http://cvf.pengpengdd.cyou

[Q19] 范围查询
来源：http://lia.gotoacloud.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://cfo.ybcxt.top

[Q20] IN 列表
来源：http://kpg.yuanzhike.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://zri.hnxiangtu.top

[Q21] 空值判断
来源：http://jwg.xziqi.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://xiy.ivvv.top

[Q22] 排序
来源：http://plt.ywan-chungtsiang.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://xce.birdmap.top

[Q23] 分页
来源：http://cky.zhoulong.xyz

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://icu.sufxvd.cn

[Q24] 去重
来源：http://pkr.pycfn.com

SELECT DISTINCT city FROM users;
来源：http://rod.xziqi.cn

[Q25] 只取前 N 条
来源：http://tcb.shanyushiyangkeji.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://bor.zdbjq.cn

[Q26] 计数
来源：http://pje.xuetiantiany.cn

SELECT COUNT(*) FROM users;
来源：http://enh.vehdjk.com

[Q27] 条件计数
来源：http://cjm.zhaomingkeji.xyz

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://oeh.haohaochexian.top

[Q28] 求和与平均
来源：http://hkm.fzhhl.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mtz.snrcjt.cn

[Q29] 最大最小值
来源：http://gyd.zdqjudy.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://nub.sxryk.cn

[Q30] 分组统计
来源：http://qel.aibaodan.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://puh.gaohongyu789.top

[Q31] 分组后过滤
来源：http://izk.bjfxy.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://jko.hywenlv.cn

[Q32] 分组拼接字符串
来源：http://ioa.hongshengwenyu.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://gtn.hnxiangtu.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://rzy.ydjk.org.cn

[Q33] 多列分组
来源：http://nvd.shanyushiyangkeji.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://onh.zhiwuduotai.top

[Q34] 每组取第一条
来源：http://cwo.jinyuanbaomall.cn

SELECT * FROM (
来源：http://tap.aizwys.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://oon.shanyushiyangtech.top

) t WHERE rn = 1;
来源：http://kyf.sufxvd.cn

[Q35] 内连接
来源：http://irn.jinqigfzy.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://pdu.nanxinkj.top

[Q36] 左连接
来源：http://fki.zdqjudy.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://qdd.hcnkem.com

[Q37] 右连接
来源：http://pbw.yangfankeji.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mgp.shangyingyoupin.top

[Q38] 全外连接（PostgreSQL）
来源：http://apx.316326.xyz

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://qax.c1oappe.top

[Q39] 自连接（查上下级）
来源：http://rca.yueranfly.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://twk.chenzaomai.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://zuq.316326.xyz

[Q40] 交叉连接（笛卡尔积）
来源：http://xio.daria6918.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://tux.cheryme.top

[Q41] 多表连接
来源：http://bpm.zhongyouzk.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://wgr.aibaodan.cn

JOIN users u ON u.id = o.user_id
来源：http://val.fanxiaobao.xyz

JOIN products p ON p.id = o.product_id;
来源：http://yce.gogol.net.cn

[Q42] 连接条件附加过滤
来源：http://dnu.zhongyouzk.top

SELECT u.name, o.amount FROM users u
来源：http://mmx.quarkkingdee.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://qdc.redwolf501.top

[Q43] 标量子查询
来源：http://nqt.yj20258888.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mma.jyoumei.cn

[Q44] IN 子查询
来源：http://axb.meibo888.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://dkp.jqgfzy.top

[Q45] EXISTS 判断存在
来源：http://olw.feifeiyinyue.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ztc.meibo888.top

[Q46] NOT EXISTS 判断不存在
来源：http://ljd.chenlongwang.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://pbz.sxryk.cn

[Q47] 与平均值比较
来源：http://hyi.ctjpmb.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://cma.ywan-chungtsiang.top

[Q48] CTE 公用表表达式
来源：http://uff.jinqigfzy.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hzm.ehwqpu.com

SELECT * FROM t WHERE c > 5;
来源：http://uxg.hongshengwenyu.top

[Q49] 更新单行
来源：http://gqp.yueranfly.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://xfb.snrcjt.cn

[Q50] 批量更新
来源：http://qxc.yuxming.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://kxd.yueranfly.top

[Q51] 用子查询更新
来源：http://pmp.bbcook.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://pvb.shangyingyoupin.top

[Q52] 删除指定行
来源：http://txc.aizwys.cn

DELETE FROM users WHERE id = 10;
来源：http://hrs.nanxinkj.top

[Q53] 按条件删除
来源：http://khe.epnwcf.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://gia.jyoumei.cn

[Q54] 清空表
来源：http://kgq.daxiang520.top

TRUNCATE TABLE logs;
来源：http://csj.aizwys.cn

[Q55] 排名（并列占位）
来源：http://ouz.cheryme.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://oad.ywan-chungtsiang.top

[Q56] 密集排名（并列不占位）
来源：http://umr.sweek.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mcj.aibaodan.cn

[Q57] 行号
来源：http://dtq.jiagoushi.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://beq.kuanghao11.cn

[Q58] 累计求和
来源：http://toj.mhx1999.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hih.shanyushiyangkeji.top

[Q59] 分组内累计
来源：http://cra.nwbrower.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://zxg.aizwys.cn

[Q60] 取上一行 / 下一行
来源：http://nat.shangyingyoupin.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wvv.jinqigfzy.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://bnw.jinqigfzy.top

[Q61] 移动平均
来源：http://rog.daria6918.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://dey.yueranfly.top

[Q62] 分组占比
来源：http://yhp.jinqigufen.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://dnf.zhixingplan.top

[Q63] 开启事务
来源：http://kif.chenlongwang.top

START TRANSACTION;                -- 或 BEGIN
来源：http://pir.wangshuangyany.cn

[Q64] 提交事务
来源：http://ohd.sufxvd.cn

COMMIT;
来源：http://owe.epnwcf.com

[Q65] 回滚事务
来源：http://gxu.svipenyu.cn

ROLLBACK;
来源：http://sui.hnqzz.top

[Q66] 行锁查询
来源：http://sdq.daria6918.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://crx.cdnleiting.top

[Q67] 设置隔离级别
来源：http://bah.ehwqpu.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://dvi.chenjidiqi.icu

[Q68] 保存点
来源：http://dgj.xziqi.cn

SAVEPOINT sp1;
来源：http://ayy.havefunace.top

ROLLBACK TO sp1;
来源：http://ggc.kuanghao11.cn

[Q69] 查看执行计划
来源：http://jyy.hcnkem.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://equ.yuanzhike.top

[Q70] 更新统计信息
来源：http://ban.shzxlz.cn

ANALYZE TABLE users;
来源：http://zuc.ybcxt.top

[Q71] 查看建表语句
来源：http://akj.chenjidiqi.icu

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://igc.feifeiyinyue.top

[Q72] 查看索引
来源：http://bnb.sysykeji.top

SHOW INDEX FROM users;
来源：http://weg.yanxiufei.cn

[Q73] 查看表状态
来源：http://ttj.9152youxi.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://qtc.tian-w.cn

[Q74] 强制使用索引
来源：http://ebw.cqqwz.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://pyx.ybcxt.top

[Q75] 日期格式化
来源：http://hvk.hcnkem.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ani.redwolf501.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://zjt.jqgufenzy.top

[Q76] 按天统计
来源：http://efs.tianlin.xyz

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ipp.gzhubu.top

[Q77] 时间加减
来源：http://zkm.zhiwuduotai.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://aex.jqgfzy.top

[Q78] 当前时间
来源：http://uly.vqdsnc.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://omv.yuanzhike.top

[Q79] 字符串拼接
来源：http://own.iojbl.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://pit.tian-w.cn

[Q80] 字符串截取
来源：http://rri.yj20258888.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://uos.dashuyun.cn

[Q81] 字符串替换
来源：http://vsj.nanxuanxn.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://xin.shanyushiyangtech.top

[Q82] 字符长度与字节长度
来源：http://fwa.jinqigufen.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://bwb.gzhubu.top

[Q83] 大小写转换
来源：http://zek.vqdsnc.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://zoe.wangdashe.top

[Q84] 去除首尾空格
来源：http://gws.zhixingplan.top

SELECT TRIM(name) FROM users;
来源：http://doj.epnwcf.com

[Q85] 数值取整
来源：http://hvo.haohaochexian.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://iku.jiagoushi.top

[Q86] 读取 JSON 字段
来源：http://htv.yvedp.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://fim.vehdjk.com

[Q87] JSON 字段做条件
来源：http://woc.redwolf501.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://vke.dianchejie.cn

[Q88] 行转列（条件聚合）
来源：http://itd.sjlbkw.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://xnh.yvedp.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://bdr.nanxuanxn.top

[Q89] 判断表是否存在
来源：http://otw.aibaodan.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hcc.zdqjudy.top

[Q90] 生成序号列
来源：http://bnc.chenzaomai.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wyb.fengsongda.top

================================================================================
来源：http://asx.hcnkem.com

R. Bash 专题
来源：http://pfk.jianghu66.top

================================================================================
来源：http://brk.gotoacloud.top

[R01] shebang 与严格模式
来源：http://fuj.yanxiufei.cn

#!/usr/bin/env bash
来源：http://rry.sxryk.cn

set -euo pipefail
来源：http://aik.andypj.xyz

[R02] 变量赋值与使用
来源：http://icc.xuanzx.com

name="Tom"; echo "$name"
来源：http://dcj.jiagoushi.top

[R03] 只读变量
来源：http://jgt.yj20258.top

readonly PI=3.14
来源：http://lrl.yongpay.top

[R04] 位置参数
来源：http://ygt.jlsjyb.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ntk.ctjpmb.com

[R05] 参数默认值
来源：http://gmv.wangdashe.top

name="${1:-default}"
来源：http://gdj.fktsv.cn

[R06] 判断命令是否存在
来源：http://lsq.guowangkeji.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://vsl.meibo888.top

[R07] if 判断文件
来源：http://rjk.hcnkem.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://eji.meibo888.top

[R08] 数值比较
来源：http://muh.jianghu66.top

if (( a > b )); then echo "a 更大"; fi
来源：http://jin.jqgufenzy.top

[R09] 字符串比较
来源：http://oxi.fzhhl.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ves.hammf.cn

[R10] 正则匹配
来源：http://dmd.ehwqpu.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://acg.epnwcf.com

[R11] case 多分支
来源：http://gwa.cheryme.top

case "$1" in
来源：http://rqj.9152youxi.cn

start) echo "启动" ;;
来源：http://yls.jiagoushi.top

stop)  echo "停止" ;;
来源：http://ayj.mhx1999.top

*)     echo "未知命令" ;;
来源：http://obr.iojbl.cn

esac
来源：http://ujr.snrcjt.cn

[R12] for 遍历文件
来源：http://nof.zhongyouzk.top

for f in *.txt; do echo "$f"; done
来源：http://wpv.fktsv.cn

[R13] for 计数循环
来源：http://zgw.jiagoushi.top

for i in {1..10}; do echo "$i"; done
来源：http://ymq.fzhhl.top

[R14] C 风格 for
来源：http://ost.bbcook.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://uin.yuanzhike.top

[R15] while 逐行读文件
来源：http://drm.pengpengdd.cyou

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://qsr.nanxuanxn.top

[R16] until 等待条件
来源：http://lfa.zhijiandao.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://udl.ppjwa.cn

[R17] 数组定义与取值
来源：http://knz.52xcode.cn

arr=(a b c); echo "${arr[0]}"
来源：http://njr.dashuyun.cn

[R18] 遍历数组
来源：http://zss.gzhubu.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ikv.mhx1999.top

[R19] 数组长度
来源：http://rrm.ydjk.org.cn

echo "${#arr[@]}"
来源：http://wjm.cucudq.cn

[R20] 关联数组（字典）
来源：http://cnd.ivvv.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://rfh.yanxiufei.cn

[R21] 字符串长度
来源：http://ovz.haohaochexian.top

echo "${#s}"
来源：http://bct.pycfn.com

[R22] 截取子串
来源：http://vwu.fehbvm.com

echo "${s:0:5}"
来源：http://far.nanxinkj.top

[R23] 字符串替换
来源：http://eha.jqgufenzy.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://fzy.hongshengwenyu.top

[R24] 大小写转换
来源：http://kjs.chenzaomai.com

echo "${s^^}"; echo "${s,,}"
来源：http://zqt.meibo888.top

[R25] 去后缀 / 去前缀
来源：http://mfs.yuanzhike.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://dal.ctjpmb.com

[R26] 命令替换
来源：http://lwq.chenjidiqi.icu

now=$(date +%F); echo "$now"
来源：http://cqa.birdmap.top

[R27] 算术展开
来源：http://pcr.zdqjudy.top

echo $((1 + 2 * 3))
来源：http://yra.zdbjq.cn

[R28] 浮点运算
来源：http://jkb.kuanghao11.cn

echo "scale=2; 10/3" | bc
来源：http://yao.xinyue.icu

[R29] 定义函数
来源：http://wev.fzhhl.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://pdm.ydjk.org.cn

[R30] 函数返回状态码
来源：http://sbg.ybcxt.top

f() { return 0; }; f || echo "失败了"
来源：http://hly.iojbl.cn

[R31] 局部变量
来源：http://gtx.hammf.cn

f() { local x=1; echo "$x"; }
来源：http://qwh.smart0.xyz

[R32] 参数个数校验
来源：http://dfq.gaohongyu789.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://idw.zhongyouzk.top

[R33] 捕获错误并提示行号
来源：http://zyt.ctjpmb.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://eeg.jqgufenzy.top

[R34] 退出时清理
来源：http://csm.guannengcc.top

trap 'rm -f "$tmp"' EXIT
来源：http://elv.tian-w.cn

[R35] 后台执行并等待
来源：http://tut.xuetiantiany.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://cbf.chenjidiqi.icu

[R36] 并发执行多个任务
来源：http://gep.tian-w.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://luh.xuetiantiany.cn

[R37] 把输出赋给变量
来源：http://spc.nanxinkj.top

files=$(ls -1)
来源：http://rox.meibo888.top

[R38] 管道串联
来源：http://euq.cqqwz.cn

cat a.txt | grep -i error | wc -l
来源：http://sht.0kj1m.cn

[R39] 重定向标准输出与错误
来源：http://nsm.wangdashe.top

cmd > out.log 2>&1
来源：http://upc.daria6918.cn

[R40] 追加写日志
来源：http://kay.quarkkingdee.top

echo "log" >> out.log
来源：http://alt.kuanghao11.cn

[R41] 丢弃输出
来源：http://knv.sysykeji.top

cmd >/dev/null 2>&1
来源：http://zoe.yueranfly.top

[R42] 输入重定向
来源：http://wns.jlsjyb.cn

wc -l < a.txt
来源：http://ufn.jiagoushi.top

[R43] 按名字查找文件
来源：http://coe.jiagoushi.top

find . -name "*.log" -type f
来源：http://grz.zdbjq.cn

[R44] 按修改时间查找
来源：http://egg.xuanzx.com

find . -mtime -7 -type f
来源：http://pnj.yvedp.cn

[R45] 批量删除
来源：http://ygr.yueranfly.top

find . -name "*.tmp" -delete
来源：http://tkq.pycfn.com

[R46] 递归替换文件内容
来源：http://knw.mhx1999.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://cje.zhoulong.xyz

[R47] sed 单行替换
来源：http://jnq.birdmap.top

sed -i 's/foo/bar/g' a.txt
来源：http://foy.tanke756.top

[R48] awk 取指定列
来源：http://hux.guowangkeji.top

awk '{print $1, $3}' a.txt
来源：http://caa.jyoumei.cn

[R49] awk 带条件
来源：http://gfa.yongpay.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://pid.vehdjk.com

[R50] awk 求和
来源：http://igi.fzhhl.top

awk '{s += $2} END {print s}' a.txt
来源：http://jkj.dashuyun.cn

[R51] 排序去重取前几
来源：http://tly.zhoulong.xyz


<!-- 参考信息 -->