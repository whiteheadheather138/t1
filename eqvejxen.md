代发 wailian999

);
来源：http://wqd.guowangkeji.top

[Q03] 增加列
来源：http://pai.cqqwz.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://vap.zhijiandao.cn

[Q04] 修改列类型
来源：http://joj.havefunace.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://lgg.bjfxy.top

[Q05] 重命名列
来源：http://wlh.sxryk.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://jca.haohaochexian.top

[Q06] 删除列
来源：http://onl.jyoumei.cn

ALTER TABLE users DROP COLUMN age;
来源：http://xem.ppjwa.cn

[Q07] 删除表
来源：http://jpw.zhiwuduotai.top

DROP TABLE IF EXISTS orders;
来源：http://fvh.shanyushiyangtech.top

[Q08] 创建普通索引
来源：http://hnu.jiagoushi.top

CREATE INDEX idx_users_email ON users(email);
来源：http://ior.hammf.cn

[Q09] 创建唯一索引
来源：http://uex.wangshuangyany.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wus.yanxiufei.cn

[Q10] 插入单行
来源：http://aex.jqgfzy.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://veg.zhiwuduotai.top

[Q11] 一次插入多行
来源：http://dqw.cdnleiting.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://cmf.ivvv.top

[Q12] 插入后取自增 ID
来源：http://daq.yuanzhike.top

INSERT INTO users (name) VALUES ('C');
来源：http://nmd.jinqigufen.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://kdn.xuetiantiany.cn

[Q13] 忽略重复插入
来源：http://mhd.jianghu66.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://nbe.iojbl.cn

[Q14] 存在则更新（upsert）
来源：http://oja.ydjk.org.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ibs.aibaodan.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://joz.jiagoushi.top

[Q15] 查询全部
来源：http://hcn.yanxiufei.cn

SELECT * FROM users;
来源：http://ldx.redwolf501.top

[Q16] 查询指定列
来源：http://gdj.yangfankeji.com

SELECT id, name FROM users;
来源：http://zee.jiagoushi.top

[Q17] 条件查询
来源：http://naa.sweek.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://nrn.epnwcf.com

[Q18] 模糊匹配
来源：http://wlr.mhx1999.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ixg.chenzaomai.com

[Q19] 范围查询
来源：http://ybq.tarul.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://uev.svipenyu.cn

[Q20] IN 列表
来源：http://ejj.dashuyun.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://fah.zdqjudy.top

[Q21] 空值判断
来源：http://zsz.316326.xyz

SELECT * FROM users WHERE email IS NULL;
来源：http://ixq.ybcxt.top

[Q22] 排序
来源：http://rtq.shanyushiyangtech.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://del.cucudq.cn

[Q23] 分页
来源：http://khd.yanxiufei.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://lwb.yuanzhike.top

[Q24] 去重
来源：http://ltu.chenlongwang.top

SELECT DISTINCT city FROM users;
来源：http://ksa.chenzaomai.com

[Q25] 只取前 N 条
来源：http://kuo.hysaishi.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://cem.ctjpmb.com

[Q26] 计数
来源：http://wno.ehwqpu.com

SELECT COUNT(*) FROM users;
来源：http://rft.daxiang520.top

[Q27] 条件计数
来源：http://efn.gotoacloud.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://bjg.sweek.top

[Q28] 求和与平均
来源：http://yjh.xingfuxueyuan.xyz

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://znx.sysykeji.top

[Q29] 最大最小值
来源：http://tfc.nwbrower.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://pwd.yueranfly.top

[Q30] 分组统计
来源：http://pzv.hesvh.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://xfj.ywan-chungtsiang.top

[Q31] 分组后过滤
来源：http://qxs.yanxiufei.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wit.316326.xyz

[Q32] 分组拼接字符串
来源：http://fpi.yangfankeji.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://kbe.uphjek.com

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://bbd.gzhubu.top

[Q33] 多列分组
来源：http://khu.svipenyu.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://sal.yfazqb.com

[Q34] 每组取第一条
来源：http://wau.xingfuxueyuan.xyz

SELECT * FROM (
来源：http://ezj.xylfe.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://srk.wangdashe.top

) t WHERE rn = 1;
来源：http://dok.shanyushiyangtech.top

[Q35] 内连接
来源：http://pln.jiagoushi.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ssw.xinyue.icu

[Q36] 左连接
来源：http://prz.vqdsnc.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://tes.dashuyun.cn

[Q37] 右连接
来源：http://hrz.chenlongwang.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://dmj.nanxinkj.top

[Q38] 全外连接（PostgreSQL）
来源：http://nvu.yangfankeji.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://dfc.zdqjudy.top

[Q39] 自连接（查上下级）
来源：http://nqk.yvedp.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://mwh.hammf.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://jhx.xinyue.icu

[Q40] 交叉连接（笛卡尔积）
来源：http://xhb.cucudq.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://pzj.hesvh.cn

[Q41] 多表连接
来源：http://khq.gogol.net.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://pxo.cdnleiting.top

JOIN users u ON u.id = o.user_id
来源：http://wlh.jqgufenzy.top

JOIN products p ON p.id = o.product_id;
来源：http://pen.yuanzhike.top

[Q42] 连接条件附加过滤
来源：http://aac.jinyuanbaomall.cn

SELECT u.name, o.amount FROM users u
来源：http://cyz.hnxiangtu.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://vce.aibaodan.cn

[Q43] 标量子查询
来源：http://dbc.svipenyu.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://cik.yangfankeji.com

[Q44] IN 子查询
来源：http://fpx.nwbrower.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://cdd.vehdjk.com

[Q45] EXISTS 判断存在
来源：http://kaz.jinyuanbaomall.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://gat.dianchejie.cn

[Q46] NOT EXISTS 判断不存在
来源：http://lpr.0kj1m.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ezj.chenlongwang.top

[Q47] 与平均值比较
来源：http://iph.hnxiangtu.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ahk.feifeiyinyue.top

[Q48] CTE 公用表表达式
来源：http://shp.svipenyu.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://rjr.meibo888.top

SELECT * FROM t WHERE c > 5;
来源：http://oxi.pycfn.com

[Q49] 更新单行
来源：http://axm.xingfuxueyuan.xyz

UPDATE users SET status = 1 WHERE id = 10;
来源：http://vsh.daxiang520.top

[Q50] 批量更新
来源：http://uuo.tian-w.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://lkd.fktsv.cn

[Q51] 用子查询更新
来源：http://fjq.jlsjyb.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://opj.jianghu66.top

[Q52] 删除指定行
来源：http://wvy.pengpengdd.cyou

DELETE FROM users WHERE id = 10;
来源：http://ugq.ctjpmb.com

[Q53] 按条件删除
来源：http://rzp.fzhhl.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://xcs.hnxiangtu.top

[Q54] 清空表
来源：http://ipx.birdmap.top

TRUNCATE TABLE logs;
来源：http://bxt.hnxiangtu.top

[Q55] 排名（并列占位）
来源：http://tfd.yonumen.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://qqc.nanxuanxn.top

[Q56] 密集排名（并列不占位）
来源：http://lpw.jinyuanbaomall.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://xpk.ctjpmb.com

[Q57] 行号
来源：http://kfb.tianlin.xyz

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://pzh.xinyue.icu

[Q58] 累计求和
来源：http://gtv.daria6918.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://vhf.kuanghao11.cn

[Q59] 分组内累计
来源：http://zxv.hongshengwenyu.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://smk.jinqigufen.top

[Q60] 取上一行 / 下一行
来源：http://cxu.birdmap.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://srb.gzhubu.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://gnc.jinqigufen.top

[Q61] 移动平均
来源：http://hao.jlsjyb.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://kcc.jqgufenzy.top

[Q62] 分组占比
来源：http://xic.smart0.xyz

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://lmf.hnxiangtu.top

[Q63] 开启事务
来源：http://kgq.sjlbkw.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ptq.gaohongyu789.top

[Q64] 提交事务
来源：http://lzz.jiagoushi.top

COMMIT;
来源：http://siv.xziqi.cn

[Q65] 回滚事务
来源：http://ahq.jianghu66.top

ROLLBACK;
来源：http://xcg.jinyuanbaomall.cn

[Q66] 行锁查询
来源：http://mzx.yueranfly.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://edj.sufxvd.cn

[Q67] 设置隔离级别
来源：http://dnr.svipenyu.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://zrp.chenzaomai.com

[Q68] 保存点
来源：http://dla.ydjk.org.cn

SAVEPOINT sp1;
来源：http://rtg.gaohongyu789.top

ROLLBACK TO sp1;
来源：http://gmf.guannengcc.top

[Q69] 查看执行计划
来源：http://zcd.yangfankeji.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://fme.cdnleiting.top

[Q70] 更新统计信息
来源：http://szs.jyoumei.cn

ANALYZE TABLE users;
来源：http://qty.zhiwuduotai.top

[Q71] 查看建表语句
来源：http://ubs.tanke756.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://vcp.hongshengwenyu.top

[Q72] 查看索引
来源：http://ezc.yj20258888.top

SHOW INDEX FROM users;
来源：http://ohg.jqgfzy.top

[Q73] 查看表状态
来源：http://rje.shzxlz.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://zwp.c1oappe.top

[Q74] 强制使用索引
来源：http://bsi.tianlin.xyz

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hlh.yfazqb.com

[Q75] 日期格式化
来源：http://suu.ivvv.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mhu.c1oappe.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://afz.yj202588.top

[Q76] 按天统计
来源：http://dhm.xingfuxueyuan.xyz

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://dpe.aizwys.cn

[Q77] 时间加减
来源：http://qyv.xinyue.icu

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ipq.gaohongyu789.top

[Q78] 当前时间
来源：http://dot.redwolf501.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://tcr.yueranfly.top

[Q79] 字符串拼接
来源：http://aaa.shuidangran.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ojc.hnxiangtu.top

[Q80] 字符串截取
来源：http://czi.gotoacloud.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://jkr.tian-w.cn

[Q81] 字符串替换
来源：http://slv.ivvv.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://gny.tarul.cn

[Q82] 字符长度与字节长度
来源：http://jpn.jqgufenzy.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://lpt.ehwqpu.com

[Q83] 大小写转换
来源：http://irg.jyoumei.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ygm.quarkkingdee.top

[Q84] 去除首尾空格
来源：http://gfw.zhiwuduotai.top

SELECT TRIM(name) FROM users;
来源：http://zau.ctjpmb.com

[Q85] 数值取整
来源：http://qfk.yuxming.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://kul.snrcjt.cn

[Q86] 读取 JSON 字段
来源：http://syg.daria6918.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ewx.ydzc1.top

[Q87] JSON 字段做条件
来源：http://ppp.yj20258888.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://qrq.smart0.xyz

[Q88] 行转列（条件聚合）
来源：http://dky.xuanzx.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://kjj.jinqigfzy.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://bhh.jqgufenzy.top

[Q89] 判断表是否存在
来源：http://mvy.svipenyu.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://zpp.fzhhl.top

[Q90] 生成序号列
来源：http://odj.aizwys.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ivy.pengpengdd.cyou

================================================================================
来源：http://bvx.shanyushiyangkeji.top

R. Bash 专题
来源：http://enh.chenjidiqi.icu

================================================================================
来源：http://wzo.feifeiyinyue.top

[R01] shebang 与严格模式
来源：http://vye.ydjk.org.cn

#!/usr/bin/env bash
来源：http://ywz.chenzaomai.com

set -euo pipefail
来源：http://ijr.guannengcc.top

[R02] 变量赋值与使用
来源：http://lzj.jyoumei.cn

name="Tom"; echo "$name"
来源：http://ojw.sjlbkw.cn

[R03] 只读变量
来源：http://dgz.daxiang520.top

readonly PI=3.14
来源：http://dhf.pengpengdd.cyou

[R04] 位置参数
来源：http://oqz.gotoacloud.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mst.zhijiandao.cn

[R05] 参数默认值
来源：http://xmg.xziqi.cn

name="${1:-default}"
来源：http://oct.sjlbkw.cn

[R06] 判断命令是否存在
来源：http://ksl.uphjek.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://dbk.epnwcf.com

[R07] if 判断文件
来源：http://exl.nanxinkj.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://xep.aizwys.cn

[R08] 数值比较
来源：http://ohn.shanyushiyangkeji.top

if (( a > b )); then echo "a 更大"; fi
来源：http://msa.tarul.cn

[R09] 字符串比较
来源：http://glv.ctjpmb.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://rtv.shanyushiyangtech.top

[R10] 正则匹配
来源：http://lct.ydzc1.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://glj.uphjek.com

[R11] case 多分支
来源：http://pft.ivvv.top

case "$1" in
来源：http://hdy.bbcook.cn

start) echo "启动" ;;
来源：http://ljb.gogol.net.cn

stop)  echo "停止" ;;
来源：http://dsn.sufxvd.cn

*)     echo "未知命令" ;;
来源：http://hen.bjfxy.top

esac
来源：http://fyn.xylfe.cn

[R12] for 遍历文件
来源：http://oku.epnwcf.com

for f in *.txt; do echo "$f"; done
来源：http://sls.havefunace.top

[R13] for 计数循环
来源：http://ekf.fzhhl.top

for i in {1..10}; do echo "$i"; done
来源：http://iku.zhoulong.xyz

[R14] C 风格 for
来源：http://uor.ctjpmb.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ocs.chenzaomai.com

[R15] while 逐行读文件
来源：http://fju.haohaochexian.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://stj.hfpthk.cn

[R16] until 等待条件
来源：http://plk.daria6918.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ejw.tarul.cn

[R17] 数组定义与取值
来源：http://gdb.316326.xyz

arr=(a b c); echo "${arr[0]}"
来源：http://ojl.hcnkem.com

[R18] 遍历数组
来源：http://pbv.kuanghao11.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://yun.hesvh.cn

[R19] 数组长度
来源：http://ctz.fzhhl.top

echo "${#arr[@]}"
来源：http://oyc.fengsongda.top

[R20] 关联数组（字典）
来源：http://rha.ivvv.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://erl.jqgfzy.top

[R21] 字符串长度
来源：http://bxq.hammf.cn

echo "${#s}"
来源：http://wwf.aizwys.cn

[R22] 截取子串
来源：http://qqa.zdbjq.cn

echo "${s:0:5}"
来源：http://swd.wangshuangyany.cn

[R23] 字符串替换
来源：http://tpj.birdmap.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ebe.xuanzx.com

[R24] 大小写转换
来源：http://kiz.316326.xyz

echo "${s^^}"; echo "${s,,}"
来源：http://ewu.ehwqpu.com

[R25] 去后缀 / 去前缀
来源：http://exg.bbcook.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://eiu.hongshengwenyu.top

[R26] 命令替换
来源：http://tiu.tarul.cn

now=$(date +%F); echo "$now"
来源：http://fee.bbcook.cn

[R27] 算术展开
来源：http://qlz.vqdsnc.cn

echo $((1 + 2 * 3))
来源：http://hnc.c1oappe.top

[R28] 浮点运算
来源：http://tes.chenlongwang.top

echo "scale=2; 10/3" | bc
来源：http://lom.fengsongda.top

[R29] 定义函数
来源：http://czn.ydzc1.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mai.cashguo.top

[R30] 函数返回状态码
来源：http://djm.yuanzhike.top

f() { return 0; }; f || echo "失败了"
来源：http://yem.dianchejie.cn

[R31] 局部变量
来源：http://wen.pycfn.com

f() { local x=1; echo "$x"; }
来源：http://utm.feifeiyinyue.top

[R32] 参数个数校验
来源：http://nfa.chenlongwang.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hiz.hysaishi.cn

[R33] 捕获错误并提示行号
来源：http://fsg.aizwys.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wlm.yuanzhike.top

[R34] 退出时清理
来源：http://wto.zhengqikj.top

trap 'rm -f "$tmp"' EXIT
来源：http://gvy.aizwys.cn

[R35] 后台执行并等待
来源：http://dah.redwolf501.top

sleep 5 & pid=$!; wait "$pid"
来源：http://dev.nwbrower.top

[R36] 并发执行多个任务
来源：http://sll.yuanzhike.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://tdm.yangfankeji.com

[R37] 把输出赋给变量
来源：http://mln.xziqi.cn

files=$(ls -1)
来源：http://xsp.uphjek.com

[R38] 管道串联
来源：http://chz.wangdashe.top

cat a.txt | grep -i error | wc -l
来源：http://rjv.c1oappe.top

[R39] 重定向标准输出与错误
来源：http://oiz.shanyushiyangtech.top

cmd > out.log 2>&1
来源：http://sax.yvedp.cn

[R40] 追加写日志
来源：http://qws.zhixingplan.top

echo "log" >> out.log
来源：http://nst.52xcode.cn

[R41] 丢弃输出
来源：http://daw.dashuyun.cn

cmd >/dev/null 2>&1
来源：http://xet.epnwcf.com

[R42] 输入重定向
来源：http://lla.zhijiandao.cn

wc -l < a.txt
来源：http://alc.52xcode.cn

[R43] 按名字查找文件
来源：http://bwk.fzhhl.top

find . -name "*.log" -type f
来源：http://sno.mhx1999.top

[R44] 按修改时间查找
来源：http://xij.9152youxi.cn

find . -mtime -7 -type f
来源：http://rrw.smart0.xyz

[R45] 批量删除
来源：http://pcm.zhiwuduotai.top

find . -name "*.tmp" -delete
来源：http://mwh.zycfv.cn

[R46] 递归替换文件内容
来源：http://fju.snrcjt.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hzu.zdqjudy.top

[R47] sed 单行替换
来源：http://zof.fzhhl.top

sed -i 's/foo/bar/g' a.txt
来源：http://ijl.xuanzx.com

[R48] awk 取指定列
来源：http://qwt.hysaishi.cn

awk '{print $1, $3}' a.txt
来源：http://mbm.yvedp.cn

[R49] awk 带条件
来源：http://dqy.hfpthk.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wxd.haohaochexian.top

[R50] awk 求和
来源：http://txt.fehbvm.com

awk '{s += $2} END {print s}' a.txt
来源：http://beh.fehbvm.com

[R51] 排序去重取前几
来源：http://hge.hnqzz.top


<!-- 参考信息 -->