代发 wailian999

CREATE INDEX idx_users_email ON users(email);
来源：http://dca.mhx1999.top

[Q09] 创建唯一索引
来源：http://dvv.yj20258888.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ntf.hcnkem.com

[Q10] 插入单行
来源：http://oid.zhoulong.xyz

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://msc.daxiang520.top

[Q11] 一次插入多行
来源：http://wdy.nanxinkj.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://zrm.hnxiangtu.top

[Q12] 插入后取自增 ID
来源：http://bzr.quarkkingdee.top

INSERT INTO users (name) VALUES ('C');
来源：http://uwt.fktsv.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://svc.xuetiantiany.cn

[Q13] 忽略重复插入
来源：http://pol.bjfxy.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://lpu.yonumen.top

[Q14] 存在则更新（upsert）
来源：http://gdx.yj20258.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://oci.zdqjudy.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://krp.pengpengdd.cyou

[Q15] 查询全部
来源：http://zjw.yangfankeji.com

SELECT * FROM users;
来源：http://swi.zhiwuduotai.top

[Q16] 查询指定列
来源：http://anw.xziqi.cn

SELECT id, name FROM users;
来源：http://pjs.ydjk.org.cn

[Q17] 条件查询
来源：http://vac.bbcook.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wqv.gotoacloud.top

[Q18] 模糊匹配
来源：http://ufk.hnqzz.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://lkg.jianghu66.top

[Q19] 范围查询
来源：http://gwu.zdqjudy.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://akz.snrcjt.cn

[Q20] IN 列表
来源：http://yfd.sysykeji.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://nfo.zhaomingkeji.xyz

[Q21] 空值判断
来源：http://wik.hnxiangtu.top

SELECT * FROM users WHERE email IS NULL;
来源：http://eaa.yuanzhike.top

[Q22] 排序
来源：http://bac.shzxlz.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://tzy.gogol.net.cn

[Q23] 分页
来源：http://bcs.yuxming.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://yuu.jianghu66.top

[Q24] 去重
来源：http://nqn.fehbvm.com

SELECT DISTINCT city FROM users;
来源：http://npn.gaohongyu789.top

[Q25] 只取前 N 条
来源：http://ojn.daria6918.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://dfp.cheryme.top

[Q26] 计数
来源：http://rbw.zdbjq.cn

SELECT COUNT(*) FROM users;
来源：http://tzc.bjfxy.top

[Q27] 条件计数
来源：http://yqm.daxiang520.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://bjw.tianlin.xyz

[Q28] 求和与平均
来源：http://pko.shzxlz.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://end.yj202588.top

[Q29] 最大最小值
来源：http://tmr.gaohongyu789.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://jfw.snrcjt.cn

[Q30] 分组统计
来源：http://hsj.zhaomingkeji.xyz

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://kwq.xziqi.cn

[Q31] 分组后过滤
来源：http://gwr.52xcode.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wtu.zhengqikj.top

[Q32] 分组拼接字符串
来源：http://vml.pengpengdd.cyou

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ill.kuanghao11.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://tch.tianlin.xyz

[Q33] 多列分组
来源：http://uwz.wangshuangyany.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://qmi.cdnleiting.top

[Q34] 每组取第一条
来源：http://yey.jinghuilouyu.cn

SELECT * FROM (
来源：http://vvz.9152youxi.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://oas.sjlbkw.cn

) t WHERE rn = 1;
来源：http://igp.fehbvm.com

[Q35] 内连接
来源：http://nyb.zhixingplan.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ejh.jinghuilouyu.cn

[Q36] 左连接
来源：http://noy.quarkkingdee.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://exo.jinghuilouyu.cn

[Q37] 右连接
来源：http://uts.jinghuilouyu.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hqn.cheryme.top

[Q38] 全外连接（PostgreSQL）
来源：http://lek.shangyingyoupin.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://onw.tarul.cn

[Q39] 自连接（查上下级）
来源：http://vfv.nanxinkj.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://ptv.shzxlz.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://gto.yueranfly.top

[Q40] 交叉连接（笛卡尔积）
来源：http://lkc.pengpengdd.cyou

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hnd.smart0.xyz

[Q41] 多表连接
来源：http://hfl.uphjek.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://nel.cashguo.top

JOIN users u ON u.id = o.user_id
来源：http://hzu.fehbvm.com

JOIN products p ON p.id = o.product_id;
来源：http://oeg.andypj.xyz

[Q42] 连接条件附加过滤
来源：http://czq.52xcode.cn

SELECT u.name, o.amount FROM users u
来源：http://zgg.ppjwa.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://fjh.nanxinkj.top

[Q43] 标量子查询
来源：http://spp.xuanzx.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://taz.sxryk.cn

[Q44] IN 子查询
来源：http://edy.yj20258888.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://nrl.hongshengwenyu.top

[Q45] EXISTS 判断存在
来源：http://vkb.yanxiufei.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ovo.uphjek.com

[Q46] NOT EXISTS 判断不存在
来源：http://cap.shzxlz.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://eyp.shzxlz.cn

[Q47] 与平均值比较
来源：http://jnl.shuidangran.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://gdk.birdmap.top

[Q48] CTE 公用表表达式
来源：http://mck.cqqwz.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ssx.ppjwa.cn

SELECT * FROM t WHERE c > 5;
来源：http://jcs.hysaishi.cn

[Q49] 更新单行
来源：http://yjj.sweek.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://irh.ivvv.top

[Q50] 批量更新
来源：http://ezw.zycfv.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://bco.yvedp.cn

[Q51] 用子查询更新
来源：http://dua.jinqigfzy.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hhr.tarul.cn

[Q52] 删除指定行
来源：http://lte.yuanzhike.top

DELETE FROM users WHERE id = 10;
来源：http://yfj.uphjek.com

[Q53] 按条件删除
来源：http://zbg.wangdashe.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wxs.kuanghao11.cn

[Q54] 清空表
来源：http://ipi.jlsjyb.cn

TRUNCATE TABLE logs;
来源：http://svc.tanke756.top

[Q55] 排名（并列占位）
来源：http://mbq.zhixingplan.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://aex.gogol.net.cn

[Q56] 密集排名（并列不占位）
来源：http://gaz.hywenlv.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://tgj.xuanzx.com

[Q57] 行号
来源：http://phs.xingfuxueyuan.xyz

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mbn.fengsongda.top

[Q58] 累计求和
来源：http://pfc.hywenlv.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://bte.yangfankeji.com

[Q59] 分组内累计
来源：http://gnw.guowangkeji.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://fxu.xuetiantiany.cn

[Q60] 取上一行 / 下一行
来源：http://rqd.daxiang520.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://bpg.cucudq.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mdg.dashuyun.cn

[Q61] 移动平均
来源：http://hpj.yj20258.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://zek.redwolf501.top

[Q62] 分组占比
来源：http://zte.aibaodan.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://xpb.sxryk.cn

[Q63] 开启事务
来源：http://pnv.9152youxi.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://aqm.cucudq.cn

[Q64] 提交事务
来源：http://qmz.hcnkem.com

COMMIT;
来源：http://iuh.feifeiyinyue.top

[Q65] 回滚事务
来源：http://rbv.ppjwa.cn

ROLLBACK;
来源：http://zcq.cqqwz.cn

[Q66] 行锁查询
来源：http://nrd.sysykeji.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mqe.tanke756.top

[Q67] 设置隔离级别
来源：http://rja.316326.xyz

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://gvf.uphjek.com

[Q68] 保存点
来源：http://pmn.chenjidiqi.icu

SAVEPOINT sp1;
来源：http://gui.ydzc1.top

ROLLBACK TO sp1;
来源：http://kkq.chenlongwang.top

[Q69] 查看执行计划
来源：http://avn.c1oappe.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://scv.cheryme.top

[Q70] 更新统计信息
来源：http://oms.iojbl.cn

ANALYZE TABLE users;
来源：http://ams.gotoacloud.top

[Q71] 查看建表语句
来源：http://uak.bbcook.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hbp.zhongyouzk.top

[Q72] 查看索引
来源：http://ypa.ydjk.org.cn

SHOW INDEX FROM users;
来源：http://gzw.ehwqpu.com

[Q73] 查看表状态
来源：http://fgo.zhoulong.xyz

SHOW TABLE STATUS LIKE 'users';
来源：http://hne.xuanzx.com

[Q74] 强制使用索引
来源：http://saw.redwolf501.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://uen.cheryme.top

[Q75] 日期格式化
来源：http://zmr.sweek.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://cvk.sufxvd.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://rht.svipenyu.cn

[Q76] 按天统计
来源：http://bee.tarul.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ief.zhoulong.xyz

[Q77] 时间加减
来源：http://hgx.feifeiyinyue.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://pkz.316326.xyz

[Q78] 当前时间
来源：http://eyc.yj202588.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://dwa.cashguo.top

[Q79] 字符串拼接
来源：http://dmx.ywan-chungtsiang.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ghz.jinqigfzy.top

[Q80] 字符串截取
来源：http://elj.nwbrower.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://rso.nanxinkj.top

[Q81] 字符串替换
来源：http://esq.ctjpmb.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://vtx.sufxvd.cn

[Q82] 字符长度与字节长度
来源：http://tyt.birdmap.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://nwa.chenjidiqi.icu

[Q83] 大小写转换
来源：http://lqm.jyoumei.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://czy.zhoulong.xyz

[Q84] 去除首尾空格
来源：http://phj.sufxvd.cn

SELECT TRIM(name) FROM users;
来源：http://tzl.aizwys.cn

[Q85] 数值取整
来源：http://xot.hesvh.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wpe.zhixingplan.top

[Q86] 读取 JSON 字段
来源：http://mpc.hesvh.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ebg.uphjek.com

[Q87] JSON 字段做条件
来源：http://izp.sufxvd.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://pmt.tarul.cn

[Q88] 行转列（条件聚合）
来源：http://ftv.c1oappe.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://auf.yuanzhike.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://aar.zdqjudy.top

[Q89] 判断表是否存在
来源：http://mjm.smart0.xyz

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://lpr.pycfn.com

[Q90] 生成序号列
来源：http://dyt.cdnleiting.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://zul.yj20258888.top

================================================================================
来源：http://ahr.c1oappe.top

R. Bash 专题
来源：http://ota.jinghuilouyu.cn

================================================================================
来源：http://tvq.smart0.xyz

[R01] shebang 与严格模式
来源：http://zzg.bjfxy.top

#!/usr/bin/env bash
来源：http://aun.yongpay.top

set -euo pipefail
来源：http://pay.daria6918.cn

[R02] 变量赋值与使用
来源：http://pcs.feifeiyinyue.top

name="Tom"; echo "$name"
来源：http://wth.zhiwuduotai.top

[R03] 只读变量
来源：http://jnp.hongshengwenyu.top

readonly PI=3.14
来源：http://eyk.svipenyu.cn

[R04] 位置参数
来源：http://xhd.guowangkeji.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://myq.zhixingplan.top

[R05] 参数默认值
来源：http://nhp.vehdjk.com

name="${1:-default}"
来源：http://sex.jinghuilouyu.cn

[R06] 判断命令是否存在
来源：http://xqa.ydjk.org.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://gta.jinghuilouyu.cn

[R07] if 判断文件
来源：http://quy.yangfankeji.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://tlq.tanke756.top

[R08] 数值比较
来源：http://cio.sxryk.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://qsy.hnqzz.top

[R09] 字符串比较
来源：http://lvi.nanxinkj.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ucy.jqgufenzy.top

[R10] 正则匹配
来源：http://qub.vqdsnc.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hrp.sjlbkw.cn

[R11] case 多分支
来源：http://dtl.zhijiandao.cn

case "$1" in
来源：http://leo.yonumen.top

start) echo "启动" ;;
来源：http://adv.tianlin.xyz

stop)  echo "停止" ;;
来源：http://jsj.0kj1m.cn

*)     echo "未知命令" ;;
来源：http://iwj.xuanzx.com

esac
来源：http://sxb.fanxiaobao.xyz

[R12] for 遍历文件
来源：http://cwy.hcnkem.com

for f in *.txt; do echo "$f"; done
来源：http://ras.vehdjk.com

[R13] for 计数循环
来源：http://pwj.yuanzhike.top

for i in {1..10}; do echo "$i"; done
来源：http://eql.gotoacloud.top

[R14] C 风格 for
来源：http://omf.hcnkem.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://dui.hnqzz.top

[R15] while 逐行读文件
来源：http://tnd.zhixingplan.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://vim.bjfxy.top

[R16] until 等待条件
来源：http://xpm.epnwcf.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://pdn.jyoumei.cn

[R17] 数组定义与取值
来源：http://uhx.andypj.xyz

arr=(a b c); echo "${arr[0]}"
来源：http://wmh.yangfankeji.com

[R18] 遍历数组
来源：http://byq.hfpthk.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://odo.cdnleiting.top

[R19] 数组长度
来源：http://wql.epnwcf.com

echo "${#arr[@]}"
来源：http://pxa.tian-w.cn

[R20] 关联数组（字典）
来源：http://clz.sxryk.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://qhu.xuetiantiany.cn

[R21] 字符串长度
来源：http://wqs.fktsv.cn

echo "${#s}"
来源：http://mpt.haohaochexian.top

[R22] 截取子串
来源：http://noa.jinqigfzy.top

echo "${s:0:5}"
来源：http://lqd.cdnleiting.top

[R23] 字符串替换
来源：http://udi.zhaomingkeji.xyz

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://lmy.0kj1m.cn

[R24] 大小写转换
来源：http://fyu.guowangkeji.top

echo "${s^^}"; echo "${s,,}"
来源：http://tgg.316326.xyz

[R25] 去后缀 / 去前缀
来源：http://ibb.zhoulong.xyz

echo "${f%.txt}"; echo "${f#./}"
来源：http://jac.sjlbkw.cn

[R26] 命令替换
来源：http://vzw.gzhubu.top

now=$(date +%F); echo "$now"
来源：http://xrp.vehdjk.com

[R27] 算术展开
来源：http://hjh.hongshengwenyu.top

echo $((1 + 2 * 3))
来源：http://lov.xziqi.cn

[R28] 浮点运算
来源：http://lez.sysykeji.top

echo "scale=2; 10/3" | bc
来源：http://pgf.hnxiangtu.top

[R29] 定义函数
来源：http://kou.shanyushiyangtech.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://xpk.birdmap.top

[R30] 函数返回状态码
来源：http://omg.sxryk.cn

f() { return 0; }; f || echo "失败了"
来源：http://sdn.vqdsnc.cn

[R31] 局部变量
来源：http://imo.sufxvd.cn

f() { local x=1; echo "$x"; }
来源：http://qed.ybcxt.top

[R32] 参数个数校验
来源：http://wnh.yfazqb.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://iej.aibaodan.cn

[R33] 捕获错误并提示行号
来源：http://rux.hywenlv.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://scg.sysykeji.top

[R34] 退出时清理
来源：http://zod.fengsongda.top

trap 'rm -f "$tmp"' EXIT
来源：http://cud.nanxuanxn.top

[R35] 后台执行并等待
来源：http://bdw.tarul.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://gye.ywan-chungtsiang.top

[R36] 并发执行多个任务
来源：http://ovw.quarkkingdee.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://zfr.svipenyu.cn

[R37] 把输出赋给变量
来源：http://jyc.chenzaomai.com

files=$(ls -1)
来源：http://gku.gotoacloud.top

[R38] 管道串联
来源：http://hli.vehdjk.com

cat a.txt | grep -i error | wc -l
来源：http://mxb.pengpengdd.cyou

[R39] 重定向标准输出与错误
来源：http://uvq.zhengqikj.top

cmd > out.log 2>&1
来源：http://xgx.jqgfzy.top

[R40] 追加写日志
来源：http://sgr.zhijiandao.cn

echo "log" >> out.log
来源：http://trh.sweek.top

[R41] 丢弃输出
来源：http://qtd.fehbvm.com

cmd >/dev/null 2>&1
来源：http://vdv.hnqzz.top

[R42] 输入重定向
来源：http://ozi.daria6918.cn

wc -l < a.txt
来源：http://yrn.zhengqikj.top

[R43] 按名字查找文件
来源：http://dod.ppjwa.cn

find . -name "*.log" -type f
来源：http://gxb.hfpthk.cn

[R44] 按修改时间查找
来源：http://nnw.xinyue.icu

find . -mtime -7 -type f
来源：http://jlq.feifeiyinyue.top

[R45] 批量删除
来源：http://cpz.ydjk.org.cn

find . -name "*.tmp" -delete
来源：http://klv.sufxvd.cn

[R46] 递归替换文件内容
来源：http://jqp.cdnleiting.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://kdm.shangyingyoupin.top

[R47] sed 单行替换
来源：http://yps.nanxinkj.top

sed -i 's/foo/bar/g' a.txt
来源：http://pbu.0kj1m.cn

[R48] awk 取指定列
来源：http://kiq.hysaishi.cn

awk '{print $1, $3}' a.txt
来源：http://noj.xingfuxueyuan.xyz

[R49] awk 带条件
来源：http://vnm.wangshuangyany.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mhy.quarkkingdee.top

[R50] awk 求和
来源：http://acg.gotoacloud.top

awk '{s += $2} END {print s}' a.txt
来源：http://fqv.iojbl.cn

[R51] 排序去重取前几
来源：http://cbz.hfpthk.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://zvz.cashguo.top

[R52] 统计行数
来源：http://kdc.c1oappe.top

wc -l a.txt
来源：http://jxl.jinyuanbaomall.cn

[R53] 查看文件头与实时尾
来源：http://iqo.andypj.xyz

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://tqi.dianchejie.cn

[R54] 比较两个文件
来源：http://smu.pengpengdd.cyou

diff a.txt b.txt
来源：http://qry.316326.xyz

[R55] 压缩与解压
来源：http://abf.shanyushiyangkeji.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hcd.yj20258.top

[R56] 远程拷贝
来源：http://efg.zdbjq.cn

scp file user@host:/path/
来源：http://aht.cashguo.top

[R57] 远程执行命令
来源：http://spc.mhx1999.top


<!-- 参考信息 -->