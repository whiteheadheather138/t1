代发 wailian999

INSERT INTO users (name) VALUES ('C');
来源：http://rjo.cdnleiting.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://jtt.fengsongda.top

[Q13] 忽略重复插入
来源：http://lqg.yueranfly.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://siy.ctjpmb.com

[Q14] 存在则更新（upsert）
来源：http://oxd.cqqwz.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://uar.shuidangran.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wef.ivvv.top

[Q15] 查询全部
来源：http://qxb.sufxvd.cn

SELECT * FROM users;
来源：http://ruv.birdmap.top

[Q16] 查询指定列
来源：http://hsy.chenjidiqi.icu

SELECT id, name FROM users;
来源：http://qry.shanyushiyangkeji.top

[Q17] 条件查询
来源：http://fqs.dianchejie.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://fwb.jyoumei.cn

[Q18] 模糊匹配
来源：http://cbw.cashguo.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://vcn.tarul.cn

[Q19] 范围查询
来源：http://nqz.hongshengwenyu.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://vld.redwolf501.top

[Q20] IN 列表
来源：http://ohd.zhongyouzk.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://dke.ybcxt.top

[Q21] 空值判断
来源：http://tyn.sufxvd.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://cqb.xingfuxueyuan.xyz

[Q22] 排序
来源：http://qkw.wangshuangyany.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://xkp.hysaishi.cn

[Q23] 分页
来源：http://xas.zhengqikj.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://jyt.quarkkingdee.top

[Q24] 去重
来源：http://trr.zdbjq.cn

SELECT DISTINCT city FROM users;
来源：http://rzh.epnwcf.com

[Q25] 只取前 N 条
来源：http://qdj.yangfankeji.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://odj.haohaochexian.top

[Q26] 计数
来源：http://bsd.svipenyu.cn

SELECT COUNT(*) FROM users;
来源：http://dfw.iojbl.cn

[Q27] 条件计数
来源：http://zkx.tian-w.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://rxn.uphjek.com

[Q28] 求和与平均
来源：http://aeo.gotoacloud.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://akb.gogol.net.cn

[Q29] 最大最小值
来源：http://ewq.iojbl.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://lfo.yuanzhike.top

[Q30] 分组统计
来源：http://xyq.ctjpmb.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://not.daria6918.cn

[Q31] 分组后过滤
来源：http://ild.zhiwuduotai.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://noc.svipenyu.cn

[Q32] 分组拼接字符串
来源：http://vbb.xingfuxueyuan.xyz

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://bqf.hesvh.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://fbx.hywenlv.cn

[Q33] 多列分组
来源：http://ewl.0kj1m.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://nwq.hammf.cn

[Q34] 每组取第一条
来源：http://szh.chenjidiqi.icu

SELECT * FROM (
来源：http://ppx.yongpay.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://yoo.gzhubu.top

) t WHERE rn = 1;
来源：http://sno.jlsjyb.cn

[Q35] 内连接
来源：http://dlv.52xcode.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://muw.zhixingplan.top

[Q36] 左连接
来源：http://oic.epnwcf.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://gdp.bjfxy.top

[Q37] 右连接
来源：http://xdc.zhoulong.xyz

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://jdx.tianlin.xyz

[Q38] 全外连接（PostgreSQL）
来源：http://zzk.fengsongda.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://juu.hywenlv.cn

[Q39] 自连接（查上下级）
来源：http://ozi.xinyue.icu

SELECT e.name, m.name AS manager FROM employees e
来源：http://pma.bbcook.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://uzh.quarkkingdee.top

[Q40] 交叉连接（笛卡尔积）
来源：http://fhs.fehbvm.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://adw.ivvv.top

[Q41] 多表连接
来源：http://ive.iojbl.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://bij.ivvv.top

JOIN users u ON u.id = o.user_id
来源：http://dyf.ydzc1.top

JOIN products p ON p.id = o.product_id;
来源：http://plp.mhx1999.top

[Q42] 连接条件附加过滤
来源：http://onh.ydjk.org.cn

SELECT u.name, o.amount FROM users u
来源：http://ymi.zdbjq.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://spw.shzxlz.cn

[Q43] 标量子查询
来源：http://rvp.aibaodan.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://age.yvedp.cn

[Q44] IN 子查询
来源：http://yrr.birdmap.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hvk.ydzc1.top

[Q45] EXISTS 判断存在
来源：http://qvx.jianghu66.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zzz.xuanzx.com

[Q46] NOT EXISTS 判断不存在
来源：http://jfu.hysaishi.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://meb.zhengqikj.top

[Q47] 与平均值比较
来源：http://mze.xuetiantiany.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://yax.ctjpmb.com

[Q48] CTE 公用表表达式
来源：http://gpk.cashguo.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://guu.jiagoushi.top

SELECT * FROM t WHERE c > 5;
来源：http://mkg.yonumen.top

[Q49] 更新单行
来源：http://ang.ppjwa.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hww.chenzaomai.com

[Q50] 批量更新
来源：http://unw.ivvv.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://nwa.dianchejie.cn

[Q51] 用子查询更新
来源：http://ztv.ctjpmb.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://brl.fehbvm.com

[Q52] 删除指定行
来源：http://pgv.ywan-chungtsiang.top

DELETE FROM users WHERE id = 10;
来源：http://huh.dianchejie.cn

[Q53] 按条件删除
来源：http://cqz.sxryk.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://uay.dianchejie.cn

[Q54] 清空表
来源：http://rkb.fehbvm.com

TRUNCATE TABLE logs;
来源：http://mvh.pycfn.com

[Q55] 排名（并列占位）
来源：http://vci.fengsongda.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hgi.yueranfly.top

[Q56] 密集排名（并列不占位）
来源：http://xhe.zhongyouzk.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://efl.yueranfly.top

[Q57] 行号
来源：http://pbz.jyoumei.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://qay.zdbjq.cn

[Q58] 累计求和
来源：http://lco.hcnkem.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://qmn.jyoumei.cn

[Q59] 分组内累计
来源：http://gqb.shangyingyoupin.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://sxi.shuidangran.top

[Q60] 取上一行 / 下一行
来源：http://ovc.xylfe.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://oky.bbcook.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mvk.ctjpmb.com

[Q61] 移动平均
来源：http://amr.fehbvm.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://lro.tanke756.top

[Q62] 分组占比
来源：http://mky.jinghuilouyu.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://imb.cheryme.top

[Q63] 开启事务
来源：http://iig.sweek.top

START TRANSACTION;                -- 或 BEGIN
来源：http://czr.yueranfly.top

[Q64] 提交事务
来源：http://tob.zdbjq.cn

COMMIT;
来源：http://lmt.vqdsnc.cn

[Q65] 回滚事务
来源：http://nxc.uphjek.com

ROLLBACK;
来源：http://eig.fanxiaobao.xyz

[Q66] 行锁查询
来源：http://ahp.daxiang520.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://sgf.zhiwuduotai.top

[Q67] 设置隔离级别
来源：http://mcd.wangdashe.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://sum.zycfv.cn

[Q68] 保存点
来源：http://oik.hfpthk.cn

SAVEPOINT sp1;
来源：http://kbq.zdbjq.cn

ROLLBACK TO sp1;
来源：http://oxv.iojbl.cn

[Q69] 查看执行计划
来源：http://ejc.ydzc1.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://kgz.zhengqikj.top

[Q70] 更新统计信息
来源：http://iiy.havefunace.top

ANALYZE TABLE users;
来源：http://ctg.pengpengdd.cyou

[Q71] 查看建表语句
来源：http://lyk.kuanghao11.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://nnk.chenlongwang.top

[Q72] 查看索引
来源：http://vkb.yangfankeji.com

SHOW INDEX FROM users;
来源：http://bkq.andypj.xyz

[Q73] 查看表状态
来源：http://yjf.quarkkingdee.top

SHOW TABLE STATUS LIKE 'users';
来源：http://nfl.gogol.net.cn

[Q74] 强制使用索引
来源：http://zyv.hfpthk.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://zqu.ybcxt.top

[Q75] 日期格式化
来源：http://ieo.guowangkeji.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ubi.jinqigfzy.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://qcf.ppjwa.cn

[Q76] 按天统计
来源：http://agy.nanxinkj.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://dsw.zhijiandao.cn

[Q77] 时间加减
来源：http://tdo.haohaochexian.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://lve.shanyushiyangkeji.top

[Q78] 当前时间
来源：http://ygt.hcnkem.com

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://pqn.zhaomingkeji.xyz

[Q79] 字符串拼接
来源：http://fps.quarkkingdee.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://duh.yvedp.cn

[Q80] 字符串截取
来源：http://gtq.jyoumei.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hmd.svipenyu.cn

[Q81] 字符串替换
来源：http://uny.quarkkingdee.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://kec.andypj.xyz

[Q82] 字符长度与字节长度
来源：http://fxd.zhiwuduotai.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://eiw.hesvh.cn

[Q83] 大小写转换
来源：http://pey.xylfe.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://xor.vqdsnc.cn

[Q84] 去除首尾空格
来源：http://iez.yongpay.top

SELECT TRIM(name) FROM users;
来源：http://ycw.bbcook.cn

[Q85] 数值取整
来源：http://sye.wangshuangyany.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://udi.tanke756.top

[Q86] 读取 JSON 字段
来源：http://oks.yj202588.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://rfl.hywenlv.cn

[Q87] JSON 字段做条件
来源：http://zhm.hongshengwenyu.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://onn.c1oappe.top

[Q88] 行转列（条件聚合）
来源：http://fsz.shzxlz.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://vlh.hywenlv.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://afi.tian-w.cn

[Q89] 判断表是否存在
来源：http://nus.ctjpmb.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://uug.svipenyu.cn

[Q90] 生成序号列
来源：http://sbp.hnqzz.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://csu.cucudq.cn

================================================================================
来源：http://kvj.guannengcc.top

R. Bash 专题
来源：http://zjc.yj20258.top

================================================================================
来源：http://gzs.kuanghao11.cn

[R01] shebang 与严格模式
来源：http://nfs.chenlongwang.top

#!/usr/bin/env bash
来源：http://vbu.yfazqb.com

set -euo pipefail
来源：http://xtu.tianlin.xyz

[R02] 变量赋值与使用
来源：http://vdt.yongpay.top

name="Tom"; echo "$name"
来源：http://cbi.dashuyun.cn

[R03] 只读变量
来源：http://ank.sjlbkw.cn

readonly PI=3.14
来源：http://nbe.vehdjk.com

[R04] 位置参数
来源：http://etd.zycfv.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://tcu.zhoulong.xyz

[R05] 参数默认值
来源：http://acv.hywenlv.cn

name="${1:-default}"
来源：http://lgz.hywenlv.cn

[R06] 判断命令是否存在
来源：http://ley.cucudq.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://rjt.hfpthk.cn

[R07] if 判断文件
来源：http://wte.hysaishi.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://dks.jinghuilouyu.cn

[R08] 数值比较
来源：http://ycf.jianghu66.top

if (( a > b )); then echo "a 更大"; fi
来源：http://gjp.epnwcf.com

[R09] 字符串比较
来源：http://clc.zhiwuduotai.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://vrb.xuetiantiany.cn

[R10] 正则匹配
来源：http://afy.tianlin.xyz

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://pxp.yueranfly.top

[R11] case 多分支
来源：http://xdd.snrcjt.cn

case "$1" in
来源：http://ifi.vehdjk.com

start) echo "启动" ;;
来源：http://unq.tarul.cn

stop)  echo "停止" ;;
来源：http://wlo.yvedp.cn

*)     echo "未知命令" ;;
来源：http://whh.jyoumei.cn

esac
来源：http://otl.daxiang520.top

[R12] for 遍历文件
来源：http://lbj.tarul.cn

for f in *.txt; do echo "$f"; done
来源：http://hnq.jlsjyb.cn

[R13] for 计数循环
来源：http://sou.ppjwa.cn

for i in {1..10}; do echo "$i"; done
来源：http://jzb.sysykeji.top

[R14] C 风格 for
来源：http://bel.mhx1999.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://iko.yvedp.cn

[R15] while 逐行读文件
来源：http://plg.cashguo.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://cdt.xziqi.cn

[R16] until 等待条件
来源：http://wal.zhongyouzk.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://fzq.yvedp.cn

[R17] 数组定义与取值
来源：http://uqm.xinyue.icu

arr=(a b c); echo "${arr[0]}"
来源：http://okt.kuanghao11.cn

[R18] 遍历数组
来源：http://lav.jinqigfzy.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://jgq.xingfuxueyuan.xyz

[R19] 数组长度
来源：http://upu.ehwqpu.com

echo "${#arr[@]}"
来源：http://imx.jinghuilouyu.cn

[R20] 关联数组（字典）
来源：http://kzh.tianlin.xyz

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://syc.kuanghao11.cn

[R21] 字符串长度
来源：http://uvq.shuidangran.top

echo "${#s}"
来源：http://rwk.hfpthk.cn

[R22] 截取子串
来源：http://hoo.chenzaomai.com

echo "${s:0:5}"
来源：http://cfy.zycfv.cn

[R23] 字符串替换
来源：http://ijy.52xcode.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wth.vehdjk.com

[R24] 大小写转换
来源：http://osp.nanxinkj.top

echo "${s^^}"; echo "${s,,}"
来源：http://per.jinyuanbaomall.cn

[R25] 去后缀 / 去前缀
来源：http://kvc.jianghu66.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://ife.daria6918.cn

[R26] 命令替换
来源：http://xpu.hnqzz.top

now=$(date +%F); echo "$now"
来源：http://vtw.hnqzz.top

[R27] 算术展开
来源：http://uda.fanxiaobao.xyz

echo $((1 + 2 * 3))
来源：http://gro.bbcook.cn

[R28] 浮点运算
来源：http://qsl.hnqzz.top

echo "scale=2; 10/3" | bc
来源：http://szn.vehdjk.com

[R29] 定义函数
来源：http://qdk.xuetiantiany.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wwv.havefunace.top

[R30] 函数返回状态码
来源：http://ksm.svipenyu.cn

f() { return 0; }; f || echo "失败了"
来源：http://rwm.yj202588.top

[R31] 局部变量
来源：http://zkw.jqgufenzy.top

f() { local x=1; echo "$x"; }
来源：http://ucz.shangyingyoupin.top

[R32] 参数个数校验
来源：http://nds.fanxiaobao.xyz

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://yna.gzhubu.top

[R33] 捕获错误并提示行号
来源：http://iah.cdnleiting.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hzc.chenjidiqi.icu

[R34] 退出时清理
来源：http://wvk.yfazqb.com

trap 'rm -f "$tmp"' EXIT
来源：http://hgr.ppjwa.cn

[R35] 后台执行并等待
来源：http://ddh.shangyingyoupin.top

sleep 5 & pid=$!; wait "$pid"
来源：http://rmn.cheryme.top

[R36] 并发执行多个任务
来源：http://wue.smart0.xyz

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://nwk.jinqigufen.top

[R37] 把输出赋给变量
来源：http://eit.yuanzhike.top

files=$(ls -1)
来源：http://aah.hcnkem.com

[R38] 管道串联
来源：http://fpi.bbcook.cn

cat a.txt | grep -i error | wc -l
来源：http://jqt.bjfxy.top

[R39] 重定向标准输出与错误
来源：http://snw.jyoumei.cn

cmd > out.log 2>&1
来源：http://kqx.zdqjudy.top

[R40] 追加写日志
来源：http://zei.zdqjudy.top

echo "log" >> out.log
来源：http://frf.shzxlz.cn

[R41] 丢弃输出
来源：http://uzm.pengpengdd.cyou

cmd >/dev/null 2>&1
来源：http://pjy.quarkkingdee.top

[R42] 输入重定向
来源：http://bgw.pengpengdd.cyou

wc -l < a.txt
来源：http://mau.cheryme.top

[R43] 按名字查找文件
来源：http://qwv.0kj1m.cn

find . -name "*.log" -type f
来源：http://pkh.hcnkem.com

[R44] 按修改时间查找
来源：http://ogp.zycfv.cn

find . -mtime -7 -type f
来源：http://cor.zhijiandao.cn

[R45] 批量删除
来源：http://jcz.hcnkem.com

find . -name "*.tmp" -delete
来源：http://thr.bbcook.cn

[R46] 递归替换文件内容
来源：http://drm.sxryk.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://sor.tian-w.cn

[R47] sed 单行替换
来源：http://odh.meibo888.top

sed -i 's/foo/bar/g' a.txt
来源：http://fnd.birdmap.top

[R48] awk 取指定列
来源：http://kxe.jinqigufen.top

awk '{print $1, $3}' a.txt
来源：http://ncj.fanxiaobao.xyz

[R49] awk 带条件
来源：http://ofz.zhongyouzk.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://jxw.dashuyun.cn

[R50] awk 求和
来源：http://uoq.smart0.xyz

awk '{s += $2} END {print s}' a.txt
来源：http://yow.sweek.top

[R51] 排序去重取前几
来源：http://zds.hfpthk.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://eez.ppjwa.cn

[R52] 统计行数
来源：http://icc.iojbl.cn

wc -l a.txt
来源：http://mmp.yj20258888.top

[R53] 查看文件头与实时尾
来源：http://hap.daria6918.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://srk.mhx1999.top

[R54] 比较两个文件
来源：http://jep.vqdsnc.cn

diff a.txt b.txt
来源：http://bvr.hywenlv.cn

[R55] 压缩与解压
来源：http://vzn.jlsjyb.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ygo.dianchejie.cn

[R56] 远程拷贝
来源：http://laj.cdnleiting.top

scp file user@host:/path/
来源：http://peg.xylfe.cn

[R57] 远程执行命令
来源：http://kvt.bjfxy.top

ssh user@host 'uptime'
来源：http://miq.hammf.cn

[R58] 下载文件
来源：http://nxc.wangshuangyany.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://kbs.tanke756.top

[R59] 发 POST JSON
来源：http://ijq.gzhubu.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://uuh.yongpay.top

[R60] 只看 HTTP 状态码
来源：http://xqj.fehbvm.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://war.guowangkeji.top

[R61] 磁盘占用
来源：http://leg.cucudq.cn


<!-- 参考信息 -->