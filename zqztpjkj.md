代发 wailian999

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://keb.hnqzz.top

[Q11] 一次插入多行
来源：http://vag.pycfn.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://yqo.cucudq.cn

[Q12] 插入后取自增 ID
来源：http://kxh.jinghuilouyu.cn

INSERT INTO users (name) VALUES ('C');
来源：http://keb.quarkkingdee.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://klm.nanxuanxn.top

[Q13] 忽略重复插入
来源：http://fyw.zhijiandao.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ynl.yongpay.top

[Q14] 存在则更新（upsert）
来源：http://wah.tian-w.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://lit.cashguo.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://xmg.hongshengwenyu.top

[Q15] 查询全部
来源：http://lye.yj20258888.top

SELECT * FROM users;
来源：http://oal.quarkkingdee.top

[Q16] 查询指定列
来源：http://jnl.xinyue.icu

SELECT id, name FROM users;
来源：http://vqj.guowangkeji.top

[Q17] 条件查询
来源：http://urm.fktsv.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://lyd.52xcode.cn

[Q18] 模糊匹配
来源：http://buk.zhixingplan.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hrw.snrcjt.cn

[Q19] 范围查询
来源：http://zej.guannengcc.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://caw.chenlongwang.top

[Q20] IN 列表
来源：http://hgk.cqqwz.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://rjm.hnxiangtu.top

[Q21] 空值判断
来源：http://qxh.zhaomingkeji.xyz

SELECT * FROM users WHERE email IS NULL;
来源：http://rmu.zhixingplan.top

[Q22] 排序
来源：http://jsl.xinyue.icu

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://fje.zhiwuduotai.top

[Q23] 分页
来源：http://shw.ywan-chungtsiang.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://xvy.wangshuangyany.cn

[Q24] 去重
来源：http://uww.hammf.cn

SELECT DISTINCT city FROM users;
来源：http://rft.zdbjq.cn

[Q25] 只取前 N 条
来源：http://qdi.iojbl.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://pqg.cdnleiting.top

[Q26] 计数
来源：http://bfc.xuanzx.com

SELECT COUNT(*) FROM users;
来源：http://ebx.hfpthk.cn

[Q27] 条件计数
来源：http://dfv.kuanghao11.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://yml.xuanzx.com

[Q28] 求和与平均
来源：http://vde.mhx1999.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ioy.guannengcc.top

[Q29] 最大最小值
来源：http://zur.hysaishi.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://dma.ppjwa.cn

[Q30] 分组统计
来源：http://jpx.ctjpmb.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://xui.iojbl.cn

[Q31] 分组后过滤
来源：http://lyo.hfpthk.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://nta.zhixingplan.top

[Q32] 分组拼接字符串
来源：http://iyo.pengpengdd.cyou

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://oju.yonumen.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ntj.shuidangran.top

[Q33] 多列分组
来源：http://son.tanke756.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://fwu.xziqi.cn

[Q34] 每组取第一条
来源：http://yja.xinyue.icu

SELECT * FROM (
来源：http://mnz.haohaochexian.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://yry.shanyushiyangtech.top

) t WHERE rn = 1;
来源：http://prf.ehwqpu.com

[Q35] 内连接
来源：http://fci.ydjk.org.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://jtd.fanxiaobao.xyz

[Q36] 左连接
来源：http://pxv.fengsongda.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://yxy.xylfe.cn

[Q37] 右连接
来源：http://aeo.cashguo.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://gij.ivvv.top

[Q38] 全外连接（PostgreSQL）
来源：http://wig.havefunace.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ung.jinghuilouyu.cn

[Q39] 自连接（查上下级）
来源：http://fkf.xingfuxueyuan.xyz

SELECT e.name, m.name AS manager FROM employees e
来源：http://ilb.yj20258888.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://olu.yuxming.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://kqy.gaohongyu789.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://vuq.dashuyun.cn

[Q41] 多表连接
来源：http://pzx.zycfv.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://xvv.dianchejie.cn

JOIN users u ON u.id = o.user_id
来源：http://xbn.guannengcc.top

JOIN products p ON p.id = o.product_id;
来源：http://cgu.fanxiaobao.xyz

[Q42] 连接条件附加过滤
来源：http://oyd.wangdashe.top

SELECT u.name, o.amount FROM users u
来源：http://vjq.tian-w.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://qlo.fanxiaobao.xyz

[Q43] 标量子查询
来源：http://ymz.birdmap.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://fhr.hesvh.cn

[Q44] IN 子查询
来源：http://bio.cucudq.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://jjf.yfazqb.com

[Q45] EXISTS 判断存在
来源：http://ers.ywan-chungtsiang.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bqa.sysykeji.top

[Q46] NOT EXISTS 判断不存在
来源：http://kkj.snrcjt.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kkj.fktsv.cn

[Q47] 与平均值比较
来源：http://pqz.fktsv.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://vip.hnxiangtu.top

[Q48] CTE 公用表表达式
来源：http://mxv.xylfe.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://csp.yuanzhike.top

SELECT * FROM t WHERE c > 5;
来源：http://fko.wangshuangyany.cn

[Q49] 更新单行
来源：http://afy.ydjk.org.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://lub.zhengqikj.top

[Q50] 批量更新
来源：http://xzr.shanyushiyangtech.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://akb.jinghuilouyu.cn

[Q51] 用子查询更新
来源：http://bbj.redwolf501.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://utq.shzxlz.cn

[Q52] 删除指定行
来源：http://cwi.zhaomingkeji.xyz

DELETE FROM users WHERE id = 10;
来源：http://pgp.uphjek.com

[Q53] 按条件删除
来源：http://hhn.hammf.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://eua.zhongyouzk.top

[Q54] 清空表
来源：http://gzf.jinyuanbaomall.cn

TRUNCATE TABLE logs;
来源：http://tau.ybcxt.top

[Q55] 排名（并列占位）
来源：http://zlq.yvedp.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://axj.jyoumei.cn

[Q56] 密集排名（并列不占位）
来源：http://ads.zhijiandao.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://tei.guannengcc.top

[Q57] 行号
来源：http://jkk.aizwys.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://vtd.jlsjyb.cn

[Q58] 累计求和
来源：http://dge.gaohongyu789.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://jph.jinyuanbaomall.cn

[Q59] 分组内累计
来源：http://oww.tarul.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://sjy.vqdsnc.cn

[Q60] 取上一行 / 下一行
来源：http://izv.zdbjq.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://bxt.guowangkeji.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://bmf.sweek.top

[Q61] 移动平均
来源：http://diy.cheryme.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://zrg.zhoulong.xyz

[Q62] 分组占比
来源：http://uyf.hongshengwenyu.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://diy.havefunace.top

[Q63] 开启事务
来源：http://ynj.feifeiyinyue.top

START TRANSACTION;                -- 或 BEGIN
来源：http://zto.fanxiaobao.xyz

[Q64] 提交事务
来源：http://mox.guowangkeji.top

COMMIT;
来源：http://syw.aibaodan.cn

[Q65] 回滚事务
来源：http://iez.bbcook.cn

ROLLBACK;
来源：http://iip.snrcjt.cn

[Q66] 行锁查询
来源：http://flq.cashguo.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://zbx.svipenyu.cn

[Q67] 设置隔离级别
来源：http://xfc.hcnkem.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://vwp.ctjpmb.com

[Q68] 保存点
来源：http://azk.guowangkeji.top

SAVEPOINT sp1;
来源：http://lyr.aibaodan.cn

ROLLBACK TO sp1;
来源：http://kkp.chenlongwang.top

[Q69] 查看执行计划
来源：http://aww.dashuyun.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hhw.fzhhl.top

[Q70] 更新统计信息
来源：http://kfl.0kj1m.cn

ANALYZE TABLE users;
来源：http://fxh.pengpengdd.cyou

[Q71] 查看建表语句
来源：http://mpc.daria6918.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://qao.birdmap.top

[Q72] 查看索引
来源：http://deg.ydzc1.top

SHOW INDEX FROM users;
来源：http://lbo.zdbjq.cn

[Q73] 查看表状态
来源：http://vnj.chenjidiqi.icu

SHOW TABLE STATUS LIKE 'users';
来源：http://lti.ydzc1.top

[Q74] 强制使用索引
来源：http://bta.jqgfzy.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mgz.svipenyu.cn

[Q75] 日期格式化
来源：http://cay.chenzaomai.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://gtc.cqqwz.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://cmg.dashuyun.cn

[Q76] 按天统计
来源：http://fqp.ybcxt.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://kgo.epnwcf.com

[Q77] 时间加减
来源：http://jqo.c1oappe.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://fud.gotoacloud.top

[Q78] 当前时间
来源：http://bnf.nanxinkj.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://dus.tianlin.xyz

[Q79] 字符串拼接
来源：http://hao.xuetiantiany.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://kqk.nanxuanxn.top

[Q80] 字符串截取
来源：http://rka.cqqwz.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://jyr.redwolf501.top

[Q81] 字符串替换
来源：http://lng.feifeiyinyue.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://kdy.sjlbkw.cn

[Q82] 字符长度与字节长度
来源：http://tft.jianghu66.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://raz.pycfn.com

[Q83] 大小写转换
来源：http://nwf.redwolf501.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://pfy.shanyushiyangtech.top

[Q84] 去除首尾空格
来源：http://xvj.jiagoushi.top

SELECT TRIM(name) FROM users;
来源：http://ejq.guannengcc.top

[Q85] 数值取整
来源：http://ehl.zhaomingkeji.xyz

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://moj.gotoacloud.top

[Q86] 读取 JSON 字段
来源：http://shu.9152youxi.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mql.zhongyouzk.top

[Q87] JSON 字段做条件
来源：http://sow.hongshengwenyu.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://pip.zhiwuduotai.top

[Q88] 行转列（条件聚合）
来源：http://hue.guannengcc.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://kra.yueranfly.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mpi.xylfe.cn

[Q89] 判断表是否存在
来源：http://lqq.ywan-chungtsiang.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://zmc.cheryme.top

[Q90] 生成序号列
来源：http://tll.redwolf501.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://rbb.ctjpmb.com

================================================================================
来源：http://yaq.ppjwa.cn

R. Bash 专题
来源：http://jba.cdnleiting.top

================================================================================
来源：http://dwo.xuetiantiany.cn

[R01] shebang 与严格模式
来源：http://ofo.bjfxy.top

#!/usr/bin/env bash
来源：http://gbe.xinyue.icu

set -euo pipefail
来源：http://egl.hammf.cn

[R02] 变量赋值与使用
来源：http://gct.fanxiaobao.xyz

name="Tom"; echo "$name"
来源：http://atx.xinyue.icu

[R03] 只读变量
来源：http://lic.yvedp.cn

readonly PI=3.14
来源：http://njx.jinyuanbaomall.cn

[R04] 位置参数
来源：http://pml.smart0.xyz

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://beo.shanyushiyangtech.top

[R05] 参数默认值
来源：http://fuo.zycfv.cn

name="${1:-default}"
来源：http://xgp.chenlongwang.top

[R06] 判断命令是否存在
来源：http://nmx.chenjidiqi.icu

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://lcv.wangshuangyany.cn

[R07] if 判断文件
来源：http://mox.ybcxt.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://jhh.gzhubu.top

[R08] 数值比较
来源：http://cqd.jinyuanbaomall.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://tji.yfazqb.com

[R09] 字符串比较
来源：http://mnq.fzhhl.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://isk.fengsongda.top

[R10] 正则匹配
来源：http://bkg.hnqzz.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mzp.hcnkem.com

[R11] case 多分支
来源：http://feg.yongpay.top

case "$1" in
来源：http://evv.xylfe.cn

start) echo "启动" ;;
来源：http://zqa.zhaomingkeji.xyz

stop)  echo "停止" ;;
来源：http://fww.yanxiufei.cn

*)     echo "未知命令" ;;
来源：http://uoj.hywenlv.cn

esac
来源：http://ytc.dianchejie.cn

[R12] for 遍历文件
来源：http://dfe.yj20258888.top

for f in *.txt; do echo "$f"; done
来源：http://lgs.yuxming.cn

[R13] for 计数循环
来源：http://yxa.daxiang520.top

for i in {1..10}; do echo "$i"; done
来源：http://kum.daria6918.cn

[R14] C 风格 for
来源：http://hfg.yfazqb.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ddr.pycfn.com

[R15] while 逐行读文件
来源：http://owq.cheryme.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://sfa.jianghu66.top

[R16] until 等待条件
来源：http://wwp.yj20258888.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hqw.aizwys.cn

[R17] 数组定义与取值
来源：http://tcf.xuetiantiany.cn

arr=(a b c); echo "${arr[0]}"
来源：http://hhf.fengsongda.top

[R18] 遍历数组
来源：http://xdy.redwolf501.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://npk.fanxiaobao.xyz

[R19] 数组长度
来源：http://dax.xuanzx.com

echo "${#arr[@]}"
来源：http://sgf.chenjidiqi.icu

[R20] 关联数组（字典）
来源：http://yhz.jqgfzy.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://tmj.svipenyu.cn

[R21] 字符串长度
来源：http://ivh.yj20258.top

echo "${#s}"
来源：http://xja.zhongyouzk.top

[R22] 截取子串
来源：http://bvn.yueranfly.top

echo "${s:0:5}"
来源：http://hbo.ehwqpu.com

[R23] 字符串替换
来源：http://chc.52xcode.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://pwi.vqdsnc.cn

[R24] 大小写转换
来源：http://auq.zhaomingkeji.xyz

echo "${s^^}"; echo "${s,,}"
来源：http://bqj.ivvv.top

[R25] 去后缀 / 去前缀
来源：http://unk.snrcjt.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://qjs.yongpay.top

[R26] 命令替换
来源：http://coh.bbcook.cn

now=$(date +%F); echo "$now"
来源：http://avs.zhengqikj.top

[R27] 算术展开
来源：http://mii.zhixingplan.top

echo $((1 + 2 * 3))
来源：http://jnp.wangshuangyany.cn

[R28] 浮点运算
来源：http://ieh.ybcxt.top

echo "scale=2; 10/3" | bc
来源：http://wmu.jinqigufen.top

[R29] 定义函数
来源：http://tlf.jinghuilouyu.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ndy.guannengcc.top

[R30] 函数返回状态码
来源：http://bjt.jinqigfzy.top

f() { return 0; }; f || echo "失败了"
来源：http://rrt.epnwcf.com

[R31] 局部变量
来源：http://bxl.jiagoushi.top

f() { local x=1; echo "$x"; }
来源：http://xjl.hfpthk.cn

[R32] 参数个数校验
来源：http://dbi.hammf.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://jwi.xuanzx.com

[R33] 捕获错误并提示行号
来源：http://wlv.zhaomingkeji.xyz

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://rov.xuanzx.com

[R34] 退出时清理
来源：http://cln.nwbrower.top

trap 'rm -f "$tmp"' EXIT
来源：http://apk.316326.xyz

[R35] 后台执行并等待
来源：http://daw.fengsongda.top

sleep 5 & pid=$!; wait "$pid"
来源：http://tkz.nanxinkj.top

[R36] 并发执行多个任务
来源：http://khn.dashuyun.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://drf.aibaodan.cn

[R37] 把输出赋给变量
来源：http://bbl.fanxiaobao.xyz

files=$(ls -1)
来源：http://nhf.0kj1m.cn

[R38] 管道串联
来源：http://rnj.zhaomingkeji.xyz

cat a.txt | grep -i error | wc -l
来源：http://yyn.vehdjk.com

[R39] 重定向标准输出与错误
来源：http://cyv.52xcode.cn

cmd > out.log 2>&1
来源：http://zxy.yfazqb.com

[R40] 追加写日志
来源：http://hsx.gotoacloud.top

echo "log" >> out.log
来源：http://xrv.zhoulong.xyz

[R41] 丢弃输出
来源：http://dia.uphjek.com

cmd >/dev/null 2>&1
来源：http://oez.pengpengdd.cyou

[R42] 输入重定向
来源：http://yyd.sysykeji.top

wc -l < a.txt
来源：http://mwh.uphjek.com

[R43] 按名字查找文件
来源：http://rru.jianghu66.top

find . -name "*.log" -type f
来源：http://umk.svipenyu.cn

[R44] 按修改时间查找
来源：http://jvj.hesvh.cn

find . -mtime -7 -type f
来源：http://tyv.yj20258888.top

[R45] 批量删除
来源：http://lyx.hesvh.cn

find . -name "*.tmp" -delete
来源：http://dyo.9152youxi.cn

[R46] 递归替换文件内容
来源：http://igr.jinqigufen.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://qfj.hnxiangtu.top

[R47] sed 单行替换
来源：http://jae.bbcook.cn

sed -i 's/foo/bar/g' a.txt
来源：http://fam.quarkkingdee.top

[R48] awk 取指定列
来源：http://rmb.zhengqikj.top

awk '{print $1, $3}' a.txt
来源：http://ubn.chenjidiqi.icu

[R49] awk 带条件
来源：http://iqs.daxiang520.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ihn.vqdsnc.cn

[R50] awk 求和
来源：http://unu.jinqigfzy.top

awk '{s += $2} END {print s}' a.txt
来源：http://tjj.cheryme.top

[R51] 排序去重取前几
来源：http://sxb.mhx1999.top

sort a.txt | uniq -c | sort -rn | head
来源：http://vob.dianchejie.cn

[R52] 统计行数
来源：http://iue.jinghuilouyu.cn

wc -l a.txt
来源：http://pdo.0kj1m.cn

[R53] 查看文件头与实时尾
来源：http://psr.yj20258.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://tjb.jinyuanbaomall.cn

[R54] 比较两个文件
来源：http://nrt.9152youxi.cn

diff a.txt b.txt
来源：http://kew.cashguo.top

[R55] 压缩与解压
来源：http://mge.fanxiaobao.xyz

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://oiw.shanyushiyangkeji.top

[R56] 远程拷贝
来源：http://yjp.ctjpmb.com

scp file user@host:/path/
来源：http://pqs.cucudq.cn

[R57] 远程执行命令
来源：http://vza.nanxinkj.top

ssh user@host 'uptime'
来源：http://bwk.smart0.xyz

[R58] 下载文件
来源：http://llb.9152youxi.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://zyc.tianlin.xyz

[R59] 发 POST JSON
来源：http://ccr.xingfuxueyuan.xyz


<!-- 参考信息 -->