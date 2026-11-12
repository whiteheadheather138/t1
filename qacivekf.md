代发 wailian999

SELECT * FROM users WHERE email IS NULL;
来源：http://uqs.fehbvm.com

[Q22] 排序
来源：http://ptc.epnwcf.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://jmm.jqgufenzy.top

[Q23] 分页
来源：http://woy.ctjpmb.com

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mcb.316326.xyz

[Q24] 去重
来源：http://hjn.jqgufenzy.top

SELECT DISTINCT city FROM users;
来源：http://szm.jinqigufen.top

[Q25] 只取前 N 条
来源：http://brj.jqgufenzy.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://myl.0kj1m.cn

[Q26] 计数
来源：http://qkk.xuanzx.com

SELECT COUNT(*) FROM users;
来源：http://jrq.9152youxi.cn

[Q27] 条件计数
来源：http://mvv.yuanzhike.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://dwj.xuanzx.com

[Q28] 求和与平均
来源：http://fxr.hesvh.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://rxk.nwbrower.top

[Q29] 最大最小值
来源：http://eoh.yangfankeji.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://vik.cheryme.top

[Q30] 分组统计
来源：http://shi.hongshengwenyu.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://fdw.jqgufenzy.top

[Q31] 分组后过滤
来源：http://frq.haohaochexian.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://rcq.redwolf501.top

[Q32] 分组拼接字符串
来源：http://ldg.sufxvd.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hpp.iojbl.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ohh.cucudq.cn

[Q33] 多列分组
来源：http://ndo.jinyuanbaomall.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://zfc.yvedp.cn

[Q34] 每组取第一条
来源：http://dbr.tianlin.xyz

SELECT * FROM (
来源：http://qhe.shanyushiyangkeji.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://fmb.epnwcf.com

) t WHERE rn = 1;
来源：http://fdb.zhijiandao.cn

[Q35] 内连接
来源：http://ufy.52xcode.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://jii.ybcxt.top

[Q36] 左连接
来源：http://oki.hnxiangtu.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://lac.jianghu66.top

[Q37] 右连接
来源：http://uuh.jianghu66.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://tav.bjfxy.top

[Q38] 全外连接（PostgreSQL）
来源：http://xtv.fzhhl.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ajx.ywan-chungtsiang.top

[Q39] 自连接（查上下级）
来源：http://jvx.feifeiyinyue.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://rdk.hnqzz.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://adg.haohaochexian.top

[Q40] 交叉连接（笛卡尔积）
来源：http://jnv.xylfe.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://nll.ydzc1.top

[Q41] 多表连接
来源：http://dlq.wangdashe.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://nvv.shuidangran.top

JOIN users u ON u.id = o.user_id
来源：http://hqw.mhx1999.top

JOIN products p ON p.id = o.product_id;
来源：http://zaw.dashuyun.cn

[Q42] 连接条件附加过滤
来源：http://kiz.tarul.cn

SELECT u.name, o.amount FROM users u
来源：http://sfq.yj202588.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://gsu.nwbrower.top

[Q43] 标量子查询
来源：http://wbh.fengsongda.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://len.ppjwa.cn

[Q44] IN 子查询
来源：http://dzu.yanxiufei.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://nii.ydzc1.top

[Q45] EXISTS 判断存在
来源：http://tqt.tianlin.xyz

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://nfr.andypj.xyz

[Q46] NOT EXISTS 判断不存在
来源：http://jma.zdbjq.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hmt.guowangkeji.top

[Q47] 与平均值比较
来源：http://kto.ppjwa.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://zim.cqqwz.cn

[Q48] CTE 公用表表达式
来源：http://ulh.iojbl.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://lfa.yueranfly.top

SELECT * FROM t WHERE c > 5;
来源：http://kkw.yfazqb.com

[Q49] 更新单行
来源：http://gik.yuanzhike.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://gad.ydzc1.top

[Q50] 批量更新
来源：http://ali.zhongyouzk.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://uyy.hnxiangtu.top

[Q51] 用子查询更新
来源：http://cvy.mhx1999.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ski.cashguo.top

[Q52] 删除指定行
来源：http://ykd.fzhhl.top

DELETE FROM users WHERE id = 10;
来源：http://ytf.xziqi.cn

[Q53] 按条件删除
来源：http://qcq.chenzaomai.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://zqa.fktsv.cn

[Q54] 清空表
来源：http://vbd.meibo888.top

TRUNCATE TABLE logs;
来源：http://che.mhx1999.top

[Q55] 排名（并列占位）
来源：http://txe.shanyushiyangtech.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://sud.ehwqpu.com

[Q56] 密集排名（并列不占位）
来源：http://okg.gaohongyu789.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://dup.ctjpmb.com

[Q57] 行号
来源：http://tjw.hesvh.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://obx.hywenlv.cn

[Q58] 累计求和
来源：http://eez.ydzc1.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://gxs.jinghuilouyu.cn

[Q59] 分组内累计
来源：http://cdq.fengsongda.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hal.jinqigufen.top

[Q60] 取上一行 / 下一行
来源：http://whb.uphjek.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ffu.ivvv.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://rym.tian-w.cn

[Q61] 移动平均
来源：http://exe.ivvv.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://dlu.0kj1m.cn

[Q62] 分组占比
来源：http://mrr.yj202588.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://tgh.iojbl.cn

[Q63] 开启事务
来源：http://gbs.xinyue.icu

START TRANSACTION;                -- 或 BEGIN
来源：http://szl.iojbl.cn

[Q64] 提交事务
来源：http://pty.bbcook.cn

COMMIT;
来源：http://mfa.sjlbkw.cn

[Q65] 回滚事务
来源：http://amp.snrcjt.cn

ROLLBACK;
来源：http://dnu.hesvh.cn

[Q66] 行锁查询
来源：http://arx.hesvh.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://rkj.dashuyun.cn

[Q67] 设置隔离级别
来源：http://htz.hcnkem.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://zgp.chenjidiqi.icu

[Q68] 保存点
来源：http://pgq.sysykeji.top

SAVEPOINT sp1;
来源：http://ojq.shangyingyoupin.top

ROLLBACK TO sp1;
来源：http://mwa.svipenyu.cn

[Q69] 查看执行计划
来源：http://yjy.jiagoushi.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://dgc.tian-w.cn

[Q70] 更新统计信息
来源：http://wyu.shzxlz.cn

ANALYZE TABLE users;
来源：http://cjx.guowangkeji.top

[Q71] 查看建表语句
来源：http://ide.daxiang520.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ino.sjlbkw.cn

[Q72] 查看索引
来源：http://wpf.zhiwuduotai.top

SHOW INDEX FROM users;
来源：http://ntq.nanxuanxn.top

[Q73] 查看表状态
来源：http://qim.tarul.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://xyu.jqgfzy.top

[Q74] 强制使用索引
来源：http://bne.snrcjt.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://gch.yongpay.top

[Q75] 日期格式化
来源：http://hey.pycfn.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://fhb.zhongyouzk.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://kdi.vehdjk.com

[Q76] 按天统计
来源：http://hqw.dianchejie.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://stl.c1oappe.top

[Q77] 时间加减
来源：http://gup.hongshengwenyu.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://iqa.316326.xyz

[Q78] 当前时间
来源：http://eyx.andypj.xyz

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://obl.havefunace.top

[Q79] 字符串拼接
来源：http://rvz.hammf.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hdl.daxiang520.top

[Q80] 字符串截取
来源：http://ola.hongshengwenyu.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://krq.guannengcc.top

[Q81] 字符串替换
来源：http://ybm.tianlin.xyz

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wvi.hesvh.cn

[Q82] 字符长度与字节长度
来源：http://twp.yuanzhike.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ohi.yvedp.cn

[Q83] 大小写转换
来源：http://ynw.zycfv.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://xif.shzxlz.cn

[Q84] 去除首尾空格
来源：http://kus.xylfe.cn

SELECT TRIM(name) FROM users;
来源：http://fvl.hcnkem.com

[Q85] 数值取整
来源：http://vyp.xuanzx.com

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ktz.gotoacloud.top

[Q86] 读取 JSON 字段
来源：http://nbd.fktsv.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://dta.iojbl.cn

[Q87] JSON 字段做条件
来源：http://zjc.hcnkem.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://uns.quarkkingdee.top

[Q88] 行转列（条件聚合）
来源：http://kuu.haohaochexian.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://nvz.hongshengwenyu.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://yha.feifeiyinyue.top

[Q89] 判断表是否存在
来源：http://cdi.hnxiangtu.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hmm.vehdjk.com

[Q90] 生成序号列
来源：http://oup.xinyue.icu

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://xfn.ydjk.org.cn

================================================================================
来源：http://uee.sufxvd.cn

R. Bash 专题
来源：http://dir.tanke756.top

================================================================================
来源：http://dhl.cashguo.top

[R01] shebang 与严格模式
来源：http://npw.pycfn.com

#!/usr/bin/env bash
来源：http://moo.hesvh.cn

set -euo pipefail
来源：http://maj.svipenyu.cn

[R02] 变量赋值与使用
来源：http://xdz.nwbrower.top

name="Tom"; echo "$name"
来源：http://jkm.yuanzhike.top

[R03] 只读变量
来源：http://eow.daxiang520.top

readonly PI=3.14
来源：http://afe.zhiwuduotai.top

[R04] 位置参数
来源：http://wtv.tian-w.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://vep.xuanzx.com

[R05] 参数默认值
来源：http://vkk.dashuyun.cn

name="${1:-default}"
来源：http://xzf.gaohongyu789.top

[R06] 判断命令是否存在
来源：http://bak.guowangkeji.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://jhd.aibaodan.cn

[R07] if 判断文件
来源：http://hxm.hesvh.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://zvq.zhongyouzk.top

[R08] 数值比较
来源：http://npz.jinqigufen.top

if (( a > b )); then echo "a 更大"; fi
来源：http://maj.iojbl.cn

[R09] 字符串比较
来源：http://gdx.sweek.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://pic.jianghu66.top

[R10] 正则匹配
来源：http://pjh.sjlbkw.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://djx.svipenyu.cn

[R11] case 多分支
来源：http://qfl.sxryk.cn

case "$1" in
来源：http://nax.iojbl.cn

start) echo "启动" ;;
来源：http://uzg.fktsv.cn

stop)  echo "停止" ;;
来源：http://vmq.birdmap.top

*)     echo "未知命令" ;;
来源：http://szg.hywenlv.cn

esac
来源：http://pid.zhixingplan.top

[R12] for 遍历文件
来源：http://gcu.gotoacloud.top

for f in *.txt; do echo "$f"; done
来源：http://spd.jqgufenzy.top

[R13] for 计数循环
来源：http://qbl.52xcode.cn

for i in {1..10}; do echo "$i"; done
来源：http://shi.yj202588.top

[R14] C 风格 for
来源：http://lfp.nwbrower.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://xhl.smart0.xyz

[R15] while 逐行读文件
来源：http://xva.jinqigufen.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://prf.tian-w.cn

[R16] until 等待条件
来源：http://yqb.hnxiangtu.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://bfc.vqdsnc.cn

[R17] 数组定义与取值
来源：http://flh.ivvv.top

arr=(a b c); echo "${arr[0]}"
来源：http://ook.chenzaomai.com

[R18] 遍历数组
来源：http://hqs.gogol.net.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://udd.hnxiangtu.top

[R19] 数组长度
来源：http://zbb.yuanzhike.top

echo "${#arr[@]}"
来源：http://hoh.sjlbkw.cn

[R20] 关联数组（字典）
来源：http://srl.guannengcc.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://lzx.aibaodan.cn

[R21] 字符串长度
来源：http://ieh.yj20258.top

echo "${#s}"
来源：http://ban.wangdashe.top

[R22] 截取子串
来源：http://wrg.smart0.xyz

echo "${s:0:5}"
来源：http://dxg.guannengcc.top

[R23] 字符串替换
来源：http://ubw.yuanzhike.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://qej.tarul.cn

[R24] 大小写转换
来源：http://fhl.0kj1m.cn

echo "${s^^}"; echo "${s,,}"
来源：http://jxi.yj20258.top

[R25] 去后缀 / 去前缀
来源：http://sdl.hnqzz.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://aue.mhx1999.top

[R26] 命令替换
来源：http://evx.sufxvd.cn

now=$(date +%F); echo "$now"
来源：http://sto.ivvv.top

[R27] 算术展开
来源：http://ryf.zdbjq.cn

echo $((1 + 2 * 3))
来源：http://gnd.pycfn.com

[R28] 浮点运算
来源：http://obe.hysaishi.cn

echo "scale=2; 10/3" | bc
来源：http://tbh.zhijiandao.cn

[R29] 定义函数
来源：http://chx.hcnkem.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://kkl.fengsongda.top

[R30] 函数返回状态码
来源：http://pvg.wangshuangyany.cn

f() { return 0; }; f || echo "失败了"
来源：http://kth.xziqi.cn

[R31] 局部变量
来源：http://tdy.hywenlv.cn

f() { local x=1; echo "$x"; }
来源：http://ksg.hnxiangtu.top

[R32] 参数个数校验
来源：http://las.nanxinkj.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ube.jlsjyb.cn

[R33] 捕获错误并提示行号
来源：http://toc.yueranfly.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://xoq.jiagoushi.top

[R34] 退出时清理
来源：http://tlw.yj202588.top

trap 'rm -f "$tmp"' EXIT
来源：http://wop.gogol.net.cn

[R35] 后台执行并等待
来源：http://jrg.pengpengdd.cyou

sleep 5 & pid=$!; wait "$pid"
来源：http://jzi.ctjpmb.com

[R36] 并发执行多个任务
来源：http://uxz.zhoulong.xyz

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://eeu.hnqzz.top

[R37] 把输出赋给变量
来源：http://cyp.yj20258.top

files=$(ls -1)
来源：http://fuk.ppjwa.cn

[R38] 管道串联
来源：http://luq.316326.xyz

cat a.txt | grep -i error | wc -l
来源：http://noc.fktsv.cn

[R39] 重定向标准输出与错误
来源：http://gjb.yuxming.cn

cmd > out.log 2>&1
来源：http://fym.chenlongwang.top

[R40] 追加写日志
来源：http://acm.cashguo.top

echo "log" >> out.log
来源：http://ctn.bjfxy.top

[R41] 丢弃输出
来源：http://aji.tian-w.cn

cmd >/dev/null 2>&1
来源：http://upr.hongshengwenyu.top

[R42] 输入重定向
来源：http://lab.jyoumei.cn

wc -l < a.txt
来源：http://xsy.cqqwz.cn

[R43] 按名字查找文件
来源：http://kxm.yfazqb.com

find . -name "*.log" -type f
来源：http://mkf.ydjk.org.cn

[R44] 按修改时间查找
来源：http://ocr.sysykeji.top

find . -mtime -7 -type f
来源：http://elh.yanxiufei.cn

[R45] 批量删除
来源：http://nvc.yj20258888.top

find . -name "*.tmp" -delete
来源：http://pcs.uphjek.com

[R46] 递归替换文件内容
来源：http://tyz.haohaochexian.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ben.nanxinkj.top

[R47] sed 单行替换
来源：http://avn.daxiang520.top

sed -i 's/foo/bar/g' a.txt
来源：http://xxy.wangshuangyany.cn

[R48] awk 取指定列
来源：http://ciu.zhongyouzk.top

awk '{print $1, $3}' a.txt
来源：http://kdx.jlsjyb.cn

[R49] awk 带条件
来源：http://dym.fehbvm.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://cts.shanyushiyangkeji.top

[R50] awk 求和
来源：http://yut.chenjidiqi.icu

awk '{s += $2} END {print s}' a.txt
来源：http://oxd.jyoumei.cn

[R51] 排序去重取前几
来源：http://ehb.jyoumei.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://zcg.chenlongwang.top

[R52] 统计行数
来源：http://jph.316326.xyz

wc -l a.txt
来源：http://xaf.guowangkeji.top

[R53] 查看文件头与实时尾
来源：http://ick.quarkkingdee.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://bvo.jianghu66.top

[R54] 比较两个文件
来源：http://mot.tianlin.xyz

diff a.txt b.txt
来源：http://ral.nwbrower.top

[R55] 压缩与解压
来源：http://qht.shanyushiyangtech.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://zex.ywan-chungtsiang.top

[R56] 远程拷贝
来源：http://uch.daria6918.cn

scp file user@host:/path/
来源：http://jhg.haohaochexian.top

[R57] 远程执行命令
来源：http://jud.redwolf501.top

ssh user@host 'uptime'
来源：http://pbg.jinyuanbaomall.cn

[R58] 下载文件
来源：http://pcj.aizwys.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mkh.chenjidiqi.icu

[R59] 发 POST JSON
来源：http://odn.yfazqb.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://pmn.daria6918.cn

[R60] 只看 HTTP 状态码
来源：http://arp.jianghu66.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://icy.hesvh.cn

[R61] 磁盘占用
来源：http://fsm.dashuyun.cn

df -h;  du -sh *
来源：http://sbv.bjfxy.top

[R62] 找最占空间的文件
来源：http://lsf.yfazqb.com

du -ah . | sort -rh | head -10
来源：http://iju.cdnleiting.top

[R63] 内存与进程
来源：http://puo.zhaomingkeji.xyz

free -h;  ps aux | grep nginx
来源：http://nik.havefunace.top

[R64] 结束进程
来源：http://yaq.hesvh.cn

kill -9 $(pgrep -f app.py)
来源：http://pmo.zhiwuduotai.top

[R65] 查看端口占用
来源：http://krc.ppjwa.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://nbq.gzhubu.top

[R66] 定时任务
来源：http://vze.zhongyouzk.top

crontab -e;  crontab -l
来源：http://utg.nanxinkj.top

[R67] 生成随机十六进制串
来源：http://vzn.ppjwa.cn

openssl rand -hex 16
来源：http://vuu.wangdashe.top

[R68] 计算文件校验值
来源：http://thn.zhijiandao.cn

sha256sum a.txt;  md5sum a.txt
来源：http://gra.haohaochexian.top

[R69] 生成随机密码
来源：http://yck.hfpthk.cn

head -c 16 /dev/urandom | base64
来源：http://hlh.c1oappe.top

[R70] 时间戳与互转
来源：http://sor.yj20258888.top

date +%s;  date -d @1700000000
来源：http://vty.hfpthk.cn

[R71] 日期格式化
来源：http://mrm.cheryme.top


<!-- 参考信息 -->