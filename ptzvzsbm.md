代发 wailian999

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://nax.vehdjk.com

[Q18] 模糊匹配
来源：http://ykv.hfpthk.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://vcz.fanxiaobao.xyz

[Q19] 范围查询
来源：http://gga.zdqjudy.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://moi.vqdsnc.cn

[Q20] IN 列表
来源：http://lax.316326.xyz

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://tpz.jyoumei.cn

[Q21] 空值判断
来源：http://ysx.meibo888.top

SELECT * FROM users WHERE email IS NULL;
来源：http://gwa.fengsongda.top

[Q22] 排序
来源：http://sla.aibaodan.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wof.redwolf501.top

[Q23] 分页
来源：http://yzi.jiagoushi.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hic.hesvh.cn

[Q24] 去重
来源：http://caz.yj20258.top

SELECT DISTINCT city FROM users;
来源：http://vkb.birdmap.top

[Q25] 只取前 N 条
来源：http://aqh.xuanzx.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://omu.snrcjt.cn

[Q26] 计数
来源：http://ouy.birdmap.top

SELECT COUNT(*) FROM users;
来源：http://gzp.epnwcf.com

[Q27] 条件计数
来源：http://keh.sxryk.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://azd.hesvh.cn

[Q28] 求和与平均
来源：http://dor.ctjpmb.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://fgi.hammf.cn

[Q29] 最大最小值
来源：http://few.jqgfzy.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://hkw.uphjek.com

[Q30] 分组统计
来源：http://vjl.jqgufenzy.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://bqe.shangyingyoupin.top

[Q31] 分组后过滤
来源：http://jfz.zdbjq.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ifo.zhongyouzk.top

[Q32] 分组拼接字符串
来源：http://tff.chenzaomai.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://pbc.jiagoushi.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://fbz.c1oappe.top

[Q33] 多列分组
来源：http://qem.zycfv.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://cwb.chenjidiqi.icu

[Q34] 每组取第一条
来源：http://nzk.xinyue.icu

SELECT * FROM (
来源：http://jvi.bbcook.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wqr.hcnkem.com

) t WHERE rn = 1;
来源：http://pxy.uphjek.com

[Q35] 内连接
来源：http://mtq.jlsjyb.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://jcy.zdqjudy.top

[Q36] 左连接
来源：http://wyh.wangdashe.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://gkp.jlsjyb.cn

[Q37] 右连接
来源：http://ena.daxiang520.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://rwx.andypj.xyz

[Q38] 全外连接（PostgreSQL）
来源：http://fbd.yueranfly.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://rqx.gaohongyu789.top

[Q39] 自连接（查上下级）
来源：http://zll.bbcook.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://zpu.shzxlz.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://itn.yongpay.top

[Q40] 交叉连接（笛卡尔积）
来源：http://xjb.hywenlv.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://fok.yj20258888.top

[Q41] 多表连接
来源：http://ekf.vqdsnc.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://xer.jianghu66.top

JOIN users u ON u.id = o.user_id
来源：http://dlk.tanke756.top

JOIN products p ON p.id = o.product_id;
来源：http://rma.hfpthk.cn

[Q42] 连接条件附加过滤
来源：http://zuq.zycfv.cn

SELECT u.name, o.amount FROM users u
来源：http://lvx.nanxinkj.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ygt.jinqigufen.top

[Q43] 标量子查询
来源：http://kcw.shzxlz.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wnv.zhiwuduotai.top

[Q44] IN 子查询
来源：http://gra.yongpay.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://uvx.yangfankeji.com

[Q45] EXISTS 判断存在
来源：http://ngr.ywan-chungtsiang.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://anh.hammf.cn

[Q46] NOT EXISTS 判断不存在
来源：http://uzy.ivvv.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wqf.zhiwuduotai.top

[Q47] 与平均值比较
来源：http://qqb.yj202588.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://vpr.vehdjk.com

[Q48] CTE 公用表表达式
来源：http://kop.chenjidiqi.icu

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hcm.wangshuangyany.cn

SELECT * FROM t WHERE c > 5;
来源：http://dhm.jlsjyb.cn

[Q49] 更新单行
来源：http://yba.fanxiaobao.xyz

UPDATE users SET status = 1 WHERE id = 10;
来源：http://agy.c1oappe.top

[Q50] 批量更新
来源：http://uuo.yfazqb.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://uhl.xylfe.cn

[Q51] 用子查询更新
来源：http://hrt.xziqi.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://qxw.havefunace.top

[Q52] 删除指定行
来源：http://arm.shuidangran.top

DELETE FROM users WHERE id = 10;
来源：http://met.ydjk.org.cn

[Q53] 按条件删除
来源：http://smb.zdbjq.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://siz.ywan-chungtsiang.top

[Q54] 清空表
来源：http://hna.yj20258888.top

TRUNCATE TABLE logs;
来源：http://mgb.hfpthk.cn

[Q55] 排名（并列占位）
来源：http://nvt.hammf.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://unb.shanyushiyangkeji.top

[Q56] 密集排名（并列不占位）
来源：http://jga.xinyue.icu

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://utw.hammf.cn

[Q57] 行号
来源：http://pds.yj20258888.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://nil.vehdjk.com

[Q58] 累计求和
来源：http://oal.yangfankeji.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://exp.jiagoushi.top

[Q59] 分组内累计
来源：http://mqn.xziqi.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://oos.0kj1m.cn

[Q60] 取上一行 / 下一行
来源：http://xhd.yongpay.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://tml.yuxming.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://coz.xylfe.cn

[Q61] 移动平均
来源：http://ojb.xuanzx.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mmc.zhaomingkeji.xyz

[Q62] 分组占比
来源：http://jwt.xziqi.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wdc.zhengqikj.top

[Q63] 开启事务
来源：http://poj.jinqigfzy.top

START TRANSACTION;                -- 或 BEGIN
来源：http://zpw.uphjek.com

[Q64] 提交事务
来源：http://nji.zhongyouzk.top

COMMIT;
来源：http://rnp.chenzaomai.com

[Q65] 回滚事务
来源：http://idu.haohaochexian.top

ROLLBACK;
来源：http://rmu.meibo888.top

[Q66] 行锁查询
来源：http://fnh.zhengqikj.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://zhh.ywan-chungtsiang.top

[Q67] 设置隔离级别
来源：http://cot.hnxiangtu.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://piv.jyoumei.cn

[Q68] 保存点
来源：http://eqi.smart0.xyz

SAVEPOINT sp1;
来源：http://dwm.pycfn.com

ROLLBACK TO sp1;
来源：http://lbs.cqqwz.cn

[Q69] 查看执行计划
来源：http://ymy.snrcjt.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://jwj.zhaomingkeji.xyz

[Q70] 更新统计信息
来源：http://btf.cheryme.top

ANALYZE TABLE users;
来源：http://fjx.tanke756.top

[Q71] 查看建表语句
来源：http://hei.jinqigufen.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://pgf.quarkkingdee.top

[Q72] 查看索引
来源：http://tfo.tanke756.top

SHOW INDEX FROM users;
来源：http://zud.pengpengdd.cyou

[Q73] 查看表状态
来源：http://kus.svipenyu.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://vot.ctjpmb.com

[Q74] 强制使用索引
来源：http://ckj.dianchejie.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://cpy.hywenlv.cn

[Q75] 日期格式化
来源：http://aus.zycfv.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://qxy.ydzc1.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://rpz.vehdjk.com

[Q76] 按天统计
来源：http://zvl.yueranfly.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://yxe.yueranfly.top

[Q77] 时间加减
来源：http://vbn.shanyushiyangtech.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ihz.redwolf501.top

[Q78] 当前时间
来源：http://ogc.0kj1m.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://rsg.jinqigfzy.top

[Q79] 字符串拼接
来源：http://bmo.sweek.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://jry.fengsongda.top

[Q80] 字符串截取
来源：http://smj.tarul.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://kxs.vqdsnc.cn

[Q81] 字符串替换
来源：http://csb.ctjpmb.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://duy.hammf.cn

[Q82] 字符长度与字节长度
来源：http://ipy.hywenlv.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://qho.cdnleiting.top

[Q83] 大小写转换
来源：http://bbz.pengpengdd.cyou

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mvz.gotoacloud.top

[Q84] 去除首尾空格
来源：http://lqn.yonumen.top

SELECT TRIM(name) FROM users;
来源：http://akc.sufxvd.cn

[Q85] 数值取整
来源：http://uik.tianlin.xyz

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://rpo.shzxlz.cn

[Q86] 读取 JSON 字段
来源：http://nej.xuanzx.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mix.xuetiantiany.cn

[Q87] JSON 字段做条件
来源：http://usq.zhixingplan.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://usp.ywan-chungtsiang.top

[Q88] 行转列（条件聚合）
来源：http://jod.0kj1m.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://btq.nwbrower.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://vsh.cdnleiting.top

[Q89] 判断表是否存在
来源：http://vuv.ehwqpu.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://bpd.sxryk.cn

[Q90] 生成序号列
来源：http://prx.hongshengwenyu.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://xma.chenlongwang.top

================================================================================
来源：http://csw.yuxming.cn

R. Bash 专题
来源：http://daf.zhaomingkeji.xyz

================================================================================
来源：http://dci.sufxvd.cn

[R01] shebang 与严格模式
来源：http://xut.sxryk.cn

#!/usr/bin/env bash
来源：http://ykk.hongshengwenyu.top

set -euo pipefail
来源：http://czs.jinqigufen.top

[R02] 变量赋值与使用
来源：http://vmt.ctjpmb.com

name="Tom"; echo "$name"
来源：http://pfb.zhengqikj.top

[R03] 只读变量
来源：http://ttw.yj202588.top

readonly PI=3.14
来源：http://arq.yj20258.top

[R04] 位置参数
来源：http://rcz.yj20258888.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://onf.aizwys.cn

[R05] 参数默认值
来源：http://hpz.hesvh.cn

name="${1:-default}"
来源：http://rrc.pengpengdd.cyou

[R06] 判断命令是否存在
来源：http://bws.zhijiandao.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://vpd.zycfv.cn

[R07] if 判断文件
来源：http://sxk.epnwcf.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mss.shangyingyoupin.top

[R08] 数值比较
来源：http://ndv.tianlin.xyz

if (( a > b )); then echo "a 更大"; fi
来源：http://ayq.jinyuanbaomall.cn

[R09] 字符串比较
来源：http://hua.ehwqpu.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://zbz.yfazqb.com

[R10] 正则匹配
来源：http://ttk.feifeiyinyue.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://thz.yvedp.cn

[R11] case 多分支
来源：http://gil.gogol.net.cn

case "$1" in
来源：http://xcb.daria6918.cn

start) echo "启动" ;;
来源：http://pxr.smart0.xyz

stop)  echo "停止" ;;
来源：http://ayw.xylfe.cn

*)     echo "未知命令" ;;
来源：http://qjc.aibaodan.cn

esac
来源：http://fwa.hysaishi.cn

[R12] for 遍历文件
来源：http://vdb.chenlongwang.top

for f in *.txt; do echo "$f"; done
来源：http://xpf.bbcook.cn

[R13] for 计数循环
来源：http://wga.zdqjudy.top

for i in {1..10}; do echo "$i"; done
来源：http://ioa.guannengcc.top

[R14] C 风格 for
来源：http://dwt.zhaomingkeji.xyz

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://yjz.cashguo.top

[R15] while 逐行读文件
来源：http://hbe.wangshuangyany.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://crl.shuidangran.top

[R16] until 等待条件
来源：http://yol.ydzc1.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://gge.9152youxi.cn

[R17] 数组定义与取值
来源：http://aqn.sufxvd.cn

arr=(a b c); echo "${arr[0]}"
来源：http://rbm.yuxming.cn

[R18] 遍历数组
来源：http://brk.haohaochexian.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://crb.xuetiantiany.cn

[R19] 数组长度
来源：http://akg.jinqigufen.top

echo "${#arr[@]}"
来源：http://puj.meibo888.top

[R20] 关联数组（字典）
来源：http://qav.fehbvm.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://obw.jlsjyb.cn

[R21] 字符串长度
来源：http://sqp.0kj1m.cn

echo "${#s}"
来源：http://yjs.yuxming.cn

[R22] 截取子串
来源：http://yoj.cashguo.top

echo "${s:0:5}"
来源：http://yvt.shanyushiyangtech.top

[R23] 字符串替换
来源：http://eav.jinqigufen.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mok.kuanghao11.cn

[R24] 大小写转换
来源：http://rjc.yvedp.cn

echo "${s^^}"; echo "${s,,}"
来源：http://nnh.cucudq.cn

[R25] 去后缀 / 去前缀
来源：http://ght.shangyingyoupin.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://olg.fanxiaobao.xyz

[R26] 命令替换
来源：http://kpf.quarkkingdee.top

now=$(date +%F); echo "$now"
来源：http://cpn.yongpay.top

[R27] 算术展开
来源：http://gok.fanxiaobao.xyz

echo $((1 + 2 * 3))
来源：http://epd.zhaomingkeji.xyz

[R28] 浮点运算
来源：http://twf.pengpengdd.cyou

echo "scale=2; 10/3" | bc
来源：http://nqf.sjlbkw.cn

[R29] 定义函数
来源：http://znx.smart0.xyz

add() { echo $(($1 + $2)); }; add 1 2
来源：http://qwr.svipenyu.cn

[R30] 函数返回状态码
来源：http://cln.sjlbkw.cn

f() { return 0; }; f || echo "失败了"
来源：http://ket.cqqwz.cn

[R31] 局部变量
来源：http://qok.snrcjt.cn

f() { local x=1; echo "$x"; }
来源：http://gfh.chenzaomai.com

[R32] 参数个数校验
来源：http://lcy.ywan-chungtsiang.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://llf.fzhhl.top

[R33] 捕获错误并提示行号
来源：http://nvr.shangyingyoupin.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://nij.ybcxt.top

[R34] 退出时清理
来源：http://odg.nwbrower.top

trap 'rm -f "$tmp"' EXIT
来源：http://lff.yj20258.top

[R35] 后台执行并等待
来源：http://gpb.sufxvd.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://xzd.hammf.cn

[R36] 并发执行多个任务
来源：http://lgt.bbcook.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hwj.jinqigufen.top

[R37] 把输出赋给变量
来源：http://zbx.yj20258888.top

files=$(ls -1)
来源：http://uzn.aizwys.cn

[R38] 管道串联
来源：http://djd.fzhhl.top

cat a.txt | grep -i error | wc -l
来源：http://mmv.shzxlz.cn

[R39] 重定向标准输出与错误
来源：http://ewg.chenlongwang.top

cmd > out.log 2>&1
来源：http://wzo.vqdsnc.cn

[R40] 追加写日志
来源：http://xqd.jinqigfzy.top

echo "log" >> out.log
来源：http://vmh.ppjwa.cn

[R41] 丢弃输出
来源：http://epu.tian-w.cn

cmd >/dev/null 2>&1
来源：http://otc.sysykeji.top

[R42] 输入重定向
来源：http://ptm.jlsjyb.cn

wc -l < a.txt
来源：http://jbe.316326.xyz

[R43] 按名字查找文件
来源：http://zkh.yanxiufei.cn

find . -name "*.log" -type f
来源：http://kyl.wangdashe.top

[R44] 按修改时间查找
来源：http://juc.ivvv.top

find . -mtime -7 -type f
来源：http://vnb.hesvh.cn

[R45] 批量删除
来源：http://fxc.chenlongwang.top

find . -name "*.tmp" -delete
来源：http://gyt.fanxiaobao.xyz

[R46] 递归替换文件内容
来源：http://dlq.cdnleiting.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://rby.pycfn.com

[R47] sed 单行替换
来源：http://wnt.yanxiufei.cn

sed -i 's/foo/bar/g' a.txt
来源：http://oji.tarul.cn

[R48] awk 取指定列
来源：http://qav.svipenyu.cn

awk '{print $1, $3}' a.txt
来源：http://yps.hnxiangtu.top

[R49] awk 带条件
来源：http://vja.svipenyu.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://qdh.chenlongwang.top

[R50] awk 求和
来源：http://mda.xingfuxueyuan.xyz

awk '{s += $2} END {print s}' a.txt
来源：http://pbp.kuanghao11.cn

[R51] 排序去重取前几
来源：http://qow.zycfv.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://gqs.hfpthk.cn

[R52] 统计行数
来源：http://gur.cheryme.top

wc -l a.txt
来源：http://grp.ctjpmb.com

[R53] 查看文件头与实时尾
来源：http://luv.sufxvd.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://bdc.gzhubu.top

[R54] 比较两个文件
来源：http://brh.bjfxy.top

diff a.txt b.txt
来源：http://lly.aizwys.cn

[R55] 压缩与解压
来源：http://htd.jinghuilouyu.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://qbw.xziqi.cn

[R56] 远程拷贝
来源：http://qck.jinyuanbaomall.cn

scp file user@host:/path/
来源：http://oty.9152youxi.cn

[R57] 远程执行命令
来源：http://art.sjlbkw.cn

ssh user@host 'uptime'
来源：http://mvg.ppjwa.cn

[R58] 下载文件
来源：http://zry.yvedp.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ied.uphjek.com

[R59] 发 POST JSON
来源：http://yca.jiagoushi.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ydh.smart0.xyz

[R60] 只看 HTTP 状态码
来源：http://obl.hnqzz.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://rpb.hfpthk.cn

[R61] 磁盘占用
来源：http://mbt.yangfankeji.com

df -h;  du -sh *
来源：http://jmf.haohaochexian.top

[R62] 找最占空间的文件
来源：http://wpp.zhengqikj.top

du -ah . | sort -rh | head -10
来源：http://rnl.vehdjk.com

[R63] 内存与进程
来源：http://vag.jinyuanbaomall.cn

free -h;  ps aux | grep nginx
来源：http://pxh.cheryme.top

[R64] 结束进程
来源：http://zer.jinqigufen.top

kill -9 $(pgrep -f app.py)
来源：http://tnp.wangshuangyany.cn

[R65] 查看端口占用
来源：http://omi.sweek.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://byl.nanxuanxn.top

[R66] 定时任务
来源：http://ljc.gogol.net.cn

crontab -e;  crontab -l
来源：http://rzu.jinyuanbaomall.cn

[R67] 生成随机十六进制串
来源：http://xgn.yj20258.top


<!-- 参考信息 -->