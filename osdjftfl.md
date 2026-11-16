代发 wailian999

[Q14] 存在则更新（upsert）
来源：http://vuu.yj202588.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ijk.xziqi.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://zul.yueranfly.top

[Q15] 查询全部
来源：http://glc.zdqjudy.top

SELECT * FROM users;
来源：http://jit.hywenlv.cn

[Q16] 查询指定列
来源：http://vtx.fanxiaobao.xyz

SELECT id, name FROM users;
来源：http://qch.zhengqikj.top

[Q17] 条件查询
来源：http://yha.hongshengwenyu.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hxf.gogol.net.cn

[Q18] 模糊匹配
来源：http://cci.pengpengdd.cyou

SELECT * FROM users WHERE name LIKE '张%';
来源：http://zns.wangdashe.top

[Q19] 范围查询
来源：http://pmb.bbcook.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://fdq.zhijiandao.cn

[Q20] IN 列表
来源：http://qzr.feifeiyinyue.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mvx.quarkkingdee.top

[Q21] 空值判断
来源：http://try.cucudq.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://qdq.hnqzz.top

[Q22] 排序
来源：http://mph.snrcjt.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://gil.zycfv.cn

[Q23] 分页
来源：http://drm.ybcxt.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://lsr.kuanghao11.cn

[Q24] 去重
来源：http://muj.hcnkem.com

SELECT DISTINCT city FROM users;
来源：http://twq.sysykeji.top

[Q25] 只取前 N 条
来源：http://asd.ppjwa.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ylx.zdqjudy.top

[Q26] 计数
来源：http://xod.jinyuanbaomall.cn

SELECT COUNT(*) FROM users;
来源：http://shr.feifeiyinyue.top

[Q27] 条件计数
来源：http://zke.yanxiufei.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://fag.c1oappe.top

[Q28] 求和与平均
来源：http://jvc.tianlin.xyz

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://evf.yvedp.cn

[Q29] 最大最小值
来源：http://pey.tanke756.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://edo.ybcxt.top

[Q30] 分组统计
来源：http://inz.fzhhl.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://puc.xinyue.icu

[Q31] 分组后过滤
来源：http://xts.feifeiyinyue.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://cpw.ywan-chungtsiang.top

[Q32] 分组拼接字符串
来源：http://wfy.zhaomingkeji.xyz

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hea.zhoulong.xyz

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://yjv.ydjk.org.cn

[Q33] 多列分组
来源：http://jcx.zhoulong.xyz

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ijo.jinqigufen.top

[Q34] 每组取第一条
来源：http://ixq.hfpthk.cn

SELECT * FROM (
来源：http://cqw.nanxinkj.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wqb.ehwqpu.com

) t WHERE rn = 1;
来源：http://mqm.shzxlz.cn

[Q35] 内连接
来源：http://atb.gogol.net.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://sox.sxryk.cn

[Q36] 左连接
来源：http://zbz.uphjek.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://gmf.xylfe.cn

[Q37] 右连接
来源：http://ois.52xcode.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://iyn.tianlin.xyz

[Q38] 全外连接（PostgreSQL）
来源：http://txt.gotoacloud.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://llk.hfpthk.cn

[Q39] 自连接（查上下级）
来源：http://jmv.zhoulong.xyz

SELECT e.name, m.name AS manager FROM employees e
来源：http://opu.yvedp.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://zow.zhijiandao.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://kwy.shuidangran.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://pny.tarul.cn

[Q41] 多表连接
来源：http://mhl.nwbrower.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://mzc.zhixingplan.top

JOIN users u ON u.id = o.user_id
来源：http://eqq.ehwqpu.com

JOIN products p ON p.id = o.product_id;
来源：http://sqd.fanxiaobao.xyz

[Q42] 连接条件附加过滤
来源：http://drs.nwbrower.top

SELECT u.name, o.amount FROM users u
来源：http://kba.ivvv.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://iot.52xcode.cn

[Q43] 标量子查询
来源：http://jke.ybcxt.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://bra.gaohongyu789.top

[Q44] IN 子查询
来源：http://pxf.quarkkingdee.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://aia.9152youxi.cn

[Q45] EXISTS 判断存在
来源：http://vpx.redwolf501.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kbm.zhixingplan.top

[Q46] NOT EXISTS 判断不存在
来源：http://rbe.jqgufenzy.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://quj.yuxming.cn

[Q47] 与平均值比较
来源：http://pxo.nanxuanxn.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://aez.chenlongwang.top

[Q48] CTE 公用表表达式
来源：http://wnk.ydzc1.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://epv.gotoacloud.top

SELECT * FROM t WHERE c > 5;
来源：http://wvj.quarkkingdee.top

[Q49] 更新单行
来源：http://unf.ppjwa.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://uma.daxiang520.top

[Q50] 批量更新
来源：http://yey.zdqjudy.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://tpe.xinyue.icu

[Q51] 用子查询更新
来源：http://vjl.bbcook.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://muk.zhengqikj.top

[Q52] 删除指定行
来源：http://ljq.sxryk.cn

DELETE FROM users WHERE id = 10;
来源：http://yuo.jianghu66.top

[Q53] 按条件删除
来源：http://lzv.zhiwuduotai.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://zlw.shanyushiyangtech.top

[Q54] 清空表
来源：http://her.yanxiufei.cn

TRUNCATE TABLE logs;
来源：http://ttm.yongpay.top

[Q55] 排名（并列占位）
来源：http://nsq.shanyushiyangtech.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://rnk.redwolf501.top

[Q56] 密集排名（并列不占位）
来源：http://ehr.redwolf501.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://faw.jinghuilouyu.cn

[Q57] 行号
来源：http://dob.gogol.net.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://pef.0kj1m.cn

[Q58] 累计求和
来源：http://zky.nanxuanxn.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://uvy.ybcxt.top

[Q59] 分组内累计
来源：http://dka.iojbl.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://lfp.ctjpmb.com

[Q60] 取上一行 / 下一行
来源：http://xep.havefunace.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wno.cashguo.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mlc.wangdashe.top

[Q61] 移动平均
来源：http://dzg.ehwqpu.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://cog.tarul.cn

[Q62] 分组占比
来源：http://goo.svipenyu.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://zen.hongshengwenyu.top

[Q63] 开启事务
来源：http://pol.c1oappe.top

START TRANSACTION;                -- 或 BEGIN
来源：http://npa.jianghu66.top

[Q64] 提交事务
来源：http://dqx.daxiang520.top

COMMIT;
来源：http://evw.smart0.xyz

[Q65] 回滚事务
来源：http://wws.chenjidiqi.icu

ROLLBACK;
来源：http://ayd.gogol.net.cn

[Q66] 行锁查询
来源：http://sof.wangshuangyany.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://gzc.mhx1999.top

[Q67] 设置隔离级别
来源：http://cwp.ydjk.org.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://rvj.zdqjudy.top

[Q68] 保存点
来源：http://bep.zhoulong.xyz

SAVEPOINT sp1;
来源：http://rzo.sjlbkw.cn

ROLLBACK TO sp1;
来源：http://kdr.svipenyu.cn

[Q69] 查看执行计划
来源：http://kuj.jqgufenzy.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://zsv.wangshuangyany.cn

[Q70] 更新统计信息
来源：http://chz.kuanghao11.cn

ANALYZE TABLE users;
来源：http://hhc.xingfuxueyuan.xyz

[Q71] 查看建表语句
来源：http://dyn.shanyushiyangkeji.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://pud.jinqigfzy.top

[Q72] 查看索引
来源：http://okm.vehdjk.com

SHOW INDEX FROM users;
来源：http://wrs.fktsv.cn

[Q73] 查看表状态
来源：http://jli.yonumen.top

SHOW TABLE STATUS LIKE 'users';
来源：http://uyx.fehbvm.com

[Q74] 强制使用索引
来源：http://giy.guannengcc.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://jua.xingfuxueyuan.xyz

[Q75] 日期格式化
来源：http://dal.gogol.net.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://jge.snrcjt.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://fvw.yongpay.top

[Q76] 按天统计
来源：http://vnc.zhixingplan.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://vhn.chenzaomai.com

[Q77] 时间加减
来源：http://zma.hammf.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://xpf.xuetiantiany.cn

[Q78] 当前时间
来源：http://sjl.chenjidiqi.icu

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://qsx.zhijiandao.cn

[Q79] 字符串拼接
来源：http://lms.mhx1999.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://yjw.havefunace.top

[Q80] 字符串截取
来源：http://yck.shanyushiyangkeji.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hpu.vqdsnc.cn

[Q81] 字符串替换
来源：http://wgs.aibaodan.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://kom.nwbrower.top

[Q82] 字符长度与字节长度
来源：http://vhm.nwbrower.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://iir.uphjek.com

[Q83] 大小写转换
来源：http://mzx.feifeiyinyue.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://vio.jinyuanbaomall.cn

[Q84] 去除首尾空格
来源：http://qng.hongshengwenyu.top

SELECT TRIM(name) FROM users;
来源：http://ggu.zhongyouzk.top

[Q85] 数值取整
来源：http://rlc.shangyingyoupin.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://kfi.316326.xyz

[Q86] 读取 JSON 字段
来源：http://whl.guowangkeji.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://jxa.xylfe.cn

[Q87] JSON 字段做条件
来源：http://xln.tanke756.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://xfw.chenlongwang.top

[Q88] 行转列（条件聚合）
来源：http://zwk.aibaodan.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://gki.jinghuilouyu.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://sxx.meibo888.top

[Q89] 判断表是否存在
来源：http://kyi.xuetiantiany.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ccd.zhijiandao.cn

[Q90] 生成序号列
来源：http://omy.guannengcc.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://znc.shangyingyoupin.top

================================================================================
来源：http://kmk.birdmap.top

R. Bash 专题
来源：http://ynu.chenzaomai.com

================================================================================
来源：http://opb.9152youxi.cn

[R01] shebang 与严格模式
来源：http://guo.xingfuxueyuan.xyz

#!/usr/bin/env bash
来源：http://bwv.zhaomingkeji.xyz

set -euo pipefail
来源：http://otf.yonumen.top

[R02] 变量赋值与使用
来源：http://hzt.epnwcf.com

name="Tom"; echo "$name"
来源：http://fzd.smart0.xyz

[R03] 只读变量
来源：http://vty.gogol.net.cn

readonly PI=3.14
来源：http://cnc.guowangkeji.top

[R04] 位置参数
来源：http://vhk.jqgufenzy.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://iut.bjfxy.top

[R05] 参数默认值
来源：http://qjs.hysaishi.cn

name="${1:-default}"
来源：http://eus.daxiang520.top

[R06] 判断命令是否存在
来源：http://nzu.ydjk.org.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://krn.316326.xyz

[R07] if 判断文件
来源：http://wpn.quarkkingdee.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://vuc.tarul.cn

[R08] 数值比较
来源：http://lnm.chenjidiqi.icu

if (( a > b )); then echo "a 更大"; fi
来源：http://dqw.jinghuilouyu.cn

[R09] 字符串比较
来源：http://til.316326.xyz

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://vak.shanyushiyangtech.top

[R10] 正则匹配
来源：http://pzl.wangshuangyany.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://pyu.chenzaomai.com

[R11] case 多分支
来源：http://mqs.ctjpmb.com

case "$1" in
来源：http://qsn.epnwcf.com

start) echo "启动" ;;
来源：http://qvk.andypj.xyz

stop)  echo "停止" ;;
来源：http://rsn.gaohongyu789.top

*)     echo "未知命令" ;;
来源：http://skv.zhiwuduotai.top

esac
来源：http://ocp.fktsv.cn

[R12] for 遍历文件
来源：http://mam.zhixingplan.top

for f in *.txt; do echo "$f"; done
来源：http://klx.xuanzx.com

[R13] for 计数循环
来源：http://wsx.xylfe.cn

for i in {1..10}; do echo "$i"; done
来源：http://yfs.fzhhl.top

[R14] C 风格 for
来源：http://zoi.redwolf501.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://jro.jiagoushi.top

[R15] while 逐行读文件
来源：http://jgj.jinghuilouyu.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://vje.guannengcc.top

[R16] until 等待条件
来源：http://uyf.shzxlz.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://gmy.gaohongyu789.top

[R17] 数组定义与取值
来源：http://hgu.ehwqpu.com

arr=(a b c); echo "${arr[0]}"
来源：http://yvv.hesvh.cn

[R18] 遍历数组
来源：http://zfc.sysykeji.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://rjj.jinyuanbaomall.cn

[R19] 数组长度
来源：http://gtl.feifeiyinyue.top

echo "${#arr[@]}"
来源：http://xhz.zycfv.cn

[R20] 关联数组（字典）
来源：http://xcg.zdbjq.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://sgh.gogol.net.cn

[R21] 字符串长度
来源：http://jst.jyoumei.cn

echo "${#s}"
来源：http://aub.chenlongwang.top

[R22] 截取子串
来源：http://fmi.yonumen.top

echo "${s:0:5}"
来源：http://upy.guannengcc.top

[R23] 字符串替换
来源：http://alj.zhixingplan.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://puj.zhongyouzk.top

[R24] 大小写转换
来源：http://xjb.guowangkeji.top

echo "${s^^}"; echo "${s,,}"
来源：http://kdj.tian-w.cn

[R25] 去后缀 / 去前缀
来源：http://epb.yangfankeji.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://shv.tian-w.cn

[R26] 命令替换
来源：http://svu.zhaomingkeji.xyz

now=$(date +%F); echo "$now"
来源：http://owg.gaohongyu789.top

[R27] 算术展开
来源：http://ljk.xuetiantiany.cn

echo $((1 + 2 * 3))
来源：http://uvp.havefunace.top

[R28] 浮点运算
来源：http://cfo.xuanzx.com

echo "scale=2; 10/3" | bc
来源：http://kwk.hywenlv.cn

[R29] 定义函数
来源：http://tqx.tianlin.xyz

add() { echo $(($1 + $2)); }; add 1 2
来源：http://myd.chenjidiqi.icu

[R30] 函数返回状态码
来源：http://egq.ppjwa.cn

f() { return 0; }; f || echo "失败了"
来源：http://ldu.sysykeji.top

[R31] 局部变量
来源：http://nxr.guannengcc.top

f() { local x=1; echo "$x"; }
来源：http://ndb.jqgfzy.top

[R32] 参数个数校验
来源：http://okj.nanxuanxn.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://dyx.ehwqpu.com

[R33] 捕获错误并提示行号
来源：http://xwq.yangfankeji.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://vqj.iojbl.cn

[R34] 退出时清理
来源：http://peb.meibo888.top

trap 'rm -f "$tmp"' EXIT
来源：http://zms.xinyue.icu

[R35] 后台执行并等待
来源：http://ymq.jiagoushi.top

sleep 5 & pid=$!; wait "$pid"
来源：http://azi.ywan-chungtsiang.top

[R36] 并发执行多个任务
来源：http://hpt.sysykeji.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://nxj.pengpengdd.cyou

[R37] 把输出赋给变量
来源：http://xyb.gzhubu.top

files=$(ls -1)
来源：http://fcz.svipenyu.cn

[R38] 管道串联
来源：http://rlm.ybcxt.top

cat a.txt | grep -i error | wc -l
来源：http://unk.nwbrower.top

[R39] 重定向标准输出与错误
来源：http://rfh.guannengcc.top

cmd > out.log 2>&1
来源：http://gxp.redwolf501.top

[R40] 追加写日志
来源：http://uev.jyoumei.cn

echo "log" >> out.log
来源：http://evk.fktsv.cn

[R41] 丢弃输出
来源：http://eim.tianlin.xyz

cmd >/dev/null 2>&1
来源：http://qpk.yuxming.cn

[R42] 输入重定向
来源：http://vuo.bbcook.cn

wc -l < a.txt
来源：http://fvw.wangshuangyany.cn

[R43] 按名字查找文件
来源：http://vin.jinqigufen.top

find . -name "*.log" -type f
来源：http://bit.cqqwz.cn

[R44] 按修改时间查找
来源：http://zkp.52xcode.cn

find . -mtime -7 -type f
来源：http://uwa.hysaishi.cn

[R45] 批量删除
来源：http://ggm.shuidangran.top

find . -name "*.tmp" -delete
来源：http://buv.bjfxy.top

[R46] 递归替换文件内容
来源：http://wod.yj20258.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ygy.52xcode.cn

[R47] sed 单行替换
来源：http://kqm.shuidangran.top

sed -i 's/foo/bar/g' a.txt
来源：http://rfu.chenzaomai.com

[R48] awk 取指定列
来源：http://wqa.xinyue.icu

awk '{print $1, $3}' a.txt
来源：http://ggi.svipenyu.cn

[R49] awk 带条件
来源：http://axn.wangshuangyany.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ije.tianlin.xyz

[R50] awk 求和
来源：http://rsw.shanyushiyangtech.top

awk '{s += $2} END {print s}' a.txt
来源：http://xiw.tian-w.cn

[R51] 排序去重取前几
来源：http://ehm.jinghuilouyu.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://qkp.zdqjudy.top

[R52] 统计行数
来源：http://arq.bjfxy.top

wc -l a.txt
来源：http://qnm.zdqjudy.top

[R53] 查看文件头与实时尾
来源：http://tpd.wangdashe.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ajq.wangdashe.top

[R54] 比较两个文件
来源：http://xin.tanke756.top

diff a.txt b.txt
来源：http://nxj.haohaochexian.top

[R55] 压缩与解压
来源：http://mkd.zhixingplan.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://azg.shuidangran.top

[R56] 远程拷贝
来源：http://hid.jianghu66.top

scp file user@host:/path/
来源：http://lbs.shzxlz.cn

[R57] 远程执行命令
来源：http://euf.cheryme.top

ssh user@host 'uptime'
来源：http://tdq.jinqigufen.top

[R58] 下载文件
来源：http://bgo.yangfankeji.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://iad.fehbvm.com

[R59] 发 POST JSON
来源：http://lzt.yuxming.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://syq.xuanzx.com

[R60] 只看 HTTP 状态码
来源：http://hkn.iojbl.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://bjt.jinqigufen.top

[R61] 磁盘占用
来源：http://ktl.jianghu66.top

df -h;  du -sh *
来源：http://gut.smart0.xyz

[R62] 找最占空间的文件
来源：http://wvr.yfazqb.com

du -ah . | sort -rh | head -10
来源：http://lch.havefunace.top

[R63] 内存与进程
来源：http://orm.yj20258.top


<!-- 参考信息 -->