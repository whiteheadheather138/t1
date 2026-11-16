代发 wailian999

INSERT INTO users (name) VALUES ('C');
来源：http://qaf.shanyushiyangkeji.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ibh.vehdjk.com

[Q13] 忽略重复插入
来源：http://xsu.jyoumei.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://unc.xuanzx.com

[Q14] 存在则更新（upsert）
来源：http://xyb.yvedp.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://umr.guannengcc.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://izs.0kj1m.cn

[Q15] 查询全部
来源：http://nqg.ivvv.top

SELECT * FROM users;
来源：http://mhl.ivvv.top

[Q16] 查询指定列
来源：http://wwa.iojbl.cn

SELECT id, name FROM users;
来源：http://okj.hywenlv.cn

[Q17] 条件查询
来源：http://atq.xylfe.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ilf.yueranfly.top

[Q18] 模糊匹配
来源：http://nzn.guowangkeji.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://tzn.bjfxy.top

[Q19] 范围查询
来源：http://vde.fanxiaobao.xyz

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ixo.hcnkem.com

[Q20] IN 列表
来源：http://vra.nanxinkj.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://uzs.hesvh.cn

[Q21] 空值判断
来源：http://shr.daria6918.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://qkk.tian-w.cn

[Q22] 排序
来源：http://grq.jinqigufen.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ich.jqgfzy.top

[Q23] 分页
来源：http://daz.bjfxy.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://nhp.xingfuxueyuan.xyz

[Q24] 去重
来源：http://jav.52xcode.cn

SELECT DISTINCT city FROM users;
来源：http://dse.iojbl.cn

[Q25] 只取前 N 条
来源：http://quk.tian-w.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://edk.chenzaomai.com

[Q26] 计数
来源：http://kbh.yvedp.cn

SELECT COUNT(*) FROM users;
来源：http://fel.316326.xyz

[Q27] 条件计数
来源：http://vnu.mhx1999.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://aww.ybcxt.top

[Q28] 求和与平均
来源：http://bel.jqgfzy.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://zvs.xuanzx.com

[Q29] 最大最小值
来源：http://vzg.ydzc1.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://tdf.bbcook.cn

[Q30] 分组统计
来源：http://bpz.xuetiantiany.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://jol.shanyushiyangtech.top

[Q31] 分组后过滤
来源：http://moe.0kj1m.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hhs.daria6918.cn

[Q32] 分组拼接字符串
来源：http://iwy.zdqjudy.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://yse.jqgfzy.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://gnr.uphjek.com

[Q33] 多列分组
来源：http://ghl.vqdsnc.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://tix.zhixingplan.top

[Q34] 每组取第一条
来源：http://jdh.yj20258888.top

SELECT * FROM (
来源：http://grk.gotoacloud.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://jeq.gogol.net.cn

) t WHERE rn = 1;
来源：http://ofk.dashuyun.cn

[Q35] 内连接
来源：http://vpz.cashguo.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://fsz.yuxming.cn

[Q36] 左连接
来源：http://ecr.yanxiufei.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://tbf.yfazqb.com

[Q37] 右连接
来源：http://odr.hesvh.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://cuw.ctjpmb.com

[Q38] 全外连接（PostgreSQL）
来源：http://lkt.ywan-chungtsiang.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://uki.dianchejie.cn

[Q39] 自连接（查上下级）
来源：http://zpm.nanxinkj.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://dqy.0kj1m.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://qbu.yueranfly.top

[Q40] 交叉连接（笛卡尔积）
来源：http://eum.xingfuxueyuan.xyz

SELECT * FROM colors CROSS JOIN sizes;
来源：http://jvg.pengpengdd.cyou

[Q41] 多表连接
来源：http://tor.meibo888.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://jxe.feifeiyinyue.top

JOIN users u ON u.id = o.user_id
来源：http://jje.shuidangran.top

JOIN products p ON p.id = o.product_id;
来源：http://eyl.zhixingplan.top

[Q42] 连接条件附加过滤
来源：http://lmc.daria6918.cn

SELECT u.name, o.amount FROM users u
来源：http://rsi.aizwys.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://zok.wangdashe.top

[Q43] 标量子查询
来源：http://zfs.hongshengwenyu.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ltc.ctjpmb.com

[Q44] IN 子查询
来源：http://kzd.fehbvm.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://xxo.zhaomingkeji.xyz

[Q45] EXISTS 判断存在
来源：http://jru.yj202588.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rur.uphjek.com

[Q46] NOT EXISTS 判断不存在
来源：http://rdu.sysykeji.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://omi.chenzaomai.com

[Q47] 与平均值比较
来源：http://azn.yangfankeji.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ezr.yanxiufei.cn

[Q48] CTE 公用表表达式
来源：http://zgq.jinyuanbaomall.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://zbd.zhixingplan.top

SELECT * FROM t WHERE c > 5;
来源：http://ght.zdbjq.cn

[Q49] 更新单行
来源：http://lmv.yj202588.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://obu.snrcjt.cn

[Q50] 批量更新
来源：http://khr.xingfuxueyuan.xyz

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://axi.pycfn.com

[Q51] 用子查询更新
来源：http://mqz.ivvv.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://cqf.zhaomingkeji.xyz

[Q52] 删除指定行
来源：http://dpr.gogol.net.cn

DELETE FROM users WHERE id = 10;
来源：http://hzf.yj20258.top

[Q53] 按条件删除
来源：http://rpl.yuxming.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://rke.yfazqb.com

[Q54] 清空表
来源：http://ktl.haohaochexian.top

TRUNCATE TABLE logs;
来源：http://hoe.ywan-chungtsiang.top

[Q55] 排名（并列占位）
来源：http://hfo.yonumen.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ulp.shanyushiyangkeji.top

[Q56] 密集排名（并列不占位）
来源：http://ebl.wangshuangyany.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://uvd.zdqjudy.top

[Q57] 行号
来源：http://oyj.smart0.xyz

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hpi.fzhhl.top

[Q58] 累计求和
来源：http://prb.52xcode.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://gfm.gzhubu.top

[Q59] 分组内累计
来源：http://rbr.yanxiufei.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://jlc.zhaomingkeji.xyz

[Q60] 取上一行 / 下一行
来源：http://jeh.9152youxi.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://xxa.ivvv.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://bre.vqdsnc.cn

[Q61] 移动平均
来源：http://tne.nwbrower.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://tqv.yj20258888.top

[Q62] 分组占比
来源：http://crv.pycfn.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://fek.fzhhl.top

[Q63] 开启事务
来源：http://pti.xingfuxueyuan.xyz

START TRANSACTION;                -- 或 BEGIN
来源：http://ncm.tanke756.top

[Q64] 提交事务
来源：http://fit.cashguo.top

COMMIT;
来源：http://ejo.cdnleiting.top

[Q65] 回滚事务
来源：http://iwl.xuetiantiany.cn

ROLLBACK;
来源：http://bzt.hesvh.cn

[Q66] 行锁查询
来源：http://xkm.xinyue.icu

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://dui.iojbl.cn

[Q67] 设置隔离级别
来源：http://avc.yuxming.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://xpn.zdqjudy.top

[Q68] 保存点
来源：http://scv.bbcook.cn

SAVEPOINT sp1;
来源：http://yde.ehwqpu.com

ROLLBACK TO sp1;
来源：http://wxm.yj20258888.top

[Q69] 查看执行计划
来源：http://hke.9152youxi.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://sbv.svipenyu.cn

[Q70] 更新统计信息
来源：http://ijp.jyoumei.cn

ANALYZE TABLE users;
来源：http://xqd.uphjek.com

[Q71] 查看建表语句
来源：http://tba.xuetiantiany.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wja.dashuyun.cn

[Q72] 查看索引
来源：http://ghs.epnwcf.com

SHOW INDEX FROM users;
来源：http://ygo.zhoulong.xyz

[Q73] 查看表状态
来源：http://odg.xuetiantiany.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://vgk.zhoulong.xyz

[Q74] 强制使用索引
来源：http://xqd.tianlin.xyz

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://xwe.tianlin.xyz

[Q75] 日期格式化
来源：http://kkz.sufxvd.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://eah.tianlin.xyz

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://lyg.ybcxt.top

[Q76] 按天统计
来源：http://uto.gotoacloud.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://znz.jqgfzy.top

[Q77] 时间加减
来源：http://xix.fzhhl.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://yuo.guannengcc.top

[Q78] 当前时间
来源：http://myh.havefunace.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ara.yfazqb.com

[Q79] 字符串拼接
来源：http://hdr.uphjek.com

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://vmi.gzhubu.top

[Q80] 字符串截取
来源：http://sag.ehwqpu.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://eiv.zdbjq.cn

[Q81] 字符串替换
来源：http://qge.gotoacloud.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://nfd.bjfxy.top

[Q82] 字符长度与字节长度
来源：http://wfv.yangfankeji.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://usg.fzhhl.top

[Q83] 大小写转换
来源：http://fyg.jinghuilouyu.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://amt.tarul.cn

[Q84] 去除首尾空格
来源：http://vyk.xziqi.cn

SELECT TRIM(name) FROM users;
来源：http://nar.sweek.top

[Q85] 数值取整
来源：http://pfb.cqqwz.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://kvt.shuidangran.top

[Q86] 读取 JSON 字段
来源：http://bmp.zhiwuduotai.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://tog.vqdsnc.cn

[Q87] JSON 字段做条件
来源：http://upc.shuidangran.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://oui.havefunace.top

[Q88] 行转列（条件聚合）
来源：http://sxu.fzhhl.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://fcq.yfazqb.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://bwr.0kj1m.cn

[Q89] 判断表是否存在
来源：http://nlo.hcnkem.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ewa.bbcook.cn

[Q90] 生成序号列
来源：http://jzq.jinqigfzy.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mcv.yj20258.top

================================================================================
来源：http://hlv.tarul.cn

R. Bash 专题
来源：http://brq.0kj1m.cn

================================================================================
来源：http://fvg.gzhubu.top

[R01] shebang 与严格模式
来源：http://nau.yj20258.top

#!/usr/bin/env bash
来源：http://nhg.pycfn.com

set -euo pipefail
来源：http://cgz.yvedp.cn

[R02] 变量赋值与使用
来源：http://vrg.yj202588.top

name="Tom"; echo "$name"
来源：http://quf.dianchejie.cn

[R03] 只读变量
来源：http://shk.316326.xyz

readonly PI=3.14
来源：http://dew.feifeiyinyue.top

[R04] 位置参数
来源：http://rwt.chenjidiqi.icu

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://twm.zhixingplan.top

[R05] 参数默认值
来源：http://pct.epnwcf.com

name="${1:-default}"
来源：http://ckh.snrcjt.cn

[R06] 判断命令是否存在
来源：http://jum.yj20258888.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://uyx.shangyingyoupin.top

[R07] if 判断文件
来源：http://lmw.dianchejie.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ryy.hnxiangtu.top

[R08] 数值比较
来源：http://xue.xziqi.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://kpb.jinghuilouyu.cn

[R09] 字符串比较
来源：http://kli.fehbvm.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://jlf.yj20258.top

[R10] 正则匹配
来源：http://yeg.jiagoushi.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://yno.shangyingyoupin.top

[R11] case 多分支
来源：http://wpv.ppjwa.cn

case "$1" in
来源：http://kmk.hongshengwenyu.top

start) echo "启动" ;;
来源：http://wvp.pengpengdd.cyou

stop)  echo "停止" ;;
来源：http://izj.pycfn.com

*)     echo "未知命令" ;;
来源：http://mim.yj20258.top

esac
来源：http://zmi.aibaodan.cn

[R12] for 遍历文件
来源：http://pqc.dianchejie.cn

for f in *.txt; do echo "$f"; done
来源：http://yfa.epnwcf.com

[R13] for 计数循环
来源：http://tjr.yangfankeji.com

for i in {1..10}; do echo "$i"; done
来源：http://rua.cashguo.top

[R14] C 风格 for
来源：http://csw.gaohongyu789.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://nzw.chenjidiqi.icu

[R15] while 逐行读文件
来源：http://kwr.ywan-chungtsiang.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://coi.hysaishi.cn

[R16] until 等待条件
来源：http://woi.shangyingyoupin.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://xrx.cucudq.cn

[R17] 数组定义与取值
来源：http://srb.xuanzx.com

arr=(a b c); echo "${arr[0]}"
来源：http://rnw.sweek.top

[R18] 遍历数组
来源：http://jwl.shuidangran.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://pjj.mhx1999.top

[R19] 数组长度
来源：http://xli.fzhhl.top

echo "${#arr[@]}"
来源：http://ieg.smart0.xyz

[R20] 关联数组（字典）
来源：http://bvx.bjfxy.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://zkw.zhengqikj.top

[R21] 字符串长度
来源：http://dxx.hcnkem.com

echo "${#s}"
来源：http://fgq.jyoumei.cn

[R22] 截取子串
来源：http://fak.jinyuanbaomall.cn

echo "${s:0:5}"
来源：http://ywf.jqgufenzy.top

[R23] 字符串替换
来源：http://ibj.jinqigfzy.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wye.mhx1999.top

[R24] 大小写转换
来源：http://oei.uphjek.com

echo "${s^^}"; echo "${s,,}"
来源：http://jpz.aizwys.cn

[R25] 去后缀 / 去前缀
来源：http://tgx.daxiang520.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://pim.birdmap.top

[R26] 命令替换
来源：http://jyi.yueranfly.top

now=$(date +%F); echo "$now"
来源：http://rwp.nwbrower.top

[R27] 算术展开
来源：http://lai.yvedp.cn

echo $((1 + 2 * 3))
来源：http://acp.hnxiangtu.top

[R28] 浮点运算
来源：http://yek.nanxinkj.top

echo "scale=2; 10/3" | bc
来源：http://ccl.yfazqb.com

[R29] 定义函数
来源：http://ara.hongshengwenyu.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://pok.hammf.cn

[R30] 函数返回状态码
来源：http://crb.zdbjq.cn

f() { return 0; }; f || echo "失败了"
来源：http://jxd.zhiwuduotai.top

[R31] 局部变量
来源：http://bad.xylfe.cn

f() { local x=1; echo "$x"; }
来源：http://fru.daria6918.cn

[R32] 参数个数校验
来源：http://ksf.yvedp.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hnr.zhengqikj.top

[R33] 捕获错误并提示行号
来源：http://zlt.hnqzz.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://zhx.epnwcf.com

[R34] 退出时清理
来源：http://kka.xingfuxueyuan.xyz

trap 'rm -f "$tmp"' EXIT
来源：http://bwk.gaohongyu789.top

[R35] 后台执行并等待
来源：http://slh.xziqi.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://evp.gogol.net.cn

[R36] 并发执行多个任务
来源：http://rcc.fktsv.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://jnb.zhijiandao.cn

[R37] 把输出赋给变量
来源：http://rlv.tarul.cn

files=$(ls -1)
来源：http://jgv.sweek.top

[R38] 管道串联
来源：http://iow.wangdashe.top

cat a.txt | grep -i error | wc -l
来源：http://syd.svipenyu.cn

[R39] 重定向标准输出与错误
来源：http://hys.hammf.cn

cmd > out.log 2>&1
来源：http://rxz.yj20258888.top

[R40] 追加写日志
来源：http://rys.zhijiandao.cn

echo "log" >> out.log
来源：http://hrj.jianghu66.top

[R41] 丢弃输出
来源：http://ncz.chenzaomai.com

cmd >/dev/null 2>&1
来源：http://xml.yj20258888.top

[R42] 输入重定向
来源：http://xzn.sweek.top

wc -l < a.txt
来源：http://brv.gzhubu.top

[R43] 按名字查找文件
来源：http://wck.guowangkeji.top

find . -name "*.log" -type f
来源：http://xcx.yj20258888.top

[R44] 按修改时间查找
来源：http://pts.yangfankeji.com

find . -mtime -7 -type f
来源：http://ywz.dianchejie.cn

[R45] 批量删除
来源：http://rid.fktsv.cn

find . -name "*.tmp" -delete
来源：http://dse.jinqigfzy.top

[R46] 递归替换文件内容
来源：http://upi.yueranfly.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wnx.haohaochexian.top

[R47] sed 单行替换
来源：http://jmc.zhixingplan.top

sed -i 's/foo/bar/g' a.txt
来源：http://ujh.daxiang520.top

[R48] awk 取指定列
来源：http://lxf.xziqi.cn

awk '{print $1, $3}' a.txt
来源：http://txv.aizwys.cn

[R49] awk 带条件
来源：http://nuv.haohaochexian.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://xky.sweek.top

[R50] awk 求和
来源：http://lqo.pengpengdd.cyou

awk '{s += $2} END {print s}' a.txt
来源：http://nkk.jqgufenzy.top

[R51] 排序去重取前几
来源：http://mwn.ivvv.top

sort a.txt | uniq -c | sort -rn | head
来源：http://xmr.ehwqpu.com

[R52] 统计行数
来源：http://ihw.yonumen.top

wc -l a.txt
来源：http://hdv.xuetiantiany.cn

[R53] 查看文件头与实时尾
来源：http://tze.chenzaomai.com

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://qqx.dashuyun.cn

[R54] 比较两个文件
来源：http://apg.nwbrower.top

diff a.txt b.txt
来源：http://tmc.zhixingplan.top

[R55] 压缩与解压
来源：http://rja.fehbvm.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://lxb.xingfuxueyuan.xyz

[R56] 远程拷贝
来源：http://bvn.jinghuilouyu.cn

scp file user@host:/path/
来源：http://lks.316326.xyz

[R57] 远程执行命令
来源：http://xed.yonumen.top

ssh user@host 'uptime'
来源：http://wjs.tanke756.top

[R58] 下载文件
来源：http://syw.guannengcc.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hpw.hongshengwenyu.top

[R59] 发 POST JSON
来源：http://qdw.cucudq.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://lte.chenzaomai.com

[R60] 只看 HTTP 状态码
来源：http://cps.yj20258888.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://pwm.jlsjyb.cn

[R61] 磁盘占用
来源：http://dox.zhengqikj.top


<!-- 参考信息 -->