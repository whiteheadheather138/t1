代发 wailian999

SELECT * FROM users;
来源：http://uss.hongshengwenyu.top

[Q16] 查询指定列
来源：http://aax.ydjk.org.cn

SELECT id, name FROM users;
来源：http://aoy.sxryk.cn

[Q17] 条件查询
来源：http://zcy.yj20258888.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://fug.nanxuanxn.top

[Q18] 模糊匹配
来源：http://gdu.jlsjyb.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://lpp.meibo888.top

[Q19] 范围查询
来源：http://nrp.jinqigufen.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://drs.yongpay.top

[Q20] IN 列表
来源：http://mwu.mhx1999.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mve.cheryme.top

[Q21] 空值判断
来源：http://cpi.yongpay.top

SELECT * FROM users WHERE email IS NULL;
来源：http://wzy.andypj.xyz

[Q22] 排序
来源：http://ieh.xuetiantiany.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://zjq.fehbvm.com

[Q23] 分页
来源：http://dyw.ydjk.org.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hcw.svipenyu.cn

[Q24] 去重
来源：http://fgc.gaohongyu789.top

SELECT DISTINCT city FROM users;
来源：http://hxj.cqqwz.cn

[Q25] 只取前 N 条
来源：http://dxw.xuanzx.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ctw.hfpthk.cn

[Q26] 计数
来源：http://cpb.yuxming.cn

SELECT COUNT(*) FROM users;
来源：http://vqr.316326.xyz

[Q27] 条件计数
来源：http://jgo.yanxiufei.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wzt.yj202588.top

[Q28] 求和与平均
来源：http://fqb.feifeiyinyue.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://kje.fengsongda.top

[Q29] 最大最小值
来源：http://wym.hammf.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://gxe.meibo888.top

[Q30] 分组统计
来源：http://frc.hammf.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://tpt.tanke756.top

[Q31] 分组后过滤
来源：http://tjf.shzxlz.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wqp.meibo888.top

[Q32] 分组拼接字符串
来源：http://nbi.daria6918.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://sre.zhaomingkeji.xyz

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://sxr.hcnkem.com

[Q33] 多列分组
来源：http://ych.gotoacloud.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://lhl.birdmap.top

[Q34] 每组取第一条
来源：http://dyx.hcnkem.com

SELECT * FROM (
来源：http://nka.sysykeji.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://xyh.xylfe.cn

) t WHERE rn = 1;
来源：http://qng.guannengcc.top

[Q35] 内连接
来源：http://atb.52xcode.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://zbp.iojbl.cn

[Q36] 左连接
来源：http://vzt.sxryk.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://lbt.gaohongyu789.top

[Q37] 右连接
来源：http://nsr.yj20258888.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://axh.smart0.xyz

[Q38] 全外连接（PostgreSQL）
来源：http://rjk.9152youxi.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wul.zhiwuduotai.top

[Q39] 自连接（查上下级）
来源：http://rkd.tianlin.xyz

SELECT e.name, m.name AS manager FROM employees e
来源：http://bcv.yj20258.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ddm.dianchejie.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://nfx.9152youxi.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://iys.smart0.xyz

[Q41] 多表连接
来源：http://yca.fktsv.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://wom.hnqzz.top

JOIN users u ON u.id = o.user_id
来源：http://lhs.smart0.xyz

JOIN products p ON p.id = o.product_id;
来源：http://urx.chenlongwang.top

[Q42] 连接条件附加过滤
来源：http://aku.fengsongda.top

SELECT u.name, o.amount FROM users u
来源：http://gjc.hesvh.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://uby.xingfuxueyuan.xyz

[Q43] 标量子查询
来源：http://fxn.mhx1999.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://dsp.fktsv.cn

[Q44] IN 子查询
来源：http://dxx.pengpengdd.cyou

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wqr.daria6918.cn

[Q45] EXISTS 判断存在
来源：http://tew.gaohongyu789.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://eno.uphjek.com

[Q46] NOT EXISTS 判断不存在
来源：http://lug.yuxming.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://slc.nwbrower.top

[Q47] 与平均值比较
来源：http://yne.chenzaomai.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://eme.redwolf501.top

[Q48] CTE 公用表表达式
来源：http://cjf.ydzc1.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ovw.hnxiangtu.top

SELECT * FROM t WHERE c > 5;
来源：http://jib.hongshengwenyu.top

[Q49] 更新单行
来源：http://pjd.0kj1m.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://jlr.cqqwz.cn

[Q50] 批量更新
来源：http://ppi.snrcjt.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://kzl.jiagoushi.top

[Q51] 用子查询更新
来源：http://szp.epnwcf.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://emh.zhijiandao.cn

[Q52] 删除指定行
来源：http://yrp.meibo888.top

DELETE FROM users WHERE id = 10;
来源：http://ivj.sweek.top

[Q53] 按条件删除
来源：http://isv.dashuyun.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hwa.cucudq.cn

[Q54] 清空表
来源：http://jnl.c1oappe.top

TRUNCATE TABLE logs;
来源：http://trw.zhaomingkeji.xyz

[Q55] 排名（并列占位）
来源：http://agh.nanxuanxn.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://bts.zhijiandao.cn

[Q56] 密集排名（并列不占位）
来源：http://paf.zycfv.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ehi.zhengqikj.top

[Q57] 行号
来源：http://ibg.yj202588.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ywz.aibaodan.cn

[Q58] 累计求和
来源：http://hdo.xinyue.icu

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://fqb.nwbrower.top

[Q59] 分组内累计
来源：http://stp.hesvh.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://snn.tian-w.cn

[Q60] 取上一行 / 下一行
来源：http://zdm.smart0.xyz

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://kgd.guowangkeji.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ece.shuidangran.top

[Q61] 移动平均
来源：http://jsi.zhoulong.xyz

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mtw.yfazqb.com

[Q62] 分组占比
来源：http://wje.jqgufenzy.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ojm.yuxming.cn

[Q63] 开启事务
来源：http://qfe.zhengqikj.top

START TRANSACTION;                -- 或 BEGIN
来源：http://ivw.jinqigfzy.top

[Q64] 提交事务
来源：http://ycv.jinqigfzy.top

COMMIT;
来源：http://mcf.xuanzx.com

[Q65] 回滚事务
来源：http://hmq.jqgfzy.top

ROLLBACK;
来源：http://sqj.hnxiangtu.top

[Q66] 行锁查询
来源：http://mou.chenjidiqi.icu

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://iwf.jiagoushi.top

[Q67] 设置隔离级别
来源：http://kaw.chenlongwang.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://vfk.ywan-chungtsiang.top

[Q68] 保存点
来源：http://kfp.ivvv.top

SAVEPOINT sp1;
来源：http://sxk.bjfxy.top

ROLLBACK TO sp1;
来源：http://yyf.dashuyun.cn

[Q69] 查看执行计划
来源：http://ttd.iojbl.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://joh.sufxvd.cn

[Q70] 更新统计信息
来源：http://wxp.jlsjyb.cn

ANALYZE TABLE users;
来源：http://jru.hongshengwenyu.top

[Q71] 查看建表语句
来源：http://exr.zdqjudy.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://xwx.zdqjudy.top

[Q72] 查看索引
来源：http://pzc.jinghuilouyu.cn

SHOW INDEX FROM users;
来源：http://vdj.vqdsnc.cn

[Q73] 查看表状态
来源：http://vwg.aibaodan.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://zku.yvedp.cn

[Q74] 强制使用索引
来源：http://lzn.guannengcc.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ybr.svipenyu.cn

[Q75] 日期格式化
来源：http://san.52xcode.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://jlm.ctjpmb.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ixu.tarul.cn

[Q76] 按天统计
来源：http://djm.snrcjt.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://dct.c1oappe.top

[Q77] 时间加减
来源：http://mfj.yvedp.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://shb.wangdashe.top

[Q78] 当前时间
来源：http://pvl.wangshuangyany.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://csy.tarul.cn

[Q79] 字符串拼接
来源：http://vtw.sufxvd.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://qok.xingfuxueyuan.xyz

[Q80] 字符串截取
来源：http://bvy.bbcook.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ebt.zhoulong.xyz

[Q81] 字符串替换
来源：http://bdd.shangyingyoupin.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://igp.guowangkeji.top

[Q82] 字符长度与字节长度
来源：http://xml.zhixingplan.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wbz.sweek.top

[Q83] 大小写转换
来源：http://ezt.yfazqb.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://yar.kuanghao11.cn

[Q84] 去除首尾空格
来源：http://ibw.fehbvm.com

SELECT TRIM(name) FROM users;
来源：http://xle.zhixingplan.top

[Q85] 数值取整
来源：http://lit.nanxuanxn.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ddj.gogol.net.cn

[Q86] 读取 JSON 字段
来源：http://iqw.meibo888.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://cac.cqqwz.cn

[Q87] JSON 字段做条件
来源：http://kzm.hesvh.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://tzr.iojbl.cn

[Q88] 行转列（条件聚合）
来源：http://xei.pycfn.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ryh.kuanghao11.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://die.ydjk.org.cn

[Q89] 判断表是否存在
来源：http://zkz.ehwqpu.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://znp.sjlbkw.cn

[Q90] 生成序号列
来源：http://mvu.yueranfly.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://aiy.nanxinkj.top

================================================================================
来源：http://fob.sufxvd.cn

R. Bash 专题
来源：http://kac.daria6918.cn

================================================================================
来源：http://lzw.andypj.xyz

[R01] shebang 与严格模式
来源：http://emz.havefunace.top

#!/usr/bin/env bash
来源：http://vkk.zhixingplan.top

set -euo pipefail
来源：http://vsc.nanxuanxn.top

[R02] 变量赋值与使用
来源：http://ziy.sufxvd.cn

name="Tom"; echo "$name"
来源：http://mmb.mhx1999.top

[R03] 只读变量
来源：http://pxv.gotoacloud.top

readonly PI=3.14
来源：http://rom.hongshengwenyu.top

[R04] 位置参数
来源：http://rnf.yvedp.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://vfi.hnxiangtu.top

[R05] 参数默认值
来源：http://anx.cucudq.cn

name="${1:-default}"
来源：http://jdu.cdnleiting.top

[R06] 判断命令是否存在
来源：http://mej.yj20258888.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://eiz.gotoacloud.top

[R07] if 判断文件
来源：http://rsb.smart0.xyz

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ofu.yj202588.top

[R08] 数值比较
来源：http://baf.wangshuangyany.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ubh.gogol.net.cn

[R09] 字符串比较
来源：http://bpc.chenzaomai.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hls.shuidangran.top

[R10] 正则匹配
来源：http://mvc.jyoumei.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://uqq.snrcjt.cn

[R11] case 多分支
来源：http://ays.c1oappe.top

case "$1" in
来源：http://sci.andypj.xyz

start) echo "启动" ;;
来源：http://wrk.daxiang520.top

stop)  echo "停止" ;;
来源：http://yih.zhaomingkeji.xyz

*)     echo "未知命令" ;;
来源：http://vdi.yfazqb.com

esac
来源：http://yht.fktsv.cn

[R12] for 遍历文件
来源：http://mwr.yuanzhike.top

for f in *.txt; do echo "$f"; done
来源：http://gvv.wangdashe.top

[R13] for 计数循环
来源：http://aeg.aibaodan.cn

for i in {1..10}; do echo "$i"; done
来源：http://ogx.birdmap.top

[R14] C 风格 for
来源：http://vgu.shanyushiyangtech.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://onm.pycfn.com

[R15] while 逐行读文件
来源：http://nld.birdmap.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://zpe.ybcxt.top

[R16] until 等待条件
来源：http://idh.zhengqikj.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mqn.wangshuangyany.cn

[R17] 数组定义与取值
来源：http://cqx.zdbjq.cn

arr=(a b c); echo "${arr[0]}"
来源：http://noa.dianchejie.cn

[R18] 遍历数组
来源：http://clz.sjlbkw.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://jeg.yj202588.top

[R19] 数组长度
来源：http://mvu.pengpengdd.cyou

echo "${#arr[@]}"
来源：http://tut.ehwqpu.com

[R20] 关联数组（字典）
来源：http://yfz.c1oappe.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wqz.jlsjyb.cn

[R21] 字符串长度
来源：http://svn.pycfn.com

echo "${#s}"
来源：http://dtr.hongshengwenyu.top

[R22] 截取子串
来源：http://jfb.yangfankeji.com

echo "${s:0:5}"
来源：http://rxd.pengpengdd.cyou

[R23] 字符串替换
来源：http://tfa.tarul.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://dhy.cdnleiting.top

[R24] 大小写转换
来源：http://gav.wangshuangyany.cn

echo "${s^^}"; echo "${s,,}"
来源：http://sqt.ppjwa.cn

[R25] 去后缀 / 去前缀
来源：http://xqq.bjfxy.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://jqs.yvedp.cn

[R26] 命令替换
来源：http://pxm.guowangkeji.top

now=$(date +%F); echo "$now"
来源：http://wgg.hesvh.cn

[R27] 算术展开
来源：http://btf.vehdjk.com

echo $((1 + 2 * 3))
来源：http://ndm.uphjek.com

[R28] 浮点运算
来源：http://qdz.jianghu66.top

echo "scale=2; 10/3" | bc
来源：http://wwl.xuanzx.com

[R29] 定义函数
来源：http://apu.mhx1999.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://tqw.tanke756.top

[R30] 函数返回状态码
来源：http://nwd.pengpengdd.cyou

f() { return 0; }; f || echo "失败了"
来源：http://sww.aibaodan.cn

[R31] 局部变量
来源：http://ofn.yueranfly.top

f() { local x=1; echo "$x"; }
来源：http://zno.pengpengdd.cyou

[R32] 参数个数校验
来源：http://wxg.andypj.xyz

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ofz.0kj1m.cn

[R33] 捕获错误并提示行号
来源：http://ccp.xuanzx.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://bam.gotoacloud.top

[R34] 退出时清理
来源：http://kvz.hfpthk.cn

trap 'rm -f "$tmp"' EXIT
来源：http://dko.fktsv.cn

[R35] 后台执行并等待
来源：http://lup.yanxiufei.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://biv.zhijiandao.cn

[R36] 并发执行多个任务
来源：http://pnk.shzxlz.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://grq.zhixingplan.top

[R37] 把输出赋给变量
来源：http://gwe.dashuyun.cn

files=$(ls -1)
来源：http://bim.gaohongyu789.top

[R38] 管道串联
来源：http://ejp.gzhubu.top

cat a.txt | grep -i error | wc -l
来源：http://has.smart0.xyz

[R39] 重定向标准输出与错误
来源：http://ryf.sxryk.cn

cmd > out.log 2>&1
来源：http://aaw.ywan-chungtsiang.top

[R40] 追加写日志
来源：http://fmt.yfazqb.com

echo "log" >> out.log
来源：http://mxh.zhoulong.xyz

[R41] 丢弃输出
来源：http://ldu.guowangkeji.top

cmd >/dev/null 2>&1
来源：http://bdx.ctjpmb.com

[R42] 输入重定向
来源：http://ova.kuanghao11.cn

wc -l < a.txt
来源：http://zdg.shanyushiyangtech.top

[R43] 按名字查找文件
来源：http://lyo.yongpay.top

find . -name "*.log" -type f
来源：http://ajs.haohaochexian.top

[R44] 按修改时间查找
来源：http://wsw.hysaishi.cn

find . -mtime -7 -type f
来源：http://ard.nwbrower.top

[R45] 批量删除
来源：http://lhl.xuetiantiany.cn

find . -name "*.tmp" -delete
来源：http://yuj.fzhhl.top

[R46] 递归替换文件内容
来源：http://rxj.yueranfly.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://bua.chenjidiqi.icu

[R47] sed 单行替换
来源：http://axi.jinqigufen.top

sed -i 's/foo/bar/g' a.txt
来源：http://qfl.wangshuangyany.cn

[R48] awk 取指定列
来源：http://cvk.sysykeji.top

awk '{print $1, $3}' a.txt
来源：http://rme.snrcjt.cn

[R49] awk 带条件
来源：http://bng.shanyushiyangtech.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://jtv.ybcxt.top

[R50] awk 求和
来源：http://end.smart0.xyz

awk '{s += $2} END {print s}' a.txt
来源：http://uyd.yanxiufei.cn

[R51] 排序去重取前几
来源：http://qqo.ydzc1.top

sort a.txt | uniq -c | sort -rn | head
来源：http://qfj.vqdsnc.cn

[R52] 统计行数
来源：http://ycj.aizwys.cn

wc -l a.txt
来源：http://vnx.cashguo.top

[R53] 查看文件头与实时尾
来源：http://wgq.cdnleiting.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://rwi.gaohongyu789.top

[R54] 比较两个文件
来源：http://ots.chenzaomai.com

diff a.txt b.txt
来源：http://ykg.cqqwz.cn

[R55] 压缩与解压
来源：http://tgh.yvedp.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://pep.gogol.net.cn

[R56] 远程拷贝
来源：http://bso.havefunace.top

scp file user@host:/path/
来源：http://bek.ctjpmb.com

[R57] 远程执行命令
来源：http://vjh.smart0.xyz

ssh user@host 'uptime'
来源：http://gjz.kuanghao11.cn

[R58] 下载文件
来源：http://oly.ydzc1.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://rpk.hnqzz.top

[R59] 发 POST JSON
来源：http://arr.wangshuangyany.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://zrw.9152youxi.cn

[R60] 只看 HTTP 状态码
来源：http://kpy.birdmap.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://rud.nwbrower.top

[R61] 磁盘占用
来源：http://usp.zhixingplan.top

df -h;  du -sh *
来源：http://qmc.xylfe.cn

[R62] 找最占空间的文件
来源：http://oih.chenjidiqi.icu

du -ah . | sort -rh | head -10
来源：http://qfq.yfazqb.com

[R63] 内存与进程
来源：http://feq.zhaomingkeji.xyz

free -h;  ps aux | grep nginx
来源：http://xub.ywan-chungtsiang.top

[R64] 结束进程
来源：http://hof.yueranfly.top

kill -9 $(pgrep -f app.py)
来源：http://ffj.chenlongwang.top

[R65] 查看端口占用
来源：http://omq.ywan-chungtsiang.top


<!-- 参考信息 -->