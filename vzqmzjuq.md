代发 wailian999

INSERT INTO users (name) VALUES ('C');
来源：http://mja.aibaodan.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://axe.sysykeji.top

[Q13] 忽略重复插入
来源：http://ecl.aibaodan.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://nne.ivvv.top

[Q14] 存在则更新（upsert）
来源：http://myl.pengpengdd.cyou

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://byx.mhx1999.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wka.jlsjyb.cn

[Q15] 查询全部
来源：http://jhv.birdmap.top

SELECT * FROM users;
来源：http://hxi.52xcode.cn

[Q16] 查询指定列
来源：http://dfp.fktsv.cn

SELECT id, name FROM users;
来源：http://rrk.jqgfzy.top

[Q17] 条件查询
来源：http://hof.epnwcf.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://fdm.hammf.cn

[Q18] 模糊匹配
来源：http://yuu.xylfe.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://xkm.zycfv.cn

[Q19] 范围查询
来源：http://asx.gogol.net.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://vxj.jqgufenzy.top

[Q20] IN 列表
来源：http://smt.gogol.net.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mie.xuetiantiany.cn

[Q21] 空值判断
来源：http://jrd.quarkkingdee.top

SELECT * FROM users WHERE email IS NULL;
来源：http://lsl.gogol.net.cn

[Q22] 排序
来源：http://drw.dianchejie.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://fnq.zhixingplan.top

[Q23] 分页
来源：http://qpl.feifeiyinyue.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ajp.hammf.cn

[Q24] 去重
来源：http://nof.wangdashe.top

SELECT DISTINCT city FROM users;
来源：http://bqh.ctjpmb.com

[Q25] 只取前 N 条
来源：http://zyy.aibaodan.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://dio.shanyushiyangkeji.top

[Q26] 计数
来源：http://tqm.andypj.xyz

SELECT COUNT(*) FROM users;
来源：http://bmg.bjfxy.top

[Q27] 条件计数
来源：http://olb.ydjk.org.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://clz.ppjwa.cn

[Q28] 求和与平均
来源：http://qod.shzxlz.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://vco.yfazqb.com

[Q29] 最大最小值
来源：http://rja.ydjk.org.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://gth.gaohongyu789.top

[Q30] 分组统计
来源：http://mfo.hnqzz.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://kea.feifeiyinyue.top

[Q31] 分组后过滤
来源：http://zcf.haohaochexian.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hyz.jqgufenzy.top

[Q32] 分组拼接字符串
来源：http://hgz.chenzaomai.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://idu.zhixingplan.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://lnv.xingfuxueyuan.xyz

[Q33] 多列分组
来源：http://cqn.hesvh.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wsi.tanke756.top

[Q34] 每组取第一条
来源：http://qqt.zhijiandao.cn

SELECT * FROM (
来源：http://ogj.pycfn.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://uok.hfpthk.cn

) t WHERE rn = 1;
来源：http://zvy.ybcxt.top

[Q35] 内连接
来源：http://fwq.nanxuanxn.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://lck.ivvv.top

[Q36] 左连接
来源：http://oik.yueranfly.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://vow.c1oappe.top

[Q37] 右连接
来源：http://zbh.gogol.net.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wep.xylfe.cn

[Q38] 全外连接（PostgreSQL）
来源：http://lbg.gzhubu.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://etu.snrcjt.cn

[Q39] 自连接（查上下级）
来源：http://jqd.sweek.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://zkt.hongshengwenyu.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://clm.gaohongyu789.top

[Q40] 交叉连接（笛卡尔积）
来源：http://rha.jiagoushi.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://nzr.zhijiandao.cn

[Q41] 多表连接
来源：http://fby.hfpthk.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://bdo.ywan-chungtsiang.top

JOIN users u ON u.id = o.user_id
来源：http://kdn.pycfn.com

JOIN products p ON p.id = o.product_id;
来源：http://zrc.gzhubu.top

[Q42] 连接条件附加过滤
来源：http://ald.yangfankeji.com

SELECT u.name, o.amount FROM users u
来源：http://nip.shuidangran.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://adp.cheryme.top

[Q43] 标量子查询
来源：http://gan.chenjidiqi.icu

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://cot.yuxming.cn

[Q44] IN 子查询
来源：http://hig.shangyingyoupin.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://kfk.fzhhl.top

[Q45] EXISTS 判断存在
来源：http://gjc.epnwcf.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xvq.jqgfzy.top

[Q46] NOT EXISTS 判断不存在
来源：http://jur.zhaomingkeji.xyz

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://klw.yfazqb.com

[Q47] 与平均值比较
来源：http://rme.chenjidiqi.icu

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://bue.aizwys.cn

[Q48] CTE 公用表表达式
来源：http://muf.chenjidiqi.icu

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://upa.tian-w.cn

SELECT * FROM t WHERE c > 5;
来源：http://xod.jinyuanbaomall.cn

[Q49] 更新单行
来源：http://qgt.jinqigufen.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://zom.birdmap.top

[Q50] 批量更新
来源：http://vbp.ydzc1.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://xfi.sysykeji.top

[Q51] 用子查询更新
来源：http://jud.wangdashe.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mds.smart0.xyz

[Q52] 删除指定行
来源：http://yif.shzxlz.cn

DELETE FROM users WHERE id = 10;
来源：http://rpt.sysykeji.top

[Q53] 按条件删除
来源：http://nuw.hywenlv.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://kas.pengpengdd.cyou

[Q54] 清空表
来源：http://yro.jinyuanbaomall.cn

TRUNCATE TABLE logs;
来源：http://otl.bbcook.cn

[Q55] 排名（并列占位）
来源：http://est.jinqigufen.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://xbl.iojbl.cn

[Q56] 密集排名（并列不占位）
来源：http://rwg.haohaochexian.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://bhs.zhoulong.xyz

[Q57] 行号
来源：http://bti.jinqigfzy.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://lck.cqqwz.cn

[Q58] 累计求和
来源：http://lvk.jianghu66.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://nkv.yj202588.top

[Q59] 分组内累计
来源：http://tcm.cashguo.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://lgm.wangdashe.top

[Q60] 取上一行 / 下一行
来源：http://tkb.0kj1m.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hxw.haohaochexian.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://lcq.sufxvd.cn

[Q61] 移动平均
来源：http://umi.cashguo.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://xhc.fzhhl.top

[Q62] 分组占比
来源：http://rew.cheryme.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://dnu.zdbjq.cn

[Q63] 开启事务
来源：http://fpy.ydjk.org.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://syx.quarkkingdee.top

[Q64] 提交事务
来源：http://jfw.zhongyouzk.top

COMMIT;
来源：http://ixt.ybcxt.top

[Q65] 回滚事务
来源：http://yno.xziqi.cn

ROLLBACK;
来源：http://zce.mhx1999.top

[Q66] 行锁查询
来源：http://fue.yj20258.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://fwk.zycfv.cn

[Q67] 设置隔离级别
来源：http://tem.yangfankeji.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://svy.andypj.xyz

[Q68] 保存点
来源：http://aan.gogol.net.cn

SAVEPOINT sp1;
来源：http://jrv.pycfn.com

ROLLBACK TO sp1;
来源：http://xnv.yongpay.top

[Q69] 查看执行计划
来源：http://upp.yanxiufei.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://vvu.gaohongyu789.top

[Q70] 更新统计信息
来源：http://nti.andypj.xyz

ANALYZE TABLE users;
来源：http://lvq.wangdashe.top

[Q71] 查看建表语句
来源：http://uuz.sxryk.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://apm.yuxming.cn

[Q72] 查看索引
来源：http://xvx.bjfxy.top

SHOW INDEX FROM users;
来源：http://wbe.316326.xyz

[Q73] 查看表状态
来源：http://bym.zdbjq.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://gio.shuidangran.top

[Q74] 强制使用索引
来源：http://hlu.vehdjk.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wma.ehwqpu.com

[Q75] 日期格式化
来源：http://mfi.zdbjq.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://tev.bbcook.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ihh.yuxming.cn

[Q76] 按天统计
来源：http://rog.guowangkeji.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ufw.ppjwa.cn

[Q77] 时间加减
来源：http://uqo.xylfe.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://elh.fanxiaobao.xyz

[Q78] 当前时间
来源：http://vru.jinyuanbaomall.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://fjd.jqgfzy.top

[Q79] 字符串拼接
来源：http://fla.sjlbkw.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://obe.c1oappe.top

[Q80] 字符串截取
来源：http://wwc.hnxiangtu.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://xgx.nanxuanxn.top

[Q81] 字符串替换
来源：http://kwx.bbcook.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://smc.cashguo.top

[Q82] 字符长度与字节长度
来源：http://yjg.jyoumei.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://spo.ybcxt.top

[Q83] 大小写转换
来源：http://gqf.redwolf501.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://pol.sysykeji.top

[Q84] 去除首尾空格
来源：http://tjd.hywenlv.cn

SELECT TRIM(name) FROM users;
来源：http://epp.fzhhl.top

[Q85] 数值取整
来源：http://spc.jinghuilouyu.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://uev.0kj1m.cn

[Q86] 读取 JSON 字段
来源：http://wlb.yonumen.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://bow.zdqjudy.top

[Q87] JSON 字段做条件
来源：http://yyv.hesvh.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://myx.yuanzhike.top

[Q88] 行转列（条件聚合）
来源：http://feh.sxryk.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://nls.fanxiaobao.xyz

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://won.vehdjk.com

[Q89] 判断表是否存在
来源：http://jlr.hfpthk.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mcq.mhx1999.top

[Q90] 生成序号列
来源：http://vlf.zhoulong.xyz

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://kei.hesvh.cn

================================================================================
来源：http://qoj.zhoulong.xyz

R. Bash 专题
来源：http://pmp.hfpthk.cn

================================================================================
来源：http://ceo.ydjk.org.cn

[R01] shebang 与严格模式
来源：http://uvq.iojbl.cn

#!/usr/bin/env bash
来源：http://uts.jianghu66.top

set -euo pipefail
来源：http://tcv.aibaodan.cn

[R02] 变量赋值与使用
来源：http://uyg.gotoacloud.top

name="Tom"; echo "$name"
来源：http://oxl.jqgfzy.top

[R03] 只读变量
来源：http://gdh.guowangkeji.top

readonly PI=3.14
来源：http://nit.fehbvm.com

[R04] 位置参数
来源：http://hzn.cqqwz.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://dbe.xingfuxueyuan.xyz

[R05] 参数默认值
来源：http://jdp.feifeiyinyue.top

name="${1:-default}"
来源：http://nct.gaohongyu789.top

[R06] 判断命令是否存在
来源：http://mmy.hywenlv.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://tir.sweek.top

[R07] if 判断文件
来源：http://nvr.jqgfzy.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://uqo.ydzc1.top

[R08] 数值比较
来源：http://jds.gzhubu.top

if (( a > b )); then echo "a 更大"; fi
来源：http://nst.shanyushiyangtech.top

[R09] 字符串比较
来源：http://dck.jinqigufen.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wdo.guannengcc.top

[R10] 正则匹配
来源：http://zlx.ehwqpu.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://nmr.bjfxy.top

[R11] case 多分支
来源：http://urk.yj202588.top

case "$1" in
来源：http://aas.quarkkingdee.top

start) echo "启动" ;;
来源：http://zsn.xuetiantiany.cn

stop)  echo "停止" ;;
来源：http://uej.zdbjq.cn

*)     echo "未知命令" ;;
来源：http://lqr.wangdashe.top

esac
来源：http://cgb.316326.xyz

[R12] for 遍历文件
来源：http://grr.sjlbkw.cn

for f in *.txt; do echo "$f"; done
来源：http://lha.svipenyu.cn

[R13] for 计数循环
来源：http://jwk.dashuyun.cn

for i in {1..10}; do echo "$i"; done
来源：http://lio.zdbjq.cn

[R14] C 风格 for
来源：http://big.sjlbkw.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://dpb.guannengcc.top

[R15] while 逐行读文件
来源：http://fpb.ydjk.org.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://fci.haohaochexian.top

[R16] until 等待条件
来源：http://agu.fktsv.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://zgh.sufxvd.cn

[R17] 数组定义与取值
来源：http://pex.sysykeji.top

arr=(a b c); echo "${arr[0]}"
来源：http://pqb.hnqzz.top

[R18] 遍历数组
来源：http://zyi.yvedp.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ntg.yj20258888.top

[R19] 数组长度
来源：http://zsz.fehbvm.com

echo "${#arr[@]}"
来源：http://zom.gogol.net.cn

[R20] 关联数组（字典）
来源：http://wco.feifeiyinyue.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://vhw.ctjpmb.com

[R21] 字符串长度
来源：http://klx.mhx1999.top

echo "${#s}"
来源：http://wts.jinqigufen.top

[R22] 截取子串
来源：http://krq.hesvh.cn

echo "${s:0:5}"
来源：http://nlg.sysykeji.top

[R23] 字符串替换
来源：http://xix.cdnleiting.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://cml.yuanzhike.top

[R24] 大小写转换
来源：http://ofi.jyoumei.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ypv.nanxinkj.top

[R25] 去后缀 / 去前缀
来源：http://myo.hnxiangtu.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://elc.shzxlz.cn

[R26] 命令替换
来源：http://bis.havefunace.top

now=$(date +%F); echo "$now"
来源：http://ovz.fktsv.cn

[R27] 算术展开
来源：http://zug.jinqigfzy.top

echo $((1 + 2 * 3))
来源：http://flv.sufxvd.cn

[R28] 浮点运算
来源：http://bmr.hnqzz.top

echo "scale=2; 10/3" | bc
来源：http://olz.bjfxy.top

[R29] 定义函数
来源：http://fgg.ehwqpu.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mhc.sxryk.cn

[R30] 函数返回状态码
来源：http://pmu.guannengcc.top

f() { return 0; }; f || echo "失败了"
来源：http://bpl.zdqjudy.top

[R31] 局部变量
来源：http://iub.jiagoushi.top

f() { local x=1; echo "$x"; }
来源：http://uez.haohaochexian.top

[R32] 参数个数校验
来源：http://cab.yfazqb.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://lre.zhiwuduotai.top

[R33] 捕获错误并提示行号
来源：http://bor.yfazqb.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ocv.zhaomingkeji.xyz

[R34] 退出时清理
来源：http://vzx.jqgfzy.top

trap 'rm -f "$tmp"' EXIT
来源：http://ozp.yvedp.cn

[R35] 后台执行并等待
来源：http://qjj.sjlbkw.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://mxo.nanxinkj.top

[R36] 并发执行多个任务
来源：http://vou.jlsjyb.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://dbi.xylfe.cn

[R37] 把输出赋给变量
来源：http://oio.birdmap.top

files=$(ls -1)
来源：http://arn.shzxlz.cn

[R38] 管道串联
来源：http://ozu.meibo888.top

cat a.txt | grep -i error | wc -l
来源：http://lvi.gaohongyu789.top

[R39] 重定向标准输出与错误
来源：http://hcp.yj202588.top

cmd > out.log 2>&1
来源：http://hpl.fengsongda.top

[R40] 追加写日志
来源：http://bqn.jlsjyb.cn

echo "log" >> out.log
来源：http://auo.uphjek.com

[R41] 丢弃输出
来源：http://wkw.fengsongda.top

cmd >/dev/null 2>&1
来源：http://bgp.cqqwz.cn

[R42] 输入重定向
来源：http://sou.kuanghao11.cn

wc -l < a.txt
来源：http://jwi.quarkkingdee.top

[R43] 按名字查找文件
来源：http://wmq.zhengqikj.top

find . -name "*.log" -type f
来源：http://cey.xingfuxueyuan.xyz

[R44] 按修改时间查找
来源：http://gsa.aizwys.cn

find . -mtime -7 -type f
来源：http://yej.haohaochexian.top

[R45] 批量删除
来源：http://cyo.hnqzz.top

find . -name "*.tmp" -delete
来源：http://qvj.jinqigufen.top

[R46] 递归替换文件内容
来源：http://qpw.bbcook.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://kka.sxryk.cn

[R47] sed 单行替换
来源：http://bef.jinqigfzy.top

sed -i 's/foo/bar/g' a.txt
来源：http://ybc.sysykeji.top

[R48] awk 取指定列
来源：http://lrt.jinghuilouyu.cn

awk '{print $1, $3}' a.txt
来源：http://emy.iojbl.cn

[R49] awk 带条件
来源：http://wph.shuidangran.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://dif.smart0.xyz

[R50] awk 求和
来源：http://owy.pycfn.com

awk '{s += $2} END {print s}' a.txt
来源：http://itm.hesvh.cn

[R51] 排序去重取前几
来源：http://vul.zhiwuduotai.top

sort a.txt | uniq -c | sort -rn | head
来源：http://ity.gzhubu.top

[R52] 统计行数
来源：http://cym.snrcjt.cn

wc -l a.txt
来源：http://hmb.yuanzhike.top

[R53] 查看文件头与实时尾
来源：http://het.gogol.net.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://kzh.mhx1999.top

[R54] 比较两个文件
来源：http://rao.hysaishi.cn

diff a.txt b.txt
来源：http://yms.daxiang520.top

[R55] 压缩与解压
来源：http://ljj.xingfuxueyuan.xyz

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://lxn.vqdsnc.cn

[R56] 远程拷贝
来源：http://lnh.gzhubu.top

scp file user@host:/path/
来源：http://wxs.yj20258.top

[R57] 远程执行命令
来源：http://lzy.snrcjt.cn

ssh user@host 'uptime'
来源：http://wyj.yuanzhike.top

[R58] 下载文件
来源：http://lvq.hesvh.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://zod.jiagoushi.top

[R59] 发 POST JSON
来源：http://fqt.nwbrower.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://aam.gogol.net.cn

[R60] 只看 HTTP 状态码
来源：http://eef.hysaishi.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://eok.guowangkeji.top

[R61] 磁盘占用
来源：http://hud.aizwys.cn


<!-- 参考信息 -->