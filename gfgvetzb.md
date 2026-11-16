代发 wailian999

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ypw.fehbvm.com

[Q11] 一次插入多行
来源：http://ose.yvedp.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://shk.daxiang520.top

[Q12] 插入后取自增 ID
来源：http://evv.yj20258.top

INSERT INTO users (name) VALUES ('C');
来源：http://fck.yanxiufei.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://fej.yanxiufei.cn

[Q13] 忽略重复插入
来源：http://afm.zhijiandao.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://loy.zhongyouzk.top

[Q14] 存在则更新（upsert）
来源：http://lho.tanke756.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://zzo.hongshengwenyu.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://pie.yueranfly.top

[Q15] 查询全部
来源：http://zny.sufxvd.cn

SELECT * FROM users;
来源：http://evy.wangdashe.top

[Q16] 查询指定列
来源：http://vec.ybcxt.top

SELECT id, name FROM users;
来源：http://cna.smart0.xyz

[Q17] 条件查询
来源：http://yhz.xuetiantiany.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ung.svipenyu.cn

[Q18] 模糊匹配
来源：http://vdx.yvedp.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://kyk.xuanzx.com

[Q19] 范围查询
来源：http://rti.sufxvd.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://vgd.hfpthk.cn

[Q20] IN 列表
来源：http://oed.tianlin.xyz

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://yks.ppjwa.cn

[Q21] 空值判断
来源：http://kpj.shuidangran.top

SELECT * FROM users WHERE email IS NULL;
来源：http://vxk.gogol.net.cn

[Q22] 排序
来源：http://mtp.havefunace.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ubw.shanyushiyangtech.top

[Q23] 分页
来源：http://vuv.ehwqpu.com

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://qnc.hysaishi.cn

[Q24] 去重
来源：http://fov.cheryme.top

SELECT DISTINCT city FROM users;
来源：http://hig.xinyue.icu

[Q25] 只取前 N 条
来源：http://sdf.uphjek.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://kwk.pengpengdd.cyou

[Q26] 计数
来源：http://ban.tianlin.xyz

SELECT COUNT(*) FROM users;
来源：http://aww.0kj1m.cn

[Q27] 条件计数
来源：http://ida.hysaishi.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://nzl.hysaishi.cn

[Q28] 求和与平均
来源：http://zue.daria6918.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://eri.aizwys.cn

[Q29] 最大最小值
来源：http://erw.fengsongda.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://ryl.chenzaomai.com

[Q30] 分组统计
来源：http://iix.yangfankeji.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://gpq.chenzaomai.com

[Q31] 分组后过滤
来源：http://kge.sxryk.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://rya.bjfxy.top

[Q32] 分组拼接字符串
来源：http://xsp.yonumen.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://knk.nwbrower.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://uzz.fanxiaobao.xyz

[Q33] 多列分组
来源：http://zvg.yongpay.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://dhy.dashuyun.cn

[Q34] 每组取第一条
来源：http://zhz.cdnleiting.top

SELECT * FROM (
来源：http://cuf.snrcjt.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://tyb.jinyuanbaomall.cn

) t WHERE rn = 1;
来源：http://bxt.cucudq.cn

[Q35] 内连接
来源：http://tha.yfazqb.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://eeo.cqqwz.cn

[Q36] 左连接
来源：http://nwm.cdnleiting.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://gaw.xziqi.cn

[Q37] 右连接
来源：http://tws.wangdashe.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://gkv.ybcxt.top

[Q38] 全外连接（PostgreSQL）
来源：http://bkr.fehbvm.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ror.redwolf501.top

[Q39] 自连接（查上下级）
来源：http://ccq.gogol.net.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://hap.shanyushiyangkeji.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://oee.yongpay.top

[Q40] 交叉连接（笛卡尔积）
来源：http://nwk.dashuyun.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://bqx.xuanzx.com

[Q41] 多表连接
来源：http://rqe.hnxiangtu.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://jxi.ivvv.top

JOIN users u ON u.id = o.user_id
来源：http://qdj.shanyushiyangkeji.top

JOIN products p ON p.id = o.product_id;
来源：http://ehs.cheryme.top

[Q42] 连接条件附加过滤
来源：http://ewt.jqgufenzy.top

SELECT u.name, o.amount FROM users u
来源：http://hud.bbcook.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://jwn.zhixingplan.top

[Q43] 标量子查询
来源：http://ist.sxryk.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://eyq.yfazqb.com

[Q44] IN 子查询
来源：http://jib.zycfv.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ybt.zhijiandao.cn

[Q45] EXISTS 判断存在
来源：http://xcs.jiagoushi.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jix.sweek.top

[Q46] NOT EXISTS 判断不存在
来源：http://hqf.snrcjt.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kud.jinqigfzy.top

[Q47] 与平均值比较
来源：http://iqb.tian-w.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wqk.cucudq.cn

[Q48] CTE 公用表表达式
来源：http://wnz.xziqi.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://oga.yvedp.cn

SELECT * FROM t WHERE c > 5;
来源：http://kul.birdmap.top

[Q49] 更新单行
来源：http://ssv.cdnleiting.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://vov.tarul.cn

[Q50] 批量更新
来源：http://tpt.guannengcc.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ejq.jinqigfzy.top

[Q51] 用子查询更新
来源：http://jzp.yueranfly.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://sre.birdmap.top

[Q52] 删除指定行
来源：http://wur.jlsjyb.cn

DELETE FROM users WHERE id = 10;
来源：http://rwe.daxiang520.top

[Q53] 按条件删除
来源：http://psz.xuanzx.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://bpr.zhixingplan.top

[Q54] 清空表
来源：http://use.zdqjudy.top

TRUNCATE TABLE logs;
来源：http://nbr.zhongyouzk.top

[Q55] 排名（并列占位）
来源：http://rwr.c1oappe.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://lhm.gogol.net.cn

[Q56] 密集排名（并列不占位）
来源：http://qvq.nwbrower.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://nuv.c1oappe.top

[Q57] 行号
来源：http://hdy.jyoumei.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://qsx.sufxvd.cn

[Q58] 累计求和
来源：http://dfo.yonumen.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hxd.epnwcf.com

[Q59] 分组内累计
来源：http://gms.tianlin.xyz

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://lkt.kuanghao11.cn

[Q60] 取上一行 / 下一行
来源：http://mdz.c1oappe.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://xza.fengsongda.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://plz.ywan-chungtsiang.top

[Q61] 移动平均
来源：http://ctd.xziqi.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://och.tanke756.top

[Q62] 分组占比
来源：http://qmv.pengpengdd.cyou

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://dkh.ctjpmb.com

[Q63] 开启事务
来源：http://tyv.hfpthk.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://uka.shangyingyoupin.top

[Q64] 提交事务
来源：http://imb.jqgfzy.top

COMMIT;
来源：http://uuj.sxryk.cn

[Q65] 回滚事务
来源：http://qbt.xingfuxueyuan.xyz

ROLLBACK;
来源：http://bgn.meibo888.top

[Q66] 行锁查询
来源：http://mqb.xziqi.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://dho.zdqjudy.top

[Q67] 设置隔离级别
来源：http://ujn.feifeiyinyue.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://qui.cashguo.top

[Q68] 保存点
来源：http://feh.shuidangran.top

SAVEPOINT sp1;
来源：http://hgk.vqdsnc.cn

ROLLBACK TO sp1;
来源：http://izp.mhx1999.top

[Q69] 查看执行计划
来源：http://vav.tianlin.xyz

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://kcp.sjlbkw.cn

[Q70] 更新统计信息
来源：http://vtv.vehdjk.com

ANALYZE TABLE users;
来源：http://noy.gogol.net.cn

[Q71] 查看建表语句
来源：http://xue.jqgfzy.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://gvu.jiagoushi.top

[Q72] 查看索引
来源：http://odo.zhongyouzk.top

SHOW INDEX FROM users;
来源：http://abi.chenjidiqi.icu

[Q73] 查看表状态
来源：http://hqf.sysykeji.top

SHOW TABLE STATUS LIKE 'users';
来源：http://shm.bbcook.cn

[Q74] 强制使用索引
来源：http://tfn.jinqigfzy.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://eey.nwbrower.top

[Q75] 日期格式化
来源：http://ijj.cucudq.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ill.jiagoushi.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://kwc.shanyushiyangtech.top

[Q76] 按天统计
来源：http://zpd.tanke756.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ips.epnwcf.com

[Q77] 时间加减
来源：http://pax.ehwqpu.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://kho.jyoumei.cn

[Q78] 当前时间
来源：http://nuu.hcnkem.com

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://quu.pycfn.com

[Q79] 字符串拼接
来源：http://kyq.svipenyu.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://xqi.gogol.net.cn

[Q80] 字符串截取
来源：http://rzw.tanke756.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hal.andypj.xyz

[Q81] 字符串替换
来源：http://teb.jlsjyb.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mmu.yj20258.top

[Q82] 字符长度与字节长度
来源：http://raf.wangshuangyany.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ewq.cucudq.cn

[Q83] 大小写转换
来源：http://elg.cashguo.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://dsh.ywan-chungtsiang.top

[Q84] 去除首尾空格
来源：http://pew.hcnkem.com

SELECT TRIM(name) FROM users;
来源：http://byu.pengpengdd.cyou

[Q85] 数值取整
来源：http://vyq.daxiang520.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ars.dashuyun.cn

[Q86] 读取 JSON 字段
来源：http://mhr.xingfuxueyuan.xyz

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://seb.xuanzx.com

[Q87] JSON 字段做条件
来源：http://tfk.shzxlz.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://gac.shanyushiyangtech.top

[Q88] 行转列（条件聚合）
来源：http://jrf.snrcjt.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://tnn.316326.xyz

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://sjt.52xcode.cn

[Q89] 判断表是否存在
来源：http://kch.yueranfly.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://zjr.meibo888.top

[Q90] 生成序号列
来源：http://ama.zhiwuduotai.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://csn.guowangkeji.top

================================================================================
来源：http://noe.wangshuangyany.cn

R. Bash 专题
来源：http://qiw.yongpay.top

================================================================================
来源：http://ykk.shuidangran.top

[R01] shebang 与严格模式
来源：http://dzm.hcnkem.com

#!/usr/bin/env bash
来源：http://fav.zhiwuduotai.top

set -euo pipefail
来源：http://uaa.sweek.top

[R02] 变量赋值与使用
来源：http://xfi.gaohongyu789.top

name="Tom"; echo "$name"
来源：http://hdt.guowangkeji.top

[R03] 只读变量
来源：http://uic.snrcjt.cn

readonly PI=3.14
来源：http://rue.yj20258888.top

[R04] 位置参数
来源：http://uor.fktsv.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://vms.yuxming.cn

[R05] 参数默认值
来源：http://iky.shangyingyoupin.top

name="${1:-default}"
来源：http://qax.jinghuilouyu.cn

[R06] 判断命令是否存在
来源：http://gpl.hysaishi.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://qyj.fehbvm.com

[R07] if 判断文件
来源：http://hif.shanyushiyangtech.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://nth.cucudq.cn

[R08] 数值比较
来源：http://bbm.jiagoushi.top

if (( a > b )); then echo "a 更大"; fi
来源：http://iwv.hesvh.cn

[R09] 字符串比较
来源：http://wza.tian-w.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://xtd.epnwcf.com

[R10] 正则匹配
来源：http://hlz.cdnleiting.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://egj.zhixingplan.top

[R11] case 多分支
来源：http://maw.nanxinkj.top

case "$1" in
来源：http://exc.zhaomingkeji.xyz

start) echo "启动" ;;
来源：http://aru.yueranfly.top

stop)  echo "停止" ;;
来源：http://xqg.wangdashe.top

*)     echo "未知命令" ;;
来源：http://mux.shanyushiyangtech.top

esac
来源：http://imo.zhijiandao.cn

[R12] for 遍历文件
来源：http://jlq.fanxiaobao.xyz

for f in *.txt; do echo "$f"; done
来源：http://abm.fehbvm.com

[R13] for 计数循环
来源：http://azx.fktsv.cn

for i in {1..10}; do echo "$i"; done
来源：http://fpa.hnqzz.top

[R14] C 风格 for
来源：http://mrd.wangdashe.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://gzp.guowangkeji.top

[R15] while 逐行读文件
来源：http://ubk.jinqigfzy.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://syi.ivvv.top

[R16] until 等待条件
来源：http://pnl.iojbl.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://rji.hongshengwenyu.top

[R17] 数组定义与取值
来源：http://gkk.pycfn.com

arr=(a b c); echo "${arr[0]}"
来源：http://clv.kuanghao11.cn

[R18] 遍历数组
来源：http://xvi.jinqigufen.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://lpj.cheryme.top

[R19] 数组长度
来源：http://sqo.fanxiaobao.xyz

echo "${#arr[@]}"
来源：http://hxv.xuetiantiany.cn

[R20] 关联数组（字典）
来源：http://rnr.gzhubu.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://skt.chenjidiqi.icu

[R21] 字符串长度
来源：http://mjc.chenjidiqi.icu

echo "${#s}"
来源：http://gxt.ybcxt.top

[R22] 截取子串
来源：http://qui.vehdjk.com

echo "${s:0:5}"
来源：http://dvt.mhx1999.top

[R23] 字符串替换
来源：http://isr.ivvv.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://jim.bjfxy.top

[R24] 大小写转换
来源：http://rqj.52xcode.cn

echo "${s^^}"; echo "${s,,}"
来源：http://uwx.feifeiyinyue.top

[R25] 去后缀 / 去前缀
来源：http://kft.meibo888.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://ygh.cheryme.top

[R26] 命令替换
来源：http://yom.tarul.cn

now=$(date +%F); echo "$now"
来源：http://tni.pengpengdd.cyou

[R27] 算术展开
来源：http://rxr.yanxiufei.cn

echo $((1 + 2 * 3))
来源：http://fgb.chenjidiqi.icu

[R28] 浮点运算
来源：http://mwd.hongshengwenyu.top

echo "scale=2; 10/3" | bc
来源：http://qlp.jianghu66.top

[R29] 定义函数
来源：http://ipk.jinyuanbaomall.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://xpx.gaohongyu789.top

[R30] 函数返回状态码
来源：http://dwt.fehbvm.com

f() { return 0; }; f || echo "失败了"
来源：http://dwg.nanxinkj.top

[R31] 局部变量
来源：http://hyk.hnxiangtu.top

f() { local x=1; echo "$x"; }
来源：http://qpv.tarul.cn

[R32] 参数个数校验
来源：http://let.tian-w.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://pls.yuxming.cn

[R33] 捕获错误并提示行号
来源：http://ayw.meibo888.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://dzs.shuidangran.top

[R34] 退出时清理
来源：http://scx.52xcode.cn

trap 'rm -f "$tmp"' EXIT
来源：http://poy.shanyushiyangtech.top

[R35] 后台执行并等待
来源：http://pvt.jinqigfzy.top

sleep 5 & pid=$!; wait "$pid"
来源：http://obu.aibaodan.cn

[R36] 并发执行多个任务
来源：http://djs.hcnkem.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://odg.9152youxi.cn

[R37] 把输出赋给变量
来源：http://njl.xuetiantiany.cn

files=$(ls -1)
来源：http://bzt.gogol.net.cn

[R38] 管道串联
来源：http://biq.xziqi.cn

cat a.txt | grep -i error | wc -l
来源：http://ced.gogol.net.cn

[R39] 重定向标准输出与错误
来源：http://iwj.ctjpmb.com

cmd > out.log 2>&1
来源：http://jup.xziqi.cn

[R40] 追加写日志
来源：http://gto.xingfuxueyuan.xyz

echo "log" >> out.log
来源：http://vwk.hysaishi.cn

[R41] 丢弃输出
来源：http://vak.cashguo.top

cmd >/dev/null 2>&1
来源：http://yvx.jlsjyb.cn

[R42] 输入重定向
来源：http://mcb.zhixingplan.top

wc -l < a.txt
来源：http://qri.aizwys.cn

[R43] 按名字查找文件
来源：http://uzt.cqqwz.cn

find . -name "*.log" -type f
来源：http://xlb.hnqzz.top

[R44] 按修改时间查找
来源：http://zkt.cheryme.top

find . -mtime -7 -type f
来源：http://ulo.ehwqpu.com

[R45] 批量删除
来源：http://umx.shuidangran.top

find . -name "*.tmp" -delete
来源：http://okk.jinghuilouyu.cn

[R46] 递归替换文件内容
来源：http://fwa.ctjpmb.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://vtq.wangshuangyany.cn

[R47] sed 单行替换
来源：http://zun.shuidangran.top

sed -i 's/foo/bar/g' a.txt
来源：http://dow.zhixingplan.top

[R48] awk 取指定列
来源：http://ghq.zhaomingkeji.xyz

awk '{print $1, $3}' a.txt
来源：http://cvd.dianchejie.cn

[R49] awk 带条件
来源：http://hkz.yongpay.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://suj.iojbl.cn

[R50] awk 求和
来源：http://xmx.feifeiyinyue.top

awk '{s += $2} END {print s}' a.txt
来源：http://psj.nwbrower.top

[R51] 排序去重取前几
来源：http://kpe.0kj1m.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://zcd.shzxlz.cn

[R52] 统计行数
来源：http://lsa.jlsjyb.cn

wc -l a.txt
来源：http://xan.dashuyun.cn

[R53] 查看文件头与实时尾
来源：http://doi.iojbl.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://aqx.yvedp.cn

[R54] 比较两个文件
来源：http://xvx.chenzaomai.com

diff a.txt b.txt
来源：http://qij.yvedp.cn

[R55] 压缩与解压
来源：http://nni.pengpengdd.cyou

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://grg.hesvh.cn

[R56] 远程拷贝
来源：http://vsp.yuanzhike.top

scp file user@host:/path/
来源：http://lfr.zdbjq.cn

[R57] 远程执行命令
来源：http://uwg.gogol.net.cn

ssh user@host 'uptime'
来源：http://pdl.xinyue.icu

[R58] 下载文件
来源：http://msd.nanxinkj.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://cjm.snrcjt.cn

[R59] 发 POST JSON
来源：http://zac.hcnkem.com


<!-- 参考信息 -->