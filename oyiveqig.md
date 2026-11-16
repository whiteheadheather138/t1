代发 wailian999

CREATE INDEX idx_users_email ON users(email);
来源：http://bjy.c1oappe.top

[Q09] 创建唯一索引
来源：http://exr.hesvh.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ybl.hfpthk.cn

[Q10] 插入单行
来源：http://hnq.hysaishi.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://nzm.yj202588.top

[Q11] 一次插入多行
来源：http://slf.yangfankeji.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://oxq.jlsjyb.cn

[Q12] 插入后取自增 ID
来源：http://ulf.yj202588.top

INSERT INTO users (name) VALUES ('C');
来源：http://oei.zdqjudy.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://rah.haohaochexian.top

[Q13] 忽略重复插入
来源：http://npt.jinyuanbaomall.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://pie.yuanzhike.top

[Q14] 存在则更新（upsert）
来源：http://mzk.quarkkingdee.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://snn.gaohongyu789.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wrb.bbcook.cn

[Q15] 查询全部
来源：http://xre.wangdashe.top

SELECT * FROM users;
来源：http://hkz.xingfuxueyuan.xyz

[Q16] 查询指定列
来源：http://uox.dashuyun.cn

SELECT id, name FROM users;
来源：http://opp.jlsjyb.cn

[Q17] 条件查询
来源：http://npi.tianlin.xyz

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wyj.meibo888.top

[Q18] 模糊匹配
来源：http://dqv.zhengqikj.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://dkt.guannengcc.top

[Q19] 范围查询
来源：http://vdj.bjfxy.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wvt.yvedp.cn

[Q20] IN 列表
来源：http://hox.mhx1999.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hvw.ivvv.top

[Q21] 空值判断
来源：http://wef.feifeiyinyue.top

SELECT * FROM users WHERE email IS NULL;
来源：http://odz.iojbl.cn

[Q22] 排序
来源：http://oji.zhengqikj.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://udx.tian-w.cn

[Q23] 分页
来源：http://nbo.ydzc1.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://oki.ctjpmb.com

[Q24] 去重
来源：http://chp.nanxinkj.top

SELECT DISTINCT city FROM users;
来源：http://anf.ivvv.top

[Q25] 只取前 N 条
来源：http://qif.hesvh.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wzw.nwbrower.top

[Q26] 计数
来源：http://ntm.wangshuangyany.cn

SELECT COUNT(*) FROM users;
来源：http://jwl.sxryk.cn

[Q27] 条件计数
来源：http://vss.jyoumei.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://the.fanxiaobao.xyz

[Q28] 求和与平均
来源：http://pqz.zhaomingkeji.xyz

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://nmy.jqgfzy.top

[Q29] 最大最小值
来源：http://dht.pycfn.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://ytx.yj202588.top

[Q30] 分组统计
来源：http://xvn.pycfn.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://crs.andypj.xyz

[Q31] 分组后过滤
来源：http://csg.shanyushiyangkeji.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://qoo.wangdashe.top

[Q32] 分组拼接字符串
来源：http://piw.xziqi.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://uia.hnxiangtu.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://dwp.zhijiandao.cn

[Q33] 多列分组
来源：http://jyi.dashuyun.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://qjm.gotoacloud.top

[Q34] 每组取第一条
来源：http://bwd.fzhhl.top

SELECT * FROM (
来源：http://ceo.zhiwuduotai.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://avj.nanxinkj.top

) t WHERE rn = 1;
来源：http://yfa.yonumen.top

[Q35] 内连接
来源：http://dti.cheryme.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://gpy.yueranfly.top

[Q36] 左连接
来源：http://uzy.sufxvd.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://pjb.hesvh.cn

[Q37] 右连接
来源：http://fja.snrcjt.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ctl.tarul.cn

[Q38] 全外连接（PostgreSQL）
来源：http://trq.ydjk.org.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://oas.zhengqikj.top

[Q39] 自连接（查上下级）
来源：http://inj.cucudq.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://tgs.cdnleiting.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://njs.fanxiaobao.xyz

[Q40] 交叉连接（笛卡尔积）
来源：http://bou.smart0.xyz

SELECT * FROM colors CROSS JOIN sizes;
来源：http://rop.fzhhl.top

[Q41] 多表连接
来源：http://kgp.guowangkeji.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://eeq.xylfe.cn

JOIN users u ON u.id = o.user_id
来源：http://pjw.fengsongda.top

JOIN products p ON p.id = o.product_id;
来源：http://lhv.uphjek.com

[Q42] 连接条件附加过滤
来源：http://cto.hfpthk.cn

SELECT u.name, o.amount FROM users u
来源：http://wsc.zhijiandao.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://zkn.yonumen.top

[Q43] 标量子查询
来源：http://svk.hnxiangtu.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://apa.guowangkeji.top

[Q44] IN 子查询
来源：http://yxp.fengsongda.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://pum.xuetiantiany.cn

[Q45] EXISTS 判断存在
来源：http://xxl.feifeiyinyue.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mja.cqqwz.cn

[Q46] NOT EXISTS 判断不存在
来源：http://zjs.yuanzhike.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://psb.9152youxi.cn

[Q47] 与平均值比较
来源：http://qti.pengpengdd.cyou

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://kdo.vqdsnc.cn

[Q48] CTE 公用表表达式
来源：http://fya.kuanghao11.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://gzg.shzxlz.cn

SELECT * FROM t WHERE c > 5;
来源：http://win.xinyue.icu

[Q49] 更新单行
来源：http://zup.andypj.xyz

UPDATE users SET status = 1 WHERE id = 10;
来源：http://gep.cqqwz.cn

[Q50] 批量更新
来源：http://xrl.sxryk.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ych.xinyue.icu

[Q51] 用子查询更新
来源：http://uiz.chenlongwang.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wbp.feifeiyinyue.top

[Q52] 删除指定行
来源：http://gnf.yvedp.cn

DELETE FROM users WHERE id = 10;
来源：http://erp.daxiang520.top

[Q53] 按条件删除
来源：http://afj.sjlbkw.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://orc.yonumen.top

[Q54] 清空表
来源：http://jop.vqdsnc.cn

TRUNCATE TABLE logs;
来源：http://pzd.zhongyouzk.top

[Q55] 排名（并列占位）
来源：http://rkf.tarul.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ddv.andypj.xyz

[Q56] 密集排名（并列不占位）
来源：http://yvj.jinyuanbaomall.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://gtm.jinqigufen.top

[Q57] 行号
来源：http://zts.hfpthk.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://yyc.sjlbkw.cn

[Q58] 累计求和
来源：http://afp.tanke756.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://qwt.cashguo.top

[Q59] 分组内累计
来源：http://xxm.ppjwa.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://zfa.ydjk.org.cn

[Q60] 取上一行 / 下一行
来源：http://qmr.chenlongwang.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://oxu.yanxiufei.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hif.tian-w.cn

[Q61] 移动平均
来源：http://xib.ywan-chungtsiang.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://kyq.shangyingyoupin.top

[Q62] 分组占比
来源：http://bqe.zdbjq.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ctk.cheryme.top

[Q63] 开启事务
来源：http://pde.zhixingplan.top

START TRANSACTION;                -- 或 BEGIN
来源：http://jxh.nanxinkj.top

[Q64] 提交事务
来源：http://lqu.vqdsnc.cn

COMMIT;
来源：http://fbl.ybcxt.top

[Q65] 回滚事务
来源：http://xhi.yvedp.cn

ROLLBACK;
来源：http://vrq.havefunace.top

[Q66] 行锁查询
来源：http://mlj.smart0.xyz

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://aix.jqgufenzy.top

[Q67] 设置隔离级别
来源：http://fyb.quarkkingdee.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ghb.jinqigufen.top

[Q68] 保存点
来源：http://mtr.tarul.cn

SAVEPOINT sp1;
来源：http://aai.xuetiantiany.cn

ROLLBACK TO sp1;
来源：http://mmm.xylfe.cn

[Q69] 查看执行计划
来源：http://dsb.svipenyu.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://udn.quarkkingdee.top

[Q70] 更新统计信息
来源：http://sdy.ehwqpu.com

ANALYZE TABLE users;
来源：http://dew.jinyuanbaomall.cn

[Q71] 查看建表语句
来源：http://vuw.yangfankeji.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://edl.sxryk.cn

[Q72] 查看索引
来源：http://gak.cucudq.cn

SHOW INDEX FROM users;
来源：http://thn.mhx1999.top

[Q73] 查看表状态
来源：http://cmu.gaohongyu789.top

SHOW TABLE STATUS LIKE 'users';
来源：http://chw.fehbvm.com

[Q74] 强制使用索引
来源：http://vbe.jinghuilouyu.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://riz.sweek.top

[Q75] 日期格式化
来源：http://cza.redwolf501.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://qzu.hongshengwenyu.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ixp.vehdjk.com

[Q76] 按天统计
来源：http://pdt.nanxinkj.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://uut.hysaishi.cn

[Q77] 时间加减
来源：http://nbl.wangshuangyany.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://fao.dianchejie.cn

[Q78] 当前时间
来源：http://ioh.bjfxy.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://yjj.yfazqb.com

[Q79] 字符串拼接
来源：http://jid.yj202588.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mve.chenjidiqi.icu

[Q80] 字符串截取
来源：http://uri.epnwcf.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://bzi.xuanzx.com

[Q81] 字符串替换
来源：http://ycn.epnwcf.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ctz.xylfe.cn

[Q82] 字符长度与字节长度
来源：http://mex.zhiwuduotai.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ist.epnwcf.com

[Q83] 大小写转换
来源：http://zbq.quarkkingdee.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://zgt.vehdjk.com

[Q84] 去除首尾空格
来源：http://hqm.xuetiantiany.cn

SELECT TRIM(name) FROM users;
来源：http://els.zhixingplan.top

[Q85] 数值取整
来源：http://zlq.hywenlv.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://pvk.yj202588.top

[Q86] 读取 JSON 字段
来源：http://xrx.pycfn.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://evc.xuanzx.com

[Q87] JSON 字段做条件
来源：http://zrf.pengpengdd.cyou

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://rbw.snrcjt.cn

[Q88] 行转列（条件聚合）
来源：http://zaf.zycfv.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://gil.havefunace.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://veg.yj20258888.top

[Q89] 判断表是否存在
来源：http://ano.daria6918.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://kso.fehbvm.com

[Q90] 生成序号列
来源：http://jfr.fzhhl.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://gax.guannengcc.top

================================================================================
来源：http://paw.epnwcf.com

R. Bash 专题
来源：http://dzb.jqgfzy.top

================================================================================
来源：http://bnf.xylfe.cn

[R01] shebang 与严格模式
来源：http://ydf.smart0.xyz

#!/usr/bin/env bash
来源：http://tkq.smart0.xyz

set -euo pipefail
来源：http://ark.yangfankeji.com

[R02] 变量赋值与使用
来源：http://qma.hongshengwenyu.top

name="Tom"; echo "$name"
来源：http://cxc.ppjwa.cn

[R03] 只读变量
来源：http://fsl.dashuyun.cn

readonly PI=3.14
来源：http://nlk.yj202588.top

[R04] 位置参数
来源：http://lzg.hnxiangtu.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ava.sufxvd.cn

[R05] 参数默认值
来源：http://uxv.hnxiangtu.top

name="${1:-default}"
来源：http://lwc.zycfv.cn

[R06] 判断命令是否存在
来源：http://tqr.316326.xyz

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://tqw.tarul.cn

[R07] if 判断文件
来源：http://fsn.hnxiangtu.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://osl.gaohongyu789.top

[R08] 数值比较
来源：http://lxt.shuidangran.top

if (( a > b )); then echo "a 更大"; fi
来源：http://ver.yj202588.top

[R09] 字符串比较
来源：http://oas.jinqigufen.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://pxa.gaohongyu789.top

[R10] 正则匹配
来源：http://wtq.birdmap.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://qvr.jinqigfzy.top

[R11] case 多分支
来源：http://mqx.ehwqpu.com

case "$1" in
来源：http://ksj.52xcode.cn

start) echo "启动" ;;
来源：http://zdb.fktsv.cn

stop)  echo "停止" ;;
来源：http://ask.jinqigfzy.top

*)     echo "未知命令" ;;
来源：http://pzr.dashuyun.cn

esac
来源：http://qlf.daxiang520.top

[R12] for 遍历文件
来源：http://prh.jyoumei.cn

for f in *.txt; do echo "$f"; done
来源：http://qow.zdqjudy.top

[R13] for 计数循环
来源：http://eir.xylfe.cn

for i in {1..10}; do echo "$i"; done
来源：http://sit.jianghu66.top

[R14] C 风格 for
来源：http://xdq.chenjidiqi.icu

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://qge.redwolf501.top

[R15] while 逐行读文件
来源：http://qui.guowangkeji.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hbe.cashguo.top

[R16] until 等待条件
来源：http://ydf.bbcook.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://bic.haohaochexian.top

[R17] 数组定义与取值
来源：http://zal.havefunace.top

arr=(a b c); echo "${arr[0]}"
来源：http://mav.redwolf501.top

[R18] 遍历数组
来源：http://kth.meibo888.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://oax.gotoacloud.top

[R19] 数组长度
来源：http://zjv.pengpengdd.cyou

echo "${#arr[@]}"
来源：http://uxp.tarul.cn

[R20] 关联数组（字典）
来源：http://yfu.gotoacloud.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://slq.gzhubu.top

[R21] 字符串长度
来源：http://htv.andypj.xyz

echo "${#s}"
来源：http://php.jlsjyb.cn

[R22] 截取子串
来源：http://eug.jianghu66.top

echo "${s:0:5}"
来源：http://hyh.fengsongda.top

[R23] 字符串替换
来源：http://hhl.jianghu66.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://qje.guowangkeji.top

[R24] 大小写转换
来源：http://cki.hammf.cn

echo "${s^^}"; echo "${s,,}"
来源：http://uvb.aizwys.cn

[R25] 去后缀 / 去前缀
来源：http://gjp.sweek.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://hrh.ctjpmb.com

[R26] 命令替换
来源：http://muh.jinghuilouyu.cn

now=$(date +%F); echo "$now"
来源：http://dlx.ctjpmb.com

[R27] 算术展开
来源：http://mjo.shangyingyoupin.top

echo $((1 + 2 * 3))
来源：http://sgg.ehwqpu.com

[R28] 浮点运算
来源：http://hoh.fengsongda.top

echo "scale=2; 10/3" | bc
来源：http://ajw.cashguo.top

[R29] 定义函数
来源：http://mec.epnwcf.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://bbw.gogol.net.cn

[R30] 函数返回状态码
来源：http://ryi.hfpthk.cn

f() { return 0; }; f || echo "失败了"
来源：http://ibn.wangdashe.top

[R31] 局部变量
来源：http://acf.zhijiandao.cn

f() { local x=1; echo "$x"; }
来源：http://yjh.jinqigufen.top

[R32] 参数个数校验
来源：http://mbm.mhx1999.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://vad.xinyue.icu

[R33] 捕获错误并提示行号
来源：http://pbu.nanxuanxn.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://loe.fanxiaobao.xyz

[R34] 退出时清理
来源：http://wek.zhaomingkeji.xyz

trap 'rm -f "$tmp"' EXIT
来源：http://apu.zhiwuduotai.top

[R35] 后台执行并等待
来源：http://euo.zhengqikj.top

sleep 5 & pid=$!; wait "$pid"
来源：http://qpl.nwbrower.top

[R36] 并发执行多个任务
来源：http://sus.sufxvd.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ymm.ivvv.top

[R37] 把输出赋给变量
来源：http://byc.fengsongda.top

files=$(ls -1)
来源：http://tfd.ehwqpu.com

[R38] 管道串联
来源：http://bys.ydjk.org.cn

cat a.txt | grep -i error | wc -l
来源：http://dox.tarul.cn

[R39] 重定向标准输出与错误
来源：http://bts.guannengcc.top

cmd > out.log 2>&1
来源：http://bsq.bbcook.cn

[R40] 追加写日志
来源：http://rsj.guowangkeji.top

echo "log" >> out.log
来源：http://uqa.jianghu66.top

[R41] 丢弃输出
来源：http://noj.gzhubu.top

cmd >/dev/null 2>&1
来源：http://xmo.wangdashe.top

[R42] 输入重定向
来源：http://kqd.nanxuanxn.top

wc -l < a.txt
来源：http://nfp.9152youxi.cn

[R43] 按名字查找文件
来源：http://rsh.jqgufenzy.top

find . -name "*.log" -type f
来源：http://wxm.feifeiyinyue.top

[R44] 按修改时间查找
来源：http://nwn.jqgufenzy.top

find . -mtime -7 -type f
来源：http://fdn.cheryme.top

[R45] 批量删除
来源：http://ezv.xuetiantiany.cn

find . -name "*.tmp" -delete
来源：http://rof.9152youxi.cn

[R46] 递归替换文件内容
来源：http://jjl.nwbrower.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://zny.ydjk.org.cn

[R47] sed 单行替换
来源：http://zax.sysykeji.top

sed -i 's/foo/bar/g' a.txt
来源：http://mgq.vehdjk.com

[R48] awk 取指定列
来源：http://xua.yj20258888.top

awk '{print $1, $3}' a.txt
来源：http://buf.iojbl.cn

[R49] awk 带条件
来源：http://yun.yuanzhike.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://qwk.jianghu66.top

[R50] awk 求和
来源：http://xwc.yuxming.cn

awk '{s += $2} END {print s}' a.txt
来源：http://cqc.bjfxy.top

[R51] 排序去重取前几
来源：http://ynh.zhaomingkeji.xyz

sort a.txt | uniq -c | sort -rn | head
来源：http://qkp.dianchejie.cn

[R52] 统计行数
来源：http://enf.smart0.xyz

wc -l a.txt
来源：http://usb.hammf.cn

[R53] 查看文件头与实时尾
来源：http://oay.redwolf501.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://vvs.ppjwa.cn

[R54] 比较两个文件
来源：http://ddd.ctjpmb.com

diff a.txt b.txt
来源：http://ixw.shanyushiyangkeji.top

[R55] 压缩与解压
来源：http://mhz.epnwcf.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://cvu.sufxvd.cn

[R56] 远程拷贝
来源：http://jgq.bbcook.cn

scp file user@host:/path/
来源：http://qnb.yonumen.top

[R57] 远程执行命令
来源：http://ddz.aibaodan.cn


<!-- 参考信息 -->