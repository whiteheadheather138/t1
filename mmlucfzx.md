代发 wailian999

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://shr.zhongyouzk.top

[Q11] 一次插入多行
来源：http://xeg.shangyingyoupin.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mxb.sufxvd.cn

[Q12] 插入后取自增 ID
来源：http://tug.aibaodan.cn

INSERT INTO users (name) VALUES ('C');
来源：http://bxe.quarkkingdee.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://lap.pengpengdd.cyou

[Q13] 忽略重复插入
来源：http://sln.zhixingplan.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://qox.yanxiufei.cn

[Q14] 存在则更新（upsert）
来源：http://vee.xinyue.icu

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://yuc.jlsjyb.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://byy.gotoacloud.top

[Q15] 查询全部
来源：http://pvn.haohaochexian.top

SELECT * FROM users;
来源：http://eje.sxryk.cn

[Q16] 查询指定列
来源：http://qnp.xuetiantiany.cn

SELECT id, name FROM users;
来源：http://anf.c1oappe.top

[Q17] 条件查询
来源：http://heg.tanke756.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://dir.jinyuanbaomall.cn

[Q18] 模糊匹配
来源：http://rpu.c1oappe.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://bgt.zycfv.cn

[Q19] 范围查询
来源：http://pul.cdnleiting.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://rsb.hysaishi.cn

[Q20] IN 列表
来源：http://foj.ppjwa.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://sun.cdnleiting.top

[Q21] 空值判断
来源：http://gfa.xylfe.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://vsl.snrcjt.cn

[Q22] 排序
来源：http://vjr.sjlbkw.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://kmt.ctjpmb.com

[Q23] 分页
来源：http://hqi.cashguo.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://akc.jqgfzy.top

[Q24] 去重
来源：http://eqs.jqgufenzy.top

SELECT DISTINCT city FROM users;
来源：http://mxb.nanxuanxn.top

[Q25] 只取前 N 条
来源：http://tfn.nanxinkj.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://zvf.shuidangran.top

[Q26] 计数
来源：http://ibb.sufxvd.cn

SELECT COUNT(*) FROM users;
来源：http://njk.dashuyun.cn

[Q27] 条件计数
来源：http://aom.ywan-chungtsiang.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://tkp.haohaochexian.top

[Q28] 求和与平均
来源：http://fjg.c1oappe.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://tca.vehdjk.com

[Q29] 最大最小值
来源：http://dmp.cheryme.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://yzg.jyoumei.cn

[Q30] 分组统计
来源：http://jqi.tianlin.xyz

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ngc.tian-w.cn

[Q31] 分组后过滤
来源：http://laf.jinghuilouyu.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://kkq.guannengcc.top

[Q32] 分组拼接字符串
来源：http://vzk.shuidangran.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://rfo.yangfankeji.com

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ubw.havefunace.top

[Q33] 多列分组
来源：http://yhl.vehdjk.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://qyw.hfpthk.cn

[Q34] 每组取第一条
来源：http://oki.jlsjyb.cn

SELECT * FROM (
来源：http://vpy.feifeiyinyue.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ues.hammf.cn

) t WHERE rn = 1;
来源：http://emt.sufxvd.cn

[Q35] 内连接
来源：http://gzp.xylfe.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://lmm.gogol.net.cn

[Q36] 左连接
来源：http://ngm.zdqjudy.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://bdk.jiagoushi.top

[Q37] 右连接
来源：http://gon.yj202588.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://xvw.nanxuanxn.top

[Q38] 全外连接（PostgreSQL）
来源：http://wsy.jinqigfzy.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wyj.hysaishi.cn

[Q39] 自连接（查上下级）
来源：http://qsc.dashuyun.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://hcv.hammf.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://dwi.redwolf501.top

[Q40] 交叉连接（笛卡尔积）
来源：http://ouk.hysaishi.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://onc.ehwqpu.com

[Q41] 多表连接
来源：http://kfe.sysykeji.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://sww.daxiang520.top

JOIN users u ON u.id = o.user_id
来源：http://orf.epnwcf.com

JOIN products p ON p.id = o.product_id;
来源：http://biw.jlsjyb.cn

[Q42] 连接条件附加过滤
来源：http://ejx.redwolf501.top

SELECT u.name, o.amount FROM users u
来源：http://lsv.meibo888.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://aef.andypj.xyz

[Q43] 标量子查询
来源：http://djt.wangdashe.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://vri.cqqwz.cn

[Q44] IN 子查询
来源：http://ghe.feifeiyinyue.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://qzb.jqgfzy.top

[Q45] EXISTS 判断存在
来源：http://dzc.hammf.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://igc.0kj1m.cn

[Q46] NOT EXISTS 判断不存在
来源：http://peo.iojbl.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://loo.sxryk.cn

[Q47] 与平均值比较
来源：http://rqv.havefunace.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://lrh.jinqigufen.top

[Q48] CTE 公用表表达式
来源：http://lin.zhengqikj.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://klp.yangfankeji.com

SELECT * FROM t WHERE c > 5;
来源：http://bye.tianlin.xyz

[Q49] 更新单行
来源：http://zyz.yfazqb.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://msp.yuxming.cn

[Q50] 批量更新
来源：http://yui.jinyuanbaomall.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://tak.hesvh.cn

[Q51] 用子查询更新
来源：http://udm.yvedp.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://bqu.jinqigufen.top

[Q52] 删除指定行
来源：http://ytb.daxiang520.top

DELETE FROM users WHERE id = 10;
来源：http://dgf.ydjk.org.cn

[Q53] 按条件删除
来源：http://mjj.ydjk.org.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://rls.316326.xyz

[Q54] 清空表
来源：http://dee.xuanzx.com

TRUNCATE TABLE logs;
来源：http://pmx.yfazqb.com

[Q55] 排名（并列占位）
来源：http://yry.chenlongwang.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://lmo.xziqi.cn

[Q56] 密集排名（并列不占位）
来源：http://qwm.vqdsnc.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://tvp.yuxming.cn

[Q57] 行号
来源：http://xor.ydjk.org.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://nkc.fengsongda.top

[Q58] 累计求和
来源：http://ejx.gzhubu.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://isb.guowangkeji.top

[Q59] 分组内累计
来源：http://amb.chenjidiqi.icu

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mlr.zhongyouzk.top

[Q60] 取上一行 / 下一行
来源：http://eyd.yongpay.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://koe.xuetiantiany.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://czl.hnxiangtu.top

[Q61] 移动平均
来源：http://hgl.dianchejie.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://qqn.zhaomingkeji.xyz

[Q62] 分组占比
来源：http://tts.9152youxi.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://udm.yj20258888.top

[Q63] 开启事务
来源：http://feu.gogol.net.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://woj.sxryk.cn

[Q64] 提交事务
来源：http://hde.yongpay.top

COMMIT;
来源：http://cqa.ybcxt.top

[Q65] 回滚事务
来源：http://isk.yj20258.top

ROLLBACK;
来源：http://dgl.ctjpmb.com

[Q66] 行锁查询
来源：http://umh.ppjwa.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://bpg.ydjk.org.cn

[Q67] 设置隔离级别
来源：http://bkr.aibaodan.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://lkz.yangfankeji.com

[Q68] 保存点
来源：http://hbg.gotoacloud.top

SAVEPOINT sp1;
来源：http://prr.316326.xyz

ROLLBACK TO sp1;
来源：http://vxu.ppjwa.cn

[Q69] 查看执行计划
来源：http://slg.yonumen.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://quc.fengsongda.top

[Q70] 更新统计信息
来源：http://unr.316326.xyz

ANALYZE TABLE users;
来源：http://qdr.fzhhl.top

[Q71] 查看建表语句
来源：http://moq.jinqigufen.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://gnj.daxiang520.top

[Q72] 查看索引
来源：http://sbc.gotoacloud.top

SHOW INDEX FROM users;
来源：http://qxn.hfpthk.cn

[Q73] 查看表状态
来源：http://nnl.snrcjt.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://iki.shanyushiyangkeji.top

[Q74] 强制使用索引
来源：http://vpf.jinqigufen.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://cqk.yfazqb.com

[Q75] 日期格式化
来源：http://oty.chenjidiqi.icu

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://lwi.vqdsnc.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://bij.uphjek.com

[Q76] 按天统计
来源：http://jhg.hfpthk.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://imc.gzhubu.top

[Q77] 时间加减
来源：http://jsr.hywenlv.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://jel.guowangkeji.top

[Q78] 当前时间
来源：http://ych.52xcode.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wiz.andypj.xyz

[Q79] 字符串拼接
来源：http://ole.jinqigfzy.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://fjk.yuanzhike.top

[Q80] 字符串截取
来源：http://fmw.yj202588.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hhw.hcnkem.com

[Q81] 字符串替换
来源：http://woe.hammf.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://klz.yj20258888.top

[Q82] 字符长度与字节长度
来源：http://aln.hesvh.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://bxc.fengsongda.top

[Q83] 大小写转换
来源：http://wxh.shangyingyoupin.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ukq.jqgfzy.top

[Q84] 去除首尾空格
来源：http://pdj.hnxiangtu.top

SELECT TRIM(name) FROM users;
来源：http://tcz.guowangkeji.top

[Q85] 数值取整
来源：http://bfv.xuetiantiany.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://btm.zhongyouzk.top

[Q86] 读取 JSON 字段
来源：http://gcs.birdmap.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hzc.yonumen.top

[Q87] JSON 字段做条件
来源：http://ukc.redwolf501.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://rpf.ywan-chungtsiang.top

[Q88] 行转列（条件聚合）
来源：http://aql.xingfuxueyuan.xyz

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://pna.xinyue.icu

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://cjx.nanxuanxn.top

[Q89] 判断表是否存在
来源：http://vcv.zhaomingkeji.xyz

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://luq.zhijiandao.cn

[Q90] 生成序号列
来源：http://nyu.zhijiandao.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://fyr.chenlongwang.top

================================================================================
来源：http://pkw.ppjwa.cn

R. Bash 专题
来源：http://uku.ydzc1.top

================================================================================
来源：http://int.jqgufenzy.top

[R01] shebang 与严格模式
来源：http://flh.yueranfly.top

#!/usr/bin/env bash
来源：http://uni.yuxming.cn

set -euo pipefail
来源：http://eic.guannengcc.top

[R02] 变量赋值与使用
来源：http://zmn.ctjpmb.com

name="Tom"; echo "$name"
来源：http://ezq.xziqi.cn

[R03] 只读变量
来源：http://vxo.52xcode.cn

readonly PI=3.14
来源：http://fng.aizwys.cn

[R04] 位置参数
来源：http://jar.vqdsnc.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://yat.hongshengwenyu.top

[R05] 参数默认值
来源：http://tuk.zhoulong.xyz

name="${1:-default}"
来源：http://nhk.chenlongwang.top

[R06] 判断命令是否存在
来源：http://gdr.gaohongyu789.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://cgv.yj20258.top

[R07] if 判断文件
来源：http://uhw.daria6918.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://scr.zdqjudy.top

[R08] 数值比较
来源：http://csc.fzhhl.top

if (( a > b )); then echo "a 更大"; fi
来源：http://kgb.gotoacloud.top

[R09] 字符串比较
来源：http://dsc.gogol.net.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://rho.snrcjt.cn

[R10] 正则匹配
来源：http://aba.fehbvm.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://rcg.jlsjyb.cn

[R11] case 多分支
来源：http://nms.nanxinkj.top

case "$1" in
来源：http://xml.aizwys.cn

start) echo "启动" ;;
来源：http://sej.sufxvd.cn

stop)  echo "停止" ;;
来源：http://xom.9152youxi.cn

*)     echo "未知命令" ;;
来源：http://jjm.yonumen.top

esac
来源：http://fid.nwbrower.top

[R12] for 遍历文件
来源：http://cys.zhongyouzk.top

for f in *.txt; do echo "$f"; done
来源：http://ljb.havefunace.top

[R13] for 计数循环
来源：http://wwz.hammf.cn

for i in {1..10}; do echo "$i"; done
来源：http://feo.yj20258.top

[R14] C 风格 for
来源：http://prx.guowangkeji.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://iva.fengsongda.top

[R15] while 逐行读文件
来源：http://ueo.iojbl.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://rke.svipenyu.cn

[R16] until 等待条件
来源：http://khw.fengsongda.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://foa.xuanzx.com

[R17] 数组定义与取值
来源：http://abu.svipenyu.cn

arr=(a b c); echo "${arr[0]}"
来源：http://xoi.ybcxt.top

[R18] 遍历数组
来源：http://dpr.snrcjt.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://rcx.ybcxt.top

[R19] 数组长度
来源：http://ige.fehbvm.com

echo "${#arr[@]}"
来源：http://wch.gotoacloud.top

[R20] 关联数组（字典）
来源：http://txa.pengpengdd.cyou

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://gvr.fengsongda.top

[R21] 字符串长度
来源：http://dej.hcnkem.com

echo "${#s}"
来源：http://nqo.gzhubu.top

[R22] 截取子串
来源：http://ovv.xuanzx.com

echo "${s:0:5}"
来源：http://mci.gaohongyu789.top

[R23] 字符串替换
来源：http://qym.jinqigfzy.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://jdt.guowangkeji.top

[R24] 大小写转换
来源：http://edn.uphjek.com

echo "${s^^}"; echo "${s,,}"
来源：http://uha.cucudq.cn

[R25] 去后缀 / 去前缀
来源：http://ttp.yuxming.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://hki.vehdjk.com

[R26] 命令替换
来源：http://lzs.c1oappe.top

now=$(date +%F); echo "$now"
来源：http://dih.zdbjq.cn

[R27] 算术展开
来源：http://jpc.fktsv.cn

echo $((1 + 2 * 3))
来源：http://ylb.hongshengwenyu.top

[R28] 浮点运算
来源：http://xqc.dashuyun.cn

echo "scale=2; 10/3" | bc
来源：http://yhi.guannengcc.top

[R29] 定义函数
来源：http://jjn.c1oappe.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://thy.aibaodan.cn

[R30] 函数返回状态码
来源：http://nmq.cheryme.top

f() { return 0; }; f || echo "失败了"
来源：http://kgo.kuanghao11.cn

[R31] 局部变量
来源：http://arf.dianchejie.cn

f() { local x=1; echo "$x"; }
来源：http://gvx.cdnleiting.top

[R32] 参数个数校验
来源：http://vob.jqgufenzy.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ire.tarul.cn

[R33] 捕获错误并提示行号
来源：http://lls.cheryme.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ixi.vqdsnc.cn

[R34] 退出时清理
来源：http://cec.hcnkem.com

trap 'rm -f "$tmp"' EXIT
来源：http://gzp.yueranfly.top

[R35] 后台执行并等待
来源：http://rwz.quarkkingdee.top

sleep 5 & pid=$!; wait "$pid"
来源：http://ewq.jianghu66.top

[R36] 并发执行多个任务
来源：http://lwi.hfpthk.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hnt.gzhubu.top

[R37] 把输出赋给变量
来源：http://aah.mhx1999.top

files=$(ls -1)
来源：http://akj.aibaodan.cn

[R38] 管道串联
来源：http://jgg.ppjwa.cn

cat a.txt | grep -i error | wc -l
来源：http://xjh.yj20258888.top

[R39] 重定向标准输出与错误
来源：http://lwk.mhx1999.top

cmd > out.log 2>&1
来源：http://ber.zhongyouzk.top

[R40] 追加写日志
来源：http://lsj.pycfn.com

echo "log" >> out.log
来源：http://rdh.guowangkeji.top

[R41] 丢弃输出
来源：http://nps.hnxiangtu.top

cmd >/dev/null 2>&1
来源：http://vrn.gotoacloud.top

[R42] 输入重定向
来源：http://kvm.cashguo.top

wc -l < a.txt
来源：http://rzy.hammf.cn

[R43] 按名字查找文件
来源：http://rhp.9152youxi.cn

find . -name "*.log" -type f
来源：http://vei.yonumen.top

[R44] 按修改时间查找
来源：http://gvm.snrcjt.cn

find . -mtime -7 -type f
来源：http://svz.ctjpmb.com

[R45] 批量删除
来源：http://nwl.yangfankeji.com

find . -name "*.tmp" -delete
来源：http://xyq.ydzc1.top

[R46] 递归替换文件内容
来源：http://dtp.iojbl.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://bfy.jinyuanbaomall.cn

[R47] sed 单行替换
来源：http://vvc.ctjpmb.com

sed -i 's/foo/bar/g' a.txt
来源：http://phw.316326.xyz

[R48] awk 取指定列
来源：http://rtd.jinghuilouyu.cn

awk '{print $1, $3}' a.txt
来源：http://xou.zhixingplan.top

[R49] awk 带条件
来源：http://ksm.zdqjudy.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://chu.gotoacloud.top

[R50] awk 求和
来源：http://aos.ybcxt.top

awk '{s += $2} END {print s}' a.txt
来源：http://wtu.xuetiantiany.cn

[R51] 排序去重取前几
来源：http://kti.ybcxt.top

sort a.txt | uniq -c | sort -rn | head
来源：http://btq.jianghu66.top

[R52] 统计行数
来源：http://iub.bbcook.cn

wc -l a.txt
来源：http://aib.gogol.net.cn

[R53] 查看文件头与实时尾
来源：http://cgr.zycfv.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wwj.ivvv.top

[R54] 比较两个文件
来源：http://ial.gogol.net.cn

diff a.txt b.txt
来源：http://xou.yonumen.top

[R55] 压缩与解压
来源：http://vtu.tian-w.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://vip.ydjk.org.cn

[R56] 远程拷贝
来源：http://xpe.gaohongyu789.top

scp file user@host:/path/
来源：http://hdy.tarul.cn

[R57] 远程执行命令
来源：http://psn.gogol.net.cn

ssh user@host 'uptime'
来源：http://ykc.sjlbkw.cn

[R58] 下载文件
来源：http://lgw.zdqjudy.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://pkl.ydzc1.top

[R59] 发 POST JSON
来源：http://ntq.hcnkem.com


<!-- 参考信息 -->