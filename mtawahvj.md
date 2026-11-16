代发 wailian999

ALTER TABLE users DROP COLUMN age;
来源：http://ggz.316326.xyz

[Q07] 删除表
来源：http://ocn.hongshengwenyu.top

DROP TABLE IF EXISTS orders;
来源：http://mzh.gogol.net.cn

[Q08] 创建普通索引
来源：http://vjv.yueranfly.top

CREATE INDEX idx_users_email ON users(email);
来源：http://iec.xziqi.cn

[Q09] 创建唯一索引
来源：http://zpg.yj20258888.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://sod.ppjwa.cn

[Q10] 插入单行
来源：http://krr.jinghuilouyu.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://rwz.bbcook.cn

[Q11] 一次插入多行
来源：http://fja.sweek.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://yvb.zhoulong.xyz

[Q12] 插入后取自增 ID
来源：http://dkb.wangshuangyany.cn

INSERT INTO users (name) VALUES ('C');
来源：http://fdb.yanxiufei.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://vax.yangfankeji.com

[Q13] 忽略重复插入
来源：http://vcr.fengsongda.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://dih.yuanzhike.top

[Q14] 存在则更新（upsert）
来源：http://fzg.cucudq.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://nur.shanyushiyangkeji.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://fwu.ctjpmb.com

[Q15] 查询全部
来源：http://hlj.aizwys.cn

SELECT * FROM users;
来源：http://ibg.aibaodan.cn

[Q16] 查询指定列
来源：http://xnl.fengsongda.top

SELECT id, name FROM users;
来源：http://jab.epnwcf.com

[Q17] 条件查询
来源：http://lhz.hnxiangtu.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hxa.zhiwuduotai.top

[Q18] 模糊匹配
来源：http://igh.nwbrower.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mro.hfpthk.cn

[Q19] 范围查询
来源：http://kwg.hongshengwenyu.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://frm.ctjpmb.com

[Q20] IN 列表
来源：http://jdu.jianghu66.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ylu.zhongyouzk.top

[Q21] 空值判断
来源：http://vot.shanyushiyangkeji.top

SELECT * FROM users WHERE email IS NULL;
来源：http://jcx.shzxlz.cn

[Q22] 排序
来源：http://lwy.xylfe.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://jyw.jqgufenzy.top

[Q23] 分页
来源：http://gil.aizwys.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://zkb.haohaochexian.top

[Q24] 去重
来源：http://fxr.tianlin.xyz

SELECT DISTINCT city FROM users;
来源：http://soe.dashuyun.cn

[Q25] 只取前 N 条
来源：http://gzd.shzxlz.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://uny.fehbvm.com

[Q26] 计数
来源：http://xge.sjlbkw.cn

SELECT COUNT(*) FROM users;
来源：http://npv.nwbrower.top

[Q27] 条件计数
来源：http://nen.zhijiandao.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mya.zhaomingkeji.xyz

[Q28] 求和与平均
来源：http://qva.52xcode.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://evp.zycfv.cn

[Q29] 最大最小值
来源：http://gde.jinqigfzy.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://ugg.aizwys.cn

[Q30] 分组统计
来源：http://lgk.dianchejie.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ceq.yj20258.top

[Q31] 分组后过滤
来源：http://uab.52xcode.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://frd.ywan-chungtsiang.top

[Q32] 分组拼接字符串
来源：http://aox.yuanzhike.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://vfh.jinqigfzy.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://zws.hysaishi.cn

[Q33] 多列分组
来源：http://cln.cqqwz.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://gjj.cucudq.cn

[Q34] 每组取第一条
来源：http://gee.sjlbkw.cn

SELECT * FROM (
来源：http://ans.gzhubu.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://vbb.cqqwz.cn

) t WHERE rn = 1;
来源：http://ywt.yangfankeji.com

[Q35] 内连接
来源：http://ggc.jinyuanbaomall.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://fll.yfazqb.com

[Q36] 左连接
来源：http://qtx.xuanzx.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://dmj.pengpengdd.cyou

[Q37] 右连接
来源：http://wvo.jyoumei.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://lby.mhx1999.top

[Q38] 全外连接（PostgreSQL）
来源：http://bhl.shuidangran.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ink.yangfankeji.com

[Q39] 自连接（查上下级）
来源：http://bnc.316326.xyz

SELECT e.name, m.name AS manager FROM employees e
来源：http://tpq.zycfv.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ikn.hysaishi.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://zjx.jqgfzy.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://lca.yj20258888.top

[Q41] 多表连接
来源：http://ahl.sxryk.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://eel.sufxvd.cn

JOIN users u ON u.id = o.user_id
来源：http://ylf.hesvh.cn

JOIN products p ON p.id = o.product_id;
来源：http://ayd.zhixingplan.top

[Q42] 连接条件附加过滤
来源：http://bot.chenzaomai.com

SELECT u.name, o.amount FROM users u
来源：http://xzd.xuanzx.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://qln.hnqzz.top

[Q43] 标量子查询
来源：http://pao.316326.xyz

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://trl.cqqwz.cn

[Q44] IN 子查询
来源：http://enx.zhoulong.xyz

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://jzr.bjfxy.top

[Q45] EXISTS 判断存在
来源：http://izr.feifeiyinyue.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hyy.sufxvd.cn

[Q46] NOT EXISTS 判断不存在
来源：http://jun.yj202588.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fvx.c1oappe.top

[Q47] 与平均值比较
来源：http://pkc.sufxvd.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://jxn.hfpthk.cn

[Q48] CTE 公用表表达式
来源：http://mpa.guannengcc.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://waq.fzhhl.top

SELECT * FROM t WHERE c > 5;
来源：http://yut.hongshengwenyu.top

[Q49] 更新单行
来源：http://boo.ctjpmb.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://nxv.zhoulong.xyz

[Q50] 批量更新
来源：http://pev.epnwcf.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wsq.xinyue.icu

[Q51] 用子查询更新
来源：http://lrh.xinyue.icu

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://nsg.jinyuanbaomall.cn

[Q52] 删除指定行
来源：http://kmu.hywenlv.cn

DELETE FROM users WHERE id = 10;
来源：http://vva.jinghuilouyu.cn

[Q53] 按条件删除
来源：http://hvx.cucudq.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://pfl.smart0.xyz

[Q54] 清空表
来源：http://whn.chenlongwang.top

TRUNCATE TABLE logs;
来源：http://ezw.xylfe.cn

[Q55] 排名（并列占位）
来源：http://fqm.nanxinkj.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ybt.zhengqikj.top

[Q56] 密集排名（并列不占位）
来源：http://zkk.ppjwa.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mut.ehwqpu.com

[Q57] 行号
来源：http://vcp.cqqwz.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://vyi.chenjidiqi.icu

[Q58] 累计求和
来源：http://qdg.chenzaomai.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ypl.gotoacloud.top

[Q59] 分组内累计
来源：http://ccf.fengsongda.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://grx.jinghuilouyu.cn

[Q60] 取上一行 / 下一行
来源：http://gne.andypj.xyz

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ohi.bbcook.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://bkj.chenlongwang.top

[Q61] 移动平均
来源：http://rec.daxiang520.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://dxd.havefunace.top

[Q62] 分组占比
来源：http://fcg.jqgfzy.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://icu.hnxiangtu.top

[Q63] 开启事务
来源：http://wuo.andypj.xyz

START TRANSACTION;                -- 或 BEGIN
来源：http://ikp.tarul.cn

[Q64] 提交事务
来源：http://yvy.jinghuilouyu.cn

COMMIT;
来源：http://cir.hongshengwenyu.top

[Q65] 回滚事务
来源：http://gjb.fanxiaobao.xyz

ROLLBACK;
来源：http://yzz.cqqwz.cn

[Q66] 行锁查询
来源：http://xix.zhixingplan.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://axm.havefunace.top

[Q67] 设置隔离级别
来源：http://ozr.pengpengdd.cyou

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://fpp.gzhubu.top

[Q68] 保存点
来源：http://tpn.sjlbkw.cn

SAVEPOINT sp1;
来源：http://xgp.sweek.top

ROLLBACK TO sp1;
来源：http://hsg.tarul.cn

[Q69] 查看执行计划
来源：http://amn.yanxiufei.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wet.yonumen.top

[Q70] 更新统计信息
来源：http://miu.kuanghao11.cn

ANALYZE TABLE users;
来源：http://qqt.shanyushiyangkeji.top

[Q71] 查看建表语句
来源：http://qsa.zdqjudy.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://xru.zhiwuduotai.top

[Q72] 查看索引
来源：http://mch.ivvv.top

SHOW INDEX FROM users;
来源：http://xlh.jinqigufen.top

[Q73] 查看表状态
来源：http://xeu.zhijiandao.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://jbx.pycfn.com

[Q74] 强制使用索引
来源：http://ekz.yfazqb.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://arm.sweek.top

[Q75] 日期格式化
来源：http://clc.chenlongwang.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://swv.sufxvd.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://pfj.yuanzhike.top

[Q76] 按天统计
来源：http://qei.yuanzhike.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mgl.pycfn.com

[Q77] 时间加减
来源：http://vdz.hywenlv.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://eqo.ybcxt.top

[Q78] 当前时间
来源：http://jhd.hfpthk.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://yga.fengsongda.top

[Q79] 字符串拼接
来源：http://uxb.yj20258888.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://vvm.jinqigfzy.top

[Q80] 字符串截取
来源：http://plw.cucudq.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://vvp.andypj.xyz

[Q81] 字符串替换
来源：http://uyg.pengpengdd.cyou

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://zqn.sysykeji.top

[Q82] 字符长度与字节长度
来源：http://lkw.yonumen.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://tip.pycfn.com

[Q83] 大小写转换
来源：http://yar.nanxuanxn.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://art.zhijiandao.cn

[Q84] 去除首尾空格
来源：http://dwb.zhengqikj.top

SELECT TRIM(name) FROM users;
来源：http://gny.jyoumei.cn

[Q85] 数值取整
来源：http://shz.zhoulong.xyz

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://upf.mhx1999.top

[Q86] 读取 JSON 字段
来源：http://ytt.jyoumei.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ncr.9152youxi.cn

[Q87] JSON 字段做条件
来源：http://jeo.fehbvm.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://rag.fktsv.cn

[Q88] 行转列（条件聚合）
来源：http://dsm.epnwcf.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://qjw.ybcxt.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://tfb.gzhubu.top

[Q89] 判断表是否存在
来源：http://ddl.sufxvd.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://uhy.zycfv.cn

[Q90] 生成序号列
来源：http://svt.tianlin.xyz

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://zrj.cashguo.top

================================================================================
来源：http://gws.chenjidiqi.icu

R. Bash 专题
来源：http://jpt.gaohongyu789.top

================================================================================
来源：http://vou.nwbrower.top

[R01] shebang 与严格模式
来源：http://dae.yuanzhike.top

#!/usr/bin/env bash
来源：http://luk.ywan-chungtsiang.top

set -euo pipefail
来源：http://kpb.aizwys.cn

[R02] 变量赋值与使用
来源：http://lvx.cucudq.cn

name="Tom"; echo "$name"
来源：http://hez.cheryme.top

[R03] 只读变量
来源：http://oat.ivvv.top

readonly PI=3.14
来源：http://fjz.dianchejie.cn

[R04] 位置参数
来源：http://siq.feifeiyinyue.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://gbg.shuidangran.top

[R05] 参数默认值
来源：http://xgi.xinyue.icu

name="${1:-default}"
来源：http://ibt.shzxlz.cn

[R06] 判断命令是否存在
来源：http://rlo.yj202588.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://sby.jinghuilouyu.cn

[R07] if 判断文件
来源：http://hrt.xingfuxueyuan.xyz

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://tvb.jlsjyb.cn

[R08] 数值比较
来源：http://wcr.yangfankeji.com

if (( a > b )); then echo "a 更大"; fi
来源：http://fpv.chenjidiqi.icu

[R09] 字符串比较
来源：http://tuz.aibaodan.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://lik.shzxlz.cn

[R10] 正则匹配
来源：http://abw.ctjpmb.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://btm.fengsongda.top

[R11] case 多分支
来源：http://yco.zhixingplan.top

case "$1" in
来源：http://hqo.xylfe.cn

start) echo "启动" ;;
来源：http://yoj.birdmap.top

stop)  echo "停止" ;;
来源：http://adl.chenzaomai.com

*)     echo "未知命令" ;;
来源：http://qol.gogol.net.cn

esac
来源：http://kcs.ydjk.org.cn

[R12] for 遍历文件
来源：http://amb.hesvh.cn

for f in *.txt; do echo "$f"; done
来源：http://rwo.ppjwa.cn

[R13] for 计数循环
来源：http://hli.jyoumei.cn

for i in {1..10}; do echo "$i"; done
来源：http://wsp.chenlongwang.top

[R14] C 风格 for
来源：http://azm.fanxiaobao.xyz

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://txg.vqdsnc.cn

[R15] while 逐行读文件
来源：http://jfa.ctjpmb.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://enf.hesvh.cn

[R16] until 等待条件
来源：http://aml.yangfankeji.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://jau.ybcxt.top

[R17] 数组定义与取值
来源：http://omk.ydzc1.top

arr=(a b c); echo "${arr[0]}"
来源：http://djk.chenlongwang.top

[R18] 遍历数组
来源：http://vas.xuetiantiany.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://afd.sxryk.cn

[R19] 数组长度
来源：http://qxy.ctjpmb.com

echo "${#arr[@]}"
来源：http://ofs.xuetiantiany.cn

[R20] 关联数组（字典）
来源：http://qig.yongpay.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://xop.uphjek.com

[R21] 字符串长度
来源：http://uax.birdmap.top

echo "${#s}"
来源：http://egk.feifeiyinyue.top

[R22] 截取子串
来源：http://wzf.daria6918.cn

echo "${s:0:5}"
来源：http://xlx.xziqi.cn

[R23] 字符串替换
来源：http://dsj.redwolf501.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://qfr.zhoulong.xyz

[R24] 大小写转换
来源：http://vee.cashguo.top

echo "${s^^}"; echo "${s,,}"
来源：http://cuc.jqgfzy.top

[R25] 去后缀 / 去前缀
来源：http://xkk.yanxiufei.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://xpl.ctjpmb.com

[R26] 命令替换
来源：http://hkt.gaohongyu789.top

now=$(date +%F); echo "$now"
来源：http://ssk.chenlongwang.top

[R27] 算术展开
来源：http://bcb.jqgfzy.top

echo $((1 + 2 * 3))
来源：http://ahw.vqdsnc.cn

[R28] 浮点运算
来源：http://znl.zhixingplan.top

echo "scale=2; 10/3" | bc
来源：http://uyn.xylfe.cn

[R29] 定义函数
来源：http://zeq.sysykeji.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ufu.chenlongwang.top

[R30] 函数返回状态码
来源：http://jgy.yvedp.cn

f() { return 0; }; f || echo "失败了"
来源：http://evd.pengpengdd.cyou

[R31] 局部变量
来源：http://xkc.guowangkeji.top

f() { local x=1; echo "$x"; }
来源：http://ibw.nanxuanxn.top

[R32] 参数个数校验
来源：http://jrr.hongshengwenyu.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://qhu.daxiang520.top

[R33] 捕获错误并提示行号
来源：http://ady.aizwys.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ijf.cqqwz.cn

[R34] 退出时清理
来源：http://abx.zdbjq.cn

trap 'rm -f "$tmp"' EXIT
来源：http://pia.xziqi.cn

[R35] 后台执行并等待
来源：http://xxg.hnqzz.top

sleep 5 & pid=$!; wait "$pid"
来源：http://ujx.hesvh.cn

[R36] 并发执行多个任务
来源：http://wny.wangshuangyany.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://zde.quarkkingdee.top

[R37] 把输出赋给变量
来源：http://lsl.cheryme.top

files=$(ls -1)
来源：http://fnc.tanke756.top

[R38] 管道串联
来源：http://qad.tarul.cn

cat a.txt | grep -i error | wc -l
来源：http://ecj.sjlbkw.cn

[R39] 重定向标准输出与错误
来源：http://xiz.nanxuanxn.top

cmd > out.log 2>&1
来源：http://jay.sweek.top

[R40] 追加写日志
来源：http://did.cheryme.top

echo "log" >> out.log
来源：http://izu.hongshengwenyu.top

[R41] 丢弃输出
来源：http://bjt.nanxuanxn.top

cmd >/dev/null 2>&1
来源：http://sgg.snrcjt.cn

[R42] 输入重定向
来源：http://mzb.nwbrower.top

wc -l < a.txt
来源：http://gis.hcnkem.com

[R43] 按名字查找文件
来源：http://udm.kuanghao11.cn

find . -name "*.log" -type f
来源：http://hhq.svipenyu.cn

[R44] 按修改时间查找
来源：http://rfp.birdmap.top

find . -mtime -7 -type f
来源：http://pjj.fehbvm.com

[R45] 批量删除
来源：http://dfu.yanxiufei.cn

find . -name "*.tmp" -delete
来源：http://mog.0kj1m.cn

[R46] 递归替换文件内容
来源：http://rok.birdmap.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hyj.hnqzz.top

[R47] sed 单行替换
来源：http://cey.jinqigufen.top

sed -i 's/foo/bar/g' a.txt
来源：http://iup.hywenlv.cn

[R48] awk 取指定列
来源：http://jrf.yonumen.top

awk '{print $1, $3}' a.txt
来源：http://oze.pengpengdd.cyou

[R49] awk 带条件
来源：http://hsp.shzxlz.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://bil.hesvh.cn

[R50] awk 求和
来源：http://jzo.sysykeji.top

awk '{s += $2} END {print s}' a.txt
来源：http://wqt.hammf.cn

[R51] 排序去重取前几
来源：http://ili.sxryk.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://twu.epnwcf.com

[R52] 统计行数
来源：http://hxy.ydjk.org.cn

wc -l a.txt
来源：http://bmp.zhiwuduotai.top

[R53] 查看文件头与实时尾
来源：http://ytu.hysaishi.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ixq.zycfv.cn

[R54] 比较两个文件
来源：http://xst.yuanzhike.top

diff a.txt b.txt
来源：http://red.nanxinkj.top

[R55] 压缩与解压
来源：http://bxw.nanxinkj.top


<!-- 参考信息 -->