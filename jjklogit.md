代发 wailian999

ALTER TABLE users DROP COLUMN age;
来源：http://eea.xziqi.cn

[Q07] 删除表
来源：http://yxz.shanyushiyangkeji.top

DROP TABLE IF EXISTS orders;
来源：http://cag.havefunace.top

[Q08] 创建普通索引
来源：http://bjw.jianghu66.top

CREATE INDEX idx_users_email ON users(email);
来源：http://oxf.c1oappe.top

[Q09] 创建唯一索引
来源：http://mfq.ppjwa.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://dcd.cqqwz.cn

[Q10] 插入单行
来源：http://rdg.snrcjt.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://kcr.zhiwuduotai.top

[Q11] 一次插入多行
来源：http://rns.jinqigfzy.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://dgd.cqqwz.cn

[Q12] 插入后取自增 ID
来源：http://qkc.jlsjyb.cn

INSERT INTO users (name) VALUES ('C');
来源：http://jsb.yj20258888.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://yuu.yuxming.cn

[Q13] 忽略重复插入
来源：http://hej.fktsv.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://zxr.zhiwuduotai.top

[Q14] 存在则更新（upsert）
来源：http://lgv.xuanzx.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://amo.shuidangran.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://kwq.yfazqb.com

[Q15] 查询全部
来源：http://zcn.sweek.top

SELECT * FROM users;
来源：http://zjo.shzxlz.cn

[Q16] 查询指定列
来源：http://qfa.chenlongwang.top

SELECT id, name FROM users;
来源：http://kgi.guowangkeji.top

[Q17] 条件查询
来源：http://arr.kuanghao11.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://goy.chenzaomai.com

[Q18] 模糊匹配
来源：http://bld.0kj1m.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ljb.tarul.cn

[Q19] 范围查询
来源：http://mem.shanyushiyangkeji.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mzd.yonumen.top

[Q20] IN 列表
来源：http://uoy.svipenyu.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://fxp.jinqigufen.top

[Q21] 空值判断
来源：http://rni.chenlongwang.top

SELECT * FROM users WHERE email IS NULL;
来源：http://kld.fzhhl.top

[Q22] 排序
来源：http://joy.jyoumei.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://thl.tanke756.top

[Q23] 分页
来源：http://oca.zycfv.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blo.dianchejie.cn

[Q24] 去重
来源：http://tof.xingfuxueyuan.xyz

SELECT DISTINCT city FROM users;
来源：http://uor.nwbrower.top

[Q25] 只取前 N 条
来源：http://pco.iojbl.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://vuq.ivvv.top

[Q26] 计数
来源：http://rms.yuanzhike.top

SELECT COUNT(*) FROM users;
来源：http://lja.yonumen.top

[Q27] 条件计数
来源：http://ree.epnwcf.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://doh.zhongyouzk.top

[Q28] 求和与平均
来源：http://ily.zycfv.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://lzh.tanke756.top

[Q29] 最大最小值
来源：http://plr.xingfuxueyuan.xyz

SELECT MAX(age), MIN(age) FROM users;
来源：http://jfx.dashuyun.cn

[Q30] 分组统计
来源：http://ocs.zdbjq.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://aes.zdqjudy.top

[Q31] 分组后过滤
来源：http://cai.yongpay.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://gxp.meibo888.top

[Q32] 分组拼接字符串
来源：http://bqj.fktsv.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://tes.xinyue.icu

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://kbg.jianghu66.top

[Q33] 多列分组
来源：http://ckf.yangfankeji.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ijm.sufxvd.cn

[Q34] 每组取第一条
来源：http://ykd.zhengqikj.top

SELECT * FROM (
来源：http://dzp.cucudq.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://vkk.yangfankeji.com

) t WHERE rn = 1;
来源：http://hvv.guannengcc.top

[Q35] 内连接
来源：http://ilx.nanxinkj.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://lhk.jinqigufen.top

[Q36] 左连接
来源：http://zqc.fanxiaobao.xyz

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://oge.ybcxt.top

[Q37] 右连接
来源：http://hco.sjlbkw.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://tyk.chenzaomai.com

[Q38] 全外连接（PostgreSQL）
来源：http://agf.chenlongwang.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://rtt.yangfankeji.com

[Q39] 自连接（查上下级）
来源：http://gbk.yongpay.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://ial.ctjpmb.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://lzh.iojbl.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://gjt.sxryk.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://las.daria6918.cn

[Q41] 多表连接
来源：http://wpp.tarul.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://fly.jinqigfzy.top

JOIN users u ON u.id = o.user_id
来源：http://cgq.jinqigufen.top

JOIN products p ON p.id = o.product_id;
来源：http://qif.ydzc1.top

[Q42] 连接条件附加过滤
来源：http://xbj.wangshuangyany.cn

SELECT u.name, o.amount FROM users u
来源：http://ttb.sxryk.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ohg.sufxvd.cn

[Q43] 标量子查询
来源：http://lxw.xylfe.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://geo.zhijiandao.cn

[Q44] IN 子查询
来源：http://hml.yangfankeji.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ydd.bjfxy.top

[Q45] EXISTS 判断存在
来源：http://yaj.xuetiantiany.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://pxq.yj20258.top

[Q46] NOT EXISTS 判断不存在
来源：http://rqc.jinqigfzy.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://srn.sysykeji.top

[Q47] 与平均值比较
来源：http://epm.guowangkeji.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://xps.pycfn.com

[Q48] CTE 公用表表达式
来源：http://imn.daria6918.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://phg.zhongyouzk.top

SELECT * FROM t WHERE c > 5;
来源：http://qio.cucudq.cn

[Q49] 更新单行
来源：http://meu.svipenyu.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://xtt.hongshengwenyu.top

[Q50] 批量更新
来源：http://rmm.daria6918.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://xrr.ybcxt.top

[Q51] 用子查询更新
来源：http://jlt.yvedp.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://bqr.yj202588.top

[Q52] 删除指定行
来源：http://buz.ywan-chungtsiang.top

DELETE FROM users WHERE id = 10;
来源：http://uht.316326.xyz

[Q53] 按条件删除
来源：http://ndo.daria6918.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wce.redwolf501.top

[Q54] 清空表
来源：http://tqo.wangshuangyany.cn

TRUNCATE TABLE logs;
来源：http://yjf.zhiwuduotai.top

[Q55] 排名（并列占位）
来源：http://ksd.ppjwa.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://rye.chenlongwang.top

[Q56] 密集排名（并列不占位）
来源：http://lqc.guannengcc.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ncg.gzhubu.top

[Q57] 行号
来源：http://ixg.9152youxi.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://onr.ybcxt.top

[Q58] 累计求和
来源：http://sho.hesvh.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://fjz.sjlbkw.cn

[Q59] 分组内累计
来源：http://jwe.shuidangran.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://liu.xuetiantiany.cn

[Q60] 取上一行 / 下一行
来源：http://kkf.xinyue.icu

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://slm.zhiwuduotai.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wco.sweek.top

[Q61] 移动平均
来源：http://mhz.xinyue.icu

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://fwd.yj20258.top

[Q62] 分组占比
来源：http://fhu.zhiwuduotai.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://bnm.xingfuxueyuan.xyz

[Q63] 开启事务
来源：http://mvj.zhiwuduotai.top

START TRANSACTION;                -- 或 BEGIN
来源：http://qbs.haohaochexian.top

[Q64] 提交事务
来源：http://ptn.cdnleiting.top

COMMIT;
来源：http://qry.316326.xyz

[Q65] 回滚事务
来源：http://jrt.smart0.xyz

ROLLBACK;
来源：http://ixj.hnxiangtu.top

[Q66] 行锁查询
来源：http://nju.gaohongyu789.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://vhy.jqgufenzy.top

[Q67] 设置隔离级别
来源：http://spl.sysykeji.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://egx.feifeiyinyue.top

[Q68] 保存点
来源：http://efl.xziqi.cn

SAVEPOINT sp1;
来源：http://rbo.shanyushiyangkeji.top

ROLLBACK TO sp1;
来源：http://yro.daria6918.cn

[Q69] 查看执行计划
来源：http://gyq.shzxlz.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ncw.jinqigfzy.top

[Q70] 更新统计信息
来源：http://idp.jqgufenzy.top

ANALYZE TABLE users;
来源：http://ztm.xylfe.cn

[Q71] 查看建表语句
来源：http://kvu.shanyushiyangtech.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://qef.fzhhl.top

[Q72] 查看索引
来源：http://bbq.zhixingplan.top

SHOW INDEX FROM users;
来源：http://shz.pengpengdd.cyou

[Q73] 查看表状态
来源：http://zwd.yvedp.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://kgp.aizwys.cn

[Q74] 强制使用索引
来源：http://rvs.shangyingyoupin.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://irp.daxiang520.top

[Q75] 日期格式化
来源：http://ujj.c1oappe.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://xmt.uphjek.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://pvw.zdqjudy.top

[Q76] 按天统计
来源：http://jsp.9152youxi.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://lyz.gotoacloud.top

[Q77] 时间加减
来源：http://gbq.jqgufenzy.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://raz.jinghuilouyu.cn

[Q78] 当前时间
来源：http://vwc.jianghu66.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://vrj.fzhhl.top

[Q79] 字符串拼接
来源：http://mkr.gogol.net.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://gsb.yangfankeji.com

[Q80] 字符串截取
来源：http://vxj.gotoacloud.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://zls.wangdashe.top

[Q81] 字符串替换
来源：http://osx.cashguo.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://cll.jianghu66.top

[Q82] 字符长度与字节长度
来源：http://qiz.redwolf501.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://odf.hongshengwenyu.top

[Q83] 大小写转换
来源：http://dfx.jqgufenzy.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ycq.hesvh.cn

[Q84] 去除首尾空格
来源：http://alb.yangfankeji.com

SELECT TRIM(name) FROM users;
来源：http://ini.daria6918.cn

[Q85] 数值取整
来源：http://aee.redwolf501.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://zus.ydjk.org.cn

[Q86] 读取 JSON 字段
来源：http://ltq.sysykeji.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://gvp.sjlbkw.cn

[Q87] JSON 字段做条件
来源：http://fog.ybcxt.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ulg.jiagoushi.top

[Q88] 行转列（条件聚合）
来源：http://ukq.jqgfzy.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://odh.zhaomingkeji.xyz

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://jqh.redwolf501.top

[Q89] 判断表是否存在
来源：http://yck.hfpthk.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://zoq.cqqwz.cn

[Q90] 生成序号列
来源：http://dro.zhiwuduotai.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://iof.jianghu66.top

================================================================================
来源：http://qit.zhaomingkeji.xyz

R. Bash 专题
来源：http://gte.uphjek.com

================================================================================
来源：http://yac.sxryk.cn

[R01] shebang 与严格模式
来源：http://wbm.jinyuanbaomall.cn

#!/usr/bin/env bash
来源：http://tuf.xuetiantiany.cn

set -euo pipefail
来源：http://kex.ivvv.top

[R02] 变量赋值与使用
来源：http://lrd.jqgufenzy.top

name="Tom"; echo "$name"
来源：http://ixk.jiagoushi.top

[R03] 只读变量
来源：http://qob.fehbvm.com

readonly PI=3.14
来源：http://wlo.mhx1999.top

[R04] 位置参数
来源：http://ysm.guannengcc.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://fsr.gaohongyu789.top

[R05] 参数默认值
来源：http://gwc.bbcook.cn

name="${1:-default}"
来源：http://xbq.zhixingplan.top

[R06] 判断命令是否存在
来源：http://yaz.xingfuxueyuan.xyz

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://fug.c1oappe.top

[R07] if 判断文件
来源：http://khc.ydjk.org.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://uwv.sjlbkw.cn

[R08] 数值比较
来源：http://ipx.ivvv.top

if (( a > b )); then echo "a 更大"; fi
来源：http://euu.tarul.cn

[R09] 字符串比较
来源：http://qjy.feifeiyinyue.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://zpg.cucudq.cn

[R10] 正则匹配
来源：http://bwn.9152youxi.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://cpy.zhengqikj.top

[R11] case 多分支
来源：http://ccf.pengpengdd.cyou

case "$1" in
来源：http://hav.xuanzx.com

start) echo "启动" ;;
来源：http://oxk.c1oappe.top

stop)  echo "停止" ;;
来源：http://oyo.pycfn.com

*)     echo "未知命令" ;;
来源：http://ohl.uphjek.com

esac
来源：http://umu.sysykeji.top

[R12] for 遍历文件
来源：http://tbl.tarul.cn

for f in *.txt; do echo "$f"; done
来源：http://kdb.yuxming.cn

[R13] for 计数循环
来源：http://nhj.pengpengdd.cyou

for i in {1..10}; do echo "$i"; done
来源：http://gzd.gotoacloud.top

[R14] C 风格 for
来源：http://aqx.snrcjt.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://uhj.yvedp.cn

[R15] while 逐行读文件
来源：http://oku.hysaishi.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://per.cdnleiting.top

[R16] until 等待条件
来源：http://etc.vehdjk.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://tfo.iojbl.cn

[R17] 数组定义与取值
来源：http://cdn.chenzaomai.com

arr=(a b c); echo "${arr[0]}"
来源：http://qwd.aizwys.cn

[R18] 遍历数组
来源：http://nkb.ivvv.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://coo.sufxvd.cn

[R19] 数组长度
来源：http://cuh.tianlin.xyz

echo "${#arr[@]}"
来源：http://hdl.jlsjyb.cn

[R20] 关联数组（字典）
来源：http://ysq.feifeiyinyue.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://umu.tian-w.cn

[R21] 字符串长度
来源：http://tma.chenlongwang.top

echo "${#s}"
来源：http://wvv.ppjwa.cn

[R22] 截取子串
来源：http://pdq.zhoulong.xyz

echo "${s:0:5}"
来源：http://drh.gogol.net.cn

[R23] 字符串替换
来源：http://iox.jlsjyb.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://kih.xuetiantiany.cn

[R24] 大小写转换
来源：http://lot.daria6918.cn

echo "${s^^}"; echo "${s,,}"
来源：http://bfb.jinqigfzy.top

[R25] 去后缀 / 去前缀
来源：http://ckk.gzhubu.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://vaz.yanxiufei.cn

[R26] 命令替换
来源：http://xxh.shangyingyoupin.top

now=$(date +%F); echo "$now"
来源：http://pqh.tanke756.top

[R27] 算术展开
来源：http://jeq.meibo888.top

echo $((1 + 2 * 3))
来源：http://bip.yanxiufei.cn

[R28] 浮点运算
来源：http://pal.shanyushiyangtech.top

echo "scale=2; 10/3" | bc
来源：http://cub.cdnleiting.top

[R29] 定义函数
来源：http://laj.pycfn.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mec.birdmap.top

[R30] 函数返回状态码
来源：http://cht.jqgfzy.top

f() { return 0; }; f || echo "失败了"
来源：http://ezq.aibaodan.cn

[R31] 局部变量
来源：http://jzg.wangshuangyany.cn

f() { local x=1; echo "$x"; }
来源：http://eaf.9152youxi.cn

[R32] 参数个数校验
来源：http://pou.bbcook.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://yms.meibo888.top

[R33] 捕获错误并提示行号
来源：http://jnv.nwbrower.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://lcw.9152youxi.cn

[R34] 退出时清理
来源：http://pvd.xingfuxueyuan.xyz

trap 'rm -f "$tmp"' EXIT
来源：http://nos.yonumen.top

[R35] 后台执行并等待
来源：http://hfb.zdbjq.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://fqa.yj20258888.top

[R36] 并发执行多个任务
来源：http://egp.c1oappe.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://smt.zhaomingkeji.xyz

[R37] 把输出赋给变量
来源：http://ixh.chenjidiqi.icu

files=$(ls -1)
来源：http://cjv.pycfn.com

[R38] 管道串联
来源：http://ess.sufxvd.cn

cat a.txt | grep -i error | wc -l
来源：http://qob.cucudq.cn

[R39] 重定向标准输出与错误
来源：http://ylo.zhiwuduotai.top

cmd > out.log 2>&1
来源：http://hyp.vehdjk.com

[R40] 追加写日志
来源：http://fpu.zhoulong.xyz

echo "log" >> out.log
来源：http://cqn.fktsv.cn

[R41] 丢弃输出
来源：http://sfc.uphjek.com

cmd >/dev/null 2>&1
来源：http://jfr.sysykeji.top

[R42] 输入重定向
来源：http://xay.hfpthk.cn

wc -l < a.txt
来源：http://llg.jqgfzy.top

[R43] 按名字查找文件
来源：http://teb.hywenlv.cn

find . -name "*.log" -type f
来源：http://bcd.yfazqb.com

[R44] 按修改时间查找
来源：http://jun.iojbl.cn

find . -mtime -7 -type f
来源：http://pxv.daxiang520.top

[R45] 批量删除
来源：http://ons.zhiwuduotai.top

find . -name "*.tmp" -delete
来源：http://acx.sxryk.cn

[R46] 递归替换文件内容
来源：http://cck.jinghuilouyu.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://cat.xingfuxueyuan.xyz

[R47] sed 单行替换
来源：http://zgl.dashuyun.cn

sed -i 's/foo/bar/g' a.txt
来源：http://hzh.aizwys.cn

[R48] awk 取指定列
来源：http://kyb.hysaishi.cn

awk '{print $1, $3}' a.txt
来源：http://cgd.xuetiantiany.cn

[R49] awk 带条件
来源：http://alq.guowangkeji.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://rmw.yangfankeji.com

[R50] awk 求和
来源：http://qbc.shuidangran.top

awk '{s += $2} END {print s}' a.txt
来源：http://yhb.shuidangran.top

[R51] 排序去重取前几
来源：http://uvx.fehbvm.com

sort a.txt | uniq -c | sort -rn | head
来源：http://awp.tarul.cn

[R52] 统计行数
来源：http://fbx.yj20258.top

wc -l a.txt
来源：http://ada.tianlin.xyz

[R53] 查看文件头与实时尾
来源：http://sdj.aizwys.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://sfo.cheryme.top

[R54] 比较两个文件
来源：http://gmd.shzxlz.cn

diff a.txt b.txt
来源：http://fwa.sysykeji.top

[R55] 压缩与解压
来源：http://gmi.andypj.xyz


<!-- 参考信息 -->