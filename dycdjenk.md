代发 wailian999

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://lkp.fzhhl.top

[Q05] 重命名列
来源：http://jzq.hnqzz.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wgc.smart0.xyz

[Q06] 删除列
来源：http://lez.aibaodan.cn

ALTER TABLE users DROP COLUMN age;
来源：http://pzt.yfazqb.com

[Q07] 删除表
来源：http://hnv.cdnleiting.top

DROP TABLE IF EXISTS orders;
来源：http://mvb.chenlongwang.top

[Q08] 创建普通索引
来源：http://uwz.ivvv.top

CREATE INDEX idx_users_email ON users(email);
来源：http://ttt.xingfuxueyuan.xyz

[Q09] 创建唯一索引
来源：http://uxb.jinyuanbaomall.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://vqb.zdqjudy.top

[Q10] 插入单行
来源：http://fuv.hcnkem.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hgv.fzhhl.top

[Q11] 一次插入多行
来源：http://qcx.gaohongyu789.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mbt.yonumen.top

[Q12] 插入后取自增 ID
来源：http://qzi.hywenlv.cn

INSERT INTO users (name) VALUES ('C');
来源：http://vrd.nanxuanxn.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ytq.uphjek.com

[Q13] 忽略重复插入
来源：http://eir.9152youxi.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hmm.jinqigufen.top

[Q14] 存在则更新（upsert）
来源：http://lhe.bjfxy.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://her.yvedp.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://xqi.chenjidiqi.icu

[Q15] 查询全部
来源：http://tpi.ctjpmb.com

SELECT * FROM users;
来源：http://aat.meibo888.top

[Q16] 查询指定列
来源：http://pqj.hnqzz.top

SELECT id, name FROM users;
来源：http://ych.andypj.xyz

[Q17] 条件查询
来源：http://keg.zdbjq.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://xqx.yonumen.top

[Q18] 模糊匹配
来源：http://wbo.yuxming.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ksb.hfpthk.cn

[Q19] 范围查询
来源：http://ceb.jlsjyb.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://aqz.gaohongyu789.top

[Q20] IN 列表
来源：http://wxa.uphjek.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://vvq.feifeiyinyue.top

[Q21] 空值判断
来源：http://emv.wangshuangyany.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://gsn.iojbl.cn

[Q22] 排序
来源：http://bps.chenjidiqi.icu

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://oup.jinghuilouyu.cn

[Q23] 分页
来源：http://jph.bjfxy.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://gmc.sjlbkw.cn

[Q24] 去重
来源：http://idd.xingfuxueyuan.xyz

SELECT DISTINCT city FROM users;
来源：http://cqh.xinyue.icu

[Q25] 只取前 N 条
来源：http://nle.chenjidiqi.icu

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wun.c1oappe.top

[Q26] 计数
来源：http://wfk.andypj.xyz

SELECT COUNT(*) FROM users;
来源：http://jmt.hcnkem.com

[Q27] 条件计数
来源：http://icj.yonumen.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://jmo.xuanzx.com

[Q28] 求和与平均
来源：http://hrj.guowangkeji.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://osg.hnqzz.top

[Q29] 最大最小值
来源：http://yok.sweek.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://xam.yj202588.top

[Q30] 分组统计
来源：http://odt.wangdashe.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://lvi.havefunace.top

[Q31] 分组后过滤
来源：http://dwn.chenlongwang.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://rkm.zdqjudy.top

[Q32] 分组拼接字符串
来源：http://pni.ivvv.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://eti.chenlongwang.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://npl.daxiang520.top

[Q33] 多列分组
来源：http://kov.9152youxi.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://spm.gotoacloud.top

[Q34] 每组取第一条
来源：http://ovx.dianchejie.cn

SELECT * FROM (
来源：http://wbt.tian-w.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://rzt.9152youxi.cn

) t WHERE rn = 1;
来源：http://cee.cdnleiting.top

[Q35] 内连接
来源：http://kxp.yj20258888.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://cer.ydjk.org.cn

[Q36] 左连接
来源：http://tup.ivvv.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mje.andypj.xyz

[Q37] 右连接
来源：http://exl.pengpengdd.cyou

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://zuf.zdbjq.cn

[Q38] 全外连接（PostgreSQL）
来源：http://qti.xingfuxueyuan.xyz

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://aiy.havefunace.top

[Q39] 自连接（查上下级）
来源：http://hbp.havefunace.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://kou.dianchejie.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ufa.ydzc1.top

[Q40] 交叉连接（笛卡尔积）
来源：http://qte.xuetiantiany.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://smf.xinyue.icu

[Q41] 多表连接
来源：http://mqu.zhixingplan.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://pro.ppjwa.cn

JOIN users u ON u.id = o.user_id
来源：http://qhw.yvedp.cn

JOIN products p ON p.id = o.product_id;
来源：http://wdb.ctjpmb.com

[Q42] 连接条件附加过滤
来源：http://zjo.52xcode.cn

SELECT u.name, o.amount FROM users u
来源：http://cmx.xinyue.icu

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://fnx.hnxiangtu.top

[Q43] 标量子查询
来源：http://xit.smart0.xyz

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://tqe.xuetiantiany.cn

[Q44] IN 子查询
来源：http://whk.ybcxt.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://uvx.jianghu66.top

[Q45] EXISTS 判断存在
来源：http://ork.fehbvm.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ktx.epnwcf.com

[Q46] NOT EXISTS 判断不存在
来源：http://azr.fzhhl.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xes.svipenyu.cn

[Q47] 与平均值比较
来源：http://irr.jiagoushi.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://nov.ppjwa.cn

[Q48] CTE 公用表表达式
来源：http://ckl.fehbvm.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://sfo.ppjwa.cn

SELECT * FROM t WHERE c > 5;
来源：http://ytl.zhixingplan.top

[Q49] 更新单行
来源：http://rst.yvedp.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wlr.gzhubu.top

[Q50] 批量更新
来源：http://jdc.zhijiandao.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://xfn.shuidangran.top

[Q51] 用子查询更新
来源：http://ftm.birdmap.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://njt.guannengcc.top

[Q52] 删除指定行
来源：http://otg.sysykeji.top

DELETE FROM users WHERE id = 10;
来源：http://zbv.zhongyouzk.top

[Q53] 按条件删除
来源：http://eyf.ehwqpu.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://swc.nwbrower.top

[Q54] 清空表
来源：http://bqg.xuanzx.com

TRUNCATE TABLE logs;
来源：http://zni.xuetiantiany.cn

[Q55] 排名（并列占位）
来源：http://gbp.zdbjq.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wdb.iojbl.cn

[Q56] 密集排名（并列不占位）
来源：http://sbl.zhixingplan.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hyk.aibaodan.cn

[Q57] 行号
来源：http://cze.hesvh.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ecd.c1oappe.top

[Q58] 累计求和
来源：http://iot.hysaishi.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wzt.yj202588.top

[Q59] 分组内累计
来源：http://jww.daria6918.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://uze.aizwys.cn

[Q60] 取上一行 / 下一行
来源：http://foo.pycfn.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://vzx.redwolf501.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mpe.zdqjudy.top

[Q61] 移动平均
来源：http://fab.cucudq.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ago.iojbl.cn

[Q62] 分组占比
来源：http://ppc.tianlin.xyz

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://vxj.vehdjk.com

[Q63] 开启事务
来源：http://pxd.yongpay.top

START TRANSACTION;                -- 或 BEGIN
来源：http://xgd.svipenyu.cn

[Q64] 提交事务
来源：http://gqb.fengsongda.top

COMMIT;
来源：http://uld.zhaomingkeji.xyz

[Q65] 回滚事务
来源：http://oru.ctjpmb.com

ROLLBACK;
来源：http://rvh.xinyue.icu

[Q66] 行锁查询
来源：http://fit.316326.xyz

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mfd.fehbvm.com

[Q67] 设置隔离级别
来源：http://djg.zhengqikj.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://xtm.birdmap.top

[Q68] 保存点
来源：http://hjy.yanxiufei.cn

SAVEPOINT sp1;
来源：http://erk.zhixingplan.top

ROLLBACK TO sp1;
来源：http://gpa.jinqigufen.top

[Q69] 查看执行计划
来源：http://kmx.ivvv.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://yzb.zdbjq.cn

[Q70] 更新统计信息
来源：http://cem.wangshuangyany.cn

ANALYZE TABLE users;
来源：http://jsf.zhixingplan.top

[Q71] 查看建表语句
来源：http://irw.andypj.xyz

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://imn.zdqjudy.top

[Q72] 查看索引
来源：http://uph.9152youxi.cn

SHOW INDEX FROM users;
来源：http://kiw.xuanzx.com

[Q73] 查看表状态
来源：http://iyo.smart0.xyz

SHOW TABLE STATUS LIKE 'users';
来源：http://cxi.snrcjt.cn

[Q74] 强制使用索引
来源：http://zcf.ehwqpu.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://urq.fehbvm.com

[Q75] 日期格式化
来源：http://ger.tarul.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://trw.yueranfly.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://gaf.xingfuxueyuan.xyz

[Q76] 按天统计
来源：http://wxf.9152youxi.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://xyb.xylfe.cn

[Q77] 时间加减
来源：http://srh.cqqwz.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hmo.yj202588.top

[Q78] 当前时间
来源：http://txh.meibo888.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://oao.cdnleiting.top

[Q79] 字符串拼接
来源：http://prn.epnwcf.com

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ryv.zdbjq.cn

[Q80] 字符串截取
来源：http://glf.nwbrower.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://pfq.feifeiyinyue.top

[Q81] 字符串替换
来源：http://ukm.jyoumei.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://xya.0kj1m.cn

[Q82] 字符长度与字节长度
来源：http://axm.zhengqikj.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://bxk.316326.xyz

[Q83] 大小写转换
来源：http://mnl.yfazqb.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://eox.wangshuangyany.cn

[Q84] 去除首尾空格
来源：http://qnj.guowangkeji.top

SELECT TRIM(name) FROM users;
来源：http://gky.jinqigufen.top

[Q85] 数值取整
来源：http://ujc.yj20258.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://qgk.cqqwz.cn

[Q86] 读取 JSON 字段
来源：http://jim.jinghuilouyu.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://iud.ppjwa.cn

[Q87] JSON 字段做条件
来源：http://mrj.cqqwz.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://pzv.jqgufenzy.top

[Q88] 行转列（条件聚合）
来源：http://jjw.zhongyouzk.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://csw.vqdsnc.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ryk.quarkkingdee.top

[Q89] 判断表是否存在
来源：http://qdq.snrcjt.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://oeg.ehwqpu.com

[Q90] 生成序号列
来源：http://zrn.cashguo.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://zwh.shuidangran.top

================================================================================
来源：http://miy.quarkkingdee.top

R. Bash 专题
来源：http://ymm.sweek.top

================================================================================
来源：http://lmp.0kj1m.cn

[R01] shebang 与严格模式
来源：http://luz.shuidangran.top

#!/usr/bin/env bash
来源：http://dxs.cashguo.top

set -euo pipefail
来源：http://hys.yuxming.cn

[R02] 变量赋值与使用
来源：http://oyf.gotoacloud.top

name="Tom"; echo "$name"
来源：http://cnv.yangfankeji.com

[R03] 只读变量
来源：http://rgv.xuanzx.com

readonly PI=3.14
来源：http://pmh.svipenyu.cn

[R04] 位置参数
来源：http://tki.svipenyu.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://njd.pengpengdd.cyou

[R05] 参数默认值
来源：http://mwz.yuanzhike.top

name="${1:-default}"
来源：http://nlp.fzhhl.top

[R06] 判断命令是否存在
来源：http://ojg.gzhubu.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://opg.smart0.xyz

[R07] if 判断文件
来源：http://tln.jinyuanbaomall.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://qrs.zhixingplan.top

[R08] 数值比较
来源：http://pin.aibaodan.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://mvr.zycfv.cn

[R09] 字符串比较
来源：http://ish.uphjek.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://pqy.cashguo.top

[R10] 正则匹配
来源：http://xcr.52xcode.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://gaz.9152youxi.cn

[R11] case 多分支
来源：http://hpd.cheryme.top

case "$1" in
来源：http://eel.jqgufenzy.top

start) echo "启动" ;;
来源：http://ray.jyoumei.cn

stop)  echo "停止" ;;
来源：http://vyt.yangfankeji.com

*)     echo "未知命令" ;;
来源：http://vle.zhongyouzk.top

esac
来源：http://ztu.ivvv.top

[R12] for 遍历文件
来源：http://ovm.sweek.top

for f in *.txt; do echo "$f"; done
来源：http://oxq.gogol.net.cn

[R13] for 计数循环
来源：http://djl.daria6918.cn

for i in {1..10}; do echo "$i"; done
来源：http://pad.cashguo.top

[R14] C 风格 for
来源：http://vze.gotoacloud.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://zcf.ppjwa.cn

[R15] while 逐行读文件
来源：http://zto.yonumen.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://erq.havefunace.top

[R16] until 等待条件
来源：http://mkg.jiagoushi.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://iwr.chenzaomai.com

[R17] 数组定义与取值
来源：http://oif.zhengqikj.top

arr=(a b c); echo "${arr[0]}"
来源：http://ixp.feifeiyinyue.top

[R18] 遍历数组
来源：http://bjl.chenjidiqi.icu

for x in "${arr[@]}"; do echo "$x"; done
来源：http://vai.chenjidiqi.icu

[R19] 数组长度
来源：http://kfs.0kj1m.cn

echo "${#arr[@]}"
来源：http://iuw.zhijiandao.cn

[R20] 关联数组（字典）
来源：http://gpw.zhongyouzk.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://zgz.52xcode.cn

[R21] 字符串长度
来源：http://cyr.zdqjudy.top

echo "${#s}"
来源：http://nwv.ydzc1.top

[R22] 截取子串
来源：http://eto.ppjwa.cn

echo "${s:0:5}"
来源：http://iqu.jinghuilouyu.cn

[R23] 字符串替换
来源：http://wdc.dashuyun.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://zwu.guowangkeji.top

[R24] 大小写转换
来源：http://yyf.52xcode.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ulr.chenzaomai.com

[R25] 去后缀 / 去前缀
来源：http://lwn.gotoacloud.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://ufn.hnxiangtu.top

[R26] 命令替换
来源：http://mst.sweek.top

now=$(date +%F); echo "$now"
来源：http://ovq.xinyue.icu

[R27] 算术展开
来源：http://ams.redwolf501.top

echo $((1 + 2 * 3))
来源：http://etf.nwbrower.top

[R28] 浮点运算
来源：http://qgg.zhixingplan.top

echo "scale=2; 10/3" | bc
来源：http://yna.xingfuxueyuan.xyz

[R29] 定义函数
来源：http://hhv.shanyushiyangtech.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://qob.chenlongwang.top

[R30] 函数返回状态码
来源：http://sxb.xziqi.cn

f() { return 0; }; f || echo "失败了"
来源：http://fbt.chenlongwang.top

[R31] 局部变量
来源：http://lgb.xziqi.cn

f() { local x=1; echo "$x"; }
来源：http://jgx.jiagoushi.top

[R32] 参数个数校验
来源：http://jyp.zhiwuduotai.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://umv.shzxlz.cn

[R33] 捕获错误并提示行号
来源：http://seo.zhaomingkeji.xyz

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://jiv.pengpengdd.cyou

[R34] 退出时清理
来源：http://lsh.yuanzhike.top

trap 'rm -f "$tmp"' EXIT
来源：http://ymm.yueranfly.top

[R35] 后台执行并等待
来源：http://xpd.kuanghao11.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://yub.fehbvm.com

[R36] 并发执行多个任务
来源：http://jyn.cdnleiting.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://knz.shzxlz.cn

[R37] 把输出赋给变量
来源：http://mdg.c1oappe.top

files=$(ls -1)
来源：http://ygt.hywenlv.cn

[R38] 管道串联
来源：http://qug.daria6918.cn

cat a.txt | grep -i error | wc -l
来源：http://pdo.yj202588.top

[R39] 重定向标准输出与错误
来源：http://ufo.daria6918.cn

cmd > out.log 2>&1
来源：http://cpg.mhx1999.top

[R40] 追加写日志
来源：http://har.ybcxt.top

echo "log" >> out.log
来源：http://ebu.yangfankeji.com

[R41] 丢弃输出
来源：http://uze.yonumen.top

cmd >/dev/null 2>&1
来源：http://lwz.sxryk.cn

[R42] 输入重定向
来源：http://ael.jinghuilouyu.cn

wc -l < a.txt
来源：http://yvh.uphjek.com

[R43] 按名字查找文件
来源：http://jlf.pengpengdd.cyou

find . -name "*.log" -type f
来源：http://jgb.shuidangran.top

[R44] 按修改时间查找
来源：http://wvb.ehwqpu.com

find . -mtime -7 -type f
来源：http://wdp.ehwqpu.com

[R45] 批量删除
来源：http://mtv.nanxinkj.top

find . -name "*.tmp" -delete
来源：http://sxj.feifeiyinyue.top

[R46] 递归替换文件内容
来源：http://ghj.c1oappe.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://aku.sufxvd.cn

[R47] sed 单行替换
来源：http://qzz.xinyue.icu

sed -i 's/foo/bar/g' a.txt
来源：http://fxz.xziqi.cn

[R48] awk 取指定列
来源：http://dcv.jinqigfzy.top

awk '{print $1, $3}' a.txt
来源：http://txj.ywan-chungtsiang.top

[R49] awk 带条件
来源：http://izk.epnwcf.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://pgx.aizwys.cn

[R50] awk 求和
来源：http://gwd.zhiwuduotai.top

awk '{s += $2} END {print s}' a.txt
来源：http://kvo.yj20258.top

[R51] 排序去重取前几
来源：http://mag.fanxiaobao.xyz

sort a.txt | uniq -c | sort -rn | head
来源：http://uzm.tianlin.xyz

[R52] 统计行数
来源：http://sxp.aizwys.cn

wc -l a.txt
来源：http://oog.yanxiufei.cn

[R53] 查看文件头与实时尾
来源：http://kxa.sweek.top


<!-- 参考信息 -->