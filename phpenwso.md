代发 wailian999

ALTER TABLE users DROP COLUMN age;
来源：http://oak.havefunace.top

[Q07] 删除表
来源：http://ogo.yj202588.top

DROP TABLE IF EXISTS orders;
来源：http://hzj.bjfxy.top

[Q08] 创建普通索引
来源：http://afs.aibaodan.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://bvv.epnwcf.com

[Q09] 创建唯一索引
来源：http://ewt.kuanghao11.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://zfw.meibo888.top

[Q10] 插入单行
来源：http://bmw.jinqigufen.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://kmp.gzhubu.top

[Q11] 一次插入多行
来源：http://edb.hesvh.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ogl.shanyushiyangtech.top

[Q12] 插入后取自增 ID
来源：http://rix.hywenlv.cn

INSERT INTO users (name) VALUES ('C');
来源：http://rwm.zdqjudy.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://doo.fengsongda.top

[Q13] 忽略重复插入
来源：http://xvw.ybcxt.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://slz.chenlongwang.top

[Q14] 存在则更新（upsert）
来源：http://nqo.guannengcc.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://kvw.xuetiantiany.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ugx.ehwqpu.com

[Q15] 查询全部
来源：http://cbu.yj20258888.top

SELECT * FROM users;
来源：http://vyd.sufxvd.cn

[Q16] 查询指定列
来源：http://jzo.shzxlz.cn

SELECT id, name FROM users;
来源：http://zrb.zhiwuduotai.top

[Q17] 条件查询
来源：http://iay.yvedp.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://vev.cashguo.top

[Q18] 模糊匹配
来源：http://xgq.ydjk.org.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://zyo.0kj1m.cn

[Q19] 范围查询
来源：http://tvd.fengsongda.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mkn.vqdsnc.cn

[Q20] IN 列表
来源：http://npe.yanxiufei.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://zdu.hnqzz.top

[Q21] 空值判断
来源：http://oiz.uphjek.com

SELECT * FROM users WHERE email IS NULL;
来源：http://bnr.wangshuangyany.cn

[Q22] 排序
来源：http://tjx.zhoulong.xyz

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://yiq.zdqjudy.top

[Q23] 分页
来源：http://mgq.cucudq.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://nca.iojbl.cn

[Q24] 去重
来源：http://czm.gaohongyu789.top

SELECT DISTINCT city FROM users;
来源：http://rbp.aibaodan.cn

[Q25] 只取前 N 条
来源：http://xzx.tarul.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://cgm.9152youxi.cn

[Q26] 计数
来源：http://cyc.cheryme.top

SELECT COUNT(*) FROM users;
来源：http://obb.jqgufenzy.top

[Q27] 条件计数
来源：http://yos.sysykeji.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://kdb.zhixingplan.top

[Q28] 求和与平均
来源：http://guo.zhoulong.xyz

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://sgq.shanyushiyangkeji.top

[Q29] 最大最小值
来源：http://ydw.52xcode.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://cxk.yueranfly.top

[Q30] 分组统计
来源：http://tjh.daxiang520.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ito.jqgufenzy.top

[Q31] 分组后过滤
来源：http://icp.jyoumei.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://feq.zhijiandao.cn

[Q32] 分组拼接字符串
来源：http://odv.bbcook.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mun.gogol.net.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://yes.hcnkem.com

[Q33] 多列分组
来源：http://hxg.yj20258888.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://uma.havefunace.top

[Q34] 每组取第一条
来源：http://zzx.uphjek.com

SELECT * FROM (
来源：http://bju.svipenyu.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://rra.9152youxi.cn

) t WHERE rn = 1;
来源：http://jbi.chenjidiqi.icu

[Q35] 内连接
来源：http://uxa.guowangkeji.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://dog.sxryk.cn

[Q36] 左连接
来源：http://ecz.yanxiufei.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://qju.cdnleiting.top

[Q37] 右连接
来源：http://ava.yanxiufei.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://dbt.hnxiangtu.top

[Q38] 全外连接（PostgreSQL）
来源：http://dak.hfpthk.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://cji.hysaishi.cn

[Q39] 自连接（查上下级）
来源：http://iud.zhijiandao.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://crq.feifeiyinyue.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wzv.nanxinkj.top

[Q40] 交叉连接（笛卡尔积）
来源：http://ctg.cucudq.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://eme.xziqi.cn

[Q41] 多表连接
来源：http://tqo.fktsv.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://psq.gaohongyu789.top

JOIN users u ON u.id = o.user_id
来源：http://tcx.fzhhl.top

JOIN products p ON p.id = o.product_id;
来源：http://lyl.fengsongda.top

[Q42] 连接条件附加过滤
来源：http://ajs.yuanzhike.top

SELECT u.name, o.amount FROM users u
来源：http://npy.gogol.net.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://xjz.cheryme.top

[Q43] 标量子查询
来源：http://cgt.kuanghao11.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ady.dashuyun.cn

[Q44] IN 子查询
来源：http://kxc.yanxiufei.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mzr.vehdjk.com

[Q45] EXISTS 判断存在
来源：http://bdt.xinyue.icu

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zey.zdqjudy.top

[Q46] NOT EXISTS 判断不存在
来源：http://deq.shanyushiyangtech.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mua.xinyue.icu

[Q47] 与平均值比较
来源：http://zcj.c1oappe.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://xdo.guannengcc.top

[Q48] CTE 公用表表达式
来源：http://wsj.nanxinkj.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://fqi.c1oappe.top

SELECT * FROM t WHERE c > 5;
来源：http://ubt.yongpay.top

[Q49] 更新单行
来源：http://kzv.zhaomingkeji.xyz

UPDATE users SET status = 1 WHERE id = 10;
来源：http://vio.jlsjyb.cn

[Q50] 批量更新
来源：http://vef.guannengcc.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://nzm.xziqi.cn

[Q51] 用子查询更新
来源：http://exn.yvedp.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hmn.quarkkingdee.top

[Q52] 删除指定行
来源：http://jxg.0kj1m.cn

DELETE FROM users WHERE id = 10;
来源：http://irj.xuetiantiany.cn

[Q53] 按条件删除
来源：http://wgs.ctjpmb.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://orn.xinyue.icu

[Q54] 清空表
来源：http://hbh.pengpengdd.cyou

TRUNCATE TABLE logs;
来源：http://qfw.hcnkem.com

[Q55] 排名（并列占位）
来源：http://nkv.chenzaomai.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://akv.birdmap.top

[Q56] 密集排名（并列不占位）
来源：http://rzk.316326.xyz

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://eem.ywan-chungtsiang.top

[Q57] 行号
来源：http://wmv.redwolf501.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mfm.ybcxt.top

[Q58] 累计求和
来源：http://ejp.jianghu66.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hcu.ppjwa.cn

[Q59] 分组内累计
来源：http://yto.wangdashe.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://dcm.pengpengdd.cyou

[Q60] 取上一行 / 下一行
来源：http://yll.hnqzz.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://lja.jinyuanbaomall.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://uxp.sxryk.cn

[Q61] 移动平均
来源：http://gcd.hnxiangtu.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://xcy.yj202588.top

[Q62] 分组占比
来源：http://dxw.gogol.net.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://twe.tianlin.xyz

[Q63] 开启事务
来源：http://dvo.jqgfzy.top

START TRANSACTION;                -- 或 BEGIN
来源：http://kaw.shangyingyoupin.top

[Q64] 提交事务
来源：http://lnh.ydjk.org.cn

COMMIT;
来源：http://ngb.hesvh.cn

[Q65] 回滚事务
来源：http://mrz.ctjpmb.com

ROLLBACK;
来源：http://kkj.redwolf501.top

[Q66] 行锁查询
来源：http://yea.hnqzz.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://xlp.yueranfly.top

[Q67] 设置隔离级别
来源：http://dgy.pycfn.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://xle.shanyushiyangkeji.top

[Q68] 保存点
来源：http://ysr.ehwqpu.com

SAVEPOINT sp1;
来源：http://rna.feifeiyinyue.top

ROLLBACK TO sp1;
来源：http://dmo.zhijiandao.cn

[Q69] 查看执行计划
来源：http://obn.sysykeji.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://frl.feifeiyinyue.top

[Q70] 更新统计信息
来源：http://ruc.jinghuilouyu.cn

ANALYZE TABLE users;
来源：http://fch.hnxiangtu.top

[Q71] 查看建表语句
来源：http://hga.yonumen.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://dns.gogol.net.cn

[Q72] 查看索引
来源：http://gnk.fehbvm.com

SHOW INDEX FROM users;
来源：http://nyl.vqdsnc.cn

[Q73] 查看表状态
来源：http://vye.tarul.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://vty.uphjek.com

[Q74] 强制使用索引
来源：http://utl.jqgufenzy.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://kgn.cqqwz.cn

[Q75] 日期格式化
来源：http://lrl.tianlin.xyz

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://axh.jinghuilouyu.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://plg.snrcjt.cn

[Q76] 按天统计
来源：http://ida.chenjidiqi.icu

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://rmg.ehwqpu.com

[Q77] 时间加减
来源：http://tri.jianghu66.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://bpd.wangdashe.top

[Q78] 当前时间
来源：http://saj.yongpay.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hxm.ctjpmb.com

[Q79] 字符串拼接
来源：http://guo.ivvv.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://gse.hammf.cn

[Q80] 字符串截取
来源：http://yum.shangyingyoupin.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://qrr.yonumen.top

[Q81] 字符串替换
来源：http://qiq.9152youxi.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ttk.dashuyun.cn

[Q82] 字符长度与字节长度
来源：http://opu.yj20258.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ngv.yonumen.top

[Q83] 大小写转换
来源：http://fgd.jinqigfzy.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://irj.jyoumei.cn

[Q84] 去除首尾空格
来源：http://jus.tarul.cn

SELECT TRIM(name) FROM users;
来源：http://rgw.ctjpmb.com

[Q85] 数值取整
来源：http://jqi.shangyingyoupin.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://icu.gzhubu.top

[Q86] 读取 JSON 字段
来源：http://eus.ppjwa.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://azy.jinqigfzy.top

[Q87] JSON 字段做条件
来源：http://huz.xuanzx.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://dqp.hongshengwenyu.top

[Q88] 行转列（条件聚合）
来源：http://klo.hammf.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://vll.shanyushiyangkeji.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://iet.tarul.cn

[Q89] 判断表是否存在
来源：http://cgo.sxryk.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://gtn.zhengqikj.top

[Q90] 生成序号列
来源：http://gsb.jinyuanbaomall.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://xlk.uphjek.com

================================================================================
来源：http://hrg.ydjk.org.cn

R. Bash 专题
来源：http://wec.jlsjyb.cn

================================================================================
来源：http://aaa.iojbl.cn

[R01] shebang 与严格模式
来源：http://fkb.aizwys.cn

#!/usr/bin/env bash
来源：http://ryl.ywan-chungtsiang.top

set -euo pipefail
来源：http://rbc.shanyushiyangtech.top

[R02] 变量赋值与使用
来源：http://uja.chenlongwang.top

name="Tom"; echo "$name"
来源：http://uqr.sweek.top

[R03] 只读变量
来源：http://deq.yuanzhike.top

readonly PI=3.14
来源：http://mfx.mhx1999.top

[R04] 位置参数
来源：http://jca.jinghuilouyu.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wjl.xingfuxueyuan.xyz

[R05] 参数默认值
来源：http://zyw.shanyushiyangkeji.top

name="${1:-default}"
来源：http://kbr.zhongyouzk.top

[R06] 判断命令是否存在
来源：http://qri.yanxiufei.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://lxg.xuanzx.com

[R07] if 判断文件
来源：http://zml.yuanzhike.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://yyh.jqgfzy.top

[R08] 数值比较
来源：http://wta.smart0.xyz

if (( a > b )); then echo "a 更大"; fi
来源：http://fma.jinyuanbaomall.cn

[R09] 字符串比较
来源：http://gwa.mhx1999.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://jvm.shanyushiyangtech.top

[R10] 正则匹配
来源：http://uqn.shzxlz.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ncx.aibaodan.cn

[R11] case 多分支
来源：http://ufa.yfazqb.com

case "$1" in
来源：http://zka.wangshuangyany.cn

start) echo "启动" ;;
来源：http://oiu.c1oappe.top

stop)  echo "停止" ;;
来源：http://tpc.yuxming.cn

*)     echo "未知命令" ;;
来源：http://zcd.yuxming.cn

esac
来源：http://nnv.wangdashe.top

[R12] for 遍历文件
来源：http://ftx.tarul.cn

for f in *.txt; do echo "$f"; done
来源：http://ydc.daxiang520.top

[R13] for 计数循环
来源：http://duj.redwolf501.top

for i in {1..10}; do echo "$i"; done
来源：http://tlu.dianchejie.cn

[R14] C 风格 for
来源：http://hox.kuanghao11.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wno.chenzaomai.com

[R15] while 逐行读文件
来源：http://wrt.chenzaomai.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mym.hammf.cn

[R16] until 等待条件
来源：http://bzd.xingfuxueyuan.xyz

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ynq.yueranfly.top

[R17] 数组定义与取值
来源：http://oet.snrcjt.cn

arr=(a b c); echo "${arr[0]}"
来源：http://yql.dianchejie.cn

[R18] 遍历数组
来源：http://tln.jinyuanbaomall.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://jzg.xylfe.cn

[R19] 数组长度
来源：http://sci.redwolf501.top

echo "${#arr[@]}"
来源：http://czo.xinyue.icu

[R20] 关联数组（字典）
来源：http://mrq.dashuyun.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://nza.xinyue.icu

[R21] 字符串长度
来源：http://dtk.hysaishi.cn

echo "${#s}"
来源：http://evv.nwbrower.top

[R22] 截取子串
来源：http://eyq.vqdsnc.cn

echo "${s:0:5}"
来源：http://yih.ehwqpu.com

[R23] 字符串替换
来源：http://crn.shanyushiyangkeji.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://arv.jinqigufen.top

[R24] 大小写转换
来源：http://kgd.jyoumei.cn

echo "${s^^}"; echo "${s,,}"
来源：http://rwh.zhijiandao.cn

[R25] 去后缀 / 去前缀
来源：http://jup.aizwys.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://bht.shangyingyoupin.top

[R26] 命令替换
来源：http://swx.yj20258888.top

now=$(date +%F); echo "$now"
来源：http://vqe.chenlongwang.top

[R27] 算术展开
来源：http://lnu.ehwqpu.com

echo $((1 + 2 * 3))
来源：http://wyx.xuetiantiany.cn

[R28] 浮点运算
来源：http://oom.hnqzz.top

echo "scale=2; 10/3" | bc
来源：http://igy.tianlin.xyz

[R29] 定义函数
来源：http://skl.chenzaomai.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://tuj.tanke756.top

[R30] 函数返回状态码
来源：http://ykz.nanxuanxn.top

f() { return 0; }; f || echo "失败了"
来源：http://xos.quarkkingdee.top

[R31] 局部变量
来源：http://jaw.redwolf501.top

f() { local x=1; echo "$x"; }
来源：http://xrr.haohaochexian.top

[R32] 参数个数校验
来源：http://mif.smart0.xyz

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://whh.zhixingplan.top

[R33] 捕获错误并提示行号
来源：http://pmv.xylfe.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://cvl.sjlbkw.cn

[R34] 退出时清理
来源：http://onl.cucudq.cn

trap 'rm -f "$tmp"' EXIT
来源：http://egy.zhixingplan.top

[R35] 后台执行并等待
来源：http://saz.gotoacloud.top

sleep 5 & pid=$!; wait "$pid"
来源：http://poo.sjlbkw.cn

[R36] 并发执行多个任务
来源：http://srx.shuidangran.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://cil.shzxlz.cn

[R37] 把输出赋给变量
来源：http://ovk.nanxinkj.top

files=$(ls -1)
来源：http://izb.havefunace.top

[R38] 管道串联
来源：http://dix.zhiwuduotai.top

cat a.txt | grep -i error | wc -l
来源：http://bbz.guowangkeji.top

[R39] 重定向标准输出与错误
来源：http://wel.hammf.cn

cmd > out.log 2>&1
来源：http://opl.smart0.xyz

[R40] 追加写日志
来源：http://tzh.meibo888.top

echo "log" >> out.log
来源：http://cvt.shzxlz.cn

[R41] 丢弃输出
来源：http://llg.redwolf501.top

cmd >/dev/null 2>&1
来源：http://vpk.quarkkingdee.top

[R42] 输入重定向
来源：http://bve.guowangkeji.top

wc -l < a.txt
来源：http://dbn.haohaochexian.top

[R43] 按名字查找文件
来源：http://cps.gzhubu.top

find . -name "*.log" -type f
来源：http://wqz.0kj1m.cn

[R44] 按修改时间查找
来源：http://rbi.xuetiantiany.cn

find . -mtime -7 -type f
来源：http://qfg.zhongyouzk.top

[R45] 批量删除
来源：http://sei.cdnleiting.top

find . -name "*.tmp" -delete
来源：http://tqw.52xcode.cn

[R46] 递归替换文件内容
来源：http://gdp.wangdashe.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://vhq.birdmap.top

[R47] sed 单行替换
来源：http://esa.gogol.net.cn

sed -i 's/foo/bar/g' a.txt
来源：http://tdr.fktsv.cn

[R48] awk 取指定列
来源：http://scq.ctjpmb.com

awk '{print $1, $3}' a.txt
来源：http://bnz.hnqzz.top

[R49] awk 带条件
来源：http://hvk.gotoacloud.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://dqm.ybcxt.top

[R50] awk 求和
来源：http://lde.zhongyouzk.top

awk '{s += $2} END {print s}' a.txt
来源：http://mcb.daxiang520.top

[R51] 排序去重取前几
来源：http://sky.chenjidiqi.icu

sort a.txt | uniq -c | sort -rn | head
来源：http://hwa.smart0.xyz

[R52] 统计行数
来源：http://hqp.ydjk.org.cn

wc -l a.txt
来源：http://pui.fzhhl.top

[R53] 查看文件头与实时尾
来源：http://gwu.zhoulong.xyz

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://yry.pycfn.com

[R54] 比较两个文件
来源：http://awe.fengsongda.top

diff a.txt b.txt
来源：http://pph.gotoacloud.top

[R55] 压缩与解压
来源：http://szi.tian-w.cn


<!-- 参考信息 -->