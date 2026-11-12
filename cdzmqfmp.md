代发 wailian999

[Q14] 存在则更新（upsert）
来源：http://qhr.zhongyouzk.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://uow.iojbl.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://jrh.jyoumei.cn

[Q15] 查询全部
来源：http://gdh.gogol.net.cn

SELECT * FROM users;
来源：http://hmj.sxryk.cn

[Q16] 查询指定列
来源：http://bmr.ehwqpu.com

SELECT id, name FROM users;
来源：http://tdu.tanke756.top

[Q17] 条件查询
来源：http://hfe.hysaishi.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ead.svipenyu.cn

[Q18] 模糊匹配
来源：http://woz.gaohongyu789.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://fas.cdnleiting.top

[Q19] 范围查询
来源：http://tra.sufxvd.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://fmk.svipenyu.cn

[Q20] IN 列表
来源：http://uvt.guowangkeji.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://qak.52xcode.cn

[Q21] 空值判断
来源：http://ynj.svipenyu.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://pxc.jinqigufen.top

[Q22] 排序
来源：http://mrz.ivvv.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://jtj.tian-w.cn

[Q23] 分页
来源：http://eyo.yangfankeji.com

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://kgp.fktsv.cn

[Q24] 去重
来源：http://uon.shangyingyoupin.top

SELECT DISTINCT city FROM users;
来源：http://woz.sysykeji.top

[Q25] 只取前 N 条
来源：http://gdd.ppjwa.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://xou.mhx1999.top

[Q26] 计数
来源：http://hvg.c1oappe.top

SELECT COUNT(*) FROM users;
来源：http://dtl.guannengcc.top

[Q27] 条件计数
来源：http://fsy.sufxvd.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://evk.vehdjk.com

[Q28] 求和与平均
来源：http://mnd.jianghu66.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://czb.iojbl.cn

[Q29] 最大最小值
来源：http://vca.yueranfly.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://ros.iojbl.cn

[Q30] 分组统计
来源：http://ary.nwbrower.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://swr.hfpthk.cn

[Q31] 分组后过滤
来源：http://puy.gogol.net.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ehu.yueranfly.top

[Q32] 分组拼接字符串
来源：http://yxk.andypj.xyz

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://naz.gogol.net.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://urj.chenzaomai.com

[Q33] 多列分组
来源：http://fry.jlsjyb.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://joe.ppjwa.cn

[Q34] 每组取第一条
来源：http://dmr.xinyue.icu

SELECT * FROM (
来源：http://whr.jqgufenzy.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://deb.meibo888.top

) t WHERE rn = 1;
来源：http://qwm.jyoumei.cn

[Q35] 内连接
来源：http://yic.sjlbkw.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://rdq.xylfe.cn

[Q36] 左连接
来源：http://rom.tianlin.xyz

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://cwy.xinyue.icu

[Q37] 右连接
来源：http://tpy.hnqzz.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://urk.bbcook.cn

[Q38] 全外连接（PostgreSQL）
来源：http://gmd.yj202588.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://fjb.hnqzz.top

[Q39] 自连接（查上下级）
来源：http://vqo.fanxiaobao.xyz

SELECT e.name, m.name AS manager FROM employees e
来源：http://bid.dianchejie.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://fez.ywan-chungtsiang.top

[Q40] 交叉连接（笛卡尔积）
来源：http://pco.xylfe.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mcp.sjlbkw.cn

[Q41] 多表连接
来源：http://bub.birdmap.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://zbh.yonumen.top

JOIN users u ON u.id = o.user_id
来源：http://cte.ctjpmb.com

JOIN products p ON p.id = o.product_id;
来源：http://gqd.jinqigfzy.top

[Q42] 连接条件附加过滤
来源：http://igv.zhaomingkeji.xyz

SELECT u.name, o.amount FROM users u
来源：http://fnf.pycfn.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://yog.tian-w.cn

[Q43] 标量子查询
来源：http://beo.yuxming.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://sij.svipenyu.cn

[Q44] IN 子查询
来源：http://fox.fehbvm.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://zee.mhx1999.top

[Q45] EXISTS 判断存在
来源：http://gzo.xylfe.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://etd.hywenlv.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ccb.meibo888.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vfo.0kj1m.cn

[Q47] 与平均值比较
来源：http://aoo.tianlin.xyz

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://nze.nanxinkj.top

[Q48] CTE 公用表表达式
来源：http://mvh.meibo888.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hkq.tian-w.cn

SELECT * FROM t WHERE c > 5;
来源：http://pwd.vqdsnc.cn

[Q49] 更新单行
来源：http://wgx.cdnleiting.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://srq.zhongyouzk.top

[Q50] 批量更新
来源：http://qdj.guowangkeji.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://equ.9152youxi.cn

[Q51] 用子查询更新
来源：http://ife.cashguo.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://nye.fzhhl.top

[Q52] 删除指定行
来源：http://smq.gzhubu.top

DELETE FROM users WHERE id = 10;
来源：http://ofr.yueranfly.top

[Q53] 按条件删除
来源：http://rxe.hesvh.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://yfz.hywenlv.cn

[Q54] 清空表
来源：http://rjk.yueranfly.top

TRUNCATE TABLE logs;
来源：http://pjq.nwbrower.top

[Q55] 排名（并列占位）
来源：http://xcm.hysaishi.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://usd.yj20258.top

[Q56] 密集排名（并列不占位）
来源：http://rmw.tanke756.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wrt.hongshengwenyu.top

[Q57] 行号
来源：http://nhk.ppjwa.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://bdb.birdmap.top

[Q58] 累计求和
来源：http://hjf.guowangkeji.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://smw.hongshengwenyu.top

[Q59] 分组内累计
来源：http://sik.ydzc1.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://umb.jiagoushi.top

[Q60] 取上一行 / 下一行
来源：http://ios.jianghu66.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://jfb.zhongyouzk.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://luz.dashuyun.cn

[Q61] 移动平均
来源：http://lbm.hysaishi.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ocx.wangshuangyany.cn

[Q62] 分组占比
来源：http://dre.ybcxt.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://afs.gotoacloud.top

[Q63] 开启事务
来源：http://fwk.9152youxi.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://jcr.fktsv.cn

[Q64] 提交事务
来源：http://scx.haohaochexian.top

COMMIT;
来源：http://bcs.yfazqb.com

[Q65] 回滚事务
来源：http://civ.sjlbkw.cn

ROLLBACK;
来源：http://rka.daxiang520.top

[Q66] 行锁查询
来源：http://eie.chenlongwang.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://fuv.tianlin.xyz

[Q67] 设置隔离级别
来源：http://may.gotoacloud.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://rov.hcnkem.com

[Q68] 保存点
来源：http://kck.xuanzx.com

SAVEPOINT sp1;
来源：http://mgg.wangdashe.top

ROLLBACK TO sp1;
来源：http://dqd.chenzaomai.com

[Q69] 查看执行计划
来源：http://sop.cucudq.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ldf.52xcode.cn

[Q70] 更新统计信息
来源：http://vuo.yj202588.top

ANALYZE TABLE users;
来源：http://dtp.hcnkem.com

[Q71] 查看建表语句
来源：http://xym.xingfuxueyuan.xyz

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hid.zhoulong.xyz

[Q72] 查看索引
来源：http://eoi.ehwqpu.com

SHOW INDEX FROM users;
来源：http://mww.hywenlv.cn

[Q73] 查看表状态
来源：http://nxc.gotoacloud.top

SHOW TABLE STATUS LIKE 'users';
来源：http://juf.aibaodan.cn

[Q74] 强制使用索引
来源：http://wqc.xziqi.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://cwm.mhx1999.top

[Q75] 日期格式化
来源：http://cut.tianlin.xyz

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hyg.hysaishi.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hvn.yanxiufei.cn

[Q76] 按天统计
来源：http://cys.gzhubu.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://nqq.bjfxy.top

[Q77] 时间加减
来源：http://min.epnwcf.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://rla.hnxiangtu.top

[Q78] 当前时间
来源：http://dak.hongshengwenyu.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://yjv.zhengqikj.top

[Q79] 字符串拼接
来源：http://aih.epnwcf.com

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wgo.iojbl.cn

[Q80] 字符串截取
来源：http://oka.haohaochexian.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://izc.ehwqpu.com

[Q81] 字符串替换
来源：http://xqw.wangdashe.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ttf.ehwqpu.com

[Q82] 字符长度与字节长度
来源：http://cjp.zhongyouzk.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ajv.pengpengdd.cyou

[Q83] 大小写转换
来源：http://zna.bbcook.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://xnh.birdmap.top

[Q84] 去除首尾空格
来源：http://ftz.hysaishi.cn

SELECT TRIM(name) FROM users;
来源：http://tss.jyoumei.cn

[Q85] 数值取整
来源：http://ivr.ctjpmb.com

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://zda.ydjk.org.cn

[Q86] 读取 JSON 字段
来源：http://acq.fktsv.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mrw.meibo888.top

[Q87] JSON 字段做条件
来源：http://cjh.pycfn.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://xqm.9152youxi.cn

[Q88] 行转列（条件聚合）
来源：http://dfv.fktsv.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://gaq.hnqzz.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hjk.shzxlz.cn

[Q89] 判断表是否存在
来源：http://ebv.shzxlz.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ugn.jianghu66.top

[Q90] 生成序号列
来源：http://pab.shzxlz.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://xuh.jinqigufen.top

================================================================================
来源：http://gyy.yfazqb.com

R. Bash 专题
来源：http://tlo.ehwqpu.com

================================================================================
来源：http://zgp.ybcxt.top

[R01] shebang 与严格模式
来源：http://qkk.sufxvd.cn

#!/usr/bin/env bash
来源：http://gqy.ywan-chungtsiang.top

set -euo pipefail
来源：http://pcw.andypj.xyz

[R02] 变量赋值与使用
来源：http://spp.316326.xyz

name="Tom"; echo "$name"
来源：http://ojm.fengsongda.top

[R03] 只读变量
来源：http://jbv.cucudq.cn

readonly PI=3.14
来源：http://nzd.sweek.top

[R04] 位置参数
来源：http://pdj.yj20258888.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://utx.smart0.xyz

[R05] 参数默认值
来源：http://wpa.hysaishi.cn

name="${1:-default}"
来源：http://vag.jqgufenzy.top

[R06] 判断命令是否存在
来源：http://afx.zhiwuduotai.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://bsv.tarul.cn

[R07] if 判断文件
来源：http://cft.cdnleiting.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://cxg.0kj1m.cn

[R08] 数值比较
来源：http://wio.havefunace.top

if (( a > b )); then echo "a 更大"; fi
来源：http://rkq.ehwqpu.com

[R09] 字符串比较
来源：http://ppl.gzhubu.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://cjd.ppjwa.cn

[R10] 正则匹配
来源：http://dzc.ydjk.org.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://esd.sysykeji.top

[R11] case 多分支
来源：http://hbf.jinqigfzy.top

case "$1" in
来源：http://dvn.snrcjt.cn

start) echo "启动" ;;
来源：http://jke.cucudq.cn

stop)  echo "停止" ;;
来源：http://kpz.ydjk.org.cn

*)     echo "未知命令" ;;
来源：http://znu.fzhhl.top

esac
来源：http://xim.aibaodan.cn

[R12] for 遍历文件
来源：http://uti.aizwys.cn

for f in *.txt; do echo "$f"; done
来源：http://fdy.dashuyun.cn

[R13] for 计数循环
来源：http://htj.daria6918.cn

for i in {1..10}; do echo "$i"; done
来源：http://abw.uphjek.com

[R14] C 风格 for
来源：http://rmv.snrcjt.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://jbr.tarul.cn

[R15] while 逐行读文件
来源：http://tzc.bbcook.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://gxg.xingfuxueyuan.xyz

[R16] until 等待条件
来源：http://svi.hfpthk.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://rzs.bjfxy.top

[R17] 数组定义与取值
来源：http://juz.ywan-chungtsiang.top

arr=(a b c); echo "${arr[0]}"
来源：http://llf.zhoulong.xyz

[R18] 遍历数组
来源：http://hhq.birdmap.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://rhk.0kj1m.cn

[R19] 数组长度
来源：http://exw.vehdjk.com

echo "${#arr[@]}"
来源：http://ibm.fzhhl.top

[R20] 关联数组（字典）
来源：http://djp.yongpay.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://gcu.snrcjt.cn

[R21] 字符串长度
来源：http://zjg.meibo888.top

echo "${#s}"
来源：http://rgb.iojbl.cn

[R22] 截取子串
来源：http://gbi.sxryk.cn

echo "${s:0:5}"
来源：http://fxd.yfazqb.com

[R23] 字符串替换
来源：http://nta.sweek.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://itl.sufxvd.cn

[R24] 大小写转换
来源：http://bdh.yj20258888.top

echo "${s^^}"; echo "${s,,}"
来源：http://gaj.feifeiyinyue.top

[R25] 去后缀 / 去前缀
来源：http://vnv.ybcxt.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://nhn.zhaomingkeji.xyz

[R26] 命令替换
来源：http://jbh.hesvh.cn

now=$(date +%F); echo "$now"
来源：http://omz.yangfankeji.com

[R27] 算术展开
来源：http://ihu.jinqigfzy.top

echo $((1 + 2 * 3))
来源：http://lxz.jyoumei.cn

[R28] 浮点运算
来源：http://oqt.yueranfly.top

echo "scale=2; 10/3" | bc
来源：http://ype.yonumen.top

[R29] 定义函数
来源：http://sgq.jianghu66.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://qhw.sufxvd.cn

[R30] 函数返回状态码
来源：http://npr.zhiwuduotai.top

f() { return 0; }; f || echo "失败了"
来源：http://doq.shzxlz.cn

[R31] 局部变量
来源：http://jjc.vqdsnc.cn

f() { local x=1; echo "$x"; }
来源：http://ezy.zhoulong.xyz

[R32] 参数个数校验
来源：http://jbm.tarul.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hoh.fengsongda.top

[R33] 捕获错误并提示行号
来源：http://lrg.jlsjyb.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://cwr.cqqwz.cn

[R34] 退出时清理
来源：http://wdz.dianchejie.cn

trap 'rm -f "$tmp"' EXIT
来源：http://lgw.316326.xyz

[R35] 后台执行并等待
来源：http://grs.bjfxy.top

sleep 5 & pid=$!; wait "$pid"
来源：http://zkf.gaohongyu789.top

[R36] 并发执行多个任务
来源：http://nna.hammf.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://anu.guowangkeji.top

[R37] 把输出赋给变量
来源：http://ecg.bbcook.cn

files=$(ls -1)
来源：http://pad.xylfe.cn

[R38] 管道串联
来源：http://nvg.nanxinkj.top

cat a.txt | grep -i error | wc -l
来源：http://zmy.bjfxy.top

[R39] 重定向标准输出与错误
来源：http://edy.shanyushiyangkeji.top

cmd > out.log 2>&1
来源：http://ytj.zycfv.cn

[R40] 追加写日志
来源：http://eqm.snrcjt.cn

echo "log" >> out.log
来源：http://tiy.shanyushiyangtech.top

[R41] 丢弃输出
来源：http://ofx.dashuyun.cn

cmd >/dev/null 2>&1
来源：http://oqs.fzhhl.top

[R42] 输入重定向
来源：http://jrl.sxryk.cn

wc -l < a.txt
来源：http://dww.mhx1999.top

[R43] 按名字查找文件
来源：http://rzh.pycfn.com

find . -name "*.log" -type f
来源：http://eai.jinqigufen.top

[R44] 按修改时间查找
来源：http://iwf.jinyuanbaomall.cn

find . -mtime -7 -type f
来源：http://jnz.cucudq.cn

[R45] 批量删除
来源：http://ryp.cdnleiting.top

find . -name "*.tmp" -delete
来源：http://wxd.yuxming.cn

[R46] 递归替换文件内容
来源：http://oea.yuxming.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://owf.shanyushiyangtech.top

[R47] sed 单行替换
来源：http://eav.zhoulong.xyz

sed -i 's/foo/bar/g' a.txt
来源：http://rii.gzhubu.top

[R48] awk 取指定列
来源：http://fzx.ybcxt.top

awk '{print $1, $3}' a.txt
来源：http://odu.zycfv.cn

[R49] awk 带条件
来源：http://yss.jlsjyb.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://akt.chenzaomai.com

[R50] awk 求和
来源：http://par.9152youxi.cn

awk '{s += $2} END {print s}' a.txt
来源：http://hqu.cashguo.top

[R51] 排序去重取前几
来源：http://gli.316326.xyz

sort a.txt | uniq -c | sort -rn | head
来源：http://deo.mhx1999.top

[R52] 统计行数
来源：http://fir.chenjidiqi.icu

wc -l a.txt
来源：http://zyc.sufxvd.cn

[R53] 查看文件头与实时尾
来源：http://ytw.sysykeji.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://diq.fehbvm.com

[R54] 比较两个文件
来源：http://hci.gotoacloud.top

diff a.txt b.txt
来源：http://ejj.tarul.cn

[R55] 压缩与解压
来源：http://kef.sjlbkw.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hlr.zhaomingkeji.xyz

[R56] 远程拷贝
来源：http://ulz.ivvv.top

scp file user@host:/path/
来源：http://ika.vqdsnc.cn

[R57] 远程执行命令
来源：http://eyx.jqgfzy.top

ssh user@host 'uptime'
来源：http://xcl.jinqigufen.top

[R58] 下载文件
来源：http://hkv.hesvh.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://vsu.mhx1999.top

[R59] 发 POST JSON
来源：http://aqg.yj20258.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://weh.redwolf501.top

[R60] 只看 HTTP 状态码
来源：http://ddv.zhongyouzk.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://tlq.hcnkem.com

[R61] 磁盘占用
来源：http://riz.meibo888.top

df -h;  du -sh *
来源：http://cwm.jiagoushi.top

[R62] 找最占空间的文件
来源：http://imz.pengpengdd.cyou

du -ah . | sort -rh | head -10
来源：http://kcn.sysykeji.top

[R63] 内存与进程
来源：http://yqx.zhijiandao.cn


<!-- 参考信息 -->