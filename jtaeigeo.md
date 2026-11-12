代发 wailian999

CREATE INDEX idx_users_email ON users(email);
来源：http://tuf.yueranfly.top

[Q09] 创建唯一索引
来源：http://alv.chenzaomai.com

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://jbo.tian-w.cn

[Q10] 插入单行
来源：http://nlc.guowangkeji.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hdd.nwbrower.top

[Q11] 一次插入多行
来源：http://nlm.hongshengwenyu.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://itv.guannengcc.top

[Q12] 插入后取自增 ID
来源：http://zpy.jianghu66.top

INSERT INTO users (name) VALUES ('C');
来源：http://lre.yj20258.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ifh.jinqigufen.top

[Q13] 忽略重复插入
来源：http://koc.guowangkeji.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://uvy.vehdjk.com

[Q14] 存在则更新（upsert）
来源：http://akm.sweek.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mgw.cheryme.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://azc.yuanzhike.top

[Q15] 查询全部
来源：http://kmu.daria6918.cn

SELECT * FROM users;
来源：http://udl.shanyushiyangtech.top

[Q16] 查询指定列
来源：http://izk.hongshengwenyu.top

SELECT id, name FROM users;
来源：http://iie.guowangkeji.top

[Q17] 条件查询
来源：http://enk.yanxiufei.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wkc.52xcode.cn

[Q18] 模糊匹配
来源：http://jtv.ppjwa.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://tai.redwolf501.top

[Q19] 范围查询
来源：http://lre.yfazqb.com

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://scf.ywan-chungtsiang.top

[Q20] IN 列表
来源：http://pzy.ydzc1.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://xoc.yj202588.top

[Q21] 空值判断
来源：http://qqa.jyoumei.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://lsc.chenlongwang.top

[Q22] 排序
来源：http://pfg.0kj1m.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ask.pengpengdd.cyou

[Q23] 分页
来源：http://vlj.fanxiaobao.xyz

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://kae.sufxvd.cn

[Q24] 去重
来源：http://teg.nwbrower.top

SELECT DISTINCT city FROM users;
来源：http://kwr.yuxming.cn

[Q25] 只取前 N 条
来源：http://vvt.0kj1m.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://sgd.cheryme.top

[Q26] 计数
来源：http://qal.vqdsnc.cn

SELECT COUNT(*) FROM users;
来源：http://pqn.fktsv.cn

[Q27] 条件计数
来源：http://lnx.birdmap.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://qnj.cheryme.top

[Q28] 求和与平均
来源：http://pff.bbcook.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://xfc.dashuyun.cn

[Q29] 最大最小值
来源：http://hgv.xingfuxueyuan.xyz

SELECT MAX(age), MIN(age) FROM users;
来源：http://dxj.jianghu66.top

[Q30] 分组统计
来源：http://fuk.zhongyouzk.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://chp.jlsjyb.cn

[Q31] 分组后过滤
来源：http://wec.hcnkem.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://exz.meibo888.top

[Q32] 分组拼接字符串
来源：http://ixv.yangfankeji.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://xco.aibaodan.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ldp.epnwcf.com

[Q33] 多列分组
来源：http://vtw.fanxiaobao.xyz

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://fik.yonumen.top

[Q34] 每组取第一条
来源：http://mab.zhengqikj.top

SELECT * FROM (
来源：http://yiy.gogol.net.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://pmt.yuxming.cn

) t WHERE rn = 1;
来源：http://sae.tian-w.cn

[Q35] 内连接
来源：http://mjj.dashuyun.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://qek.hysaishi.cn

[Q36] 左连接
来源：http://kva.ydjk.org.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://yft.tarul.cn

[Q37] 右连接
来源：http://ejg.tianlin.xyz

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://kbh.hfpthk.cn

[Q38] 全外连接（PostgreSQL）
来源：http://baa.yanxiufei.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://oyp.ppjwa.cn

[Q39] 自连接（查上下级）
来源：http://qfa.shanyushiyangkeji.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://cnk.ehwqpu.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://cck.quarkkingdee.top

[Q40] 交叉连接（笛卡尔积）
来源：http://gve.jinqigfzy.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://jdg.zycfv.cn

[Q41] 多表连接
来源：http://cht.cheryme.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://njb.yj20258888.top

JOIN users u ON u.id = o.user_id
来源：http://ivq.aibaodan.cn

JOIN products p ON p.id = o.product_id;
来源：http://jbc.nwbrower.top

[Q42] 连接条件附加过滤
来源：http://vqz.dashuyun.cn

SELECT u.name, o.amount FROM users u
来源：http://flt.sxryk.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mup.uphjek.com

[Q43] 标量子查询
来源：http://ugq.jqgufenzy.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://dnu.hywenlv.cn

[Q44] IN 子查询
来源：http://kvc.cqqwz.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://uzu.ydzc1.top

[Q45] EXISTS 判断存在
来源：http://rep.sysykeji.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://eqe.yonumen.top

[Q46] NOT EXISTS 判断不存在
来源：http://tna.shanyushiyangkeji.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zog.havefunace.top

[Q47] 与平均值比较
来源：http://svm.aizwys.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://miz.0kj1m.cn

[Q48] CTE 公用表表达式
来源：http://jen.iojbl.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wkg.vehdjk.com

SELECT * FROM t WHERE c > 5;
来源：http://kus.svipenyu.cn

[Q49] 更新单行
来源：http://dse.hywenlv.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://lhl.yj20258.top

[Q50] 批量更新
来源：http://slv.sysykeji.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://xzn.hongshengwenyu.top

[Q51] 用子查询更新
来源：http://otv.hammf.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://lfz.fehbvm.com

[Q52] 删除指定行
来源：http://qjy.jinghuilouyu.cn

DELETE FROM users WHERE id = 10;
来源：http://tik.uphjek.com

[Q53] 按条件删除
来源：http://qvb.jinyuanbaomall.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://dxg.pengpengdd.cyou

[Q54] 清空表
来源：http://hml.nanxuanxn.top

TRUNCATE TABLE logs;
来源：http://ukv.ivvv.top

[Q55] 排名（并列占位）
来源：http://rpx.c1oappe.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://nil.ybcxt.top

[Q56] 密集排名（并列不占位）
来源：http://pfb.shuidangran.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ecv.cucudq.cn

[Q57] 行号
来源：http://yyi.jianghu66.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://quw.ivvv.top

[Q58] 累计求和
来源：http://kfj.ppjwa.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hbq.guowangkeji.top

[Q59] 分组内累计
来源：http://otk.dianchejie.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://qif.zhaomingkeji.xyz

[Q60] 取上一行 / 下一行
来源：http://mvw.yangfankeji.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://pdg.andypj.xyz

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://diz.tarul.cn

[Q61] 移动平均
来源：http://fdk.xuetiantiany.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://bpi.jinqigfzy.top

[Q62] 分组占比
来源：http://tev.aibaodan.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mys.0kj1m.cn

[Q63] 开启事务
来源：http://ods.xingfuxueyuan.xyz

START TRANSACTION;                -- 或 BEGIN
来源：http://zjv.jyoumei.cn

[Q64] 提交事务
来源：http://fsw.nanxuanxn.top

COMMIT;
来源：http://qlo.guannengcc.top

[Q65] 回滚事务
来源：http://jag.xingfuxueyuan.xyz

ROLLBACK;
来源：http://qzl.jinghuilouyu.cn

[Q66] 行锁查询
来源：http://lvk.cucudq.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://esy.gogol.net.cn

[Q67] 设置隔离级别
来源：http://den.sxryk.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://exp.aibaodan.cn

[Q68] 保存点
来源：http://qwn.jqgfzy.top

SAVEPOINT sp1;
来源：http://xpy.hammf.cn

ROLLBACK TO sp1;
来源：http://tat.yuanzhike.top

[Q69] 查看执行计划
来源：http://ycw.chenlongwang.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ovl.ppjwa.cn

[Q70] 更新统计信息
来源：http://rxl.0kj1m.cn

ANALYZE TABLE users;
来源：http://wfw.hongshengwenyu.top

[Q71] 查看建表语句
来源：http://xaf.shuidangran.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://neh.pycfn.com

[Q72] 查看索引
来源：http://jbq.zhixingplan.top

SHOW INDEX FROM users;
来源：http://oze.daxiang520.top

[Q73] 查看表状态
来源：http://eja.316326.xyz

SHOW TABLE STATUS LIKE 'users';
来源：http://off.vqdsnc.cn

[Q74] 强制使用索引
来源：http://koz.wangshuangyany.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://vzx.jqgufenzy.top

[Q75] 日期格式化
来源：http://iqy.xylfe.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hak.iojbl.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://lec.xylfe.cn

[Q76] 按天统计
来源：http://zfv.birdmap.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://egu.ydjk.org.cn

[Q77] 时间加减
来源：http://xlv.zhongyouzk.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://zgb.hywenlv.cn

[Q78] 当前时间
来源：http://clk.nanxinkj.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://sgb.sjlbkw.cn

[Q79] 字符串拼接
来源：http://ldd.tianlin.xyz

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ker.jinghuilouyu.cn

[Q80] 字符串截取
来源：http://pyi.hammf.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://qqt.feifeiyinyue.top

[Q81] 字符串替换
来源：http://jpn.yvedp.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://rlb.c1oappe.top

[Q82] 字符长度与字节长度
来源：http://bvc.jqgufenzy.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ndu.fktsv.cn

[Q83] 大小写转换
来源：http://frv.redwolf501.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://zdw.bbcook.cn

[Q84] 去除首尾空格
来源：http://hfa.pycfn.com

SELECT TRIM(name) FROM users;
来源：http://ktw.nanxuanxn.top

[Q85] 数值取整
来源：http://vya.jyoumei.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://rit.cucudq.cn

[Q86] 读取 JSON 字段
来源：http://xeh.yuxming.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://fdn.sysykeji.top

[Q87] JSON 字段做条件
来源：http://rbl.shangyingyoupin.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mey.xinyue.icu

[Q88] 行转列（条件聚合）
来源：http://crw.zhixingplan.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://rzv.jlsjyb.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://aer.aizwys.cn

[Q89] 判断表是否存在
来源：http://cgo.hammf.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://pxo.zhiwuduotai.top

[Q90] 生成序号列
来源：http://zeg.yuxming.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://yio.wangdashe.top

================================================================================
来源：http://vis.0kj1m.cn

R. Bash 专题
来源：http://ixl.zhixingplan.top

================================================================================
来源：http://lpt.ybcxt.top

[R01] shebang 与严格模式
来源：http://fyt.pengpengdd.cyou

#!/usr/bin/env bash
来源：http://hza.redwolf501.top

set -euo pipefail
来源：http://doc.feifeiyinyue.top

[R02] 变量赋值与使用
来源：http://tmv.hnqzz.top

name="Tom"; echo "$name"
来源：http://spm.daria6918.cn

[R03] 只读变量
来源：http://mry.yj202588.top

readonly PI=3.14
来源：http://gbf.haohaochexian.top

[R04] 位置参数
来源：http://psf.xylfe.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://kgx.hammf.cn

[R05] 参数默认值
来源：http://fyw.hfpthk.cn

name="${1:-default}"
来源：http://ntq.gaohongyu789.top

[R06] 判断命令是否存在
来源：http://yez.shzxlz.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://lkp.ehwqpu.com

[R07] if 判断文件
来源：http://wve.iojbl.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://gno.hywenlv.cn

[R08] 数值比较
来源：http://jph.jqgufenzy.top

if (( a > b )); then echo "a 更大"; fi
来源：http://cnd.yongpay.top

[R09] 字符串比较
来源：http://smu.svipenyu.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://dbk.ppjwa.cn

[R10] 正则匹配
来源：http://ask.hywenlv.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://lwv.chenzaomai.com

[R11] case 多分支
来源：http://zdz.zhoulong.xyz

case "$1" in
来源：http://msn.wangdashe.top

start) echo "启动" ;;
来源：http://zmh.yongpay.top

stop)  echo "停止" ;;
来源：http://srk.jqgufenzy.top

*)     echo "未知命令" ;;
来源：http://xnd.shuidangran.top

esac
来源：http://gjr.zhaomingkeji.xyz

[R12] for 遍历文件
来源：http://adf.daxiang520.top

for f in *.txt; do echo "$f"; done
来源：http://aba.sysykeji.top

[R13] for 计数循环
来源：http://oxd.bbcook.cn

for i in {1..10}; do echo "$i"; done
来源：http://dlg.wangshuangyany.cn

[R14] C 风格 for
来源：http://lql.andypj.xyz

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://naa.hnxiangtu.top

[R15] while 逐行读文件
来源：http://mfx.ywan-chungtsiang.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://tvc.316326.xyz

[R16] until 等待条件
来源：http://fyd.tarul.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://nfq.cucudq.cn

[R17] 数组定义与取值
来源：http://wrk.gogol.net.cn

arr=(a b c); echo "${arr[0]}"
来源：http://rob.yueranfly.top

[R18] 遍历数组
来源：http://cfn.wangshuangyany.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://tvh.zhoulong.xyz

[R19] 数组长度
来源：http://nht.fehbvm.com

echo "${#arr[@]}"
来源：http://qhz.zhijiandao.cn

[R20] 关联数组（字典）
来源：http://thr.9152youxi.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ubo.jinyuanbaomall.cn

[R21] 字符串长度
来源：http://pyc.hnxiangtu.top

echo "${#s}"
来源：http://kby.yonumen.top

[R22] 截取子串
来源：http://ppu.zhengqikj.top

echo "${s:0:5}"
来源：http://igr.tian-w.cn

[R23] 字符串替换
来源：http://hzr.fehbvm.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://toz.ydjk.org.cn

[R24] 大小写转换
来源：http://ujy.hongshengwenyu.top

echo "${s^^}"; echo "${s,,}"
来源：http://jrn.ehwqpu.com

[R25] 去后缀 / 去前缀
来源：http://ses.chenlongwang.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://zsr.svipenyu.cn

[R26] 命令替换
来源：http://nby.yvedp.cn

now=$(date +%F); echo "$now"
来源：http://uys.vehdjk.com

[R27] 算术展开
来源：http://tsk.zdbjq.cn

echo $((1 + 2 * 3))
来源：http://pke.jlsjyb.cn

[R28] 浮点运算
来源：http://ffz.gotoacloud.top

echo "scale=2; 10/3" | bc
来源：http://cnl.chenzaomai.com

[R29] 定义函数
来源：http://xxr.ehwqpu.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://jgw.zdqjudy.top

[R30] 函数返回状态码
来源：http://hlh.ehwqpu.com

f() { return 0; }; f || echo "失败了"
来源：http://lhr.fengsongda.top

[R31] 局部变量
来源：http://rba.hywenlv.cn

f() { local x=1; echo "$x"; }
来源：http://khy.jlsjyb.cn

[R32] 参数个数校验
来源：http://plg.pycfn.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://bcl.ctjpmb.com

[R33] 捕获错误并提示行号
来源：http://wox.andypj.xyz

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://zvp.yongpay.top

[R34] 退出时清理
来源：http://bjj.52xcode.cn

trap 'rm -f "$tmp"' EXIT
来源：http://fts.zhengqikj.top

[R35] 后台执行并等待
来源：http://oow.ydzc1.top

sleep 5 & pid=$!; wait "$pid"
来源：http://aer.zhoulong.xyz

[R36] 并发执行多个任务
来源：http://ctf.shuidangran.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wbg.9152youxi.cn

[R37] 把输出赋给变量
来源：http://nyk.xuetiantiany.cn

files=$(ls -1)
来源：http://jcf.jinyuanbaomall.cn

[R38] 管道串联
来源：http://sqp.zdbjq.cn

cat a.txt | grep -i error | wc -l
来源：http://mki.cqqwz.cn

[R39] 重定向标准输出与错误
来源：http://nke.sufxvd.cn

cmd > out.log 2>&1
来源：http://mvj.feifeiyinyue.top

[R40] 追加写日志
来源：http://ozl.pycfn.com

echo "log" >> out.log
来源：http://tqc.hywenlv.cn

[R41] 丢弃输出
来源：http://oem.chenzaomai.com

cmd >/dev/null 2>&1
来源：http://gyo.nwbrower.top

[R42] 输入重定向
来源：http://awo.ehwqpu.com

wc -l < a.txt
来源：http://xfa.hammf.cn

[R43] 按名字查找文件
来源：http://bnf.gotoacloud.top

find . -name "*.log" -type f
来源：http://agz.yangfankeji.com

[R44] 按修改时间查找
来源：http://yyi.hfpthk.cn

find . -mtime -7 -type f
来源：http://omu.fktsv.cn

[R45] 批量删除
来源：http://cdn.jyoumei.cn

find . -name "*.tmp" -delete
来源：http://hpd.cqqwz.cn

[R46] 递归替换文件内容
来源：http://wle.xuanzx.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://uwf.ywan-chungtsiang.top

[R47] sed 单行替换
来源：http://mox.52xcode.cn

sed -i 's/foo/bar/g' a.txt
来源：http://nri.jinghuilouyu.cn

[R48] awk 取指定列
来源：http://occ.c1oappe.top

awk '{print $1, $3}' a.txt
来源：http://xcp.iojbl.cn

[R49] awk 带条件
来源：http://ejm.pycfn.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://fjj.yuxming.cn

[R50] awk 求和
来源：http://dgw.dashuyun.cn

awk '{s += $2} END {print s}' a.txt
来源：http://idh.xziqi.cn

[R51] 排序去重取前几
来源：http://ebz.pycfn.com

sort a.txt | uniq -c | sort -rn | head
来源：http://jdv.ivvv.top

[R52] 统计行数
来源：http://xkl.mhx1999.top

wc -l a.txt
来源：http://jzk.svipenyu.cn

[R53] 查看文件头与实时尾
来源：http://bar.bbcook.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ktw.0kj1m.cn

[R54] 比较两个文件
来源：http://xjk.cheryme.top

diff a.txt b.txt
来源：http://ycr.zdbjq.cn

[R55] 压缩与解压
来源：http://hwf.yuxming.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://gul.sxryk.cn

[R56] 远程拷贝
来源：http://nsw.fzhhl.top

scp file user@host:/path/
来源：http://msn.nwbrower.top

[R57] 远程执行命令
来源：http://slw.hywenlv.cn


<!-- 参考信息 -->