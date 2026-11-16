代发 wailian999

SELECT * FROM users;
来源：http://rmu.haohaochexian.top

[Q16] 查询指定列
来源：http://bop.vehdjk.com

SELECT id, name FROM users;
来源：http://djw.cqqwz.cn

[Q17] 条件查询
来源：http://env.shuidangran.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://imu.epnwcf.com

[Q18] 模糊匹配
来源：http://ozw.ppjwa.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://jbi.tanke756.top

[Q19] 范围查询
来源：http://nks.vqdsnc.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://edt.yueranfly.top

[Q20] IN 列表
来源：http://cpu.jiagoushi.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mrv.cheryme.top

[Q21] 空值判断
来源：http://oxq.fehbvm.com

SELECT * FROM users WHERE email IS NULL;
来源：http://zxb.c1oappe.top

[Q22] 排序
来源：http://zyz.yongpay.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://lzz.andypj.xyz

[Q23] 分页
来源：http://wfg.epnwcf.com

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://bmj.tian-w.cn

[Q24] 去重
来源：http://gdy.jqgufenzy.top

SELECT DISTINCT city FROM users;
来源：http://yff.shangyingyoupin.top

[Q25] 只取前 N 条
来源：http://cwn.yangfankeji.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://jmh.zdbjq.cn

[Q26] 计数
来源：http://qzj.zhoulong.xyz

SELECT COUNT(*) FROM users;
来源：http://jad.dianchejie.cn

[Q27] 条件计数
来源：http://hbo.yongpay.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://vva.chenlongwang.top

[Q28] 求和与平均
来源：http://esy.zhoulong.xyz

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://goz.daria6918.cn

[Q29] 最大最小值
来源：http://mcn.andypj.xyz

SELECT MAX(age), MIN(age) FROM users;
来源：http://voz.ivvv.top

[Q30] 分组统计
来源：http://sqo.jinghuilouyu.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://yap.epnwcf.com

[Q31] 分组后过滤
来源：http://oqs.jqgufenzy.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://kte.cashguo.top

[Q32] 分组拼接字符串
来源：http://jmw.zdqjudy.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://qij.shuidangran.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://jfm.gogol.net.cn

[Q33] 多列分组
来源：http://jkz.ppjwa.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ahy.ywan-chungtsiang.top

[Q34] 每组取第一条
来源：http://ubx.smart0.xyz

SELECT * FROM (
来源：http://hcl.fehbvm.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://deh.guannengcc.top

) t WHERE rn = 1;
来源：http://teu.jinyuanbaomall.cn

[Q35] 内连接
来源：http://gbl.gzhubu.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://fqb.yongpay.top

[Q36] 左连接
来源：http://hvc.gzhubu.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://oeq.jyoumei.cn

[Q37] 右连接
来源：http://iju.shzxlz.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://nqj.sxryk.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ymn.yj202588.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://jno.nwbrower.top

[Q39] 自连接（查上下级）
来源：http://pxj.meibo888.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://vld.sjlbkw.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ryb.jqgfzy.top

[Q40] 交叉连接（笛卡尔积）
来源：http://tcr.pengpengdd.cyou

SELECT * FROM colors CROSS JOIN sizes;
来源：http://iaq.vehdjk.com

[Q41] 多表连接
来源：http://ihr.guowangkeji.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://byk.chenlongwang.top

JOIN users u ON u.id = o.user_id
来源：http://zla.jinyuanbaomall.cn

JOIN products p ON p.id = o.product_id;
来源：http://tti.aizwys.cn

[Q42] 连接条件附加过滤
来源：http://smv.gotoacloud.top

SELECT u.name, o.amount FROM users u
来源：http://hww.yj202588.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://cxw.svipenyu.cn

[Q43] 标量子查询
来源：http://wmv.aibaodan.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://vpj.tianlin.xyz

[Q44] IN 子查询
来源：http://jte.shanyushiyangtech.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ehr.zycfv.cn

[Q45] EXISTS 判断存在
来源：http://gcm.jianghu66.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://diu.yongpay.top

[Q46] NOT EXISTS 判断不存在
来源：http://mew.shanyushiyangtech.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vzt.pycfn.com

[Q47] 与平均值比较
来源：http://ege.0kj1m.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://lnb.pengpengdd.cyou

[Q48] CTE 公用表表达式
来源：http://okd.gotoacloud.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://kkd.zhixingplan.top

SELECT * FROM t WHERE c > 5;
来源：http://zby.bjfxy.top

[Q49] 更新单行
来源：http://cnc.smart0.xyz

UPDATE users SET status = 1 WHERE id = 10;
来源：http://dnb.andypj.xyz

[Q50] 批量更新
来源：http://xzk.gogol.net.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://utl.zhoulong.xyz

[Q51] 用子查询更新
来源：http://vdx.tanke756.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://xyc.sufxvd.cn

[Q52] 删除指定行
来源：http://oey.0kj1m.cn

DELETE FROM users WHERE id = 10;
来源：http://sok.shuidangran.top

[Q53] 按条件删除
来源：http://oxk.shuidangran.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ovp.zhijiandao.cn

[Q54] 清空表
来源：http://efn.hcnkem.com

TRUNCATE TABLE logs;
来源：http://zbo.jinqigfzy.top

[Q55] 排名（并列占位）
来源：http://jzk.zycfv.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://exw.gogol.net.cn

[Q56] 密集排名（并列不占位）
来源：http://uly.bjfxy.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://bwg.jiagoushi.top

[Q57] 行号
来源：http://lju.iojbl.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://pvp.feifeiyinyue.top

[Q58] 累计求和
来源：http://iyv.dashuyun.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://inq.gotoacloud.top

[Q59] 分组内累计
来源：http://lec.fzhhl.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://kli.yonumen.top

[Q60] 取上一行 / 下一行
来源：http://afg.hcnkem.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://pxv.nanxinkj.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://owy.hongshengwenyu.top

[Q61] 移动平均
来源：http://yxf.ivvv.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://npn.aizwys.cn

[Q62] 分组占比
来源：http://iwm.gzhubu.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://dis.chenjidiqi.icu

[Q63] 开启事务
来源：http://hqp.yj20258.top

START TRANSACTION;                -- 或 BEGIN
来源：http://arz.fzhhl.top

[Q64] 提交事务
来源：http://fgg.dashuyun.cn

COMMIT;
来源：http://jgu.sufxvd.cn

[Q65] 回滚事务
来源：http://vel.yfazqb.com

ROLLBACK;
来源：http://pvh.zdbjq.cn

[Q66] 行锁查询
来源：http://oos.yuanzhike.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://faw.aizwys.cn

[Q67] 设置隔离级别
来源：http://qtn.cucudq.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://fgz.yanxiufei.cn

[Q68] 保存点
来源：http://chb.ppjwa.cn

SAVEPOINT sp1;
来源：http://lyz.jinyuanbaomall.cn

ROLLBACK TO sp1;
来源：http://ffp.dianchejie.cn

[Q69] 查看执行计划
来源：http://yae.redwolf501.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://iet.yvedp.cn

[Q70] 更新统计信息
来源：http://mhj.xylfe.cn

ANALYZE TABLE users;
来源：http://fpn.xylfe.cn

[Q71] 查看建表语句
来源：http://hab.yanxiufei.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://gur.ybcxt.top

[Q72] 查看索引
来源：http://vbw.yonumen.top

SHOW INDEX FROM users;
来源：http://xnw.havefunace.top

[Q73] 查看表状态
来源：http://xfs.shanyushiyangtech.top

SHOW TABLE STATUS LIKE 'users';
来源：http://tzw.cqqwz.cn

[Q74] 强制使用索引
来源：http://tsd.vehdjk.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://cpj.zhixingplan.top

[Q75] 日期格式化
来源：http://dpp.zhongyouzk.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://xbs.shuidangran.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://gpr.tian-w.cn

[Q76] 按天统计
来源：http://rdc.nanxuanxn.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://yxn.meibo888.top

[Q77] 时间加减
来源：http://ppp.quarkkingdee.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://tjx.tian-w.cn

[Q78] 当前时间
来源：http://xob.yj20258888.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://siv.jinqigufen.top

[Q79] 字符串拼接
来源：http://ahc.cashguo.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://rui.ydzc1.top

[Q80] 字符串截取
来源：http://cec.sufxvd.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://idp.yj20258.top

[Q81] 字符串替换
来源：http://qci.tian-w.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://qis.ivvv.top

[Q82] 字符长度与字节长度
来源：http://gxg.316326.xyz

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://njw.yfazqb.com

[Q83] 大小写转换
来源：http://qob.cheryme.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://dmj.yj202588.top

[Q84] 去除首尾空格
来源：http://xoo.dianchejie.cn

SELECT TRIM(name) FROM users;
来源：http://kad.gogol.net.cn

[Q85] 数值取整
来源：http://ugm.gaohongyu789.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://aqf.xziqi.cn

[Q86] 读取 JSON 字段
来源：http://gky.haohaochexian.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://rjz.jinyuanbaomall.cn

[Q87] JSON 字段做条件
来源：http://ghl.yonumen.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mlx.tianlin.xyz

[Q88] 行转列（条件聚合）
来源：http://nmn.cucudq.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://gqf.nanxuanxn.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://iei.hcnkem.com

[Q89] 判断表是否存在
来源：http://gxd.jinyuanbaomall.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://zhd.yj20258888.top

[Q90] 生成序号列
来源：http://vou.cheryme.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://tbp.fktsv.cn

================================================================================
来源：http://wee.gzhubu.top

R. Bash 专题
来源：http://hfe.jqgufenzy.top

================================================================================
来源：http://crm.shanyushiyangkeji.top

[R01] shebang 与严格模式
来源：http://zcq.jyoumei.cn

#!/usr/bin/env bash
来源：http://pqz.shanyushiyangkeji.top

set -euo pipefail
来源：http://ivf.sysykeji.top

[R02] 变量赋值与使用
来源：http://wru.gogol.net.cn

name="Tom"; echo "$name"
来源：http://yhh.shanyushiyangkeji.top

[R03] 只读变量
来源：http://wmn.yongpay.top

readonly PI=3.14
来源：http://gpk.fehbvm.com

[R04] 位置参数
来源：http://kos.uphjek.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://vph.shangyingyoupin.top

[R05] 参数默认值
来源：http://xww.ppjwa.cn

name="${1:-default}"
来源：http://rmr.smart0.xyz

[R06] 判断命令是否存在
来源：http://njn.aizwys.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://zqs.andypj.xyz

[R07] if 判断文件
来源：http://frn.jinqigufen.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://xiv.pycfn.com

[R08] 数值比较
来源：http://osi.cucudq.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://kui.kuanghao11.cn

[R09] 字符串比较
来源：http://bmy.jqgufenzy.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://won.hesvh.cn

[R10] 正则匹配
来源：http://ggi.nwbrower.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ycw.xziqi.cn

[R11] case 多分支
来源：http://zns.ehwqpu.com

case "$1" in
来源：http://qkw.shanyushiyangtech.top

start) echo "启动" ;;
来源：http://fmi.fehbvm.com

stop)  echo "停止" ;;
来源：http://cyn.jinqigufen.top

*)     echo "未知命令" ;;
来源：http://wtb.aizwys.cn

esac
来源：http://ugs.zdbjq.cn

[R12] for 遍历文件
来源：http://lqq.sweek.top

for f in *.txt; do echo "$f"; done
来源：http://nvl.andypj.xyz

[R13] for 计数循环
来源：http://esn.gzhubu.top

for i in {1..10}; do echo "$i"; done
来源：http://jdl.tarul.cn

[R14] C 风格 for
来源：http://rtg.jinghuilouyu.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://uer.yj20258888.top

[R15] while 逐行读文件
来源：http://xry.hnqzz.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://eek.feifeiyinyue.top

[R16] until 等待条件
来源：http://hpj.yueranfly.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://fda.yvedp.cn

[R17] 数组定义与取值
来源：http://yll.epnwcf.com

arr=(a b c); echo "${arr[0]}"
来源：http://ayj.aizwys.cn

[R18] 遍历数组
来源：http://brx.tanke756.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://iwd.haohaochexian.top

[R19] 数组长度
来源：http://zmx.ybcxt.top

echo "${#arr[@]}"
来源：http://iwg.jinghuilouyu.cn

[R20] 关联数组（字典）
来源：http://vdk.hnxiangtu.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wyu.tanke756.top

[R21] 字符串长度
来源：http://hsv.kuanghao11.cn

echo "${#s}"
来源：http://alz.fengsongda.top

[R22] 截取子串
来源：http://jyb.feifeiyinyue.top

echo "${s:0:5}"
来源：http://qdq.zhoulong.xyz

[R23] 字符串替换
来源：http://tla.zhijiandao.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ztm.ywan-chungtsiang.top

[R24] 大小写转换
来源：http://pha.shanyushiyangtech.top

echo "${s^^}"; echo "${s,,}"
来源：http://qeb.jianghu66.top

[R25] 去后缀 / 去前缀
来源：http://gyn.sysykeji.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://jny.zdqjudy.top

[R26] 命令替换
来源：http://oqr.nwbrower.top

now=$(date +%F); echo "$now"
来源：http://vpt.xziqi.cn

[R27] 算术展开
来源：http://djv.guowangkeji.top

echo $((1 + 2 * 3))
来源：http://fab.quarkkingdee.top

[R28] 浮点运算
来源：http://xwk.yueranfly.top

echo "scale=2; 10/3" | bc
来源：http://zlm.52xcode.cn

[R29] 定义函数
来源：http://cwe.sxryk.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://iiz.52xcode.cn

[R30] 函数返回状态码
来源：http://bep.svipenyu.cn

f() { return 0; }; f || echo "失败了"
来源：http://puo.andypj.xyz

[R31] 局部变量
来源：http://uvk.cdnleiting.top

f() { local x=1; echo "$x"; }
来源：http://jqp.tian-w.cn

[R32] 参数个数校验
来源：http://cxq.zhongyouzk.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ypd.xziqi.cn

[R33] 捕获错误并提示行号
来源：http://inu.uphjek.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mom.zhengqikj.top

[R34] 退出时清理
来源：http://utz.c1oappe.top

trap 'rm -f "$tmp"' EXIT
来源：http://ktr.fanxiaobao.xyz

[R35] 后台执行并等待
来源：http://wti.vqdsnc.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://exr.c1oappe.top

[R36] 并发执行多个任务
来源：http://xud.tianlin.xyz

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://tnt.gzhubu.top

[R37] 把输出赋给变量
来源：http://aru.ydjk.org.cn

files=$(ls -1)
来源：http://bzw.fengsongda.top

[R38] 管道串联
来源：http://xbq.wangshuangyany.cn

cat a.txt | grep -i error | wc -l
来源：http://srn.jinqigufen.top

[R39] 重定向标准输出与错误
来源：http://ceh.yfazqb.com

cmd > out.log 2>&1
来源：http://zlf.nanxinkj.top

[R40] 追加写日志
来源：http://zlp.tianlin.xyz

echo "log" >> out.log
来源：http://wlp.quarkkingdee.top

[R41] 丢弃输出
来源：http://yml.guannengcc.top

cmd >/dev/null 2>&1
来源：http://rpv.gzhubu.top

[R42] 输入重定向
来源：http://wye.ywan-chungtsiang.top

wc -l < a.txt
来源：http://nhe.xuetiantiany.cn

[R43] 按名字查找文件
来源：http://gqf.xylfe.cn

find . -name "*.log" -type f
来源：http://olf.fzhhl.top

[R44] 按修改时间查找
来源：http://alv.redwolf501.top

find . -mtime -7 -type f
来源：http://cxn.ywan-chungtsiang.top

[R45] 批量删除
来源：http://dli.wangdashe.top

find . -name "*.tmp" -delete
来源：http://bqe.jlsjyb.cn

[R46] 递归替换文件内容
来源：http://pcp.ydzc1.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://etx.fzhhl.top

[R47] sed 单行替换
来源：http://hzj.tarul.cn

sed -i 's/foo/bar/g' a.txt
来源：http://kph.zycfv.cn

[R48] awk 取指定列
来源：http://epq.zhixingplan.top

awk '{print $1, $3}' a.txt
来源：http://jxp.sufxvd.cn

[R49] awk 带条件
来源：http://vvt.zycfv.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://bit.jlsjyb.cn

[R50] awk 求和
来源：http://kys.cdnleiting.top

awk '{s += $2} END {print s}' a.txt
来源：http://mkx.jinyuanbaomall.cn

[R51] 排序去重取前几
来源：http://roi.vqdsnc.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://pfa.meibo888.top

[R52] 统计行数
来源：http://qpo.kuanghao11.cn

wc -l a.txt
来源：http://vte.aibaodan.cn

[R53] 查看文件头与实时尾
来源：http://tuf.sweek.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://bgr.jiagoushi.top

[R54] 比较两个文件
来源：http://meg.tanke756.top

diff a.txt b.txt
来源：http://yfa.yvedp.cn

[R55] 压缩与解压
来源：http://lou.zhoulong.xyz

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://vir.gzhubu.top

[R56] 远程拷贝
来源：http://eqj.nanxinkj.top

scp file user@host:/path/
来源：http://vgy.yvedp.cn

[R57] 远程执行命令
来源：http://ril.feifeiyinyue.top

ssh user@host 'uptime'
来源：http://wwr.haohaochexian.top

[R58] 下载文件
来源：http://kdz.dashuyun.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://njc.yj20258888.top

[R59] 发 POST JSON
来源：http://fge.redwolf501.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://sbn.feifeiyinyue.top

[R60] 只看 HTTP 状态码
来源：http://mao.xinyue.icu

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://gfr.bbcook.cn

[R61] 磁盘占用
来源：http://wki.bjfxy.top

df -h;  du -sh *
来源：http://emp.52xcode.cn

[R62] 找最占空间的文件
来源：http://tdo.ywan-chungtsiang.top

du -ah . | sort -rh | head -10
来源：http://tkt.xylfe.cn

[R63] 内存与进程
来源：http://had.ctjpmb.com

free -h;  ps aux | grep nginx
来源：http://hyb.chenjidiqi.icu

[R64] 结束进程
来源：http://nfh.jianghu66.top

kill -9 $(pgrep -f app.py)
来源：http://nqg.jinqigfzy.top

[R65] 查看端口占用
来源：http://qav.yj202588.top


<!-- 参考信息 -->