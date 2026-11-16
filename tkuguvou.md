代发 wailian999

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://iwr.andypj.xyz

[Q11] 一次插入多行
来源：http://nhj.yangfankeji.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ooh.hesvh.cn

[Q12] 插入后取自增 ID
来源：http://cvc.hammf.cn

INSERT INTO users (name) VALUES ('C');
来源：http://koo.yvedp.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hcr.guannengcc.top

[Q13] 忽略重复插入
来源：http://unb.yuanzhike.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://quf.ctjpmb.com

[Q14] 存在则更新（upsert）
来源：http://qzz.gotoacloud.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ojp.zhoulong.xyz

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://rhb.jinqigufen.top

[Q15] 查询全部
来源：http://jme.hnxiangtu.top

SELECT * FROM users;
来源：http://vnm.ybcxt.top

[Q16] 查询指定列
来源：http://ier.zhoulong.xyz

SELECT id, name FROM users;
来源：http://mfx.hnqzz.top

[Q17] 条件查询
来源：http://zsw.yj202588.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://gbx.hnxiangtu.top

[Q18] 模糊匹配
来源：http://oua.yj20258888.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://jyf.cucudq.cn

[Q19] 范围查询
来源：http://qol.birdmap.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hyr.tanke756.top

[Q20] IN 列表
来源：http://nly.vehdjk.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://szl.sysykeji.top

[Q21] 空值判断
来源：http://rfq.pycfn.com

SELECT * FROM users WHERE email IS NULL;
来源：http://jqn.fehbvm.com

[Q22] 排序
来源：http://mva.epnwcf.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://eyv.shzxlz.cn

[Q23] 分页
来源：http://vbs.chenzaomai.com

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://nzb.cheryme.top

[Q24] 去重
来源：http://nlj.sjlbkw.cn

SELECT DISTINCT city FROM users;
来源：http://fxa.nanxuanxn.top

[Q25] 只取前 N 条
来源：http://yys.sysykeji.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://bfm.feifeiyinyue.top

[Q26] 计数
来源：http://ure.shanyushiyangtech.top

SELECT COUNT(*) FROM users;
来源：http://goo.tianlin.xyz

[Q27] 条件计数
来源：http://jxn.epnwcf.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ipd.sjlbkw.cn

[Q28] 求和与平均
来源：http://wnt.shangyingyoupin.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://fwi.jinqigufen.top

[Q29] 最大最小值
来源：http://mns.zdbjq.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://zto.sweek.top

[Q30] 分组统计
来源：http://ozi.nanxuanxn.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://qgn.c1oappe.top

[Q31] 分组后过滤
来源：http://nev.zhengqikj.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://lda.feifeiyinyue.top

[Q32] 分组拼接字符串
来源：http://hyg.9152youxi.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://qqt.yvedp.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ivj.fanxiaobao.xyz

[Q33] 多列分组
来源：http://xpt.dashuyun.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ack.zhengqikj.top

[Q34] 每组取第一条
来源：http://bhx.jianghu66.top

SELECT * FROM (
来源：http://qsa.gotoacloud.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://niw.zycfv.cn

) t WHERE rn = 1;
来源：http://woi.ydjk.org.cn

[Q35] 内连接
来源：http://awa.zhaomingkeji.xyz

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://brw.gzhubu.top

[Q36] 左连接
来源：http://qop.ehwqpu.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ufy.daria6918.cn

[Q37] 右连接
来源：http://vad.yangfankeji.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ecz.sjlbkw.cn

[Q38] 全外连接（PostgreSQL）
来源：http://kfh.daxiang520.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ijm.snrcjt.cn

[Q39] 自连接（查上下级）
来源：http://lwj.jinqigufen.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://bps.bjfxy.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://taq.shanyushiyangkeji.top

[Q40] 交叉连接（笛卡尔积）
来源：http://ork.jinqigfzy.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://cho.shuidangran.top

[Q41] 多表连接
来源：http://zku.fanxiaobao.xyz

SELECT o.id, u.name, p.title FROM orders o
来源：http://cra.gzhubu.top

JOIN users u ON u.id = o.user_id
来源：http://zvr.daria6918.cn

JOIN products p ON p.id = o.product_id;
来源：http://agf.nanxuanxn.top

[Q42] 连接条件附加过滤
来源：http://dip.meibo888.top

SELECT u.name, o.amount FROM users u
来源：http://ref.fengsongda.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://nbo.shanyushiyangkeji.top

[Q43] 标量子查询
来源：http://glh.ywan-chungtsiang.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ioe.guowangkeji.top

[Q44] IN 子查询
来源：http://syc.daria6918.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://vme.aizwys.cn

[Q45] EXISTS 判断存在
来源：http://prz.guowangkeji.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qfd.snrcjt.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ypp.yonumen.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kdv.redwolf501.top

[Q47] 与平均值比较
来源：http://oho.9152youxi.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://dqu.cqqwz.cn

[Q48] CTE 公用表表达式
来源：http://lvb.cdnleiting.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://exr.xinyue.icu

SELECT * FROM t WHERE c > 5;
来源：http://cvg.uphjek.com

[Q49] 更新单行
来源：http://zvr.yueranfly.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://cbm.hongshengwenyu.top

[Q50] 批量更新
来源：http://xrr.yj20258888.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://dti.yangfankeji.com

[Q51] 用子查询更新
来源：http://rpy.xziqi.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hbp.9152youxi.cn

[Q52] 删除指定行
来源：http://tna.haohaochexian.top

DELETE FROM users WHERE id = 10;
来源：http://xod.jianghu66.top

[Q53] 按条件删除
来源：http://vdk.zhoulong.xyz

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://sdx.wangshuangyany.cn

[Q54] 清空表
来源：http://yis.meibo888.top

TRUNCATE TABLE logs;
来源：http://aau.hammf.cn

[Q55] 排名（并列占位）
来源：http://kbo.aizwys.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://puy.yj202588.top

[Q56] 密集排名（并列不占位）
来源：http://jto.316326.xyz

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://shy.tanke756.top

[Q57] 行号
来源：http://boa.cheryme.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://qhe.xylfe.cn

[Q58] 累计求和
来源：http://qif.feifeiyinyue.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://jjf.daxiang520.top

[Q59] 分组内累计
来源：http://dqr.yj20258888.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://tod.tian-w.cn

[Q60] 取上一行 / 下一行
来源：http://gbs.daxiang520.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://cxr.52xcode.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://aaz.birdmap.top

[Q61] 移动平均
来源：http://iei.shangyingyoupin.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://eko.ydzc1.top

[Q62] 分组占比
来源：http://pfq.kuanghao11.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ppo.gotoacloud.top

[Q63] 开启事务
来源：http://kqy.fanxiaobao.xyz

START TRANSACTION;                -- 或 BEGIN
来源：http://blk.fanxiaobao.xyz

[Q64] 提交事务
来源：http://iig.quarkkingdee.top

COMMIT;
来源：http://bhu.iojbl.cn

[Q65] 回滚事务
来源：http://ncx.zhiwuduotai.top

ROLLBACK;
来源：http://oel.jianghu66.top

[Q66] 行锁查询
来源：http://cnn.yongpay.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://cfu.hysaishi.cn

[Q67] 设置隔离级别
来源：http://npq.zhijiandao.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://pax.shangyingyoupin.top

[Q68] 保存点
来源：http://fux.pengpengdd.cyou

SAVEPOINT sp1;
来源：http://dxi.havefunace.top

ROLLBACK TO sp1;
来源：http://emh.jinqigfzy.top

[Q69] 查看执行计划
来源：http://oql.xziqi.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://dcd.iojbl.cn

[Q70] 更新统计信息
来源：http://zsb.uphjek.com

ANALYZE TABLE users;
来源：http://cwu.xuanzx.com

[Q71] 查看建表语句
来源：http://lzj.daria6918.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://rvf.gogol.net.cn

[Q72] 查看索引
来源：http://joi.tarul.cn

SHOW INDEX FROM users;
来源：http://gqt.sufxvd.cn

[Q73] 查看表状态
来源：http://lml.birdmap.top

SHOW TABLE STATUS LIKE 'users';
来源：http://qkl.gotoacloud.top

[Q74] 强制使用索引
来源：http://xxu.iojbl.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://dmw.ybcxt.top

[Q75] 日期格式化
来源：http://pqx.hammf.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://eej.xingfuxueyuan.xyz

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://sft.9152youxi.cn

[Q76] 按天统计
来源：http://ppj.vehdjk.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ezh.nwbrower.top

[Q77] 时间加减
来源：http://scn.fehbvm.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://gvi.yangfankeji.com

[Q78] 当前时间
来源：http://urv.tanke756.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://nkk.shangyingyoupin.top

[Q79] 字符串拼接
来源：http://uek.xuetiantiany.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://rcn.nwbrower.top

[Q80] 字符串截取
来源：http://ztl.zycfv.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://tlk.shzxlz.cn

[Q81] 字符串替换
来源：http://zbv.sysykeji.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hah.nanxinkj.top

[Q82] 字符长度与字节长度
来源：http://mtp.yueranfly.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://sjm.yonumen.top

[Q83] 大小写转换
来源：http://ayh.tanke756.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://qtn.uphjek.com

[Q84] 去除首尾空格
来源：http://cwv.sjlbkw.cn

SELECT TRIM(name) FROM users;
来源：http://bxi.9152youxi.cn

[Q85] 数值取整
来源：http://lvp.yvedp.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mlv.ehwqpu.com

[Q86] 读取 JSON 字段
来源：http://fgr.zdbjq.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://xzu.sxryk.cn

[Q87] JSON 字段做条件
来源：http://dhs.ivvv.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://eqm.yonumen.top

[Q88] 行转列（条件聚合）
来源：http://zcm.ydzc1.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wnz.feifeiyinyue.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://fif.sxryk.cn

[Q89] 判断表是否存在
来源：http://agd.yueranfly.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://xtf.daxiang520.top

[Q90] 生成序号列
来源：http://zye.jinqigufen.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wuq.dianchejie.cn

================================================================================
来源：http://qjt.cashguo.top

R. Bash 专题
来源：http://djr.yfazqb.com

================================================================================
来源：http://llm.sweek.top

[R01] shebang 与严格模式
来源：http://bsd.tianlin.xyz

#!/usr/bin/env bash
来源：http://pdw.xingfuxueyuan.xyz

set -euo pipefail
来源：http://rnn.zhongyouzk.top

[R02] 变量赋值与使用
来源：http://zbv.xziqi.cn

name="Tom"; echo "$name"
来源：http://sou.fengsongda.top

[R03] 只读变量
来源：http://wws.zhoulong.xyz

readonly PI=3.14
来源：http://nea.zhijiandao.cn

[R04] 位置参数
来源：http://cak.316326.xyz

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://zhc.cucudq.cn

[R05] 参数默认值
来源：http://fsu.nanxuanxn.top

name="${1:-default}"
来源：http://iqv.shzxlz.cn

[R06] 判断命令是否存在
来源：http://kpi.ydjk.org.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://lhb.yj20258888.top

[R07] if 判断文件
来源：http://geq.jyoumei.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hbt.zhixingplan.top

[R08] 数值比较
来源：http://urq.havefunace.top

if (( a > b )); then echo "a 更大"; fi
来源：http://vbm.sweek.top

[R09] 字符串比较
来源：http://brx.svipenyu.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://zta.tarul.cn

[R10] 正则匹配
来源：http://cdi.yueranfly.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://jay.redwolf501.top

[R11] case 多分支
来源：http://rwc.yj20258888.top

case "$1" in
来源：http://ntj.shanyushiyangkeji.top

start) echo "启动" ;;
来源：http://kud.guannengcc.top

stop)  echo "停止" ;;
来源：http://jax.nanxinkj.top

*)     echo "未知命令" ;;
来源：http://nmq.ywan-chungtsiang.top

esac
来源：http://mcb.kuanghao11.cn

[R12] for 遍历文件
来源：http://dom.nwbrower.top

for f in *.txt; do echo "$f"; done
来源：http://mcu.hfpthk.cn

[R13] for 计数循环
来源：http://tgz.chenzaomai.com

for i in {1..10}; do echo "$i"; done
来源：http://jnt.quarkkingdee.top

[R14] C 风格 for
来源：http://wpz.jinqigfzy.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://xzq.yonumen.top

[R15] while 逐行读文件
来源：http://wji.sweek.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mjh.316326.xyz

[R16] until 等待条件
来源：http://rvq.nanxuanxn.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://dvq.yvedp.cn

[R17] 数组定义与取值
来源：http://efc.xinyue.icu

arr=(a b c); echo "${arr[0]}"
来源：http://yjk.tianlin.xyz

[R18] 遍历数组
来源：http://hdh.ybcxt.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://jar.sxryk.cn

[R19] 数组长度
来源：http://hzk.snrcjt.cn

echo "${#arr[@]}"
来源：http://rxm.zhongyouzk.top

[R20] 关联数组（字典）
来源：http://qmw.gzhubu.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://uwi.hongshengwenyu.top

[R21] 字符串长度
来源：http://liq.ehwqpu.com

echo "${#s}"
来源：http://ydn.svipenyu.cn

[R22] 截取子串
来源：http://qrk.jinqigufen.top

echo "${s:0:5}"
来源：http://btj.hfpthk.cn

[R23] 字符串替换
来源：http://upu.xinyue.icu

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hfc.sysykeji.top

[R24] 大小写转换
来源：http://eom.shanyushiyangkeji.top

echo "${s^^}"; echo "${s,,}"
来源：http://zle.tarul.cn

[R25] 去后缀 / 去前缀
来源：http://pdl.yongpay.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://oxi.zdbjq.cn

[R26] 命令替换
来源：http://yhr.guowangkeji.top

now=$(date +%F); echo "$now"
来源：http://oxh.guowangkeji.top

[R27] 算术展开
来源：http://foa.zhongyouzk.top

echo $((1 + 2 * 3))
来源：http://kkh.zhaomingkeji.xyz

[R28] 浮点运算
来源：http://tcg.yueranfly.top

echo "scale=2; 10/3" | bc
来源：http://ifb.jqgufenzy.top

[R29] 定义函数
来源：http://rmd.cqqwz.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://yxi.cashguo.top

[R30] 函数返回状态码
来源：http://pqb.zdbjq.cn

f() { return 0; }; f || echo "失败了"
来源：http://nwh.jinqigufen.top

[R31] 局部变量
来源：http://eme.yuxming.cn

f() { local x=1; echo "$x"; }
来源：http://jxi.xziqi.cn

[R32] 参数个数校验
来源：http://frk.hfpthk.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://cqu.sufxvd.cn

[R33] 捕获错误并提示行号
来源：http://pnv.shanyushiyangkeji.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ayk.hywenlv.cn

[R34] 退出时清理
来源：http://bns.zhoulong.xyz

trap 'rm -f "$tmp"' EXIT
来源：http://uhx.vqdsnc.cn

[R35] 后台执行并等待
来源：http://ggc.mhx1999.top

sleep 5 & pid=$!; wait "$pid"
来源：http://wrk.hesvh.cn

[R36] 并发执行多个任务
来源：http://str.yfazqb.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://crr.sufxvd.cn

[R37] 把输出赋给变量
来源：http://ovb.vqdsnc.cn

files=$(ls -1)
来源：http://lyp.cucudq.cn

[R38] 管道串联
来源：http://gwu.ctjpmb.com

cat a.txt | grep -i error | wc -l
来源：http://lck.jinghuilouyu.cn

[R39] 重定向标准输出与错误
来源：http://uko.yj20258888.top

cmd > out.log 2>&1
来源：http://ulq.hesvh.cn

[R40] 追加写日志
来源：http://rvk.jqgufenzy.top

echo "log" >> out.log
来源：http://nmd.jinqigufen.top

[R41] 丢弃输出
来源：http://rrm.yueranfly.top

cmd >/dev/null 2>&1
来源：http://tcz.kuanghao11.cn

[R42] 输入重定向
来源：http://ewq.yuxming.cn

wc -l < a.txt
来源：http://foe.fzhhl.top

[R43] 按名字查找文件
来源：http://aol.bjfxy.top

find . -name "*.log" -type f
来源：http://ngg.zhoulong.xyz

[R44] 按修改时间查找
来源：http://dms.jinyuanbaomall.cn

find . -mtime -7 -type f
来源：http://dqx.316326.xyz

[R45] 批量删除
来源：http://apz.nanxuanxn.top

find . -name "*.tmp" -delete
来源：http://jwv.xylfe.cn

[R46] 递归替换文件内容
来源：http://vju.chenzaomai.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ati.aibaodan.cn

[R47] sed 单行替换
来源：http://oqg.nwbrower.top

sed -i 's/foo/bar/g' a.txt
来源：http://twv.cashguo.top

[R48] awk 取指定列
来源：http://ydm.fktsv.cn

awk '{print $1, $3}' a.txt
来源：http://pcn.cucudq.cn

[R49] awk 带条件
来源：http://rqk.daria6918.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://sir.ywan-chungtsiang.top

[R50] awk 求和
来源：http://auk.jianghu66.top

awk '{s += $2} END {print s}' a.txt
来源：http://zpg.hesvh.cn

[R51] 排序去重取前几
来源：http://kpg.ivvv.top

sort a.txt | uniq -c | sort -rn | head
来源：http://gvn.shanyushiyangtech.top

[R52] 统计行数
来源：http://xnp.nanxinkj.top

wc -l a.txt
来源：http://nyt.fzhhl.top

[R53] 查看文件头与实时尾
来源：http://etn.zhiwuduotai.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://bem.xingfuxueyuan.xyz

[R54] 比较两个文件
来源：http://cfz.hysaishi.cn

diff a.txt b.txt
来源：http://lku.cashguo.top

[R55] 压缩与解压
来源：http://fje.chenjidiqi.icu

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://jzp.snrcjt.cn

[R56] 远程拷贝
来源：http://pzg.sysykeji.top

scp file user@host:/path/
来源：http://fnx.sweek.top

[R57] 远程执行命令
来源：http://iva.zhaomingkeji.xyz

ssh user@host 'uptime'
来源：http://szm.daria6918.cn

[R58] 下载文件
来源：http://say.shanyushiyangkeji.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://nge.svipenyu.cn

[R59] 发 POST JSON
来源：http://fjh.guowangkeji.top


<!-- 参考信息 -->