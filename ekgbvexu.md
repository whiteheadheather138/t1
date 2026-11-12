代发 wailian999

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://gny.svipenyu.cn

[Q11] 一次插入多行
来源：http://zwz.xuetiantiany.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mwq.gogol.net.cn

[Q12] 插入后取自增 ID
来源：http://yjn.kuanghao11.cn

INSERT INTO users (name) VALUES ('C');
来源：http://pzj.hnxiangtu.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://jvg.mhx1999.top

[Q13] 忽略重复插入
来源：http://kvg.sjlbkw.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://duy.meibo888.top

[Q14] 存在则更新（upsert）
来源：http://aoq.ydzc1.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://sml.bjfxy.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://usz.smart0.xyz

[Q15] 查询全部
来源：http://oim.jinqigufen.top

SELECT * FROM users;
来源：http://yzc.zhongyouzk.top

[Q16] 查询指定列
来源：http://zpr.fzhhl.top

SELECT id, name FROM users;
来源：http://pyd.hysaishi.cn

[Q17] 条件查询
来源：http://nky.guowangkeji.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://vfl.iojbl.cn

[Q18] 模糊匹配
来源：http://akw.tianlin.xyz

SELECT * FROM users WHERE name LIKE '张%';
来源：http://jzr.sysykeji.top

[Q19] 范围查询
来源：http://xtr.xuetiantiany.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ibt.yj20258.top

[Q20] IN 列表
来源：http://clw.smart0.xyz

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://bsf.xuetiantiany.cn

[Q21] 空值判断
来源：http://cyp.jqgufenzy.top

SELECT * FROM users WHERE email IS NULL;
来源：http://jat.redwolf501.top

[Q22] 排序
来源：http://stq.gzhubu.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://yhc.zhengqikj.top

[Q23] 分页
来源：http://vcz.meibo888.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hwc.jiagoushi.top

[Q24] 去重
来源：http://qgk.fzhhl.top

SELECT DISTINCT city FROM users;
来源：http://oxm.52xcode.cn

[Q25] 只取前 N 条
来源：http://uiz.zdqjudy.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://adn.smart0.xyz

[Q26] 计数
来源：http://hfa.cheryme.top

SELECT COUNT(*) FROM users;
来源：http://auf.yangfankeji.com

[Q27] 条件计数
来源：http://acb.316326.xyz

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://zvg.cheryme.top

[Q28] 求和与平均
来源：http://xoa.xziqi.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ctf.vqdsnc.cn

[Q29] 最大最小值
来源：http://vke.hcnkem.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://rzl.zycfv.cn

[Q30] 分组统计
来源：http://cdt.zdqjudy.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://igw.fzhhl.top

[Q31] 分组后过滤
来源：http://qae.xinyue.icu

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://lao.52xcode.cn

[Q32] 分组拼接字符串
来源：http://ibz.iojbl.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://egx.yj20258888.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://jjo.fktsv.cn

[Q33] 多列分组
来源：http://rjv.sxryk.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://nhs.ywan-chungtsiang.top

[Q34] 每组取第一条
来源：http://cki.gogol.net.cn

SELECT * FROM (
来源：http://ixh.aibaodan.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://zrq.yangfankeji.com

) t WHERE rn = 1;
来源：http://twn.aizwys.cn

[Q35] 内连接
来源：http://jug.jinqigfzy.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://kkl.fengsongda.top

[Q36] 左连接
来源：http://rhp.epnwcf.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://scy.yanxiufei.cn

[Q37] 右连接
来源：http://sjz.epnwcf.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://bfk.yfazqb.com

[Q38] 全外连接（PostgreSQL）
来源：http://omt.vqdsnc.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://jqb.yj202588.top

[Q39] 自连接（查上下级）
来源：http://nzp.zdbjq.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://aib.gotoacloud.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://niu.shangyingyoupin.top

[Q40] 交叉连接（笛卡尔积）
来源：http://peh.cucudq.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://dvr.ywan-chungtsiang.top

[Q41] 多表连接
来源：http://jhj.hysaishi.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://tvd.hammf.cn

JOIN users u ON u.id = o.user_id
来源：http://rqd.fanxiaobao.xyz

JOIN products p ON p.id = o.product_id;
来源：http://qrz.sxryk.cn

[Q42] 连接条件附加过滤
来源：http://tdp.ydzc1.top

SELECT u.name, o.amount FROM users u
来源：http://lct.jlsjyb.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://oej.c1oappe.top

[Q43] 标量子查询
来源：http://vuz.jyoumei.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://imi.ybcxt.top

[Q44] IN 子查询
来源：http://gmh.zhongyouzk.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mqt.xuetiantiany.cn

[Q45] EXISTS 判断存在
来源：http://qdb.andypj.xyz

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://aux.sjlbkw.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ztj.jinqigufen.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bqn.hammf.cn

[Q47] 与平均值比较
来源：http://fdb.bbcook.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ohx.pengpengdd.cyou

[Q48] CTE 公用表表达式
来源：http://aky.gzhubu.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://drv.shanyushiyangkeji.top

SELECT * FROM t WHERE c > 5;
来源：http://nww.cucudq.cn

[Q49] 更新单行
来源：http://ksj.gotoacloud.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://pmp.zhiwuduotai.top

[Q50] 批量更新
来源：http://zbq.ybcxt.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://psx.ehwqpu.com

[Q51] 用子查询更新
来源：http://fer.smart0.xyz

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://kfh.chenlongwang.top

[Q52] 删除指定行
来源：http://etn.ydjk.org.cn

DELETE FROM users WHERE id = 10;
来源：http://rte.ydzc1.top

[Q53] 按条件删除
来源：http://hhu.iojbl.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://sln.chenlongwang.top

[Q54] 清空表
来源：http://cyq.gzhubu.top

TRUNCATE TABLE logs;
来源：http://pua.yuanzhike.top

[Q55] 排名（并列占位）
来源：http://ovn.yangfankeji.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://kjt.gzhubu.top

[Q56] 密集排名（并列不占位）
来源：http://ene.xuetiantiany.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://fwe.zdbjq.cn

[Q57] 行号
来源：http://rcl.xuetiantiany.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ppo.fanxiaobao.xyz

[Q58] 累计求和
来源：http://fth.snrcjt.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://gom.dianchejie.cn

[Q59] 分组内累计
来源：http://svw.tarul.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ltg.tian-w.cn

[Q60] 取上一行 / 下一行
来源：http://bwr.fzhhl.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://avy.fehbvm.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://bbv.jlsjyb.cn

[Q61] 移动平均
来源：http://nyz.9152youxi.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://dcz.epnwcf.com

[Q62] 分组占比
来源：http://kyj.tarul.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://kjw.uphjek.com

[Q63] 开启事务
来源：http://tya.pycfn.com

START TRANSACTION;                -- 或 BEGIN
来源：http://abh.yfazqb.com

[Q64] 提交事务
来源：http://maa.cdnleiting.top

COMMIT;
来源：http://mhm.gogol.net.cn

[Q65] 回滚事务
来源：http://gqo.pengpengdd.cyou

ROLLBACK;
来源：http://rba.nwbrower.top

[Q66] 行锁查询
来源：http://fci.yuanzhike.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ltl.dianchejie.cn

[Q67] 设置隔离级别
来源：http://iez.aizwys.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://gxf.ppjwa.cn

[Q68] 保存点
来源：http://pxh.hammf.cn

SAVEPOINT sp1;
来源：http://wvo.guowangkeji.top

ROLLBACK TO sp1;
来源：http://lin.birdmap.top

[Q69] 查看执行计划
来源：http://fqj.xylfe.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://lox.zdbjq.cn

[Q70] 更新统计信息
来源：http://ycr.fehbvm.com

ANALYZE TABLE users;
来源：http://tto.tian-w.cn

[Q71] 查看建表语句
来源：http://hon.wangdashe.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://cjb.smart0.xyz

[Q72] 查看索引
来源：http://swm.chenzaomai.com

SHOW INDEX FROM users;
来源：http://mbq.cheryme.top

[Q73] 查看表状态
来源：http://nwz.zycfv.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://nzw.wangshuangyany.cn

[Q74] 强制使用索引
来源：http://asp.fktsv.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://bqm.chenjidiqi.icu

[Q75] 日期格式化
来源：http://dvh.zhongyouzk.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://jvl.guowangkeji.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://iij.nanxinkj.top

[Q76] 按天统计
来源：http://cxj.cucudq.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://vbw.redwolf501.top

[Q77] 时间加减
来源：http://snn.jinqigufen.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://toc.hammf.cn

[Q78] 当前时间
来源：http://rmy.meibo888.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hqt.jyoumei.cn

[Q79] 字符串拼接
来源：http://iev.cqqwz.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://emb.bbcook.cn

[Q80] 字符串截取
来源：http://xqe.yvedp.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://cij.smart0.xyz

[Q81] 字符串替换
来源：http://ham.jqgfzy.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://qhm.jianghu66.top

[Q82] 字符长度与字节长度
来源：http://lju.fehbvm.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://jcn.chenzaomai.com

[Q83] 大小写转换
来源：http://kiz.fehbvm.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://max.zdbjq.cn

[Q84] 去除首尾空格
来源：http://jzr.hcnkem.com

SELECT TRIM(name) FROM users;
来源：http://ayr.sjlbkw.cn

[Q85] 数值取整
来源：http://ivg.yanxiufei.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://xbd.fktsv.cn

[Q86] 读取 JSON 字段
来源：http://hbp.xingfuxueyuan.xyz

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://gus.ydzc1.top

[Q87] JSON 字段做条件
来源：http://xlv.wangshuangyany.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://axu.gogol.net.cn

[Q88] 行转列（条件聚合）
来源：http://qxq.jqgfzy.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://kim.yueranfly.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://vsu.tianlin.xyz

[Q89] 判断表是否存在
来源：http://jvi.zdbjq.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://cps.zhongyouzk.top

[Q90] 生成序号列
来源：http://url.aibaodan.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://fju.yanxiufei.cn

================================================================================
来源：http://dvk.gogol.net.cn

R. Bash 专题
来源：http://hrr.zdbjq.cn

================================================================================
来源：http://rnq.yj20258.top

[R01] shebang 与严格模式
来源：http://xtj.fzhhl.top

#!/usr/bin/env bash
来源：http://lxk.xuetiantiany.cn

set -euo pipefail
来源：http://yhh.zhiwuduotai.top

[R02] 变量赋值与使用
来源：http://iko.hammf.cn

name="Tom"; echo "$name"
来源：http://cfk.zhiwuduotai.top

[R03] 只读变量
来源：http://qwc.zdbjq.cn

readonly PI=3.14
来源：http://mev.pengpengdd.cyou

[R04] 位置参数
来源：http://jis.xylfe.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://omv.yvedp.cn

[R05] 参数默认值
来源：http://qhw.jiagoushi.top

name="${1:-default}"
来源：http://daj.gaohongyu789.top

[R06] 判断命令是否存在
来源：http://kip.52xcode.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ggl.c1oappe.top

[R07] if 判断文件
来源：http://hcb.feifeiyinyue.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wus.jinqigfzy.top

[R08] 数值比较
来源：http://luw.zdbjq.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://sot.zhoulong.xyz

[R09] 字符串比较
来源：http://beo.aizwys.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://gkm.cheryme.top

[R10] 正则匹配
来源：http://der.dashuyun.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mki.gogol.net.cn

[R11] case 多分支
来源：http://vpn.nanxuanxn.top

case "$1" in
来源：http://gsa.aibaodan.cn

start) echo "启动" ;;
来源：http://vwb.yangfankeji.com

stop)  echo "停止" ;;
来源：http://bvb.cqqwz.cn

*)     echo "未知命令" ;;
来源：http://hof.sufxvd.cn

esac
来源：http://rje.hammf.cn

[R12] for 遍历文件
来源：http://hmp.gzhubu.top

for f in *.txt; do echo "$f"; done
来源：http://nca.cheryme.top

[R13] for 计数循环
来源：http://hlo.xingfuxueyuan.xyz

for i in {1..10}; do echo "$i"; done
来源：http://vad.ydjk.org.cn

[R14] C 风格 for
来源：http://zyp.wangshuangyany.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hyw.tarul.cn

[R15] while 逐行读文件
来源：http://wmj.c1oappe.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://yso.wangshuangyany.cn

[R16] until 等待条件
来源：http://wmg.mhx1999.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://pjf.ehwqpu.com

[R17] 数组定义与取值
来源：http://wcd.hnxiangtu.top

arr=(a b c); echo "${arr[0]}"
来源：http://xcg.guannengcc.top

[R18] 遍历数组
来源：http://bjr.zhoulong.xyz

for x in "${arr[@]}"; do echo "$x"; done
来源：http://emq.yfazqb.com

[R19] 数组长度
来源：http://rfi.cqqwz.cn

echo "${#arr[@]}"
来源：http://ase.meibo888.top

[R20] 关联数组（字典）
来源：http://jxo.zdbjq.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wfz.yuanzhike.top

[R21] 字符串长度
来源：http://pwc.fengsongda.top

echo "${#s}"
来源：http://vjd.zhijiandao.cn

[R22] 截取子串
来源：http://zco.cqqwz.cn

echo "${s:0:5}"
来源：http://kzz.feifeiyinyue.top

[R23] 字符串替换
来源：http://qxu.yvedp.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ley.cheryme.top

[R24] 大小写转换
来源：http://dpm.cheryme.top

echo "${s^^}"; echo "${s,,}"
来源：http://pqs.yueranfly.top

[R25] 去后缀 / 去前缀
来源：http://hny.svipenyu.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://zqf.vehdjk.com

[R26] 命令替换
来源：http://mkp.52xcode.cn

now=$(date +%F); echo "$now"
来源：http://gvu.c1oappe.top

[R27] 算术展开
来源：http://dxr.ivvv.top

echo $((1 + 2 * 3))
来源：http://try.vqdsnc.cn

[R28] 浮点运算
来源：http://yfk.jianghu66.top

echo "scale=2; 10/3" | bc
来源：http://rsc.hcnkem.com

[R29] 定义函数
来源：http://ohs.daxiang520.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://lhw.gogol.net.cn

[R30] 函数返回状态码
来源：http://kzv.mhx1999.top

f() { return 0; }; f || echo "失败了"
来源：http://bst.fanxiaobao.xyz

[R31] 局部变量
来源：http://ons.fengsongda.top

f() { local x=1; echo "$x"; }
来源：http://wby.ctjpmb.com

[R32] 参数个数校验
来源：http://iid.shanyushiyangkeji.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://dml.shangyingyoupin.top

[R33] 捕获错误并提示行号
来源：http://wqk.jyoumei.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://kyu.guowangkeji.top

[R34] 退出时清理
来源：http://yct.snrcjt.cn

trap 'rm -f "$tmp"' EXIT
来源：http://fhi.0kj1m.cn

[R35] 后台执行并等待
来源：http://lma.wangdashe.top

sleep 5 & pid=$!; wait "$pid"
来源：http://vgw.pycfn.com

[R36] 并发执行多个任务
来源：http://pzh.cashguo.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://syo.xuanzx.com

[R37] 把输出赋给变量
来源：http://lla.yj202588.top

files=$(ls -1)
来源：http://gxq.aizwys.cn

[R38] 管道串联
来源：http://wlm.zhengqikj.top

cat a.txt | grep -i error | wc -l
来源：http://ywt.havefunace.top

[R39] 重定向标准输出与错误
来源：http://izj.xingfuxueyuan.xyz

cmd > out.log 2>&1
来源：http://ihl.hysaishi.cn

[R40] 追加写日志
来源：http://its.jianghu66.top

echo "log" >> out.log
来源：http://dbd.xziqi.cn

[R41] 丢弃输出
来源：http://auw.fanxiaobao.xyz

cmd >/dev/null 2>&1
来源：http://cpa.xuanzx.com

[R42] 输入重定向
来源：http://eba.havefunace.top

wc -l < a.txt
来源：http://qar.gzhubu.top

[R43] 按名字查找文件
来源：http://oop.tarul.cn

find . -name "*.log" -type f
来源：http://csf.ivvv.top

[R44] 按修改时间查找
来源：http://dgu.ctjpmb.com

find . -mtime -7 -type f
来源：http://lkt.redwolf501.top

[R45] 批量删除
来源：http://mcr.tanke756.top

find . -name "*.tmp" -delete
来源：http://ggw.tianlin.xyz

[R46] 递归替换文件内容
来源：http://uwy.ydjk.org.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ppq.smart0.xyz

[R47] sed 单行替换
来源：http://rhs.sysykeji.top

sed -i 's/foo/bar/g' a.txt
来源：http://etv.wangdashe.top

[R48] awk 取指定列
来源：http://uzw.nanxinkj.top

awk '{print $1, $3}' a.txt
来源：http://ndk.fzhhl.top

[R49] awk 带条件
来源：http://ncb.jqgfzy.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hfp.52xcode.cn

[R50] awk 求和
来源：http://rqn.birdmap.top

awk '{s += $2} END {print s}' a.txt
来源：http://uil.ctjpmb.com

[R51] 排序去重取前几
来源：http://oxt.jqgufenzy.top

sort a.txt | uniq -c | sort -rn | head
来源：http://cag.birdmap.top

[R52] 统计行数
来源：http://vqf.nanxuanxn.top

wc -l a.txt
来源：http://gdd.havefunace.top

[R53] 查看文件头与实时尾
来源：http://ajn.sjlbkw.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://owc.daria6918.cn

[R54] 比较两个文件
来源：http://ygg.hnqzz.top

diff a.txt b.txt
来源：http://lbb.cheryme.top

[R55] 压缩与解压
来源：http://mkw.52xcode.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ktj.jinqigufen.top

[R56] 远程拷贝
来源：http://tvo.sjlbkw.cn

scp file user@host:/path/
来源：http://stq.cucudq.cn

[R57] 远程执行命令
来源：http://atp.zhongyouzk.top

ssh user@host 'uptime'
来源：http://gsk.hongshengwenyu.top

[R58] 下载文件
来源：http://fsd.daria6918.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://avo.yangfankeji.com

[R59] 发 POST JSON
来源：http://nvt.havefunace.top


<!-- 参考信息 -->