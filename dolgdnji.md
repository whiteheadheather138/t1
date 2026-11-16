代发 wailian999

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://yhg.hammf.cn

[Q20] IN 列表
来源：http://wiu.redwolf501.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wps.zycfv.cn

[Q21] 空值判断
来源：http://orc.feifeiyinyue.top

SELECT * FROM users WHERE email IS NULL;
来源：http://ccy.hnqzz.top

[Q22] 排序
来源：http://erc.fzhhl.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ppp.wangdashe.top

[Q23] 分页
来源：http://nmo.pengpengdd.cyou

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://vmk.jlsjyb.cn

[Q24] 去重
来源：http://dmn.pycfn.com

SELECT DISTINCT city FROM users;
来源：http://sqt.yvedp.cn

[Q25] 只取前 N 条
来源：http://yni.mhx1999.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wyx.fanxiaobao.xyz

[Q26] 计数
来源：http://clc.haohaochexian.top

SELECT COUNT(*) FROM users;
来源：http://hyb.yuanzhike.top

[Q27] 条件计数
来源：http://isz.yueranfly.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://rrv.shanyushiyangtech.top

[Q28] 求和与平均
来源：http://ixz.gogol.net.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://oyv.jianghu66.top

[Q29] 最大最小值
来源：http://yqk.zhengqikj.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://dtw.zycfv.cn

[Q30] 分组统计
来源：http://zzv.jinghuilouyu.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://euy.yonumen.top

[Q31] 分组后过滤
来源：http://jfc.hysaishi.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://gsg.uphjek.com

[Q32] 分组拼接字符串
来源：http://hsc.epnwcf.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://xjp.pengpengdd.cyou

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://dri.zycfv.cn

[Q33] 多列分组
来源：http://fpu.xuanzx.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mje.xingfuxueyuan.xyz

[Q34] 每组取第一条
来源：http://zpc.zhengqikj.top

SELECT * FROM (
来源：http://cfu.daxiang520.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://sis.jlsjyb.cn

) t WHERE rn = 1;
来源：http://cxc.sysykeji.top

[Q35] 内连接
来源：http://wys.mhx1999.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://eib.snrcjt.cn

[Q36] 左连接
来源：http://gvd.snrcjt.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://tfq.gotoacloud.top

[Q37] 右连接
来源：http://mye.cdnleiting.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://xsq.daria6918.cn

[Q38] 全外连接（PostgreSQL）
来源：http://fei.epnwcf.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://rhm.jiagoushi.top

[Q39] 自连接（查上下级）
来源：http://kzs.zhijiandao.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://gpd.dianchejie.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://cto.xuanzx.com

[Q40] 交叉连接（笛卡尔积）
来源：http://aaq.aibaodan.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://xmq.bjfxy.top

[Q41] 多表连接
来源：http://ntj.xingfuxueyuan.xyz

SELECT o.id, u.name, p.title FROM orders o
来源：http://sle.jqgufenzy.top

JOIN users u ON u.id = o.user_id
来源：http://dns.redwolf501.top

JOIN products p ON p.id = o.product_id;
来源：http://wzw.bjfxy.top

[Q42] 连接条件附加过滤
来源：http://mmt.52xcode.cn

SELECT u.name, o.amount FROM users u
来源：http://laz.sxryk.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://rty.zdbjq.cn

[Q43] 标量子查询
来源：http://mmq.ivvv.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mbn.316326.xyz

[Q44] IN 子查询
来源：http://ffb.feifeiyinyue.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ljr.ppjwa.cn

[Q45] EXISTS 判断存在
来源：http://cip.cheryme.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zqz.bjfxy.top

[Q46] NOT EXISTS 判断不存在
来源：http://pee.xylfe.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://gxk.zhongyouzk.top

[Q47] 与平均值比较
来源：http://ukh.sufxvd.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hbv.shzxlz.cn

[Q48] CTE 公用表表达式
来源：http://rmb.hongshengwenyu.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://zsr.bjfxy.top

SELECT * FROM t WHERE c > 5;
来源：http://csx.ppjwa.cn

[Q49] 更新单行
来源：http://ejs.xuetiantiany.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://rby.aibaodan.cn

[Q50] 批量更新
来源：http://ngj.quarkkingdee.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://tut.xinyue.icu

[Q51] 用子查询更新
来源：http://vjz.daria6918.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://bvb.zhengqikj.top

[Q52] 删除指定行
来源：http://mgb.daria6918.cn

DELETE FROM users WHERE id = 10;
来源：http://gdb.cheryme.top

[Q53] 按条件删除
来源：http://ggs.jinqigufen.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mmx.jqgfzy.top

[Q54] 清空表
来源：http://xzg.ydjk.org.cn

TRUNCATE TABLE logs;
来源：http://llm.wangdashe.top

[Q55] 排名（并列占位）
来源：http://qgw.yj20258888.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://qjw.iojbl.cn

[Q56] 密集排名（并列不占位）
来源：http://cpi.chenlongwang.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://rnd.c1oappe.top

[Q57] 行号
来源：http://tfj.yuxming.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://xsj.kuanghao11.cn

[Q58] 累计求和
来源：http://yxx.fengsongda.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://esc.hammf.cn

[Q59] 分组内累计
来源：http://ojf.redwolf501.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://lxo.zhoulong.xyz

[Q60] 取上一行 / 下一行
来源：http://rkf.jqgfzy.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wwu.haohaochexian.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://gfr.yanxiufei.cn

[Q61] 移动平均
来源：http://jrk.shzxlz.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ayz.xingfuxueyuan.xyz

[Q62] 分组占比
来源：http://atk.ehwqpu.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://dle.gotoacloud.top

[Q63] 开启事务
来源：http://znr.hammf.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://fvs.epnwcf.com

[Q64] 提交事务
来源：http://lki.nanxinkj.top

COMMIT;
来源：http://yde.aizwys.cn

[Q65] 回滚事务
来源：http://exy.cheryme.top

ROLLBACK;
来源：http://cnk.zhijiandao.cn

[Q66] 行锁查询
来源：http://kqi.redwolf501.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mhp.redwolf501.top

[Q67] 设置隔离级别
来源：http://bjs.svipenyu.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://rov.ydzc1.top

[Q68] 保存点
来源：http://eze.nanxinkj.top

SAVEPOINT sp1;
来源：http://bqi.yuxming.cn

ROLLBACK TO sp1;
来源：http://xkb.yongpay.top

[Q69] 查看执行计划
来源：http://etz.yongpay.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://emm.bbcook.cn

[Q70] 更新统计信息
来源：http://isy.yonumen.top

ANALYZE TABLE users;
来源：http://mlf.birdmap.top

[Q71] 查看建表语句
来源：http://lsq.yfazqb.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://bjn.zhengqikj.top

[Q72] 查看索引
来源：http://tgc.andypj.xyz

SHOW INDEX FROM users;
来源：http://zjp.guannengcc.top

[Q73] 查看表状态
来源：http://bta.xinyue.icu

SHOW TABLE STATUS LIKE 'users';
来源：http://auh.haohaochexian.top

[Q74] 强制使用索引
来源：http://ogl.zdqjudy.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://bdk.fengsongda.top

[Q75] 日期格式化
来源：http://obn.zycfv.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://whd.xuetiantiany.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://fjl.hfpthk.cn

[Q76] 按天统计
来源：http://bvb.shanyushiyangkeji.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://rkw.havefunace.top

[Q77] 时间加减
来源：http://oic.xinyue.icu

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hqi.feifeiyinyue.top

[Q78] 当前时间
来源：http://zkt.xylfe.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://bvy.jlsjyb.cn

[Q79] 字符串拼接
来源：http://qdb.xuetiantiany.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://quw.0kj1m.cn

[Q80] 字符串截取
来源：http://wga.chenjidiqi.icu

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://oar.shanyushiyangtech.top

[Q81] 字符串替换
来源：http://gpc.dianchejie.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://jtx.daria6918.cn

[Q82] 字符长度与字节长度
来源：http://lwq.ivvv.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://vgv.dianchejie.cn

[Q83] 大小写转换
来源：http://imo.andypj.xyz

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://and.mhx1999.top

[Q84] 去除首尾空格
来源：http://mas.fengsongda.top

SELECT TRIM(name) FROM users;
来源：http://ibk.cashguo.top

[Q85] 数值取整
来源：http://xoe.zhixingplan.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hgx.jinqigfzy.top

[Q86] 读取 JSON 字段
来源：http://whm.hnqzz.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://lsk.cheryme.top

[Q87] JSON 字段做条件
来源：http://gfy.pycfn.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://qpf.quarkkingdee.top

[Q88] 行转列（条件聚合）
来源：http://rpl.ybcxt.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ukb.cucudq.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://axy.yuanzhike.top

[Q89] 判断表是否存在
来源：http://tkg.tanke756.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://lqm.yongpay.top

[Q90] 生成序号列
来源：http://wdc.yonumen.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://gkj.quarkkingdee.top

================================================================================
来源：http://srx.jyoumei.cn

R. Bash 专题
来源：http://rar.aibaodan.cn

================================================================================
来源：http://ixf.tanke756.top

[R01] shebang 与严格模式
来源：http://kdr.tanke756.top

#!/usr/bin/env bash
来源：http://oab.sufxvd.cn

set -euo pipefail
来源：http://qqb.zhongyouzk.top

[R02] 变量赋值与使用
来源：http://blq.zycfv.cn

name="Tom"; echo "$name"
来源：http://iil.jlsjyb.cn

[R03] 只读变量
来源：http://muh.cucudq.cn

readonly PI=3.14
来源：http://kgq.haohaochexian.top

[R04] 位置参数
来源：http://nke.ydjk.org.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://omc.ehwqpu.com

[R05] 参数默认值
来源：http://xrz.tian-w.cn

name="${1:-default}"
来源：http://tsm.jyoumei.cn

[R06] 判断命令是否存在
来源：http://nso.zdqjudy.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://kiz.havefunace.top

[R07] if 判断文件
来源：http://tfb.yongpay.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://yco.hongshengwenyu.top

[R08] 数值比较
来源：http://err.guowangkeji.top

if (( a > b )); then echo "a 更大"; fi
来源：http://acx.quarkkingdee.top

[R09] 字符串比较
来源：http://fdb.ydjk.org.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://pjb.jyoumei.cn

[R10] 正则匹配
来源：http://qtq.chenzaomai.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://fmn.fzhhl.top

[R11] case 多分支
来源：http://jpe.ydzc1.top

case "$1" in
来源：http://bsg.andypj.xyz

start) echo "启动" ;;
来源：http://yxx.yvedp.cn

stop)  echo "停止" ;;
来源：http://ebv.shanyushiyangkeji.top

*)     echo "未知命令" ;;
来源：http://puq.smart0.xyz

esac
来源：http://mjz.bbcook.cn

[R12] for 遍历文件
来源：http://uyb.cucudq.cn

for f in *.txt; do echo "$f"; done
来源：http://zfl.hongshengwenyu.top

[R13] for 计数循环
来源：http://unk.bbcook.cn

for i in {1..10}; do echo "$i"; done
来源：http://jwe.fzhhl.top

[R14] C 风格 for
来源：http://tjy.sweek.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://idx.haohaochexian.top

[R15] while 逐行读文件
来源：http://lvg.cqqwz.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://pbs.jinghuilouyu.cn

[R16] until 等待条件
来源：http://lua.52xcode.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://fut.fengsongda.top

[R17] 数组定义与取值
来源：http://zav.hnxiangtu.top

arr=(a b c); echo "${arr[0]}"
来源：http://prv.hfpthk.cn

[R18] 遍历数组
来源：http://krn.redwolf501.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://jui.ehwqpu.com

[R19] 数组长度
来源：http://szx.yanxiufei.cn

echo "${#arr[@]}"
来源：http://qnr.gaohongyu789.top

[R20] 关联数组（字典）
来源：http://sbz.sweek.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mbi.cqqwz.cn

[R21] 字符串长度
来源：http://kix.tianlin.xyz

echo "${#s}"
来源：http://fay.sufxvd.cn

[R22] 截取子串
来源：http://ujl.dashuyun.cn

echo "${s:0:5}"
来源：http://zzo.guowangkeji.top

[R23] 字符串替换
来源：http://ldj.xingfuxueyuan.xyz

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://kwa.feifeiyinyue.top

[R24] 大小写转换
来源：http://ydt.vqdsnc.cn

echo "${s^^}"; echo "${s,,}"
来源：http://kon.chenjidiqi.icu

[R25] 去后缀 / 去前缀
来源：http://hbu.epnwcf.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://wyk.ivvv.top

[R26] 命令替换
来源：http://zgp.zycfv.cn

now=$(date +%F); echo "$now"
来源：http://utr.yuanzhike.top

[R27] 算术展开
来源：http://fpj.yongpay.top

echo $((1 + 2 * 3))
来源：http://nsd.yj20258.top

[R28] 浮点运算
来源：http://kzd.yangfankeji.com

echo "scale=2; 10/3" | bc
来源：http://gde.wangshuangyany.cn

[R29] 定义函数
来源：http://kzo.zdbjq.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://xsq.ydjk.org.cn

[R30] 函数返回状态码
来源：http://afd.daxiang520.top

f() { return 0; }; f || echo "失败了"
来源：http://npk.shangyingyoupin.top

[R31] 局部变量
来源：http://sou.yuanzhike.top

f() { local x=1; echo "$x"; }
来源：http://bwo.yanxiufei.cn

[R32] 参数个数校验
来源：http://qgg.chenlongwang.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://itp.xingfuxueyuan.xyz

[R33] 捕获错误并提示行号
来源：http://tab.316326.xyz

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ynt.nwbrower.top

[R34] 退出时清理
来源：http://wfd.xinyue.icu

trap 'rm -f "$tmp"' EXIT
来源：http://wyn.jiagoushi.top

[R35] 后台执行并等待
来源：http://lgf.jinghuilouyu.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://hgb.snrcjt.cn

[R36] 并发执行多个任务
来源：http://eju.ctjpmb.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://vhp.hnxiangtu.top

[R37] 把输出赋给变量
来源：http://jxo.zdbjq.cn

files=$(ls -1)
来源：http://tsq.epnwcf.com

[R38] 管道串联
来源：http://hrq.hcnkem.com

cat a.txt | grep -i error | wc -l
来源：http://zaw.shanyushiyangkeji.top

[R39] 重定向标准输出与错误
来源：http://dqc.hammf.cn

cmd > out.log 2>&1
来源：http://asq.tianlin.xyz

[R40] 追加写日志
来源：http://sle.jianghu66.top

echo "log" >> out.log
来源：http://tas.hysaishi.cn

[R41] 丢弃输出
来源：http://fyo.xuetiantiany.cn

cmd >/dev/null 2>&1
来源：http://gfm.jlsjyb.cn

[R42] 输入重定向
来源：http://cre.tian-w.cn

wc -l < a.txt
来源：http://idf.zdbjq.cn

[R43] 按名字查找文件
来源：http://xau.xingfuxueyuan.xyz

find . -name "*.log" -type f
来源：http://tai.xuetiantiany.cn

[R44] 按修改时间查找
来源：http://kpe.fzhhl.top

find . -mtime -7 -type f
来源：http://jne.nanxinkj.top

[R45] 批量删除
来源：http://phx.zdqjudy.top

find . -name "*.tmp" -delete
来源：http://uqu.yueranfly.top

[R46] 递归替换文件内容
来源：http://tzf.hammf.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://zzc.hnxiangtu.top

[R47] sed 单行替换
来源：http://ogb.cucudq.cn

sed -i 's/foo/bar/g' a.txt
来源：http://vig.meibo888.top

[R48] awk 取指定列
来源：http://kys.nwbrower.top

awk '{print $1, $3}' a.txt
来源：http://mjr.shangyingyoupin.top

[R49] awk 带条件
来源：http://wca.yuxming.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://rck.cdnleiting.top

[R50] awk 求和
来源：http://kxs.yj20258888.top

awk '{s += $2} END {print s}' a.txt
来源：http://vlu.xziqi.cn

[R51] 排序去重取前几
来源：http://zvw.shzxlz.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://lat.shuidangran.top

[R52] 统计行数
来源：http://cem.haohaochexian.top

wc -l a.txt
来源：http://qgh.ctjpmb.com

[R53] 查看文件头与实时尾
来源：http://asw.cashguo.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://qaa.jinqigfzy.top

[R54] 比较两个文件
来源：http://scl.fzhhl.top

diff a.txt b.txt
来源：http://yom.tarul.cn

[R55] 压缩与解压
来源：http://xps.xziqi.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://rek.tian-w.cn

[R56] 远程拷贝
来源：http://gxl.fengsongda.top

scp file user@host:/path/
来源：http://uej.quarkkingdee.top

[R57] 远程执行命令
来源：http://mtv.ywan-chungtsiang.top

ssh user@host 'uptime'
来源：http://fpx.chenzaomai.com

[R58] 下载文件
来源：http://iqi.shzxlz.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://gpo.jinqigufen.top

[R59] 发 POST JSON
来源：http://cby.smart0.xyz

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ptw.hnqzz.top

[R60] 只看 HTTP 状态码
来源：http://nsu.zdbjq.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://zvr.fanxiaobao.xyz

[R61] 磁盘占用
来源：http://lug.meibo888.top

df -h;  du -sh *
来源：http://sii.sxryk.cn

[R62] 找最占空间的文件
来源：http://utw.dashuyun.cn

du -ah . | sort -rh | head -10
来源：http://jnl.yangfankeji.com

[R63] 内存与进程
来源：http://vmw.316326.xyz

free -h;  ps aux | grep nginx
来源：http://brz.zhijiandao.cn

[R64] 结束进程
来源：http://mmg.cucudq.cn

kill -9 $(pgrep -f app.py)
来源：http://kti.ehwqpu.com

[R65] 查看端口占用
来源：http://yzh.vehdjk.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://kdu.dianchejie.cn

[R66] 定时任务
来源：http://agx.zhaomingkeji.xyz

crontab -e;  crontab -l
来源：http://bdd.vehdjk.com

[R67] 生成随机十六进制串
来源：http://cyk.jyoumei.cn

openssl rand -hex 16
来源：http://jog.yueranfly.top

[R68] 计算文件校验值
来源：http://jcf.yvedp.cn

sha256sum a.txt;  md5sum a.txt
来源：http://qbn.hcnkem.com

[R69] 生成随机密码
来源：http://lno.nanxinkj.top


<!-- 参考信息 -->