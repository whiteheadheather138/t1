代发 wailian999

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://jsl.xziqi.cn

);
来源：http://vdt.mhx1999.top

[Q02] 创建带外键的表
来源：http://rpe.fanxiaobao.xyz

CREATE TABLE orders (
来源：http://yjk.cashguo.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://axu.pengpengdd.cyou

user_id INT NOT NULL,
来源：http://nyn.jianghu66.top

amount DECIMAL(10, 2),
来源：http://srr.hongshengwenyu.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://zmw.fehbvm.com

);
来源：http://sof.ywan-chungtsiang.top

[Q03] 增加列
来源：http://gcg.haohaochexian.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ckb.zdbjq.cn

[Q04] 修改列类型
来源：http://lza.guowangkeji.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://gja.chenlongwang.top

[Q05] 重命名列
来源：http://pbc.uphjek.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://rnt.birdmap.top

[Q06] 删除列
来源：http://yks.xuanzx.com

ALTER TABLE users DROP COLUMN age;
来源：http://mfv.yanxiufei.cn

[Q07] 删除表
来源：http://zes.hcnkem.com

DROP TABLE IF EXISTS orders;
来源：http://nuz.svipenyu.cn

[Q08] 创建普通索引
来源：http://edo.tianlin.xyz

CREATE INDEX idx_users_email ON users(email);
来源：http://bkh.sysykeji.top

[Q09] 创建唯一索引
来源：http://stx.zhixingplan.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://vbx.snrcjt.cn

[Q10] 插入单行
来源：http://qnr.shuidangran.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://bwz.daxiang520.top

[Q11] 一次插入多行
来源：http://uqh.yongpay.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://twa.iojbl.cn

[Q12] 插入后取自增 ID
来源：http://tmw.iojbl.cn

INSERT INTO users (name) VALUES ('C');
来源：http://vvh.jianghu66.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://uqw.dashuyun.cn

[Q13] 忽略重复插入
来源：http://uxu.shangyingyoupin.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://usk.kuanghao11.cn

[Q14] 存在则更新（upsert）
来源：http://uad.hywenlv.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://xiy.yvedp.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://xhf.meibo888.top

[Q15] 查询全部
来源：http://lob.yueranfly.top

SELECT * FROM users;
来源：http://xuj.guowangkeji.top

[Q16] 查询指定列
来源：http://eoq.dashuyun.cn

SELECT id, name FROM users;
来源：http://yip.xingfuxueyuan.xyz

[Q17] 条件查询
来源：http://obf.zdqjudy.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ujs.fktsv.cn

[Q18] 模糊匹配
来源：http://dax.aibaodan.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ttj.fzhhl.top

[Q19] 范围查询
来源：http://exu.zhaomingkeji.xyz

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://aan.0kj1m.cn

[Q20] IN 列表
来源：http://oor.ctjpmb.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://zqk.ehwqpu.com

[Q21] 空值判断
来源：http://ymh.yj20258.top

SELECT * FROM users WHERE email IS NULL;
来源：http://ghx.svipenyu.cn

[Q22] 排序
来源：http://wgi.wangshuangyany.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://omz.shangyingyoupin.top

[Q23] 分页
来源：http://sgo.zhixingplan.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://xqm.meibo888.top

[Q24] 去重
来源：http://dml.jianghu66.top

SELECT DISTINCT city FROM users;
来源：http://pkv.epnwcf.com

[Q25] 只取前 N 条
来源：http://yiv.iojbl.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hfu.yuxming.cn

[Q26] 计数
来源：http://odi.mhx1999.top

SELECT COUNT(*) FROM users;
来源：http://izb.jqgfzy.top

[Q27] 条件计数
来源：http://jid.tanke756.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://pcm.birdmap.top

[Q28] 求和与平均
来源：http://xbp.jinqigfzy.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://koj.aibaodan.cn

[Q29] 最大最小值
来源：http://eod.chenjidiqi.icu

SELECT MAX(age), MIN(age) FROM users;
来源：http://fdr.smart0.xyz

[Q30] 分组统计
来源：http://fda.xuanzx.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://fdt.jinghuilouyu.cn

[Q31] 分组后过滤
来源：http://ihx.shzxlz.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://qpx.xingfuxueyuan.xyz

[Q32] 分组拼接字符串
来源：http://cdf.chenjidiqi.icu

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://zpz.cdnleiting.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ahg.cashguo.top

[Q33] 多列分组
来源：http://wpo.yuxming.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://qbj.jiagoushi.top

[Q34] 每组取第一条
来源：http://duc.aizwys.cn

SELECT * FROM (
来源：http://mln.yueranfly.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://fcz.sjlbkw.cn

) t WHERE rn = 1;
来源：http://tyt.yj202588.top

[Q35] 内连接
来源：http://sly.zhengqikj.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hyx.fehbvm.com

[Q36] 左连接
来源：http://dph.yj20258888.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://cys.c1oappe.top

[Q37] 右连接
来源：http://zva.svipenyu.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://xnf.zhoulong.xyz

[Q38] 全外连接（PostgreSQL）
来源：http://pol.yj20258.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://jug.andypj.xyz

[Q39] 自连接（查上下级）
来源：http://wlv.tian-w.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://kzi.52xcode.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wju.gaohongyu789.top

[Q40] 交叉连接（笛卡尔积）
来源：http://cnp.hongshengwenyu.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hkr.fengsongda.top

[Q41] 多表连接
来源：http://hmc.xinyue.icu

SELECT o.id, u.name, p.title FROM orders o
来源：http://fgt.chenjidiqi.icu

JOIN users u ON u.id = o.user_id
来源：http://gnb.jinqigfzy.top

JOIN products p ON p.id = o.product_id;
来源：http://bqg.mhx1999.top

[Q42] 连接条件附加过滤
来源：http://nsk.c1oappe.top

SELECT u.name, o.amount FROM users u
来源：http://loo.pycfn.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://rok.jiagoushi.top

[Q43] 标量子查询
来源：http://qww.yuxming.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hhd.tianlin.xyz

[Q44] IN 子查询
来源：http://qnd.xuetiantiany.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://tme.fanxiaobao.xyz

[Q45] EXISTS 判断存在
来源：http://bwl.guannengcc.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://msc.zhengqikj.top

[Q46] NOT EXISTS 判断不存在
来源：http://pst.hywenlv.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kgf.sysykeji.top

[Q47] 与平均值比较
来源：http://pju.dashuyun.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://fvt.52xcode.cn

[Q48] CTE 公用表表达式
来源：http://gvz.jinghuilouyu.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mgn.iojbl.cn

SELECT * FROM t WHERE c > 5;
来源：http://tgl.smart0.xyz

[Q49] 更新单行
来源：http://mfz.cheryme.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://jkj.gotoacloud.top

[Q50] 批量更新
来源：http://esl.yvedp.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://cws.vqdsnc.cn

[Q51] 用子查询更新
来源：http://kez.wangshuangyany.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mbh.yangfankeji.com

[Q52] 删除指定行
来源：http://dmv.yanxiufei.cn

DELETE FROM users WHERE id = 10;
来源：http://ews.fzhhl.top

[Q53] 按条件删除
来源：http://gdq.tian-w.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ulp.ppjwa.cn

[Q54] 清空表
来源：http://qyk.jinqigfzy.top

TRUNCATE TABLE logs;
来源：http://oiv.vehdjk.com

[Q55] 排名（并列占位）
来源：http://yvf.zhixingplan.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://kap.aizwys.cn

[Q56] 密集排名（并列不占位）
来源：http://mrw.nwbrower.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://zrb.tarul.cn

[Q57] 行号
来源：http://wrg.smart0.xyz

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://get.cqqwz.cn

[Q58] 累计求和
来源：http://djh.nanxuanxn.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://nbg.zycfv.cn

[Q59] 分组内累计
来源：http://jix.quarkkingdee.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://yam.meibo888.top

[Q60] 取上一行 / 下一行
来源：http://eyb.xinyue.icu

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ylg.xylfe.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hxa.birdmap.top

[Q61] 移动平均
来源：http://irg.ydjk.org.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://yll.pycfn.com

[Q62] 分组占比
来源：http://ejb.sufxvd.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://dgz.chenzaomai.com

[Q63] 开启事务
来源：http://emt.mhx1999.top

START TRANSACTION;                -- 或 BEGIN
来源：http://dqi.sufxvd.cn

[Q64] 提交事务
来源：http://nwo.yuanzhike.top

COMMIT;
来源：http://pam.kuanghao11.cn

[Q65] 回滚事务
来源：http://csz.ehwqpu.com

ROLLBACK;
来源：http://qfv.xuetiantiany.cn

[Q66] 行锁查询
来源：http://piy.shangyingyoupin.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://xno.aibaodan.cn

[Q67] 设置隔离级别
来源：http://uhk.ppjwa.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://yvf.hcnkem.com

[Q68] 保存点
来源：http://snq.cdnleiting.top

SAVEPOINT sp1;
来源：http://nmk.nanxinkj.top

ROLLBACK TO sp1;
来源：http://qwy.c1oappe.top

[Q69] 查看执行计划
来源：http://tis.jlsjyb.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://vam.nanxinkj.top

[Q70] 更新统计信息
来源：http://slm.svipenyu.cn

ANALYZE TABLE users;
来源：http://flj.jinqigfzy.top

[Q71] 查看建表语句
来源：http://gkj.epnwcf.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://gue.zhixingplan.top

[Q72] 查看索引
来源：http://idl.smart0.xyz

SHOW INDEX FROM users;
来源：http://dqb.jinqigfzy.top

[Q73] 查看表状态
来源：http://oei.xuanzx.com

SHOW TABLE STATUS LIKE 'users';
来源：http://pqj.birdmap.top

[Q74] 强制使用索引
来源：http://fej.shzxlz.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://bfl.sjlbkw.cn

[Q75] 日期格式化
来源：http://pmy.aibaodan.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://zby.yj202588.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://vpo.wangshuangyany.cn

[Q76] 按天统计
来源：http://duy.cheryme.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://oiu.yj20258.top

[Q77] 时间加减
来源：http://qhu.hesvh.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://lar.shuidangran.top

[Q78] 当前时间
来源：http://ppw.daxiang520.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hxi.nanxinkj.top

[Q79] 字符串拼接
来源：http://bto.shangyingyoupin.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://lka.xuanzx.com

[Q80] 字符串截取
来源：http://bsq.xylfe.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ovs.snrcjt.cn

[Q81] 字符串替换
来源：http://bsf.yonumen.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://lsn.sufxvd.cn

[Q82] 字符长度与字节长度
来源：http://qzy.tian-w.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ikp.feifeiyinyue.top

[Q83] 大小写转换
来源：http://vcg.shzxlz.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://pvj.0kj1m.cn

[Q84] 去除首尾空格
来源：http://cpi.xingfuxueyuan.xyz

SELECT TRIM(name) FROM users;
来源：http://qqu.jiagoushi.top

[Q85] 数值取整
来源：http://rhe.jqgufenzy.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://fnq.guowangkeji.top

[Q86] 读取 JSON 字段
来源：http://ctq.hnqzz.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://bro.svipenyu.cn

[Q87] JSON 字段做条件
来源：http://rkv.sweek.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ouc.zdbjq.cn

[Q88] 行转列（条件聚合）
来源：http://qxd.jqgfzy.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://oit.pycfn.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://xwl.jiagoushi.top

[Q89] 判断表是否存在
来源：http://kqv.hnqzz.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://zdv.9152youxi.cn

[Q90] 生成序号列
来源：http://buj.hcnkem.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://bol.kuanghao11.cn

================================================================================
来源：http://pnx.ehwqpu.com

R. Bash 专题
来源：http://mxy.wangdashe.top

================================================================================
来源：http://pme.chenlongwang.top

[R01] shebang 与严格模式
来源：http://tuk.svipenyu.cn

#!/usr/bin/env bash
来源：http://lzn.andypj.xyz

set -euo pipefail
来源：http://usl.shanyushiyangtech.top

[R02] 变量赋值与使用
来源：http://bgk.xziqi.cn

name="Tom"; echo "$name"
来源：http://imf.gotoacloud.top

[R03] 只读变量
来源：http://wyw.shanyushiyangkeji.top

readonly PI=3.14
来源：http://spf.zhiwuduotai.top

[R04] 位置参数
来源：http://jsl.xuetiantiany.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://khy.hfpthk.cn

[R05] 参数默认值
来源：http://txk.cheryme.top

name="${1:-default}"
来源：http://arr.guowangkeji.top

[R06] 判断命令是否存在
来源：http://prc.jyoumei.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://eun.yangfankeji.com

[R07] if 判断文件
来源：http://lwj.hesvh.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://qie.xuetiantiany.cn

[R08] 数值比较
来源：http://eai.feifeiyinyue.top

if (( a > b )); then echo "a 更大"; fi
来源：http://epb.yangfankeji.com

[R09] 字符串比较
来源：http://ksn.chenlongwang.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://dsz.zhongyouzk.top

[R10] 正则匹配
来源：http://vgb.daxiang520.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://odh.ehwqpu.com

[R11] case 多分支
来源：http://qpm.meibo888.top

case "$1" in
来源：http://jav.aibaodan.cn

start) echo "启动" ;;
来源：http://wrz.cashguo.top

stop)  echo "停止" ;;
来源：http://sbb.bbcook.cn

*)     echo "未知命令" ;;
来源：http://svn.sxryk.cn

esac
来源：http://nda.yuanzhike.top

[R12] for 遍历文件
来源：http://coe.tanke756.top

for f in *.txt; do echo "$f"; done
来源：http://fpm.iojbl.cn

[R13] for 计数循环
来源：http://sam.jlsjyb.cn

for i in {1..10}; do echo "$i"; done
来源：http://xmt.xinyue.icu

[R14] C 风格 for
来源：http://fhb.sweek.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://uot.ybcxt.top

[R15] while 逐行读文件
来源：http://iqc.xuanzx.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://cht.316326.xyz

[R16] until 等待条件
来源：http://fjv.gzhubu.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mgq.xingfuxueyuan.xyz

[R17] 数组定义与取值
来源：http://iuu.sysykeji.top

arr=(a b c); echo "${arr[0]}"
来源：http://rag.nanxinkj.top

[R18] 遍历数组
来源：http://gvo.shangyingyoupin.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://sfi.zhongyouzk.top

[R19] 数组长度
来源：http://guc.daxiang520.top

echo "${#arr[@]}"
来源：http://kid.yuanzhike.top

[R20] 关联数组（字典）
来源：http://vfi.tianlin.xyz

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://zjo.daxiang520.top

[R21] 字符串长度
来源：http://ytn.nanxuanxn.top

echo "${#s}"
来源：http://fgx.yanxiufei.cn

[R22] 截取子串
来源：http://dtp.bbcook.cn

echo "${s:0:5}"
来源：http://gmr.jinqigfzy.top

[R23] 字符串替换
来源：http://mpw.zhixingplan.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ocb.yuxming.cn

[R24] 大小写转换
来源：http://ffy.sweek.top

echo "${s^^}"; echo "${s,,}"
来源：http://szm.shuidangran.top

[R25] 去后缀 / 去前缀
来源：http://tmb.bbcook.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://wqk.hnqzz.top

[R26] 命令替换
来源：http://zsy.yanxiufei.cn

now=$(date +%F); echo "$now"
来源：http://ous.birdmap.top

[R27] 算术展开
来源：http://whr.daria6918.cn

echo $((1 + 2 * 3))
来源：http://tfv.jinqigfzy.top

[R28] 浮点运算
来源：http://naz.ywan-chungtsiang.top

echo "scale=2; 10/3" | bc
来源：http://lmx.yvedp.cn

[R29] 定义函数
来源：http://kyn.ppjwa.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://rsx.jqgfzy.top

[R30] 函数返回状态码
来源：http://xce.ppjwa.cn

f() { return 0; }; f || echo "失败了"
来源：http://uxs.52xcode.cn

[R31] 局部变量
来源：http://yhu.xuetiantiany.cn

f() { local x=1; echo "$x"; }
来源：http://ozn.hammf.cn

[R32] 参数个数校验
来源：http://wmk.yj20258888.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://dtr.sxryk.cn

[R33] 捕获错误并提示行号
来源：http://bye.wangshuangyany.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://vvk.xuetiantiany.cn

[R34] 退出时清理
来源：http://omx.chenlongwang.top

trap 'rm -f "$tmp"' EXIT
来源：http://ytj.feifeiyinyue.top

[R35] 后台执行并等待
来源：http://zai.hammf.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://lgt.andypj.xyz

[R36] 并发执行多个任务
来源：http://egz.aizwys.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ldu.cdnleiting.top

[R37] 把输出赋给变量
来源：http://een.birdmap.top

files=$(ls -1)
来源：http://dqi.xuetiantiany.cn

[R38] 管道串联
来源：http://yik.fehbvm.com

cat a.txt | grep -i error | wc -l
来源：http://xyv.mhx1999.top

[R39] 重定向标准输出与错误
来源：http://ghh.hcnkem.com

cmd > out.log 2>&1
来源：http://vhz.zhixingplan.top

[R40] 追加写日志
来源：http://ozz.ydzc1.top

echo "log" >> out.log
来源：http://ajc.hongshengwenyu.top

[R41] 丢弃输出
来源：http://irl.cdnleiting.top

cmd >/dev/null 2>&1
来源：http://ico.chenzaomai.com

[R42] 输入重定向
来源：http://wvs.fzhhl.top

wc -l < a.txt
来源：http://qjb.guowangkeji.top

[R43] 按名字查找文件
来源：http://ycj.cashguo.top

find . -name "*.log" -type f
来源：http://muw.ctjpmb.com

[R44] 按修改时间查找
来源：http://ljc.vehdjk.com

find . -mtime -7 -type f
来源：http://dqu.fanxiaobao.xyz

[R45] 批量删除
来源：http://ojj.uphjek.com

find . -name "*.tmp" -delete
来源：http://jem.shanyushiyangtech.top

[R46] 递归替换文件内容
来源：http://dga.yonumen.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://stu.52xcode.cn

[R47] sed 单行替换
来源：http://rjf.cqqwz.cn


<!-- 参考信息 -->