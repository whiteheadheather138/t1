代发 wailian999

CREATE INDEX idx_users_email ON users(email);
来源：http://lzg.cdnleiting.top

[Q09] 创建唯一索引
来源：http://dbw.ppjwa.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://rbl.yanxiufei.cn

[Q10] 插入单行
来源：http://mlb.sweek.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://fhf.jqgfzy.top

[Q11] 一次插入多行
来源：http://dvt.ywan-chungtsiang.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://qxn.hywenlv.cn

[Q12] 插入后取自增 ID
来源：http://ltr.shuidangran.top

INSERT INTO users (name) VALUES ('C');
来源：http://jtx.sxryk.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://rxi.quarkkingdee.top

[Q13] 忽略重复插入
来源：http://esi.uphjek.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://xak.nanxuanxn.top

[Q14] 存在则更新（upsert）
来源：http://jqq.cheryme.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://kdg.c1oappe.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://bpg.jiagoushi.top

[Q15] 查询全部
来源：http://ips.shzxlz.cn

SELECT * FROM users;
来源：http://oog.cashguo.top

[Q16] 查询指定列
来源：http://mhb.quarkkingdee.top

SELECT id, name FROM users;
来源：http://ahf.yuxming.cn

[Q17] 条件查询
来源：http://ovb.jinghuilouyu.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://vky.xylfe.cn

[Q18] 模糊匹配
来源：http://bcn.xuetiantiany.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://yzr.zdbjq.cn

[Q19] 范围查询
来源：http://mkz.snrcjt.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ipc.pycfn.com

[Q20] IN 列表
来源：http://hlp.yuanzhike.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://izu.ehwqpu.com

[Q21] 空值判断
来源：http://daj.cqqwz.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://uth.smart0.xyz

[Q22] 排序
来源：http://zuy.zycfv.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ojc.epnwcf.com

[Q23] 分页
来源：http://slt.hnqzz.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://xok.gzhubu.top

[Q24] 去重
来源：http://syi.zhengqikj.top

SELECT DISTINCT city FROM users;
来源：http://lpn.jqgfzy.top

[Q25] 只取前 N 条
来源：http://jer.daria6918.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://bix.xinyue.icu

[Q26] 计数
来源：http://oir.fktsv.cn

SELECT COUNT(*) FROM users;
来源：http://ubl.svipenyu.cn

[Q27] 条件计数
来源：http://gxi.yuxming.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://noq.cdnleiting.top

[Q28] 求和与平均
来源：http://tix.kuanghao11.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wcs.zhongyouzk.top

[Q29] 最大最小值
来源：http://vyb.c1oappe.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://jov.redwolf501.top

[Q30] 分组统计
来源：http://ogj.yongpay.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://sjy.hnxiangtu.top

[Q31] 分组后过滤
来源：http://hfv.jiagoushi.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://cju.yongpay.top

[Q32] 分组拼接字符串
来源：http://ehj.kuanghao11.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://nat.zdbjq.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://asx.haohaochexian.top

[Q33] 多列分组
来源：http://zox.hongshengwenyu.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://zdo.ywan-chungtsiang.top

[Q34] 每组取第一条
来源：http://hvy.chenlongwang.top

SELECT * FROM (
来源：http://vqz.bbcook.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wtb.hfpthk.cn

) t WHERE rn = 1;
来源：http://wnc.haohaochexian.top

[Q35] 内连接
来源：http://vfd.cashguo.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://lsj.nanxinkj.top

[Q36] 左连接
来源：http://uqc.tanke756.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://bht.nanxinkj.top

[Q37] 右连接
来源：http://xkc.xziqi.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://uup.ivvv.top

[Q38] 全外连接（PostgreSQL）
来源：http://rmj.quarkkingdee.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://gvu.gaohongyu789.top

[Q39] 自连接（查上下级）
来源：http://sff.yj20258.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://qpj.ywan-chungtsiang.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ncg.mhx1999.top

[Q40] 交叉连接（笛卡尔积）
来源：http://tpq.bjfxy.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ipo.gaohongyu789.top

[Q41] 多表连接
来源：http://ugn.yj202588.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://ohc.yj20258.top

JOIN users u ON u.id = o.user_id
来源：http://vit.guannengcc.top

JOIN products p ON p.id = o.product_id;
来源：http://mvw.gotoacloud.top

[Q42] 连接条件附加过滤
来源：http://vxa.hongshengwenyu.top

SELECT u.name, o.amount FROM users u
来源：http://brl.vehdjk.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://qgv.shzxlz.cn

[Q43] 标量子查询
来源：http://iba.hywenlv.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://xvm.nwbrower.top

[Q44] IN 子查询
来源：http://itx.gotoacloud.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ssd.gogol.net.cn

[Q45] EXISTS 判断存在
来源：http://smf.zhiwuduotai.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fji.quarkkingdee.top

[Q46] NOT EXISTS 判断不存在
来源：http://rht.yj20258.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://dyq.jiagoushi.top

[Q47] 与平均值比较
来源：http://rqm.nanxuanxn.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://soz.ivvv.top

[Q48] CTE 公用表表达式
来源：http://ysn.tianlin.xyz

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://lot.nanxuanxn.top

SELECT * FROM t WHERE c > 5;
来源：http://aom.gotoacloud.top

[Q49] 更新单行
来源：http://lqk.hcnkem.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://bhh.jqgufenzy.top

[Q50] 批量更新
来源：http://jdh.cheryme.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ian.ehwqpu.com

[Q51] 用子查询更新
来源：http://qug.redwolf501.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://nuy.gaohongyu789.top

[Q52] 删除指定行
来源：http://kpm.dashuyun.cn

DELETE FROM users WHERE id = 10;
来源：http://wbg.ybcxt.top

[Q53] 按条件删除
来源：http://fvk.shanyushiyangkeji.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://gaj.tanke756.top

[Q54] 清空表
来源：http://zuk.sjlbkw.cn

TRUNCATE TABLE logs;
来源：http://fbr.jlsjyb.cn

[Q55] 排名（并列占位）
来源：http://sid.ywan-chungtsiang.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://byg.cheryme.top

[Q56] 密集排名（并列不占位）
来源：http://glh.redwolf501.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://bha.daria6918.cn

[Q57] 行号
来源：http://sgi.hcnkem.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://djr.bbcook.cn

[Q58] 累计求和
来源：http://wri.shangyingyoupin.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://caa.andypj.xyz

[Q59] 分组内累计
来源：http://qby.havefunace.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://iyv.yangfankeji.com

[Q60] 取上一行 / 下一行
来源：http://csx.birdmap.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://oph.epnwcf.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://bab.tarul.cn

[Q61] 移动平均
来源：http://ayj.cdnleiting.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mnm.zhoulong.xyz

[Q62] 分组占比
来源：http://ibg.chenzaomai.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ije.yanxiufei.cn

[Q63] 开启事务
来源：http://rqo.9152youxi.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://gvs.dianchejie.cn

[Q64] 提交事务
来源：http://mxj.gotoacloud.top

COMMIT;
来源：http://apz.yanxiufei.cn

[Q65] 回滚事务
来源：http://dyv.wangshuangyany.cn

ROLLBACK;
来源：http://vcp.redwolf501.top

[Q66] 行锁查询
来源：http://ktz.wangdashe.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://vrf.ctjpmb.com

[Q67] 设置隔离级别
来源：http://emh.ctjpmb.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://dyk.c1oappe.top

[Q68] 保存点
来源：http://ejr.wangshuangyany.cn

SAVEPOINT sp1;
来源：http://mmg.sweek.top

ROLLBACK TO sp1;
来源：http://ykj.daxiang520.top

[Q69] 查看执行计划
来源：http://cpg.ywan-chungtsiang.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://kme.daria6918.cn

[Q70] 更新统计信息
来源：http://rng.ctjpmb.com

ANALYZE TABLE users;
来源：http://wac.mhx1999.top

[Q71] 查看建表语句
来源：http://lkw.feifeiyinyue.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://vrs.aizwys.cn

[Q72] 查看索引
来源：http://cew.zhiwuduotai.top

SHOW INDEX FROM users;
来源：http://gzy.zdqjudy.top

[Q73] 查看表状态
来源：http://ftr.fktsv.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://odo.hcnkem.com

[Q74] 强制使用索引
来源：http://eev.chenzaomai.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://xei.uphjek.com

[Q75] 日期格式化
来源：http://ofr.wangdashe.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://zfr.0kj1m.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://uvu.mhx1999.top

[Q76] 按天统计
来源：http://mcu.shuidangran.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://kpt.yj202588.top

[Q77] 时间加减
来源：http://niu.yanxiufei.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ztb.tian-w.cn

[Q78] 当前时间
来源：http://gbf.mhx1999.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wuy.zdbjq.cn

[Q79] 字符串拼接
来源：http://wtx.xuetiantiany.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ulf.haohaochexian.top

[Q80] 字符串截取
来源：http://kxu.xuanzx.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wuc.mhx1999.top

[Q81] 字符串替换
来源：http://ivv.sxryk.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://bxq.52xcode.cn

[Q82] 字符长度与字节长度
来源：http://kxn.ybcxt.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://sax.hesvh.cn

[Q83] 大小写转换
来源：http://krv.birdmap.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ghp.shanyushiyangtech.top

[Q84] 去除首尾空格
来源：http://vcy.jqgufenzy.top

SELECT TRIM(name) FROM users;
来源：http://njd.uphjek.com

[Q85] 数值取整
来源：http://ldt.wangdashe.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://xiw.hongshengwenyu.top

[Q86] 读取 JSON 字段
来源：http://uht.gotoacloud.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://dmc.bjfxy.top

[Q87] JSON 字段做条件
来源：http://mek.jlsjyb.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://lfa.yongpay.top

[Q88] 行转列（条件聚合）
来源：http://kjq.hnxiangtu.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blu.shangyingyoupin.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://fud.shanyushiyangkeji.top

[Q89] 判断表是否存在
来源：http://fwa.gzhubu.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://sae.havefunace.top

[Q90] 生成序号列
来源：http://nec.sjlbkw.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://fdp.daria6918.cn

================================================================================
来源：http://adw.xingfuxueyuan.xyz

R. Bash 专题
来源：http://wwa.tanke756.top

================================================================================
来源：http://nxh.xinyue.icu

[R01] shebang 与严格模式
来源：http://wfv.9152youxi.cn

#!/usr/bin/env bash
来源：http://rmo.redwolf501.top

set -euo pipefail
来源：http://wte.daxiang520.top

[R02] 变量赋值与使用
来源：http://pcv.tarul.cn

name="Tom"; echo "$name"
来源：http://tsl.wangdashe.top

[R03] 只读变量
来源：http://xvt.hnxiangtu.top

readonly PI=3.14
来源：http://cni.quarkkingdee.top

[R04] 位置参数
来源：http://nlt.xuanzx.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://fzd.yfazqb.com

[R05] 参数默认值
来源：http://eti.shanyushiyangtech.top

name="${1:-default}"
来源：http://fju.chenzaomai.com

[R06] 判断命令是否存在
来源：http://zkl.yfazqb.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://tob.hywenlv.cn

[R07] if 判断文件
来源：http://nda.ivvv.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://lli.birdmap.top

[R08] 数值比较
来源：http://tje.yj202588.top

if (( a > b )); then echo "a 更大"; fi
来源：http://bxy.jianghu66.top

[R09] 字符串比较
来源：http://wqt.guowangkeji.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mlv.ivvv.top

[R10] 正则匹配
来源：http://srg.redwolf501.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://uog.yongpay.top

[R11] case 多分支
来源：http://cuj.c1oappe.top

case "$1" in
来源：http://szq.shangyingyoupin.top

start) echo "启动" ;;
来源：http://acq.gaohongyu789.top

stop)  echo "停止" ;;
来源：http://mey.chenlongwang.top

*)     echo "未知命令" ;;
来源：http://smz.uphjek.com

esac
来源：http://gpv.ehwqpu.com

[R12] for 遍历文件
来源：http://pqb.yongpay.top

for f in *.txt; do echo "$f"; done
来源：http://njk.sysykeji.top

[R13] for 计数循环
来源：http://lea.dashuyun.cn

for i in {1..10}; do echo "$i"; done
来源：http://icf.ydjk.org.cn

[R14] C 风格 for
来源：http://wuc.jyoumei.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hpg.yuanzhike.top

[R15] while 逐行读文件
来源：http://jss.shangyingyoupin.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://chx.yfazqb.com

[R16] until 等待条件
来源：http://wbc.shuidangran.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://bjg.hywenlv.cn

[R17] 数组定义与取值
来源：http://fnf.zhaomingkeji.xyz

arr=(a b c); echo "${arr[0]}"
来源：http://hxt.cheryme.top

[R18] 遍历数组
来源：http://gck.havefunace.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mtj.meibo888.top

[R19] 数组长度
来源：http://nyp.jyoumei.cn

echo "${#arr[@]}"
来源：http://jqb.ywan-chungtsiang.top

[R20] 关联数组（字典）
来源：http://bnh.yfazqb.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://clc.aibaodan.cn

[R21] 字符串长度
来源：http://xkx.cashguo.top

echo "${#s}"
来源：http://rvo.yueranfly.top

[R22] 截取子串
来源：http://jxw.316326.xyz

echo "${s:0:5}"
来源：http://qkp.shangyingyoupin.top

[R23] 字符串替换
来源：http://xjw.hnqzz.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wji.tian-w.cn

[R24] 大小写转换
来源：http://rwa.shanyushiyangtech.top

echo "${s^^}"; echo "${s,,}"
来源：http://cnd.gzhubu.top

[R25] 去后缀 / 去前缀
来源：http://iqm.hysaishi.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://azn.yongpay.top

[R26] 命令替换
来源：http://xmw.jinqigfzy.top

now=$(date +%F); echo "$now"
来源：http://dyj.52xcode.cn

[R27] 算术展开
来源：http://ico.guowangkeji.top

echo $((1 + 2 * 3))
来源：http://eyi.guannengcc.top

[R28] 浮点运算
来源：http://evd.hywenlv.cn

echo "scale=2; 10/3" | bc
来源：http://nwn.vehdjk.com

[R29] 定义函数
来源：http://muf.gotoacloud.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://dhi.guowangkeji.top

[R30] 函数返回状态码
来源：http://bxh.xylfe.cn

f() { return 0; }; f || echo "失败了"
来源：http://zhf.smart0.xyz

[R31] 局部变量
来源：http://hde.yuxming.cn

f() { local x=1; echo "$x"; }
来源：http://ayn.xuanzx.com

[R32] 参数个数校验
来源：http://hqw.sufxvd.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://onb.guannengcc.top

[R33] 捕获错误并提示行号
来源：http://yph.hysaishi.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://qol.jianghu66.top

[R34] 退出时清理
来源：http://iye.aibaodan.cn

trap 'rm -f "$tmp"' EXIT
来源：http://pqm.hysaishi.cn

[R35] 后台执行并等待
来源：http://jbz.sysykeji.top

sleep 5 & pid=$!; wait "$pid"
来源：http://ngp.316326.xyz

[R36] 并发执行多个任务
来源：http://neo.vehdjk.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://bxr.jinghuilouyu.cn

[R37] 把输出赋给变量
来源：http://lyr.nanxinkj.top

files=$(ls -1)
来源：http://ykh.jinqigfzy.top

[R38] 管道串联
来源：http://zbj.tianlin.xyz

cat a.txt | grep -i error | wc -l
来源：http://pny.cucudq.cn

[R39] 重定向标准输出与错误
来源：http://yqn.cucudq.cn

cmd > out.log 2>&1
来源：http://cgv.hywenlv.cn

[R40] 追加写日志
来源：http://njt.ydzc1.top

echo "log" >> out.log
来源：http://tpu.fengsongda.top

[R41] 丢弃输出
来源：http://obz.zhijiandao.cn

cmd >/dev/null 2>&1
来源：http://twi.shanyushiyangtech.top

[R42] 输入重定向
来源：http://aau.dianchejie.cn

wc -l < a.txt
来源：http://tkm.c1oappe.top

[R43] 按名字查找文件
来源：http://php.aibaodan.cn

find . -name "*.log" -type f
来源：http://lmt.guowangkeji.top

[R44] 按修改时间查找
来源：http://oge.zhiwuduotai.top

find . -mtime -7 -type f
来源：http://vna.ivvv.top

[R45] 批量删除
来源：http://tpb.yangfankeji.com

find . -name "*.tmp" -delete
来源：http://cyy.quarkkingdee.top

[R46] 递归替换文件内容
来源：http://xep.zhijiandao.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://cxk.bbcook.cn

[R47] sed 单行替换
来源：http://uyo.nanxinkj.top

sed -i 's/foo/bar/g' a.txt
来源：http://rli.zhixingplan.top

[R48] awk 取指定列
来源：http://fiy.chenlongwang.top

awk '{print $1, $3}' a.txt
来源：http://hkm.nanxinkj.top

[R49] awk 带条件
来源：http://bcc.chenzaomai.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://zkt.xuanzx.com

[R50] awk 求和
来源：http://wto.xylfe.cn

awk '{s += $2} END {print s}' a.txt
来源：http://lln.9152youxi.cn

[R51] 排序去重取前几
来源：http://rvj.chenlongwang.top

sort a.txt | uniq -c | sort -rn | head
来源：http://wlh.ivvv.top

[R52] 统计行数
来源：http://zye.shanyushiyangkeji.top

wc -l a.txt
来源：http://rpq.fktsv.cn

[R53] 查看文件头与实时尾
来源：http://eii.redwolf501.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ndu.vqdsnc.cn

[R54] 比较两个文件
来源：http://yog.jinqigufen.top

diff a.txt b.txt
来源：http://rxc.vqdsnc.cn

[R55] 压缩与解压
来源：http://rck.hfpthk.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://qwi.ydjk.org.cn

[R56] 远程拷贝
来源：http://gkv.xingfuxueyuan.xyz

scp file user@host:/path/
来源：http://pty.zycfv.cn

[R57] 远程执行命令
来源：http://upt.epnwcf.com


<!-- 参考信息 -->