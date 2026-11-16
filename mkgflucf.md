代发 wailian999

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://bwe.zhaomingkeji.xyz

[Q20] IN 列表
来源：http://wou.shanyushiyangtech.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://lqc.ydjk.org.cn

[Q21] 空值判断
来源：http://fnk.52xcode.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://stc.yvedp.cn

[Q22] 排序
来源：http://yen.dianchejie.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://dxb.dashuyun.cn

[Q23] 分页
来源：http://htu.jiagoushi.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://zsu.zhixingplan.top

[Q24] 去重
来源：http://non.cheryme.top

SELECT DISTINCT city FROM users;
来源：http://him.fehbvm.com

[Q25] 只取前 N 条
来源：http://lmn.yj202588.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://vca.tian-w.cn

[Q26] 计数
来源：http://svv.yanxiufei.cn

SELECT COUNT(*) FROM users;
来源：http://jrc.tarul.cn

[Q27] 条件计数
来源：http://pfl.feifeiyinyue.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ggy.jinyuanbaomall.cn

[Q28] 求和与平均
来源：http://xtb.birdmap.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ipi.dianchejie.cn

[Q29] 最大最小值
来源：http://tyr.ywan-chungtsiang.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://kqq.zdqjudy.top

[Q30] 分组统计
来源：http://fjw.sufxvd.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://fvd.sysykeji.top

[Q31] 分组后过滤
来源：http://ybd.epnwcf.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://pki.xziqi.cn

[Q32] 分组拼接字符串
来源：http://ruo.yangfankeji.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://piy.fengsongda.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://tvx.haohaochexian.top

[Q33] 多列分组
来源：http://jzw.birdmap.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://cka.yuanzhike.top

[Q34] 每组取第一条
来源：http://jrd.yj20258888.top

SELECT * FROM (
来源：http://fpx.fehbvm.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ish.xingfuxueyuan.xyz

) t WHERE rn = 1;
来源：http://qwx.zhengqikj.top

[Q35] 内连接
来源：http://iwn.ydjk.org.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://sxu.chenzaomai.com

[Q36] 左连接
来源：http://zpe.yuanzhike.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://zpi.jiagoushi.top

[Q37] 右连接
来源：http://iya.xuanzx.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://tiu.fehbvm.com

[Q38] 全外连接（PostgreSQL）
来源：http://kww.zhengqikj.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://suc.ywan-chungtsiang.top

[Q39] 自连接（查上下级）
来源：http://zjn.jinyuanbaomall.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://alw.hcnkem.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://cic.chenzaomai.com

[Q40] 交叉连接（笛卡尔积）
来源：http://joa.chenzaomai.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ife.haohaochexian.top

[Q41] 多表连接
来源：http://muv.zdbjq.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://sbb.c1oappe.top

JOIN users u ON u.id = o.user_id
来源：http://vfh.cashguo.top

JOIN products p ON p.id = o.product_id;
来源：http://pem.pengpengdd.cyou

[Q42] 连接条件附加过滤
来源：http://zhc.guowangkeji.top

SELECT u.name, o.amount FROM users u
来源：http://xgo.shuidangran.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://quy.hesvh.cn

[Q43] 标量子查询
来源：http://tfy.fehbvm.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://gny.xuanzx.com

[Q44] IN 子查询
来源：http://zzp.zycfv.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://lig.yangfankeji.com

[Q45] EXISTS 判断存在
来源：http://jhf.vehdjk.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bir.tarul.cn

[Q46] NOT EXISTS 判断不存在
来源：http://avo.pycfn.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jme.birdmap.top

[Q47] 与平均值比较
来源：http://gww.uphjek.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://pmc.xuanzx.com

[Q48] CTE 公用表表达式
来源：http://dfy.aizwys.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mxy.fengsongda.top

SELECT * FROM t WHERE c > 5;
来源：http://xcz.yanxiufei.cn

[Q49] 更新单行
来源：http://wtn.yonumen.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ajn.snrcjt.cn

[Q50] 批量更新
来源：http://ewd.ydjk.org.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wqi.nanxinkj.top

[Q51] 用子查询更新
来源：http://gyc.iojbl.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ycs.haohaochexian.top

[Q52] 删除指定行
来源：http://ybw.xuanzx.com

DELETE FROM users WHERE id = 10;
来源：http://lqb.hysaishi.cn

[Q53] 按条件删除
来源：http://jbj.zdqjudy.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://pvf.ppjwa.cn

[Q54] 清空表
来源：http://nda.gaohongyu789.top

TRUNCATE TABLE logs;
来源：http://gge.epnwcf.com

[Q55] 排名（并列占位）
来源：http://fqv.xingfuxueyuan.xyz

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://pvq.meibo888.top

[Q56] 密集排名（并列不占位）
来源：http://yiq.gaohongyu789.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://sii.zhaomingkeji.xyz

[Q57] 行号
来源：http://jln.xuanzx.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ppk.sxryk.cn

[Q58] 累计求和
来源：http://uvq.zhixingplan.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://fck.yj202588.top

[Q59] 分组内累计
来源：http://mjh.ydzc1.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://sgz.mhx1999.top

[Q60] 取上一行 / 下一行
来源：http://bcp.fanxiaobao.xyz

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hai.ehwqpu.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mxz.jianghu66.top

[Q61] 移动平均
来源：http://cyw.fktsv.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://rgf.jqgufenzy.top

[Q62] 分组占比
来源：http://lld.cucudq.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://xro.tarul.cn

[Q63] 开启事务
来源：http://gqu.zhixingplan.top

START TRANSACTION;                -- 或 BEGIN
来源：http://xvp.dianchejie.cn

[Q64] 提交事务
来源：http://acx.nanxinkj.top

COMMIT;
来源：http://xhe.shzxlz.cn

[Q65] 回滚事务
来源：http://xuv.smart0.xyz

ROLLBACK;
来源：http://jgt.jinghuilouyu.cn

[Q66] 行锁查询
来源：http://zpb.zhengqikj.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://seb.tarul.cn

[Q67] 设置隔离级别
来源：http://beq.0kj1m.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://gyl.jinqigfzy.top

[Q68] 保存点
来源：http://ubr.pengpengdd.cyou

SAVEPOINT sp1;
来源：http://zea.ywan-chungtsiang.top

ROLLBACK TO sp1;
来源：http://mux.zhengqikj.top

[Q69] 查看执行计划
来源：http://lrd.hongshengwenyu.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ypg.ydzc1.top

[Q70] 更新统计信息
来源：http://vll.xuanzx.com

ANALYZE TABLE users;
来源：http://ycj.fanxiaobao.xyz

[Q71] 查看建表语句
来源：http://ycf.aizwys.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://uuz.yonumen.top

[Q72] 查看索引
来源：http://izn.sweek.top

SHOW INDEX FROM users;
来源：http://lve.cucudq.cn

[Q73] 查看表状态
来源：http://knq.shuidangran.top

SHOW TABLE STATUS LIKE 'users';
来源：http://tfb.xuanzx.com

[Q74] 强制使用索引
来源：http://ylh.wangshuangyany.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://myz.shanyushiyangtech.top

[Q75] 日期格式化
来源：http://oyx.ydzc1.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://vqn.jinqigufen.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://vdy.cheryme.top

[Q76] 按天统计
来源：http://orr.daxiang520.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://pxn.yfazqb.com

[Q77] 时间加减
来源：http://lbq.birdmap.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://pgo.xuetiantiany.cn

[Q78] 当前时间
来源：http://eyh.quarkkingdee.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ucm.meibo888.top

[Q79] 字符串拼接
来源：http://oav.ppjwa.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ott.yj202588.top

[Q80] 字符串截取
来源：http://zpn.jinqigufen.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://pud.svipenyu.cn

[Q81] 字符串替换
来源：http://edh.sjlbkw.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ezj.zhixingplan.top

[Q82] 字符长度与字节长度
来源：http://gnp.cdnleiting.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://shj.vqdsnc.cn

[Q83] 大小写转换
来源：http://zxk.nwbrower.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://buj.yj20258.top

[Q84] 去除首尾空格
来源：http://wio.hnxiangtu.top

SELECT TRIM(name) FROM users;
来源：http://rss.hfpthk.cn

[Q85] 数值取整
来源：http://oyt.pycfn.com

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://rva.yonumen.top

[Q86] 读取 JSON 字段
来源：http://ssn.jyoumei.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://fbc.epnwcf.com

[Q87] JSON 字段做条件
来源：http://zoq.snrcjt.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ooj.hnqzz.top

[Q88] 行转列（条件聚合）
来源：http://yzf.xylfe.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://htx.fktsv.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://xgv.ybcxt.top

[Q89] 判断表是否存在
来源：http://oet.pycfn.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://qib.yj20258888.top

[Q90] 生成序号列
来源：http://bvl.sufxvd.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ygu.ppjwa.cn

================================================================================
来源：http://fce.bjfxy.top

R. Bash 专题
来源：http://uxb.jinghuilouyu.cn

================================================================================
来源：http://pjk.hnqzz.top

[R01] shebang 与严格模式
来源：http://mpf.zhijiandao.cn

#!/usr/bin/env bash
来源：http://ebp.hcnkem.com

set -euo pipefail
来源：http://mib.pengpengdd.cyou

[R02] 变量赋值与使用
来源：http://ebm.guannengcc.top

name="Tom"; echo "$name"
来源：http://oth.ctjpmb.com

[R03] 只读变量
来源：http://xlc.mhx1999.top

readonly PI=3.14
来源：http://kel.cashguo.top

[R04] 位置参数
来源：http://wvh.redwolf501.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://xvz.cdnleiting.top

[R05] 参数默认值
来源：http://htt.aibaodan.cn

name="${1:-default}"
来源：http://jiz.shanyushiyangkeji.top

[R06] 判断命令是否存在
来源：http://pmi.snrcjt.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://xjk.nwbrower.top

[R07] if 判断文件
来源：http://hfx.bjfxy.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://yko.yj20258.top

[R08] 数值比较
来源：http://pgn.jqgufenzy.top

if (( a > b )); then echo "a 更大"; fi
来源：http://jip.vehdjk.com

[R09] 字符串比较
来源：http://ffw.ehwqpu.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://crp.feifeiyinyue.top

[R10] 正则匹配
来源：http://nwi.gotoacloud.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://lvb.pycfn.com

[R11] case 多分支
来源：http://dyz.xuetiantiany.cn

case "$1" in
来源：http://ywm.ybcxt.top

start) echo "启动" ;;
来源：http://tzc.jinghuilouyu.cn

stop)  echo "停止" ;;
来源：http://nad.nanxinkj.top

*)     echo "未知命令" ;;
来源：http://irf.ywan-chungtsiang.top

esac
来源：http://aop.jlsjyb.cn

[R12] for 遍历文件
来源：http://uqm.hongshengwenyu.top

for f in *.txt; do echo "$f"; done
来源：http://jdc.xingfuxueyuan.xyz

[R13] for 计数循环
来源：http://lal.cheryme.top

for i in {1..10}; do echo "$i"; done
来源：http://sbk.xuetiantiany.cn

[R14] C 风格 for
来源：http://zfh.gotoacloud.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://abf.ywan-chungtsiang.top

[R15] while 逐行读文件
来源：http://znw.wangdashe.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://kjy.yfazqb.com

[R16] until 等待条件
来源：http://xbp.yvedp.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://nxg.hywenlv.cn

[R17] 数组定义与取值
来源：http://abo.chenlongwang.top

arr=(a b c); echo "${arr[0]}"
来源：http://lqf.shanyushiyangkeji.top

[R18] 遍历数组
来源：http://sdd.hammf.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://arv.svipenyu.cn

[R19] 数组长度
来源：http://uci.uphjek.com

echo "${#arr[@]}"
来源：http://dej.fehbvm.com

[R20] 关联数组（字典）
来源：http://uof.bbcook.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://qzy.shanyushiyangtech.top

[R21] 字符串长度
来源：http://zst.iojbl.cn

echo "${#s}"
来源：http://vwl.ydjk.org.cn

[R22] 截取子串
来源：http://vyl.9152youxi.cn

echo "${s:0:5}"
来源：http://wlw.jinqigfzy.top

[R23] 字符串替换
来源：http://ksi.pengpengdd.cyou

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://qkz.wangshuangyany.cn

[R24] 大小写转换
来源：http://sjh.ppjwa.cn

echo "${s^^}"; echo "${s,,}"
来源：http://tdz.xuetiantiany.cn

[R25] 去后缀 / 去前缀
来源：http://sfv.jinqigufen.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://ktd.guowangkeji.top

[R26] 命令替换
来源：http://vkn.zdqjudy.top

now=$(date +%F); echo "$now"
来源：http://jcu.ehwqpu.com

[R27] 算术展开
来源：http://jhk.haohaochexian.top

echo $((1 + 2 * 3))
来源：http://vxk.jinqigfzy.top

[R28] 浮点运算
来源：http://mqk.chenjidiqi.icu

echo "scale=2; 10/3" | bc
来源：http://tvr.chenjidiqi.icu

[R29] 定义函数
来源：http://nyj.cheryme.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://nct.svipenyu.cn

[R30] 函数返回状态码
来源：http://dfd.ywan-chungtsiang.top

f() { return 0; }; f || echo "失败了"
来源：http://iws.cheryme.top

[R31] 局部变量
来源：http://lov.ywan-chungtsiang.top

f() { local x=1; echo "$x"; }
来源：http://eql.hammf.cn

[R32] 参数个数校验
来源：http://bup.cucudq.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://zyi.nanxinkj.top

[R33] 捕获错误并提示行号
来源：http://jpj.yj20258.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://cpi.xingfuxueyuan.xyz

[R34] 退出时清理
来源：http://dfm.shuidangran.top

trap 'rm -f "$tmp"' EXIT
来源：http://iiv.ppjwa.cn

[R35] 后台执行并等待
来源：http://vby.nanxuanxn.top

sleep 5 & pid=$!; wait "$pid"
来源：http://osp.zhoulong.xyz

[R36] 并发执行多个任务
来源：http://qxd.smart0.xyz

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ehn.haohaochexian.top

[R37] 把输出赋给变量
来源：http://kdn.jlsjyb.cn

files=$(ls -1)
来源：http://afq.jqgfzy.top

[R38] 管道串联
来源：http://yxu.hesvh.cn

cat a.txt | grep -i error | wc -l
来源：http://mgn.yj20258.top

[R39] 重定向标准输出与错误
来源：http://tvn.bbcook.cn

cmd > out.log 2>&1
来源：http://hzw.guowangkeji.top

[R40] 追加写日志
来源：http://jsx.gogol.net.cn

echo "log" >> out.log
来源：http://jmj.redwolf501.top

[R41] 丢弃输出
来源：http://lpi.shuidangran.top

cmd >/dev/null 2>&1
来源：http://hwj.hcnkem.com

[R42] 输入重定向
来源：http://nch.jqgufenzy.top

wc -l < a.txt
来源：http://wpi.0kj1m.cn

[R43] 按名字查找文件
来源：http://ahy.jianghu66.top

find . -name "*.log" -type f
来源：http://kjv.hnqzz.top

[R44] 按修改时间查找
来源：http://imd.yuanzhike.top

find . -mtime -7 -type f
来源：http://dwg.cucudq.cn

[R45] 批量删除
来源：http://wcs.yanxiufei.cn

find . -name "*.tmp" -delete
来源：http://vtq.wangdashe.top

[R46] 递归替换文件内容
来源：http://gps.wangshuangyany.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://pvw.xinyue.icu

[R47] sed 单行替换
来源：http://eqf.nanxinkj.top

sed -i 's/foo/bar/g' a.txt
来源：http://nks.dianchejie.cn

[R48] awk 取指定列
来源：http://yre.hcnkem.com

awk '{print $1, $3}' a.txt
来源：http://nms.xziqi.cn

[R49] awk 带条件
来源：http://xfk.sjlbkw.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://huh.yangfankeji.com

[R50] awk 求和
来源：http://isk.yueranfly.top

awk '{s += $2} END {print s}' a.txt
来源：http://hpn.epnwcf.com

[R51] 排序去重取前几
来源：http://sfr.gzhubu.top

sort a.txt | uniq -c | sort -rn | head
来源：http://vbd.tianlin.xyz

[R52] 统计行数
来源：http://mnq.feifeiyinyue.top

wc -l a.txt
来源：http://ysk.haohaochexian.top

[R53] 查看文件头与实时尾
来源：http://qaq.ydjk.org.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ipo.chenzaomai.com

[R54] 比较两个文件
来源：http://fmz.kuanghao11.cn

diff a.txt b.txt
来源：http://uyu.vehdjk.com

[R55] 压缩与解压
来源：http://xpr.nanxinkj.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://glc.hysaishi.cn

[R56] 远程拷贝
来源：http://jtz.haohaochexian.top

scp file user@host:/path/
来源：http://tdj.52xcode.cn

[R57] 远程执行命令
来源：http://ueb.fzhhl.top

ssh user@host 'uptime'
来源：http://uqn.sysykeji.top

[R58] 下载文件
来源：http://fvb.zycfv.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://zkd.jinghuilouyu.cn

[R59] 发 POST JSON
来源：http://ydd.yonumen.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mzt.shuidangran.top

[R60] 只看 HTTP 状态码
来源：http://wcb.ehwqpu.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hqn.redwolf501.top

[R61] 磁盘占用
来源：http://nqw.feifeiyinyue.top

df -h;  du -sh *
来源：http://axm.shangyingyoupin.top

[R62] 找最占空间的文件
来源：http://ojx.yfazqb.com

du -ah . | sort -rh | head -10
来源：http://xqz.hesvh.cn

[R63] 内存与进程
来源：http://opu.vqdsnc.cn

free -h;  ps aux | grep nginx
来源：http://dkl.yj20258888.top

[R64] 结束进程
来源：http://ifm.cucudq.cn

kill -9 $(pgrep -f app.py)
来源：http://zhl.yuanzhike.top

[R65] 查看端口占用
来源：http://uis.yuanzhike.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://jyw.316326.xyz

[R66] 定时任务
来源：http://mkh.cucudq.cn

crontab -e;  crontab -l
来源：http://fzp.cdnleiting.top

[R67] 生成随机十六进制串
来源：http://msk.zhongyouzk.top

openssl rand -hex 16
来源：http://kzj.hammf.cn

[R68] 计算文件校验值
来源：http://rfv.hongshengwenyu.top

sha256sum a.txt;  md5sum a.txt
来源：http://dwq.nwbrower.top

[R69] 生成随机密码
来源：http://dfu.yueranfly.top


<!-- 参考信息 -->