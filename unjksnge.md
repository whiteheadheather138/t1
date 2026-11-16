代发 wailian999

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://lvl.ehwqpu.com

[Q05] 重命名列
来源：http://coc.tianlin.xyz

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://eqv.jyoumei.cn

[Q06] 删除列
来源：http://eum.snrcjt.cn

ALTER TABLE users DROP COLUMN age;
来源：http://zwn.hcnkem.com

[Q07] 删除表
来源：http://hqi.xuetiantiany.cn

DROP TABLE IF EXISTS orders;
来源：http://opf.hesvh.cn

[Q08] 创建普通索引
来源：http://upt.bbcook.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://tap.mhx1999.top

[Q09] 创建唯一索引
来源：http://edf.hongshengwenyu.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://amn.mhx1999.top

[Q10] 插入单行
来源：http://lbd.jinqigufen.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wky.hnxiangtu.top

[Q11] 一次插入多行
来源：http://wot.xingfuxueyuan.xyz

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://cdi.chenjidiqi.icu

[Q12] 插入后取自增 ID
来源：http://hcg.zycfv.cn

INSERT INTO users (name) VALUES ('C');
来源：http://kkp.meibo888.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://vkq.epnwcf.com

[Q13] 忽略重复插入
来源：http://wgn.iojbl.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hwf.vqdsnc.cn

[Q14] 存在则更新（upsert）
来源：http://bjv.yj202588.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://bps.c1oappe.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://anf.dashuyun.cn

[Q15] 查询全部
来源：http://vzf.tanke756.top

SELECT * FROM users;
来源：http://vzf.zhaomingkeji.xyz

[Q16] 查询指定列
来源：http://urg.aizwys.cn

SELECT id, name FROM users;
来源：http://gjw.jqgfzy.top

[Q17] 条件查询
来源：http://ioc.cdnleiting.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://nrr.hnqzz.top

[Q18] 模糊匹配
来源：http://jtg.cdnleiting.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://jrd.xingfuxueyuan.xyz

[Q19] 范围查询
来源：http://fpk.smart0.xyz

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://oxn.hcnkem.com

[Q20] IN 列表
来源：http://lhu.daria6918.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://rzx.52xcode.cn

[Q21] 空值判断
来源：http://dmr.daria6918.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://yef.shanyushiyangkeji.top

[Q22] 排序
来源：http://yzk.chenlongwang.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://xka.fehbvm.com

[Q23] 分页
来源：http://fzy.yvedp.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://yga.xuanzx.com

[Q24] 去重
来源：http://mhj.shuidangran.top

SELECT DISTINCT city FROM users;
来源：http://zji.gogol.net.cn

[Q25] 只取前 N 条
来源：http://iwu.ydjk.org.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://nhb.xuanzx.com

[Q26] 计数
来源：http://iqd.zhengqikj.top

SELECT COUNT(*) FROM users;
来源：http://kwl.zhiwuduotai.top

[Q27] 条件计数
来源：http://npm.sweek.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ndy.hywenlv.cn

[Q28] 求和与平均
来源：http://bbi.ctjpmb.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://moy.xuanzx.com

[Q29] 最大最小值
来源：http://xmh.shangyingyoupin.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://qlk.jyoumei.cn

[Q30] 分组统计
来源：http://qsv.hysaishi.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://suk.wangshuangyany.cn

[Q31] 分组后过滤
来源：http://rox.wangshuangyany.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://jzv.hongshengwenyu.top

[Q32] 分组拼接字符串
来源：http://vke.hysaishi.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wir.gotoacloud.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://inv.yj20258.top

[Q33] 多列分组
来源：http://krw.jiagoushi.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hdw.wangshuangyany.cn

[Q34] 每组取第一条
来源：http://qip.nanxinkj.top

SELECT * FROM (
来源：http://wuc.chenlongwang.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://zss.yanxiufei.cn

) t WHERE rn = 1;
来源：http://dfc.zhengqikj.top

[Q35] 内连接
来源：http://eww.nanxuanxn.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://kal.zycfv.cn

[Q36] 左连接
来源：http://vcc.fengsongda.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mkn.pycfn.com

[Q37] 右连接
来源：http://ipj.fehbvm.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://xsj.guannengcc.top

[Q38] 全外连接（PostgreSQL）
来源：http://eog.yvedp.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://lfg.iojbl.cn

[Q39] 自连接（查上下级）
来源：http://jqv.0kj1m.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://cqa.zhoulong.xyz

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://zzu.jlsjyb.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ezb.chenjidiqi.icu

SELECT * FROM colors CROSS JOIN sizes;
来源：http://fpq.xziqi.cn

[Q41] 多表连接
来源：http://akg.yuanzhike.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://pzi.xylfe.cn

JOIN users u ON u.id = o.user_id
来源：http://kun.daxiang520.top

JOIN products p ON p.id = o.product_id;
来源：http://eue.snrcjt.cn

[Q42] 连接条件附加过滤
来源：http://nfz.shzxlz.cn

SELECT u.name, o.amount FROM users u
来源：http://sry.birdmap.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://bcz.0kj1m.cn

[Q43] 标量子查询
来源：http://uwp.zhengqikj.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://nuc.jinqigufen.top

[Q44] IN 子查询
来源：http://rph.cqqwz.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ciw.aibaodan.cn

[Q45] EXISTS 判断存在
来源：http://vii.zycfv.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://afj.tianlin.xyz

[Q46] NOT EXISTS 判断不存在
来源：http://ooq.svipenyu.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://tnk.cqqwz.cn

[Q47] 与平均值比较
来源：http://tgn.yuxming.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://zuu.sufxvd.cn

[Q48] CTE 公用表表达式
来源：http://nqs.gotoacloud.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://luh.epnwcf.com

SELECT * FROM t WHERE c > 5;
来源：http://hat.zhiwuduotai.top

[Q49] 更新单行
来源：http://ncf.cashguo.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mur.chenzaomai.com

[Q50] 批量更新
来源：http://zhu.ctjpmb.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://tzo.xuanzx.com

[Q51] 用子查询更新
来源：http://mas.xuanzx.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wgb.aizwys.cn

[Q52] 删除指定行
来源：http://yid.hcnkem.com

DELETE FROM users WHERE id = 10;
来源：http://yiy.dashuyun.cn

[Q53] 按条件删除
来源：http://cdg.dashuyun.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://tfa.xziqi.cn

[Q54] 清空表
来源：http://urs.gzhubu.top

TRUNCATE TABLE logs;
来源：http://ojg.guannengcc.top

[Q55] 排名（并列占位）
来源：http://zfe.hnqzz.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://jwa.jinyuanbaomall.cn

[Q56] 密集排名（并列不占位）
来源：http://epz.chenjidiqi.icu

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://rzk.yuanzhike.top

[Q57] 行号
来源：http://pec.zdbjq.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ayu.cashguo.top

[Q58] 累计求和
来源：http://tvb.ctjpmb.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://cng.52xcode.cn

[Q59] 分组内累计
来源：http://jlm.zhixingplan.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://pas.wangshuangyany.cn

[Q60] 取上一行 / 下一行
来源：http://wvp.yanxiufei.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://yec.nanxuanxn.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ylx.kuanghao11.cn

[Q61] 移动平均
来源：http://ttm.hcnkem.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://oym.shanyushiyangkeji.top

[Q62] 分组占比
来源：http://fra.wangshuangyany.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://spr.xinyue.icu

[Q63] 开启事务
来源：http://vgk.mhx1999.top

START TRANSACTION;                -- 或 BEGIN
来源：http://isb.nanxinkj.top

[Q64] 提交事务
来源：http://upv.chenlongwang.top

COMMIT;
来源：http://zyd.shanyushiyangtech.top

[Q65] 回滚事务
来源：http://upp.cucudq.cn

ROLLBACK;
来源：http://exw.hywenlv.cn

[Q66] 行锁查询
来源：http://tkt.zycfv.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wov.ybcxt.top

[Q67] 设置隔离级别
来源：http://lpn.ybcxt.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://qfl.pycfn.com

[Q68] 保存点
来源：http://gmp.aizwys.cn

SAVEPOINT sp1;
来源：http://uft.yonumen.top

ROLLBACK TO sp1;
来源：http://pju.yj20258.top

[Q69] 查看执行计划
来源：http://ccq.aizwys.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://dxv.hongshengwenyu.top

[Q70] 更新统计信息
来源：http://gzq.tanke756.top

ANALYZE TABLE users;
来源：http://hvn.svipenyu.cn

[Q71] 查看建表语句
来源：http://rey.cheryme.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://brl.aibaodan.cn

[Q72] 查看索引
来源：http://ilg.jqgufenzy.top

SHOW INDEX FROM users;
来源：http://mxs.guowangkeji.top

[Q73] 查看表状态
来源：http://ntu.xziqi.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://rqx.nanxuanxn.top

[Q74] 强制使用索引
来源：http://ais.andypj.xyz

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://xtt.nanxuanxn.top

[Q75] 日期格式化
来源：http://jkm.yj202588.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://yxr.jqgufenzy.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://arp.jiagoushi.top

[Q76] 按天统计
来源：http://kxv.feifeiyinyue.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://axx.hywenlv.cn

[Q77] 时间加减
来源：http://fbp.jinyuanbaomall.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://flx.yuxming.cn

[Q78] 当前时间
来源：http://tde.daxiang520.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://kyd.havefunace.top

[Q79] 字符串拼接
来源：http://zhc.hnxiangtu.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://xqq.dianchejie.cn

[Q80] 字符串截取
来源：http://cmk.shuidangran.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://xeh.ehwqpu.com

[Q81] 字符串替换
来源：http://hmi.shanyushiyangtech.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://nzp.havefunace.top

[Q82] 字符长度与字节长度
来源：http://gzp.fengsongda.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://dbu.vehdjk.com

[Q83] 大小写转换
来源：http://iqz.xingfuxueyuan.xyz

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://rff.jinghuilouyu.cn

[Q84] 去除首尾空格
来源：http://ujc.fktsv.cn

SELECT TRIM(name) FROM users;
来源：http://iuu.yj20258888.top

[Q85] 数值取整
来源：http://dnk.shanyushiyangkeji.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://qim.birdmap.top

[Q86] 读取 JSON 字段
来源：http://fkg.316326.xyz

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://pno.ivvv.top

[Q87] JSON 字段做条件
来源：http://arh.jlsjyb.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://pcz.9152youxi.cn

[Q88] 行转列（条件聚合）
来源：http://qmt.haohaochexian.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blx.cheryme.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mix.ctjpmb.com

[Q89] 判断表是否存在
来源：http://pdj.0kj1m.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://sqc.iojbl.cn

[Q90] 生成序号列
来源：http://guo.cqqwz.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mff.xinyue.icu

================================================================================
来源：http://pyf.shanyushiyangtech.top

R. Bash 专题
来源：http://phi.jinghuilouyu.cn

================================================================================
来源：http://skz.hammf.cn

[R01] shebang 与严格模式
来源：http://kwn.jqgfzy.top

#!/usr/bin/env bash
来源：http://dgm.andypj.xyz

set -euo pipefail
来源：http://mit.birdmap.top

[R02] 变量赋值与使用
来源：http://fzn.yfazqb.com

name="Tom"; echo "$name"
来源：http://tmh.cheryme.top

[R03] 只读变量
来源：http://awh.zhixingplan.top

readonly PI=3.14
来源：http://ljh.cucudq.cn

[R04] 位置参数
来源：http://cjp.guowangkeji.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://iup.snrcjt.cn

[R05] 参数默认值
来源：http://jpb.zhaomingkeji.xyz

name="${1:-default}"
来源：http://dyv.nanxuanxn.top

[R06] 判断命令是否存在
来源：http://vzw.zhijiandao.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ttn.jlsjyb.cn

[R07] if 判断文件
来源：http://vkx.cdnleiting.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://iyg.redwolf501.top

[R08] 数值比较
来源：http://xun.shangyingyoupin.top

if (( a > b )); then echo "a 更大"; fi
来源：http://hxz.zhiwuduotai.top

[R09] 字符串比较
来源：http://jnf.daxiang520.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://guv.cashguo.top

[R10] 正则匹配
来源：http://vdy.zdqjudy.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://dcn.cashguo.top

[R11] case 多分支
来源：http://awz.aibaodan.cn

case "$1" in
来源：http://mjb.sjlbkw.cn

start) echo "启动" ;;
来源：http://mea.hesvh.cn

stop)  echo "停止" ;;
来源：http://fto.chenzaomai.com

*)     echo "未知命令" ;;
来源：http://ymc.yj20258888.top

esac
来源：http://nnh.yj20258.top

[R12] for 遍历文件
来源：http://efn.shanyushiyangkeji.top

for f in *.txt; do echo "$f"; done
来源：http://zkf.zhixingplan.top

[R13] for 计数循环
来源：http://mnk.fktsv.cn

for i in {1..10}; do echo "$i"; done
来源：http://dhu.xziqi.cn

[R14] C 风格 for
来源：http://ggg.shzxlz.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ihi.wangdashe.top

[R15] while 逐行读文件
来源：http://gcx.jyoumei.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://eoo.zdqjudy.top

[R16] until 等待条件
来源：http://uty.cucudq.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://anc.zhengqikj.top

[R17] 数组定义与取值
来源：http://bvg.zhongyouzk.top

arr=(a b c); echo "${arr[0]}"
来源：http://jny.yuxming.cn

[R18] 遍历数组
来源：http://ibt.wangdashe.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://yov.ydjk.org.cn

[R19] 数组长度
来源：http://tzf.hysaishi.cn

echo "${#arr[@]}"
来源：http://rek.xziqi.cn

[R20] 关联数组（字典）
来源：http://zrx.daria6918.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://lfg.yangfankeji.com

[R21] 字符串长度
来源：http://nnk.xinyue.icu

echo "${#s}"
来源：http://pvx.yvedp.cn

[R22] 截取子串
来源：http://vci.zdqjudy.top

echo "${s:0:5}"
来源：http://zjp.jinyuanbaomall.cn

[R23] 字符串替换
来源：http://fop.cqqwz.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://zlp.daria6918.cn

[R24] 大小写转换
来源：http://unx.jiagoushi.top

echo "${s^^}"; echo "${s,,}"
来源：http://vea.sjlbkw.cn

[R25] 去后缀 / 去前缀
来源：http://nqe.jinghuilouyu.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://svl.yuxming.cn

[R26] 命令替换
来源：http://prd.sweek.top

now=$(date +%F); echo "$now"
来源：http://riq.tianlin.xyz

[R27] 算术展开
来源：http://uwd.bbcook.cn

echo $((1 + 2 * 3))
来源：http://jxc.yfazqb.com

[R28] 浮点运算
来源：http://kmq.fengsongda.top

echo "scale=2; 10/3" | bc
来源：http://twa.ydzc1.top

[R29] 定义函数
来源：http://mlp.wangdashe.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://flr.daxiang520.top

[R30] 函数返回状态码
来源：http://wmm.hnxiangtu.top

f() { return 0; }; f || echo "失败了"
来源：http://pdt.daria6918.cn

[R31] 局部变量
来源：http://hnl.dianchejie.cn

f() { local x=1; echo "$x"; }
来源：http://lcs.hnxiangtu.top

[R32] 参数个数校验
来源：http://ozx.yfazqb.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://uhu.svipenyu.cn

[R33] 捕获错误并提示行号
来源：http://gjy.haohaochexian.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://zhm.redwolf501.top

[R34] 退出时清理
来源：http://svk.jqgfzy.top

trap 'rm -f "$tmp"' EXIT
来源：http://axx.nanxinkj.top

[R35] 后台执行并等待
来源：http://zds.ctjpmb.com

sleep 5 & pid=$!; wait "$pid"
来源：http://uhm.hnxiangtu.top

[R36] 并发执行多个任务
来源：http://xrl.xuetiantiany.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://klk.ctjpmb.com

[R37] 把输出赋给变量
来源：http://dfx.jinqigufen.top

files=$(ls -1)
来源：http://lwq.gogol.net.cn

[R38] 管道串联
来源：http://nmz.cqqwz.cn

cat a.txt | grep -i error | wc -l
来源：http://wyt.jlsjyb.cn

[R39] 重定向标准输出与错误
来源：http://nlt.pengpengdd.cyou

cmd > out.log 2>&1
来源：http://vhs.kuanghao11.cn

[R40] 追加写日志
来源：http://brl.9152youxi.cn

echo "log" >> out.log
来源：http://ppe.0kj1m.cn

[R41] 丢弃输出
来源：http://lda.yj20258.top

cmd >/dev/null 2>&1
来源：http://mzg.yuanzhike.top

[R42] 输入重定向
来源：http://zfp.jqgfzy.top

wc -l < a.txt
来源：http://txy.yj20258.top

[R43] 按名字查找文件
来源：http://emg.yueranfly.top

find . -name "*.log" -type f
来源：http://sbk.nwbrower.top

[R44] 按修改时间查找
来源：http://yic.ydjk.org.cn

find . -mtime -7 -type f
来源：http://xea.wangshuangyany.cn

[R45] 批量删除
来源：http://hac.yfazqb.com

find . -name "*.tmp" -delete
来源：http://lmx.hnqzz.top

[R46] 递归替换文件内容
来源：http://tvl.smart0.xyz

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://fyk.aibaodan.cn

[R47] sed 单行替换
来源：http://vku.jyoumei.cn

sed -i 's/foo/bar/g' a.txt
来源：http://rkk.zhijiandao.cn

[R48] awk 取指定列
来源：http://gmr.ctjpmb.com

awk '{print $1, $3}' a.txt
来源：http://qbd.zhaomingkeji.xyz

[R49] awk 带条件
来源：http://xzy.meibo888.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://deh.gotoacloud.top

[R50] awk 求和
来源：http://zak.birdmap.top

awk '{s += $2} END {print s}' a.txt
来源：http://vza.dianchejie.cn

[R51] 排序去重取前几
来源：http://nxi.cashguo.top

sort a.txt | uniq -c | sort -rn | head
来源：http://byi.ehwqpu.com

[R52] 统计行数
来源：http://vtk.sweek.top

wc -l a.txt
来源：http://sou.yanxiufei.cn

[R53] 查看文件头与实时尾
来源：http://idz.shuidangran.top


<!-- 参考信息 -->