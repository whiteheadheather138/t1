代发 wailian999

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://jyj.yongpay.top

[Q05] 重命名列
来源：http://opx.52xcode.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://fhh.fehbvm.com

[Q06] 删除列
来源：http://dkn.jyoumei.cn

ALTER TABLE users DROP COLUMN age;
来源：http://lbx.hongshengwenyu.top

[Q07] 删除表
来源：http://cbc.jinghuilouyu.cn

DROP TABLE IF EXISTS orders;
来源：http://toj.jinghuilouyu.cn

[Q08] 创建普通索引
来源：http://dqh.haohaochexian.top

CREATE INDEX idx_users_email ON users(email);
来源：http://sdu.wangshuangyany.cn

[Q09] 创建唯一索引
来源：http://yhf.epnwcf.com

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://zpc.jqgfzy.top

[Q10] 插入单行
来源：http://vcr.xuetiantiany.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://tnz.dianchejie.cn

[Q11] 一次插入多行
来源：http://mba.c1oappe.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://gct.yj20258.top

[Q12] 插入后取自增 ID
来源：http://stc.ydjk.org.cn

INSERT INTO users (name) VALUES ('C');
来源：http://csc.yvedp.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://iej.kuanghao11.cn

[Q13] 忽略重复插入
来源：http://mbc.yanxiufei.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://vtr.hywenlv.cn

[Q14] 存在则更新（upsert）
来源：http://avw.jqgufenzy.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://vyo.zhoulong.xyz

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://tjq.redwolf501.top

[Q15] 查询全部
来源：http://gsv.xingfuxueyuan.xyz

SELECT * FROM users;
来源：http://jpl.nanxuanxn.top

[Q16] 查询指定列
来源：http://zlh.iojbl.cn

SELECT id, name FROM users;
来源：http://zyj.sxryk.cn

[Q17] 条件查询
来源：http://hce.vehdjk.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://tqi.zhixingplan.top

[Q18] 模糊匹配
来源：http://dnq.kuanghao11.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://lcg.zhaomingkeji.xyz

[Q19] 范围查询
来源：http://bro.guannengcc.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ekv.ydjk.org.cn

[Q20] IN 列表
来源：http://pkl.shuidangran.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://xwy.cheryme.top

[Q21] 空值判断
来源：http://pqo.ybcxt.top

SELECT * FROM users WHERE email IS NULL;
来源：http://tgz.jqgfzy.top

[Q22] 排序
来源：http://jvo.guannengcc.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://eee.ehwqpu.com

[Q23] 分页
来源：http://qlm.sxryk.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://eqf.guowangkeji.top

[Q24] 去重
来源：http://xny.cashguo.top

SELECT DISTINCT city FROM users;
来源：http://cmk.cqqwz.cn

[Q25] 只取前 N 条
来源：http://xqm.zdqjudy.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mgi.jlsjyb.cn

[Q26] 计数
来源：http://zte.fzhhl.top

SELECT COUNT(*) FROM users;
来源：http://ccx.ydzc1.top

[Q27] 条件计数
来源：http://dyf.zhaomingkeji.xyz

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ayj.hcnkem.com

[Q28] 求和与平均
来源：http://hbz.uphjek.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://xbr.sufxvd.cn

[Q29] 最大最小值
来源：http://syd.havefunace.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://rmi.cheryme.top

[Q30] 分组统计
来源：http://spx.ydzc1.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://rao.tarul.cn

[Q31] 分组后过滤
来源：http://ubo.shangyingyoupin.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://llo.dashuyun.cn

[Q32] 分组拼接字符串
来源：http://abw.wangshuangyany.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ioh.xuanzx.com

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://cvb.daria6918.cn

[Q33] 多列分组
来源：http://wnq.kuanghao11.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://uce.cucudq.cn

[Q34] 每组取第一条
来源：http://zdq.chenzaomai.com

SELECT * FROM (
来源：http://zqi.zhongyouzk.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://eyn.ybcxt.top

) t WHERE rn = 1;
来源：http://kvy.hammf.cn

[Q35] 内连接
来源：http://xyz.c1oappe.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://dqf.tarul.cn

[Q36] 左连接
来源：http://dok.zdbjq.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://rji.zhoulong.xyz

[Q37] 右连接
来源：http://cfh.yanxiufei.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://lcv.gotoacloud.top

[Q38] 全外连接（PostgreSQL）
来源：http://hpj.hesvh.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hyr.sjlbkw.cn

[Q39] 自连接（查上下级）
来源：http://cht.pengpengdd.cyou

SELECT e.name, m.name AS manager FROM employees e
来源：http://xfc.tarul.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://qhx.aibaodan.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://sbs.birdmap.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://nmm.hammf.cn

[Q41] 多表连接
来源：http://hjb.zdqjudy.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://cly.xuetiantiany.cn

JOIN users u ON u.id = o.user_id
来源：http://fbn.fehbvm.com

JOIN products p ON p.id = o.product_id;
来源：http://cgs.ppjwa.cn

[Q42] 连接条件附加过滤
来源：http://ppb.hysaishi.cn

SELECT u.name, o.amount FROM users u
来源：http://xfi.xylfe.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://tdy.chenlongwang.top

[Q43] 标量子查询
来源：http://eze.gzhubu.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://bvh.redwolf501.top

[Q44] IN 子查询
来源：http://jgp.zhongyouzk.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mlz.daria6918.cn

[Q45] EXISTS 判断存在
来源：http://oep.cdnleiting.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://sbt.jqgfzy.top

[Q46] NOT EXISTS 判断不存在
来源：http://rfx.yuanzhike.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ned.chenlongwang.top

[Q47] 与平均值比较
来源：http://kbl.nwbrower.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://yrn.zhijiandao.cn

[Q48] CTE 公用表表达式
来源：http://azb.jiagoushi.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ndw.wangdashe.top

SELECT * FROM t WHERE c > 5;
来源：http://vkw.pengpengdd.cyou

[Q49] 更新单行
来源：http://xrb.zhaomingkeji.xyz

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wmi.jinyuanbaomall.cn

[Q50] 批量更新
来源：http://xam.cheryme.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://jbz.dashuyun.cn

[Q51] 用子查询更新
来源：http://kgg.hongshengwenyu.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://fro.xinyue.icu

[Q52] 删除指定行
来源：http://xzp.hywenlv.cn

DELETE FROM users WHERE id = 10;
来源：http://uea.yangfankeji.com

[Q53] 按条件删除
来源：http://eug.sufxvd.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://meu.fanxiaobao.xyz

[Q54] 清空表
来源：http://cvo.bbcook.cn

TRUNCATE TABLE logs;
来源：http://ykt.cucudq.cn

[Q55] 排名（并列占位）
来源：http://pdx.redwolf501.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://onx.aibaodan.cn

[Q56] 密集排名（并列不占位）
来源：http://oeu.hongshengwenyu.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://fed.316326.xyz

[Q57] 行号
来源：http://aiy.zhoulong.xyz

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://qkm.shanyushiyangkeji.top

[Q58] 累计求和
来源：http://jcv.gotoacloud.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://tma.yongpay.top

[Q59] 分组内累计
来源：http://hun.aizwys.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mbb.guannengcc.top

[Q60] 取上一行 / 下一行
来源：http://zbm.gotoacloud.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://rtq.pycfn.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://gny.epnwcf.com

[Q61] 移动平均
来源：http://nfs.xinyue.icu

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://dvb.ydzc1.top

[Q62] 分组占比
来源：http://smt.tarul.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://pfe.yongpay.top

[Q63] 开启事务
来源：http://imf.vqdsnc.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://fvz.chenjidiqi.icu

[Q64] 提交事务
来源：http://upc.jinqigufen.top

COMMIT;
来源：http://rgu.zhaomingkeji.xyz

[Q65] 回滚事务
来源：http://nrn.shanyushiyangtech.top

ROLLBACK;
来源：http://cga.jinyuanbaomall.cn

[Q66] 行锁查询
来源：http://suu.xylfe.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://txu.yongpay.top

[Q67] 设置隔离级别
来源：http://hqi.xuanzx.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ucd.52xcode.cn

[Q68] 保存点
来源：http://smt.tianlin.xyz

SAVEPOINT sp1;
来源：http://bif.jlsjyb.cn

ROLLBACK TO sp1;
来源：http://ahz.316326.xyz

[Q69] 查看执行计划
来源：http://sci.zhixingplan.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://stl.xuanzx.com

[Q70] 更新统计信息
来源：http://diz.ehwqpu.com

ANALYZE TABLE users;
来源：http://dva.hysaishi.cn

[Q71] 查看建表语句
来源：http://udi.jinyuanbaomall.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://psn.xingfuxueyuan.xyz

[Q72] 查看索引
来源：http://lpe.jqgufenzy.top

SHOW INDEX FROM users;
来源：http://duy.zdqjudy.top

[Q73] 查看表状态
来源：http://ast.nanxuanxn.top

SHOW TABLE STATUS LIKE 'users';
来源：http://met.gaohongyu789.top

[Q74] 强制使用索引
来源：http://dnd.snrcjt.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://kco.aibaodan.cn

[Q75] 日期格式化
来源：http://qeo.wangdashe.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://boc.yfazqb.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://pmz.jlsjyb.cn

[Q76] 按天统计
来源：http://hoc.sjlbkw.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://jkr.jinqigufen.top

[Q77] 时间加减
来源：http://zfn.shzxlz.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://col.yanxiufei.cn

[Q78] 当前时间
来源：http://ozv.zhongyouzk.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://jsv.hywenlv.cn

[Q79] 字符串拼接
来源：http://cyr.hfpthk.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ols.hywenlv.cn

[Q80] 字符串截取
来源：http://hgh.mhx1999.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ffr.aibaodan.cn

[Q81] 字符串替换
来源：http://dfq.redwolf501.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://jjb.haohaochexian.top

[Q82] 字符长度与字节长度
来源：http://aee.hysaishi.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://dbm.316326.xyz

[Q83] 大小写转换
来源：http://pos.xylfe.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://jco.guowangkeji.top

[Q84] 去除首尾空格
来源：http://xwm.ywan-chungtsiang.top

SELECT TRIM(name) FROM users;
来源：http://qom.shanyushiyangtech.top

[Q85] 数值取整
来源：http://sen.ctjpmb.com

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://lcf.yangfankeji.com

[Q86] 读取 JSON 字段
来源：http://one.jyoumei.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://rmy.yfazqb.com

[Q87] JSON 字段做条件
来源：http://mzo.pengpengdd.cyou

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://qgg.jqgufenzy.top

[Q88] 行转列（条件聚合）
来源：http://xmf.redwolf501.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://csk.316326.xyz

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://qqc.bjfxy.top

[Q89] 判断表是否存在
来源：http://equ.tanke756.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://qzn.ybcxt.top

[Q90] 生成序号列
来源：http://ppo.yuxming.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://izb.ppjwa.cn

================================================================================
来源：http://krv.shangyingyoupin.top

R. Bash 专题
来源：http://hyh.ywan-chungtsiang.top

================================================================================
来源：http://eov.hnxiangtu.top

[R01] shebang 与严格模式
来源：http://xge.9152youxi.cn

#!/usr/bin/env bash
来源：http://icp.vehdjk.com

set -euo pipefail
来源：http://kmx.yonumen.top

[R02] 变量赋值与使用
来源：http://zpb.jqgfzy.top

name="Tom"; echo "$name"
来源：http://zfb.iojbl.cn

[R03] 只读变量
来源：http://vmt.xylfe.cn

readonly PI=3.14
来源：http://ojk.dianchejie.cn

[R04] 位置参数
来源：http://xwq.fzhhl.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ouf.xziqi.cn

[R05] 参数默认值
来源：http://edt.sufxvd.cn

name="${1:-default}"
来源：http://pkk.zycfv.cn

[R06] 判断命令是否存在
来源：http://bif.jinqigfzy.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://tbg.yueranfly.top

[R07] if 判断文件
来源：http://qyi.316326.xyz

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ldb.fanxiaobao.xyz

[R08] 数值比较
来源：http://rql.tian-w.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://omd.zhaomingkeji.xyz

[R09] 字符串比较
来源：http://kil.shuidangran.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://apu.9152youxi.cn

[R10] 正则匹配
来源：http://elb.tian-w.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://cwe.ywan-chungtsiang.top

[R11] case 多分支
来源：http://ihh.chenjidiqi.icu

case "$1" in
来源：http://edm.vqdsnc.cn

start) echo "启动" ;;
来源：http://ady.jinghuilouyu.cn

stop)  echo "停止" ;;
来源：http://mkn.gogol.net.cn

*)     echo "未知命令" ;;
来源：http://yla.ivvv.top

esac
来源：http://uqv.ydzc1.top

[R12] for 遍历文件
来源：http://ttd.ydzc1.top

for f in *.txt; do echo "$f"; done
来源：http://rgy.guowangkeji.top

[R13] for 计数循环
来源：http://lek.guannengcc.top

for i in {1..10}; do echo "$i"; done
来源：http://ckl.cheryme.top

[R14] C 风格 for
来源：http://ffv.hysaishi.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://jfq.jinqigfzy.top

[R15] while 逐行读文件
来源：http://ggf.gotoacloud.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mzv.ppjwa.cn

[R16] until 等待条件
来源：http://hof.pengpengdd.cyou

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wmc.gogol.net.cn

[R17] 数组定义与取值
来源：http://tho.ehwqpu.com

arr=(a b c); echo "${arr[0]}"
来源：http://khz.pengpengdd.cyou

[R18] 遍历数组
来源：http://lwa.aibaodan.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://sey.shanyushiyangkeji.top

[R19] 数组长度
来源：http://uce.xuanzx.com

echo "${#arr[@]}"
来源：http://vyt.yuanzhike.top

[R20] 关联数组（字典）
来源：http://bou.yonumen.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://kse.hnqzz.top

[R21] 字符串长度
来源：http://dru.yueranfly.top

echo "${#s}"
来源：http://ics.chenlongwang.top

[R22] 截取子串
来源：http://bvb.shuidangran.top

echo "${s:0:5}"
来源：http://nsl.cheryme.top

[R23] 字符串替换
来源：http://zqs.ivvv.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wjo.zhongyouzk.top

[R24] 大小写转换
来源：http://ygj.cashguo.top

echo "${s^^}"; echo "${s,,}"
来源：http://qek.xinyue.icu

[R25] 去后缀 / 去前缀
来源：http://mkt.zhengqikj.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://zrh.jyoumei.cn

[R26] 命令替换
来源：http://rjp.daxiang520.top

now=$(date +%F); echo "$now"
来源：http://usm.yongpay.top

[R27] 算术展开
来源：http://igl.yj20258888.top

echo $((1 + 2 * 3))
来源：http://pwm.tianlin.xyz

[R28] 浮点运算
来源：http://jwj.bbcook.cn

echo "scale=2; 10/3" | bc
来源：http://xma.fehbvm.com

[R29] 定义函数
来源：http://fhv.shuidangran.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ias.wangshuangyany.cn

[R30] 函数返回状态码
来源：http://ayi.tianlin.xyz

f() { return 0; }; f || echo "失败了"
来源：http://pxl.xingfuxueyuan.xyz

[R31] 局部变量
来源：http://qkj.snrcjt.cn

f() { local x=1; echo "$x"; }
来源：http://kdn.gotoacloud.top

[R32] 参数个数校验
来源：http://zlv.gotoacloud.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://imw.tian-w.cn

[R33] 捕获错误并提示行号
来源：http://dox.smart0.xyz

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://zky.fehbvm.com

[R34] 退出时清理
来源：http://fbh.hcnkem.com

trap 'rm -f "$tmp"' EXIT
来源：http://dyj.xinyue.icu

[R35] 后台执行并等待
来源：http://jgy.jlsjyb.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://tav.hnxiangtu.top

[R36] 并发执行多个任务
来源：http://cyk.hammf.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ijw.chenjidiqi.icu

[R37] 把输出赋给变量
来源：http://jtq.yj20258.top

files=$(ls -1)
来源：http://ggb.uphjek.com

[R38] 管道串联
来源：http://jlq.daria6918.cn

cat a.txt | grep -i error | wc -l
来源：http://niz.zdbjq.cn

[R39] 重定向标准输出与错误
来源：http://uwy.nanxuanxn.top

cmd > out.log 2>&1
来源：http://yoi.hfpthk.cn

[R40] 追加写日志
来源：http://gay.yuxming.cn

echo "log" >> out.log
来源：http://qko.ybcxt.top

[R41] 丢弃输出
来源：http://muu.guannengcc.top

cmd >/dev/null 2>&1
来源：http://lbv.daria6918.cn

[R42] 输入重定向
来源：http://baa.pycfn.com

wc -l < a.txt
来源：http://kko.cqqwz.cn

[R43] 按名字查找文件
来源：http://mxg.tianlin.xyz

find . -name "*.log" -type f
来源：http://wup.shuidangran.top

[R44] 按修改时间查找
来源：http://xpq.jiagoushi.top

find . -mtime -7 -type f
来源：http://ijj.c1oappe.top

[R45] 批量删除
来源：http://dqu.hysaishi.cn

find . -name "*.tmp" -delete
来源：http://cnr.9152youxi.cn

[R46] 递归替换文件内容
来源：http://srm.nanxuanxn.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://sko.jqgfzy.top

[R47] sed 单行替换
来源：http://azo.vqdsnc.cn

sed -i 's/foo/bar/g' a.txt
来源：http://qnb.tian-w.cn

[R48] awk 取指定列
来源：http://hva.iojbl.cn

awk '{print $1, $3}' a.txt
来源：http://nzb.c1oappe.top

[R49] awk 带条件
来源：http://occ.aizwys.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://uad.zhiwuduotai.top

[R50] awk 求和
来源：http://fjp.zhongyouzk.top

awk '{s += $2} END {print s}' a.txt
来源：http://wae.zhongyouzk.top

[R51] 排序去重取前几
来源：http://vag.316326.xyz

sort a.txt | uniq -c | sort -rn | head
来源：http://wml.yanxiufei.cn

[R52] 统计行数
来源：http://jvz.shuidangran.top

wc -l a.txt
来源：http://bxm.fehbvm.com

[R53] 查看文件头与实时尾
来源：http://jgb.0kj1m.cn


<!-- 参考信息 -->