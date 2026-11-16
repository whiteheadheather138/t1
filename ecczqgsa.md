代发 wailian999

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://yne.jinqigufen.top

[Q18] 模糊匹配
来源：http://vmd.hnqzz.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://qhr.yueranfly.top

[Q19] 范围查询
来源：http://vvm.tian-w.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://yrb.nanxinkj.top

[Q20] IN 列表
来源：http://jqy.xuetiantiany.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://lok.zhiwuduotai.top

[Q21] 空值判断
来源：http://eqt.jqgfzy.top

SELECT * FROM users WHERE email IS NULL;
来源：http://jrz.dianchejie.cn

[Q22] 排序
来源：http://jkc.hesvh.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://gwn.yfazqb.com

[Q23] 分页
来源：http://txz.tanke756.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://gdm.yvedp.cn

[Q24] 去重
来源：http://voi.gotoacloud.top

SELECT DISTINCT city FROM users;
来源：http://znp.sxryk.cn

[Q25] 只取前 N 条
来源：http://fem.yanxiufei.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wkj.dianchejie.cn

[Q26] 计数
来源：http://kdy.shuidangran.top

SELECT COUNT(*) FROM users;
来源：http://geq.jinqigfzy.top

[Q27] 条件计数
来源：http://jyk.chenjidiqi.icu

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wra.jianghu66.top

[Q28] 求和与平均
来源：http://kkl.haohaochexian.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wjf.jianghu66.top

[Q29] 最大最小值
来源：http://qit.xinyue.icu

SELECT MAX(age), MIN(age) FROM users;
来源：http://seg.daxiang520.top

[Q30] 分组统计
来源：http://qdn.jlsjyb.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ssl.cashguo.top

[Q31] 分组后过滤
来源：http://lal.yfazqb.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://gbf.tian-w.cn

[Q32] 分组拼接字符串
来源：http://oxb.jyoumei.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wgn.jinqigfzy.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://tkt.fzhhl.top

[Q33] 多列分组
来源：http://rkg.xylfe.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://cqz.pengpengdd.cyou

[Q34] 每组取第一条
来源：http://gmk.xinyue.icu

SELECT * FROM (
来源：http://mhn.zhongyouzk.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://bij.316326.xyz

) t WHERE rn = 1;
来源：http://hsm.0kj1m.cn

[Q35] 内连接
来源：http://cmv.kuanghao11.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://oxi.jianghu66.top

[Q36] 左连接
来源：http://xqg.zhoulong.xyz

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://fsx.xziqi.cn

[Q37] 右连接
来源：http://muv.pengpengdd.cyou

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://bmm.guannengcc.top

[Q38] 全外连接（PostgreSQL）
来源：http://soe.snrcjt.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ryc.dianchejie.cn

[Q39] 自连接（查上下级）
来源：http://dec.sjlbkw.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://sqs.ydjk.org.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hib.zhongyouzk.top

[Q40] 交叉连接（笛卡尔积）
来源：http://wft.zhixingplan.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://dkh.fzhhl.top

[Q41] 多表连接
来源：http://hdn.xuetiantiany.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://cgb.sxryk.cn

JOIN users u ON u.id = o.user_id
来源：http://css.zhiwuduotai.top

JOIN products p ON p.id = o.product_id;
来源：http://isu.9152youxi.cn

[Q42] 连接条件附加过滤
来源：http://uwr.ctjpmb.com

SELECT u.name, o.amount FROM users u
来源：http://awo.pengpengdd.cyou

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://oyb.ppjwa.cn

[Q43] 标量子查询
来源：http://xdr.shuidangran.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://szo.cqqwz.cn

[Q44] IN 子查询
来源：http://whd.9152youxi.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://zrf.hywenlv.cn

[Q45] EXISTS 判断存在
来源：http://hzg.cqqwz.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://tbh.fanxiaobao.xyz

[Q46] NOT EXISTS 判断不存在
来源：http://pgp.hysaishi.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vdc.epnwcf.com

[Q47] 与平均值比较
来源：http://xzh.yvedp.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://fbd.xingfuxueyuan.xyz

[Q48] CTE 公用表表达式
来源：http://oks.yfazqb.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wrp.chenzaomai.com

SELECT * FROM t WHERE c > 5;
来源：http://lgt.aizwys.cn

[Q49] 更新单行
来源：http://pbb.redwolf501.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://vta.hywenlv.cn

[Q50] 批量更新
来源：http://iub.yueranfly.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://kqp.gotoacloud.top

[Q51] 用子查询更新
来源：http://tfs.zhijiandao.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://exb.cqqwz.cn

[Q52] 删除指定行
来源：http://pog.quarkkingdee.top

DELETE FROM users WHERE id = 10;
来源：http://sjf.0kj1m.cn

[Q53] 按条件删除
来源：http://czx.ctjpmb.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://zpb.shangyingyoupin.top

[Q54] 清空表
来源：http://rld.zhongyouzk.top

TRUNCATE TABLE logs;
来源：http://poz.fanxiaobao.xyz

[Q55] 排名（并列占位）
来源：http://iqd.xingfuxueyuan.xyz

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ren.hnqzz.top

[Q56] 密集排名（并列不占位）
来源：http://ijs.cqqwz.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://nsy.wangshuangyany.cn

[Q57] 行号
来源：http://jba.tianlin.xyz

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://qsj.zdqjudy.top

[Q58] 累计求和
来源：http://ekn.zdbjq.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://gkn.0kj1m.cn

[Q59] 分组内累计
来源：http://lnt.aibaodan.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://gfp.cqqwz.cn

[Q60] 取上一行 / 下一行
来源：http://zuo.smart0.xyz

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://lmv.ydzc1.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://djv.gogol.net.cn

[Q61] 移动平均
来源：http://yeg.iojbl.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://upl.yuanzhike.top

[Q62] 分组占比
来源：http://zkw.uphjek.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://jbc.zhijiandao.cn

[Q63] 开启事务
来源：http://lvy.cdnleiting.top

START TRANSACTION;                -- 或 BEGIN
来源：http://owt.redwolf501.top

[Q64] 提交事务
来源：http://fuw.hongshengwenyu.top

COMMIT;
来源：http://awt.iojbl.cn

[Q65] 回滚事务
来源：http://abf.tarul.cn

ROLLBACK;
来源：http://bwf.havefunace.top

[Q66] 行锁查询
来源：http://gih.pycfn.com

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://vdt.hcnkem.com

[Q67] 设置隔离级别
来源：http://sla.hywenlv.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://lcl.jqgfzy.top

[Q68] 保存点
来源：http://dxc.daxiang520.top

SAVEPOINT sp1;
来源：http://zwt.zdqjudy.top

ROLLBACK TO sp1;
来源：http://lpz.yfazqb.com

[Q69] 查看执行计划
来源：http://okf.ydjk.org.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://lsj.fzhhl.top

[Q70] 更新统计信息
来源：http://fke.vehdjk.com

ANALYZE TABLE users;
来源：http://iuq.cheryme.top

[Q71] 查看建表语句
来源：http://zdi.shuidangran.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://giq.jqgfzy.top

[Q72] 查看索引
来源：http://dko.epnwcf.com

SHOW INDEX FROM users;
来源：http://uuh.jinghuilouyu.cn

[Q73] 查看表状态
来源：http://xtn.tian-w.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://rqv.gzhubu.top

[Q74] 强制使用索引
来源：http://nuk.haohaochexian.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://tyu.fktsv.cn

[Q75] 日期格式化
来源：http://ljb.zhijiandao.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://bhp.zhengqikj.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://omu.fktsv.cn

[Q76] 按天统计
来源：http://wsr.xylfe.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://gpo.fehbvm.com

[Q77] 时间加减
来源：http://qdr.wangdashe.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://bqm.hnxiangtu.top

[Q78] 当前时间
来源：http://jhq.tarul.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://dsr.zdqjudy.top

[Q79] 字符串拼接
来源：http://bnr.jinghuilouyu.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://lcw.birdmap.top

[Q80] 字符串截取
来源：http://lnh.0kj1m.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://oyy.gzhubu.top

[Q81] 字符串替换
来源：http://bid.jianghu66.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://pvr.andypj.xyz

[Q82] 字符长度与字节长度
来源：http://cng.ivvv.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mgc.shanyushiyangkeji.top

[Q83] 大小写转换
来源：http://xvi.xingfuxueyuan.xyz

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wac.fehbvm.com

[Q84] 去除首尾空格
来源：http://ilp.xylfe.cn

SELECT TRIM(name) FROM users;
来源：http://jar.uphjek.com

[Q85] 数值取整
来源：http://tan.zhoulong.xyz

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://bem.yongpay.top

[Q86] 读取 JSON 字段
来源：http://xcu.feifeiyinyue.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://kui.316326.xyz

[Q87] JSON 字段做条件
来源：http://pxd.gotoacloud.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://vpw.cdnleiting.top

[Q88] 行转列（条件聚合）
来源：http://pue.cqqwz.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://bvg.cashguo.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://xca.tarul.cn

[Q89] 判断表是否存在
来源：http://bzo.vqdsnc.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://bjt.feifeiyinyue.top

[Q90] 生成序号列
来源：http://isa.tianlin.xyz

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://gme.52xcode.cn

================================================================================
来源：http://xdc.mhx1999.top

R. Bash 专题
来源：http://law.cheryme.top

================================================================================
来源：http://yot.yongpay.top

[R01] shebang 与严格模式
来源：http://qgs.ppjwa.cn

#!/usr/bin/env bash
来源：http://mkh.sysykeji.top

set -euo pipefail
来源：http://mmd.zdqjudy.top

[R02] 变量赋值与使用
来源：http://qqf.jqgfzy.top

name="Tom"; echo "$name"
来源：http://hvp.iojbl.cn

[R03] 只读变量
来源：http://jhi.wangshuangyany.cn

readonly PI=3.14
来源：http://sxu.wangdashe.top

[R04] 位置参数
来源：http://ccf.shuidangran.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ech.jinqigfzy.top

[R05] 参数默认值
来源：http://jxo.316326.xyz

name="${1:-default}"
来源：http://hol.zhijiandao.cn

[R06] 判断命令是否存在
来源：http://gqs.dashuyun.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://yth.ydzc1.top

[R07] if 判断文件
来源：http://soj.0kj1m.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://nxy.daxiang520.top

[R08] 数值比较
来源：http://fmj.gotoacloud.top

if (( a > b )); then echo "a 更大"; fi
来源：http://ilr.shanyushiyangkeji.top

[R09] 字符串比较
来源：http://gsw.hfpthk.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://axu.ydjk.org.cn

[R10] 正则匹配
来源：http://xdt.gogol.net.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ulw.xingfuxueyuan.xyz

[R11] case 多分支
来源：http://nhn.cqqwz.cn

case "$1" in
来源：http://fjn.tian-w.cn

start) echo "启动" ;;
来源：http://ltn.vehdjk.com

stop)  echo "停止" ;;
来源：http://fal.zdqjudy.top

*)     echo "未知命令" ;;
来源：http://zuz.iojbl.cn

esac
来源：http://xgd.yvedp.cn

[R12] for 遍历文件
来源：http://iqx.chenzaomai.com

for f in *.txt; do echo "$f"; done
来源：http://vhi.52xcode.cn

[R13] for 计数循环
来源：http://krq.ybcxt.top

for i in {1..10}; do echo "$i"; done
来源：http://pta.hywenlv.cn

[R14] C 风格 for
来源：http://dfx.ehwqpu.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://aat.yuxming.cn

[R15] while 逐行读文件
来源：http://ygt.zhiwuduotai.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://gwz.jqgfzy.top

[R16] until 等待条件
来源：http://cqp.c1oappe.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mfv.sweek.top

[R17] 数组定义与取值
来源：http://lxk.xingfuxueyuan.xyz

arr=(a b c); echo "${arr[0]}"
来源：http://wxq.smart0.xyz

[R18] 遍历数组
来源：http://efk.wangdashe.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wph.svipenyu.cn

[R19] 数组长度
来源：http://pel.jianghu66.top

echo "${#arr[@]}"
来源：http://eem.yvedp.cn

[R20] 关联数组（字典）
来源：http://quv.shuidangran.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://gix.yonumen.top

[R21] 字符串长度
来源：http://vhm.hnqzz.top

echo "${#s}"
来源：http://hav.wangdashe.top

[R22] 截取子串
来源：http://uxs.dashuyun.cn

echo "${s:0:5}"
来源：http://sqg.uphjek.com

[R23] 字符串替换
来源：http://dhw.ydzc1.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://fiv.cqqwz.cn

[R24] 大小写转换
来源：http://riv.yj202588.top

echo "${s^^}"; echo "${s,,}"
来源：http://qoj.xuetiantiany.cn

[R25] 去后缀 / 去前缀
来源：http://qik.zdbjq.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://oxo.hnqzz.top

[R26] 命令替换
来源：http://ziq.shzxlz.cn

now=$(date +%F); echo "$now"
来源：http://nmj.jlsjyb.cn

[R27] 算术展开
来源：http://dvz.316326.xyz

echo $((1 + 2 * 3))
来源：http://gfv.wangdashe.top

[R28] 浮点运算
来源：http://agk.dianchejie.cn

echo "scale=2; 10/3" | bc
来源：http://gzg.hammf.cn

[R29] 定义函数
来源：http://cng.zhongyouzk.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://tgw.xziqi.cn

[R30] 函数返回状态码
来源：http://avt.chenlongwang.top

f() { return 0; }; f || echo "失败了"
来源：http://jyv.ybcxt.top

[R31] 局部变量
来源：http://gur.nanxinkj.top

f() { local x=1; echo "$x"; }
来源：http://swy.9152youxi.cn

[R32] 参数个数校验
来源：http://hmn.jiagoushi.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://zgf.gogol.net.cn

[R33] 捕获错误并提示行号
来源：http://qbl.daria6918.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://alj.cheryme.top

[R34] 退出时清理
来源：http://yba.jinghuilouyu.cn

trap 'rm -f "$tmp"' EXIT
来源：http://lin.kuanghao11.cn

[R35] 后台执行并等待
来源：http://knr.xylfe.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://mlp.sxryk.cn

[R36] 并发执行多个任务
来源：http://zke.uphjek.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://tgt.yuanzhike.top

[R37] 把输出赋给变量
来源：http://nmc.jinghuilouyu.cn

files=$(ls -1)
来源：http://bpw.chenjidiqi.icu

[R38] 管道串联
来源：http://fqm.guowangkeji.top

cat a.txt | grep -i error | wc -l
来源：http://vsl.wangdashe.top

[R39] 重定向标准输出与错误
来源：http://mie.ctjpmb.com

cmd > out.log 2>&1
来源：http://hbw.zdqjudy.top

[R40] 追加写日志
来源：http://rui.hywenlv.cn

echo "log" >> out.log
来源：http://smy.redwolf501.top

[R41] 丢弃输出
来源：http://kud.hfpthk.cn

cmd >/dev/null 2>&1
来源：http://eer.zycfv.cn

[R42] 输入重定向
来源：http://fhf.gotoacloud.top

wc -l < a.txt
来源：http://srv.jinghuilouyu.cn

[R43] 按名字查找文件
来源：http://xug.aibaodan.cn

find . -name "*.log" -type f
来源：http://dct.birdmap.top

[R44] 按修改时间查找
来源：http://jjz.dashuyun.cn

find . -mtime -7 -type f
来源：http://irp.aizwys.cn

[R45] 批量删除
来源：http://ixx.sjlbkw.cn

find . -name "*.tmp" -delete
来源：http://uwv.ivvv.top

[R46] 递归替换文件内容
来源：http://alt.zhoulong.xyz

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://zvc.yj202588.top

[R47] sed 单行替换
来源：http://kdt.kuanghao11.cn

sed -i 's/foo/bar/g' a.txt
来源：http://yjy.bbcook.cn

[R48] awk 取指定列
来源：http://uvc.vehdjk.com

awk '{print $1, $3}' a.txt
来源：http://xlf.0kj1m.cn

[R49] awk 带条件
来源：http://ihq.wangdashe.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://uqw.chenjidiqi.icu

[R50] awk 求和
来源：http://vei.xuetiantiany.cn

awk '{s += $2} END {print s}' a.txt
来源：http://jec.ydjk.org.cn

[R51] 排序去重取前几
来源：http://ppz.0kj1m.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://thu.daxiang520.top

[R52] 统计行数
来源：http://axj.havefunace.top

wc -l a.txt
来源：http://pnw.sufxvd.cn

[R53] 查看文件头与实时尾
来源：http://phb.yj20258.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://cbp.chenjidiqi.icu

[R54] 比较两个文件
来源：http://ylw.ivvv.top

diff a.txt b.txt
来源：http://mmi.xinyue.icu

[R55] 压缩与解压
来源：http://mwg.jinyuanbaomall.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://xeg.gogol.net.cn

[R56] 远程拷贝
来源：http://tmr.ppjwa.cn

scp file user@host:/path/
来源：http://hdd.hcnkem.com

[R57] 远程执行命令
来源：http://byu.cucudq.cn

ssh user@host 'uptime'
来源：http://msp.yangfankeji.com

[R58] 下载文件
来源：http://iiz.cheryme.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ysq.gaohongyu789.top

[R59] 发 POST JSON
来源：http://lxa.smart0.xyz

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://pru.shanyushiyangkeji.top

[R60] 只看 HTTP 状态码
来源：http://zvr.zhoulong.xyz

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://gsf.ivvv.top

[R61] 磁盘占用
来源：http://gqb.chenjidiqi.icu

df -h;  du -sh *
来源：http://znn.yj20258.top

[R62] 找最占空间的文件
来源：http://cec.chenzaomai.com

du -ah . | sort -rh | head -10
来源：http://bxp.shangyingyoupin.top

[R63] 内存与进程
来源：http://jkt.vqdsnc.cn

free -h;  ps aux | grep nginx
来源：http://npm.sjlbkw.cn

[R64] 结束进程
来源：http://kcu.wangshuangyany.cn

kill -9 $(pgrep -f app.py)
来源：http://ynw.hongshengwenyu.top

[R65] 查看端口占用
来源：http://puk.fktsv.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://zuw.vqdsnc.cn

[R66] 定时任务
来源：http://txg.zhiwuduotai.top

crontab -e;  crontab -l
来源：http://akb.yueranfly.top

[R67] 生成随机十六进制串
来源：http://yus.snrcjt.cn


<!-- 参考信息 -->