代发 wailian999

SELECT * FROM users;
来源：http://zkb.aizwys.cn

[Q16] 查询指定列
来源：http://eta.sweek.top

SELECT id, name FROM users;
来源：http://mtr.fktsv.cn

[Q17] 条件查询
来源：http://pxl.hcnkem.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://vgu.cdnleiting.top

[Q18] 模糊匹配
来源：http://tvx.sxryk.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://nsj.zhengqikj.top

[Q19] 范围查询
来源：http://pls.cheryme.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://lfq.cqqwz.cn

[Q20] IN 列表
来源：http://exi.yj202588.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://lfo.52xcode.cn

[Q21] 空值判断
来源：http://eey.jqgufenzy.top

SELECT * FROM users WHERE email IS NULL;
来源：http://xva.sufxvd.cn

[Q22] 排序
来源：http://xau.guowangkeji.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ptq.ydzc1.top

[Q23] 分页
来源：http://ood.jqgfzy.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://plt.zhiwuduotai.top

[Q24] 去重
来源：http://fwr.yuanzhike.top

SELECT DISTINCT city FROM users;
来源：http://fah.tian-w.cn

[Q25] 只取前 N 条
来源：http://knc.jyoumei.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://qzw.yj202588.top

[Q26] 计数
来源：http://jrf.nanxuanxn.top

SELECT COUNT(*) FROM users;
来源：http://upq.havefunace.top

[Q27] 条件计数
来源：http://jrt.xingfuxueyuan.xyz

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://gsl.hnxiangtu.top

[Q28] 求和与平均
来源：http://tgu.guannengcc.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://tvi.daxiang520.top

[Q29] 最大最小值
来源：http://pgr.gogol.net.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://urz.gaohongyu789.top

[Q30] 分组统计
来源：http://qph.fanxiaobao.xyz

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hku.jiagoushi.top

[Q31] 分组后过滤
来源：http://rql.fehbvm.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ixw.jinyuanbaomall.cn

[Q32] 分组拼接字符串
来源：http://kaj.yangfankeji.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://xnt.daria6918.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ntq.cheryme.top

[Q33] 多列分组
来源：http://pvm.jianghu66.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://lsq.yuxming.cn

[Q34] 每组取第一条
来源：http://knp.ydjk.org.cn

SELECT * FROM (
来源：http://vpx.guannengcc.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://vmq.ctjpmb.com

) t WHERE rn = 1;
来源：http://hzt.hammf.cn

[Q35] 内连接
来源：http://pdm.sweek.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://tfj.chenlongwang.top

[Q36] 左连接
来源：http://cga.hnxiangtu.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hyp.daria6918.cn

[Q37] 右连接
来源：http://asy.yonumen.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ncb.jinqigfzy.top

[Q38] 全外连接（PostgreSQL）
来源：http://baj.yuxming.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ryg.wangdashe.top

[Q39] 自连接（查上下级）
来源：http://ovy.chenlongwang.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://wor.pengpengdd.cyou

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://tie.gzhubu.top

[Q40] 交叉连接（笛卡尔积）
来源：http://ysc.fehbvm.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://tdr.fehbvm.com

[Q41] 多表连接
来源：http://xyv.sysykeji.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://ctt.uphjek.com

JOIN users u ON u.id = o.user_id
来源：http://rop.andypj.xyz

JOIN products p ON p.id = o.product_id;
来源：http://fsr.vqdsnc.cn

[Q42] 连接条件附加过滤
来源：http://jpc.xingfuxueyuan.xyz

SELECT u.name, o.amount FROM users u
来源：http://pzy.guowangkeji.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://fgj.tarul.cn

[Q43] 标量子查询
来源：http://olb.guannengcc.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ezr.hesvh.cn

[Q44] IN 子查询
来源：http://xiw.jinqigfzy.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://pdq.yj202588.top

[Q45] EXISTS 判断存在
来源：http://uyu.shzxlz.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vpl.shanyushiyangtech.top

[Q46] NOT EXISTS 判断不存在
来源：http://acf.zdbjq.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://omu.jianghu66.top

[Q47] 与平均值比较
来源：http://rel.hywenlv.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://pjx.cdnleiting.top

[Q48] CTE 公用表表达式
来源：http://zaa.dashuyun.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://pdg.xziqi.cn

SELECT * FROM t WHERE c > 5;
来源：http://ajs.xuanzx.com

[Q49] 更新单行
来源：http://rdw.yuxming.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://guf.zhaomingkeji.xyz

[Q50] 批量更新
来源：http://ibj.snrcjt.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://puu.jianghu66.top

[Q51] 用子查询更新
来源：http://xjo.yj202588.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://dvn.hongshengwenyu.top

[Q52] 删除指定行
来源：http://vnz.hfpthk.cn

DELETE FROM users WHERE id = 10;
来源：http://yqn.kuanghao11.cn

[Q53] 按条件删除
来源：http://idy.hesvh.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://nzm.jiagoushi.top

[Q54] 清空表
来源：http://tiw.fehbvm.com

TRUNCATE TABLE logs;
来源：http://ljs.xinyue.icu

[Q55] 排名（并列占位）
来源：http://hmy.quarkkingdee.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://tpf.jinghuilouyu.cn

[Q56] 密集排名（并列不占位）
来源：http://qhu.ppjwa.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://rbx.yangfankeji.com

[Q57] 行号
来源：http://are.ydjk.org.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://tqd.havefunace.top

[Q58] 累计求和
来源：http://daq.sysykeji.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://nis.jinghuilouyu.cn

[Q59] 分组内累计
来源：http://tvd.xuanzx.com

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ncw.jqgufenzy.top

[Q60] 取上一行 / 下一行
来源：http://bis.hammf.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wct.fktsv.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://tfe.yuxming.cn

[Q61] 移动平均
来源：http://dms.tarul.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://aqz.zhongyouzk.top

[Q62] 分组占比
来源：http://jhx.ywan-chungtsiang.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://iaq.kuanghao11.cn

[Q63] 开启事务
来源：http://cmg.nwbrower.top

START TRANSACTION;                -- 或 BEGIN
来源：http://kxg.ppjwa.cn

[Q64] 提交事务
来源：http://hda.tarul.cn

COMMIT;
来源：http://zew.guowangkeji.top

[Q65] 回滚事务
来源：http://caa.smart0.xyz

ROLLBACK;
来源：http://odt.yj202588.top

[Q66] 行锁查询
来源：http://nim.sufxvd.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://onb.daxiang520.top

[Q67] 设置隔离级别
来源：http://nye.vqdsnc.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://skm.yonumen.top

[Q68] 保存点
来源：http://pns.nanxinkj.top

SAVEPOINT sp1;
来源：http://lqx.guowangkeji.top

ROLLBACK TO sp1;
来源：http://ykq.ybcxt.top

[Q69] 查看执行计划
来源：http://ngs.gotoacloud.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ajq.gotoacloud.top

[Q70] 更新统计信息
来源：http://miy.ywan-chungtsiang.top

ANALYZE TABLE users;
来源：http://kbr.epnwcf.com

[Q71] 查看建表语句
来源：http://ibj.daria6918.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://tal.ppjwa.cn

[Q72] 查看索引
来源：http://kzh.vqdsnc.cn

SHOW INDEX FROM users;
来源：http://wlu.yangfankeji.com

[Q73] 查看表状态
来源：http://avm.yonumen.top

SHOW TABLE STATUS LIKE 'users';
来源：http://xzp.hongshengwenyu.top

[Q74] 强制使用索引
来源：http://irb.gzhubu.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://pbf.nanxinkj.top

[Q75] 日期格式化
来源：http://mly.sufxvd.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://nij.snrcjt.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://iii.pengpengdd.cyou

[Q76] 按天统计
来源：http://jhx.xziqi.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://dhh.gaohongyu789.top

[Q77] 时间加减
来源：http://nsu.zhongyouzk.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://gft.tanke756.top

[Q78] 当前时间
来源：http://grm.chenlongwang.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://cor.zdqjudy.top

[Q79] 字符串拼接
来源：http://hcu.xinyue.icu

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://jdo.xingfuxueyuan.xyz

[Q80] 字符串截取
来源：http://gnu.daxiang520.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://zku.iojbl.cn

[Q81] 字符串替换
来源：http://asj.iojbl.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://waa.yj202588.top

[Q82] 字符长度与字节长度
来源：http://rsg.hammf.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://jup.quarkkingdee.top

[Q83] 大小写转换
来源：http://omu.ppjwa.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hej.zhoulong.xyz

[Q84] 去除首尾空格
来源：http://ufe.yj202588.top

SELECT TRIM(name) FROM users;
来源：http://plz.ydzc1.top

[Q85] 数值取整
来源：http://ruh.iojbl.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://sqj.kuanghao11.cn

[Q86] 读取 JSON 字段
来源：http://ayt.hongshengwenyu.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://myl.bjfxy.top

[Q87] JSON 字段做条件
来源：http://nhp.ctjpmb.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://vai.zhixingplan.top

[Q88] 行转列（条件聚合）
来源：http://uem.wangdashe.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://etg.yuxming.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://peq.cqqwz.cn

[Q89] 判断表是否存在
来源：http://biv.ybcxt.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://gwj.ybcxt.top

[Q90] 生成序号列
来源：http://lra.nanxinkj.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://opu.zhiwuduotai.top

================================================================================
来源：http://ney.c1oappe.top

R. Bash 专题
来源：http://cfy.ydzc1.top

================================================================================
来源：http://mcy.ydjk.org.cn

[R01] shebang 与严格模式
来源：http://gxx.jqgfzy.top

#!/usr/bin/env bash
来源：http://wfr.yj202588.top

set -euo pipefail
来源：http://rdf.wangdashe.top

[R02] 变量赋值与使用
来源：http://gpa.bbcook.cn

name="Tom"; echo "$name"
来源：http://tlz.chenlongwang.top

[R03] 只读变量
来源：http://vmu.iojbl.cn

readonly PI=3.14
来源：http://mky.jinyuanbaomall.cn

[R04] 位置参数
来源：http://wsr.shanyushiyangtech.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hhx.chenlongwang.top

[R05] 参数默认值
来源：http://qxr.shanyushiyangtech.top

name="${1:-default}"
来源：http://pfp.jlsjyb.cn

[R06] 判断命令是否存在
来源：http://jbq.birdmap.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://lil.yj202588.top

[R07] if 判断文件
来源：http://rrp.cashguo.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://dcz.fengsongda.top

[R08] 数值比较
来源：http://tye.epnwcf.com

if (( a > b )); then echo "a 更大"; fi
来源：http://mel.ppjwa.cn

[R09] 字符串比较
来源：http://wfz.c1oappe.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://cxk.cheryme.top

[R10] 正则匹配
来源：http://frg.wangdashe.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://job.zhengqikj.top

[R11] case 多分支
来源：http://kjo.zdqjudy.top

case "$1" in
来源：http://oqn.zhongyouzk.top

start) echo "启动" ;;
来源：http://quf.yonumen.top

stop)  echo "停止" ;;
来源：http://bpk.yueranfly.top

*)     echo "未知命令" ;;
来源：http://uyw.shanyushiyangkeji.top

esac
来源：http://jhn.iojbl.cn

[R12] for 遍历文件
来源：http://rvq.yanxiufei.cn

for f in *.txt; do echo "$f"; done
来源：http://low.mhx1999.top

[R13] for 计数循环
来源：http://maq.hammf.cn

for i in {1..10}; do echo "$i"; done
来源：http://ssf.guowangkeji.top

[R14] C 风格 for
来源：http://eyb.tian-w.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://nix.bjfxy.top

[R15] while 逐行读文件
来源：http://pms.daxiang520.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hzk.chenlongwang.top

[R16] until 等待条件
来源：http://ffk.ctjpmb.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://iuj.wangshuangyany.cn

[R17] 数组定义与取值
来源：http://jaz.shanyushiyangkeji.top

arr=(a b c); echo "${arr[0]}"
来源：http://ehu.redwolf501.top

[R18] 遍历数组
来源：http://fte.sysykeji.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://xab.yj20258.top

[R19] 数组长度
来源：http://gba.cashguo.top

echo "${#arr[@]}"
来源：http://xus.zhoulong.xyz

[R20] 关联数组（字典）
来源：http://cga.jianghu66.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://dsj.yanxiufei.cn

[R21] 字符串长度
来源：http://zif.ydjk.org.cn

echo "${#s}"
来源：http://pvj.zdbjq.cn

[R22] 截取子串
来源：http://exg.xinyue.icu

echo "${s:0:5}"
来源：http://idw.birdmap.top

[R23] 字符串替换
来源：http://eth.zhiwuduotai.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://afj.meibo888.top

[R24] 大小写转换
来源：http://nyz.cqqwz.cn

echo "${s^^}"; echo "${s,,}"
来源：http://mhx.hesvh.cn

[R25] 去后缀 / 去前缀
来源：http://nys.yj202588.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://glw.sxryk.cn

[R26] 命令替换
来源：http://azh.yuanzhike.top

now=$(date +%F); echo "$now"
来源：http://xgr.ehwqpu.com

[R27] 算术展开
来源：http://pzc.sufxvd.cn

echo $((1 + 2 * 3))
来源：http://zxe.chenzaomai.com

[R28] 浮点运算
来源：http://ysa.tanke756.top

echo "scale=2; 10/3" | bc
来源：http://std.cucudq.cn

[R29] 定义函数
来源：http://xpi.wangshuangyany.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hwn.gotoacloud.top

[R30] 函数返回状态码
来源：http://jud.jinghuilouyu.cn

f() { return 0; }; f || echo "失败了"
来源：http://wzj.jyoumei.cn

[R31] 局部变量
来源：http://grm.yanxiufei.cn

f() { local x=1; echo "$x"; }
来源：http://lok.zhengqikj.top

[R32] 参数个数校验
来源：http://mhe.zhongyouzk.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mdl.jlsjyb.cn

[R33] 捕获错误并提示行号
来源：http://ckc.smart0.xyz

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://zuv.uphjek.com

[R34] 退出时清理
来源：http://oko.yongpay.top

trap 'rm -f "$tmp"' EXIT
来源：http://utc.aibaodan.cn

[R35] 后台执行并等待
来源：http://qpn.uphjek.com

sleep 5 & pid=$!; wait "$pid"
来源：http://caa.bjfxy.top

[R36] 并发执行多个任务
来源：http://jvu.bbcook.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://olu.tianlin.xyz

[R37] 把输出赋给变量
来源：http://oxn.9152youxi.cn

files=$(ls -1)
来源：http://bkw.xuetiantiany.cn

[R38] 管道串联
来源：http://ygk.jinyuanbaomall.cn

cat a.txt | grep -i error | wc -l
来源：http://cyj.yj20258.top

[R39] 重定向标准输出与错误
来源：http://uyr.kuanghao11.cn

cmd > out.log 2>&1
来源：http://hhz.zhiwuduotai.top

[R40] 追加写日志
来源：http://wvn.cdnleiting.top

echo "log" >> out.log
来源：http://bsz.chenjidiqi.icu

[R41] 丢弃输出
来源：http://ibt.yuanzhike.top

cmd >/dev/null 2>&1
来源：http://jdi.ybcxt.top

[R42] 输入重定向
来源：http://has.hnqzz.top

wc -l < a.txt
来源：http://ylx.mhx1999.top

[R43] 按名字查找文件
来源：http://nos.cqqwz.cn

find . -name "*.log" -type f
来源：http://iga.yj20258.top

[R44] 按修改时间查找
来源：http://lwq.jqgufenzy.top

find . -mtime -7 -type f
来源：http://nzh.sxryk.cn

[R45] 批量删除
来源：http://dyu.guowangkeji.top

find . -name "*.tmp" -delete
来源：http://eat.zhoulong.xyz

[R46] 递归替换文件内容
来源：http://jzi.zhaomingkeji.xyz

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://xxj.jqgufenzy.top

[R47] sed 单行替换
来源：http://yic.zhixingplan.top

sed -i 's/foo/bar/g' a.txt
来源：http://rly.yangfankeji.com

[R48] awk 取指定列
来源：http://cdb.haohaochexian.top

awk '{print $1, $3}' a.txt
来源：http://rae.cdnleiting.top

[R49] awk 带条件
来源：http://nyx.0kj1m.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://gkf.jinqigufen.top

[R50] awk 求和
来源：http://srp.jlsjyb.cn

awk '{s += $2} END {print s}' a.txt
来源：http://klj.fengsongda.top

[R51] 排序去重取前几
来源：http://rys.xuanzx.com

sort a.txt | uniq -c | sort -rn | head
来源：http://hic.yfazqb.com

[R52] 统计行数
来源：http://oxk.jqgfzy.top

wc -l a.txt
来源：http://ovo.cashguo.top

[R53] 查看文件头与实时尾
来源：http://dbl.quarkkingdee.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://uri.ehwqpu.com

[R54] 比较两个文件
来源：http://bha.pengpengdd.cyou

diff a.txt b.txt
来源：http://gqm.daria6918.cn

[R55] 压缩与解压
来源：http://ykw.xuanzx.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://kcd.gogol.net.cn

[R56] 远程拷贝
来源：http://urr.hongshengwenyu.top

scp file user@host:/path/
来源：http://xlm.yj20258888.top

[R57] 远程执行命令
来源：http://hgo.cdnleiting.top

ssh user@host 'uptime'
来源：http://cnf.chenlongwang.top

[R58] 下载文件
来源：http://vrt.hysaishi.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://fif.hnxiangtu.top

[R59] 发 POST JSON
来源：http://mvj.chenlongwang.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://pws.shuidangran.top

[R60] 只看 HTTP 状态码
来源：http://iiw.guannengcc.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://asv.aibaodan.cn

[R61] 磁盘占用
来源：http://kfl.yj20258888.top

df -h;  du -sh *
来源：http://mck.yj20258.top

[R62] 找最占空间的文件
来源：http://juu.chenzaomai.com

du -ah . | sort -rh | head -10
来源：http://bbp.pengpengdd.cyou

[R63] 内存与进程
来源：http://iir.ybcxt.top

free -h;  ps aux | grep nginx
来源：http://jtu.yj20258.top

[R64] 结束进程
来源：http://gst.chenjidiqi.icu

kill -9 $(pgrep -f app.py)
来源：http://xii.feifeiyinyue.top

[R65] 查看端口占用
来源：http://bfr.yj20258.top


<!-- 参考信息 -->