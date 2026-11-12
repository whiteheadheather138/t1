代发 wailian999

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://djh.xinyue.icu

[Q11] 一次插入多行
来源：http://zec.xinyue.icu

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://jff.havefunace.top

[Q12] 插入后取自增 ID
来源：http://xdm.aibaodan.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ohi.svipenyu.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://jdh.feifeiyinyue.top

[Q13] 忽略重复插入
来源：http://wrb.yuxming.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hgu.sufxvd.cn

[Q14] 存在则更新（upsert）
来源：http://ugr.birdmap.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://zmr.yj20258888.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://jep.zhijiandao.cn

[Q15] 查询全部
来源：http://myc.hongshengwenyu.top

SELECT * FROM users;
来源：http://rtc.uphjek.com

[Q16] 查询指定列
来源：http://ojk.chenjidiqi.icu

SELECT id, name FROM users;
来源：http://sty.hnxiangtu.top

[Q17] 条件查询
来源：http://kqx.sweek.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://oyz.pengpengdd.cyou

[Q18] 模糊匹配
来源：http://lcb.yueranfly.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://pzi.9152youxi.cn

[Q19] 范围查询
来源：http://cow.shangyingyoupin.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://dfo.chenlongwang.top

[Q20] IN 列表
来源：http://ili.bjfxy.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://woy.iojbl.cn

[Q21] 空值判断
来源：http://nam.fanxiaobao.xyz

SELECT * FROM users WHERE email IS NULL;
来源：http://iml.smart0.xyz

[Q22] 排序
来源：http://bmq.zhiwuduotai.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://rgr.zycfv.cn

[Q23] 分页
来源：http://ejl.redwolf501.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://xte.xylfe.cn

[Q24] 去重
来源：http://qlm.zdqjudy.top

SELECT DISTINCT city FROM users;
来源：http://eur.cqqwz.cn

[Q25] 只取前 N 条
来源：http://yqt.cheryme.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://dkn.hcnkem.com

[Q26] 计数
来源：http://jkt.zhoulong.xyz

SELECT COUNT(*) FROM users;
来源：http://hwn.hfpthk.cn

[Q27] 条件计数
来源：http://jlo.0kj1m.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ccp.tarul.cn

[Q28] 求和与平均
来源：http://gmq.ehwqpu.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mhb.yj202588.top

[Q29] 最大最小值
来源：http://mma.wangshuangyany.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://tec.zhoulong.xyz

[Q30] 分组统计
来源：http://les.shuidangran.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://kdg.hesvh.cn

[Q31] 分组后过滤
来源：http://xlx.ctjpmb.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://fuf.kuanghao11.cn

[Q32] 分组拼接字符串
来源：http://dqn.hcnkem.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://moe.havefunace.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://asf.yonumen.top

[Q33] 多列分组
来源：http://puh.chenlongwang.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wqi.gogol.net.cn

[Q34] 每组取第一条
来源：http://lje.uphjek.com

SELECT * FROM (
来源：http://lqa.xinyue.icu

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://vrf.ivvv.top

) t WHERE rn = 1;
来源：http://dlw.iojbl.cn

[Q35] 内连接
来源：http://eou.bbcook.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://xzf.tianlin.xyz

[Q36] 左连接
来源：http://kfr.shzxlz.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://uaq.uphjek.com

[Q37] 右连接
来源：http://yor.havefunace.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://aki.shangyingyoupin.top

[Q38] 全外连接（PostgreSQL）
来源：http://fef.aizwys.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ojw.wangshuangyany.cn

[Q39] 自连接（查上下级）
来源：http://fmz.cucudq.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://hmo.hnxiangtu.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://pyy.fanxiaobao.xyz

[Q40] 交叉连接（笛卡尔积）
来源：http://zli.zhaomingkeji.xyz

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wvc.c1oappe.top

[Q41] 多表连接
来源：http://hke.jlsjyb.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://hqz.shanyushiyangkeji.top

JOIN users u ON u.id = o.user_id
来源：http://eoi.quarkkingdee.top

JOIN products p ON p.id = o.product_id;
来源：http://fuq.hcnkem.com

[Q42] 连接条件附加过滤
来源：http://ohh.daria6918.cn

SELECT u.name, o.amount FROM users u
来源：http://zpi.ydzc1.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://uds.cqqwz.cn

[Q43] 标量子查询
来源：http://yfi.yfazqb.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://uzu.xuanzx.com

[Q44] IN 子查询
来源：http://wwh.hnxiangtu.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://rpb.epnwcf.com

[Q45] EXISTS 判断存在
来源：http://wha.svipenyu.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ksh.snrcjt.cn

[Q46] NOT EXISTS 判断不存在
来源：http://tir.smart0.xyz

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kxe.yvedp.cn

[Q47] 与平均值比较
来源：http://ygr.9152youxi.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hmj.ybcxt.top

[Q48] CTE 公用表表达式
来源：http://ido.uphjek.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ebh.fanxiaobao.xyz

SELECT * FROM t WHERE c > 5;
来源：http://kle.xuanzx.com

[Q49] 更新单行
来源：http://nmk.redwolf501.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://nrq.zhixingplan.top

[Q50] 批量更新
来源：http://zej.xuanzx.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://bsi.guowangkeji.top

[Q51] 用子查询更新
来源：http://qzm.jianghu66.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hmg.iojbl.cn

[Q52] 删除指定行
来源：http://nof.cashguo.top

DELETE FROM users WHERE id = 10;
来源：http://egi.daria6918.cn

[Q53] 按条件删除
来源：http://apr.pycfn.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://fyg.ydzc1.top

[Q54] 清空表
来源：http://eoc.yangfankeji.com

TRUNCATE TABLE logs;
来源：http://xzf.fzhhl.top

[Q55] 排名（并列占位）
来源：http://fgc.52xcode.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://fcx.pengpengdd.cyou

[Q56] 密集排名（并列不占位）
来源：http://kht.jianghu66.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ryl.wangshuangyany.cn

[Q57] 行号
来源：http://sou.yuxming.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://aqq.cheryme.top

[Q58] 累计求和
来源：http://mby.zhixingplan.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://fdw.hesvh.cn

[Q59] 分组内累计
来源：http://xye.kuanghao11.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://cot.52xcode.cn

[Q60] 取上一行 / 下一行
来源：http://bdg.shanyushiyangkeji.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://tdd.bjfxy.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://xhz.epnwcf.com

[Q61] 移动平均
来源：http://opu.gogol.net.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://xkr.tianlin.xyz

[Q62] 分组占比
来源：http://mpg.jqgufenzy.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://zsp.yuxming.cn

[Q63] 开启事务
来源：http://fxe.jqgfzy.top

START TRANSACTION;                -- 或 BEGIN
来源：http://aoq.chenzaomai.com

[Q64] 提交事务
来源：http://vdz.jinqigufen.top

COMMIT;
来源：http://smf.jlsjyb.cn

[Q65] 回滚事务
来源：http://kcm.yvedp.cn

ROLLBACK;
来源：http://orp.ydzc1.top

[Q66] 行锁查询
来源：http://kub.52xcode.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://avn.redwolf501.top

[Q67] 设置隔离级别
来源：http://kxh.jinqigfzy.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://vdn.epnwcf.com

[Q68] 保存点
来源：http://yoi.redwolf501.top

SAVEPOINT sp1;
来源：http://sty.tarul.cn

ROLLBACK TO sp1;
来源：http://eap.zhengqikj.top

[Q69] 查看执行计划
来源：http://jlz.chenzaomai.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://osi.tian-w.cn

[Q70] 更新统计信息
来源：http://pza.haohaochexian.top

ANALYZE TABLE users;
来源：http://ckk.daxiang520.top

[Q71] 查看建表语句
来源：http://oyu.9152youxi.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wpv.zhengqikj.top

[Q72] 查看索引
来源：http://lhr.cucudq.cn

SHOW INDEX FROM users;
来源：http://den.tian-w.cn

[Q73] 查看表状态
来源：http://pze.0kj1m.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://jmd.havefunace.top

[Q74] 强制使用索引
来源：http://ddg.redwolf501.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://txc.ybcxt.top

[Q75] 日期格式化
来源：http://xeh.jiagoushi.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://qts.gotoacloud.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://jfi.yfazqb.com

[Q76] 按天统计
来源：http://esj.yanxiufei.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://vxf.shanyushiyangkeji.top

[Q77] 时间加减
来源：http://ulv.pycfn.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://enx.jiagoushi.top

[Q78] 当前时间
来源：http://ljn.ybcxt.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://sli.mhx1999.top

[Q79] 字符串拼接
来源：http://cyz.snrcjt.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://tfk.mhx1999.top

[Q80] 字符串截取
来源：http://paf.feifeiyinyue.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://cwf.guowangkeji.top

[Q81] 字符串替换
来源：http://kka.hcnkem.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://sjz.bjfxy.top

[Q82] 字符长度与字节长度
来源：http://too.guowangkeji.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://bil.zdqjudy.top

[Q83] 大小写转换
来源：http://qrh.xuanzx.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://qnb.yuxming.cn

[Q84] 去除首尾空格
来源：http://rtm.shzxlz.cn

SELECT TRIM(name) FROM users;
来源：http://qkw.cheryme.top

[Q85] 数值取整
来源：http://wnj.hywenlv.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://zhz.xuanzx.com

[Q86] 读取 JSON 字段
来源：http://rtp.yfazqb.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://nxm.iojbl.cn

[Q87] JSON 字段做条件
来源：http://wix.zdbjq.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://cle.fehbvm.com

[Q88] 行转列（条件聚合）
来源：http://ukw.ivvv.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mrh.shuidangran.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://tvi.jlsjyb.cn

[Q89] 判断表是否存在
来源：http://ito.jqgufenzy.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://oar.uphjek.com

[Q90] 生成序号列
来源：http://lpz.zhaomingkeji.xyz

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://cda.chenjidiqi.icu

================================================================================
来源：http://fex.ydzc1.top

R. Bash 专题
来源：http://vik.fengsongda.top

================================================================================
来源：http://chf.yuxming.cn

[R01] shebang 与严格模式
来源：http://zij.tarul.cn

#!/usr/bin/env bash
来源：http://njn.nanxinkj.top

set -euo pipefail
来源：http://wve.kuanghao11.cn

[R02] 变量赋值与使用
来源：http://int.xuetiantiany.cn

name="Tom"; echo "$name"
来源：http://hbv.316326.xyz

[R03] 只读变量
来源：http://vxj.ybcxt.top

readonly PI=3.14
来源：http://giu.zhaomingkeji.xyz

[R04] 位置参数
来源：http://gqx.birdmap.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://cvq.yanxiufei.cn

[R05] 参数默认值
来源：http://brc.ppjwa.cn

name="${1:-default}"
来源：http://gsd.dianchejie.cn

[R06] 判断命令是否存在
来源：http://seb.yueranfly.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ytj.shzxlz.cn

[R07] if 判断文件
来源：http://bma.hfpthk.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://cfb.dianchejie.cn

[R08] 数值比较
来源：http://yln.jinghuilouyu.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://khg.jianghu66.top

[R09] 字符串比较
来源：http://cjs.zhongyouzk.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hqi.shzxlz.cn

[R10] 正则匹配
来源：http://kez.chenjidiqi.icu

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ign.gaohongyu789.top

[R11] case 多分支
来源：http://hpa.tian-w.cn

case "$1" in
来源：http://zzu.epnwcf.com

start) echo "启动" ;;
来源：http://iyd.gaohongyu789.top

stop)  echo "停止" ;;
来源：http://zab.xylfe.cn

*)     echo "未知命令" ;;
来源：http://bqb.zycfv.cn

esac
来源：http://kff.vqdsnc.cn

[R12] for 遍历文件
来源：http://nfx.zdbjq.cn

for f in *.txt; do echo "$f"; done
来源：http://ozy.yuanzhike.top

[R13] for 计数循环
来源：http://tjy.bjfxy.top

for i in {1..10}; do echo "$i"; done
来源：http://lyf.shzxlz.cn

[R14] C 风格 for
来源：http://vtp.kuanghao11.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ugj.redwolf501.top

[R15] while 逐行读文件
来源：http://woa.wangshuangyany.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://jhe.havefunace.top

[R16] until 等待条件
来源：http://tos.ywan-chungtsiang.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://xjh.hesvh.cn

[R17] 数组定义与取值
来源：http://ndg.zhengqikj.top

arr=(a b c); echo "${arr[0]}"
来源：http://sue.ybcxt.top

[R18] 遍历数组
来源：http://nbx.hammf.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ysm.sjlbkw.cn

[R19] 数组长度
来源：http://abn.xuetiantiany.cn

echo "${#arr[@]}"
来源：http://cjj.dianchejie.cn

[R20] 关联数组（字典）
来源：http://tfw.jyoumei.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://vyx.nwbrower.top

[R21] 字符串长度
来源：http://iuh.yangfankeji.com

echo "${#s}"
来源：http://ymj.bbcook.cn

[R22] 截取子串
来源：http://hun.zycfv.cn

echo "${s:0:5}"
来源：http://ksq.zhongyouzk.top

[R23] 字符串替换
来源：http://iuk.gogol.net.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://fjc.quarkkingdee.top

[R24] 大小写转换
来源：http://lnd.jinqigfzy.top

echo "${s^^}"; echo "${s,,}"
来源：http://dyc.hammf.cn

[R25] 去后缀 / 去前缀
来源：http://zke.aibaodan.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://rsb.jqgfzy.top

[R26] 命令替换
来源：http://ylr.cqqwz.cn

now=$(date +%F); echo "$now"
来源：http://ihk.ybcxt.top

[R27] 算术展开
来源：http://vms.yvedp.cn

echo $((1 + 2 * 3))
来源：http://xzm.redwolf501.top

[R28] 浮点运算
来源：http://jfw.jyoumei.cn

echo "scale=2; 10/3" | bc
来源：http://caw.jyoumei.cn

[R29] 定义函数
来源：http://ckr.wangdashe.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://krn.sufxvd.cn

[R30] 函数返回状态码
来源：http://ccx.jinyuanbaomall.cn

f() { return 0; }; f || echo "失败了"
来源：http://jmz.jinyuanbaomall.cn

[R31] 局部变量
来源：http://fqr.bbcook.cn

f() { local x=1; echo "$x"; }
来源：http://uxv.ehwqpu.com

[R32] 参数个数校验
来源：http://rvh.yanxiufei.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://fly.haohaochexian.top

[R33] 捕获错误并提示行号
来源：http://cdz.quarkkingdee.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://rbz.jinghuilouyu.cn

[R34] 退出时清理
来源：http://hrr.birdmap.top

trap 'rm -f "$tmp"' EXIT
来源：http://bpj.zhoulong.xyz

[R35] 后台执行并等待
来源：http://kjc.dianchejie.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://zhb.fzhhl.top

[R36] 并发执行多个任务
来源：http://qsh.yanxiufei.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://psx.gzhubu.top

[R37] 把输出赋给变量
来源：http://gye.ppjwa.cn

files=$(ls -1)
来源：http://qde.yj20258888.top

[R38] 管道串联
来源：http://aum.nanxuanxn.top

cat a.txt | grep -i error | wc -l
来源：http://ege.tianlin.xyz

[R39] 重定向标准输出与错误
来源：http://nkp.ybcxt.top

cmd > out.log 2>&1
来源：http://bas.bbcook.cn

[R40] 追加写日志
来源：http://pmi.ydzc1.top

echo "log" >> out.log
来源：http://bti.chenlongwang.top

[R41] 丢弃输出
来源：http://jmk.vehdjk.com

cmd >/dev/null 2>&1
来源：http://ddq.zhijiandao.cn

[R42] 输入重定向
来源：http://jbf.daxiang520.top

wc -l < a.txt
来源：http://rjm.wangshuangyany.cn

[R43] 按名字查找文件
来源：http://ubw.cucudq.cn

find . -name "*.log" -type f
来源：http://niv.sufxvd.cn

[R44] 按修改时间查找
来源：http://mpk.kuanghao11.cn

find . -mtime -7 -type f
来源：http://zwh.shanyushiyangkeji.top

[R45] 批量删除
来源：http://fbg.xziqi.cn

find . -name "*.tmp" -delete
来源：http://mxt.zhiwuduotai.top

[R46] 递归替换文件内容
来源：http://alr.ivvv.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://dxd.xylfe.cn

[R47] sed 单行替换
来源：http://orb.smart0.xyz

sed -i 's/foo/bar/g' a.txt
来源：http://hpf.hywenlv.cn

[R48] awk 取指定列
来源：http://btv.hammf.cn

awk '{print $1, $3}' a.txt
来源：http://tjv.shangyingyoupin.top

[R49] awk 带条件
来源：http://bcv.jqgufenzy.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hbg.yj20258888.top

[R50] awk 求和
来源：http://ceu.hesvh.cn

awk '{s += $2} END {print s}' a.txt
来源：http://gti.bbcook.cn

[R51] 排序去重取前几
来源：http://bww.jianghu66.top

sort a.txt | uniq -c | sort -rn | head
来源：http://xvu.hammf.cn

[R52] 统计行数
来源：http://htt.ivvv.top

wc -l a.txt
来源：http://hfv.mhx1999.top

[R53] 查看文件头与实时尾
来源：http://gel.hongshengwenyu.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://itx.jqgufenzy.top

[R54] 比较两个文件
来源：http://tcr.fengsongda.top

diff a.txt b.txt
来源：http://kgq.nanxinkj.top

[R55] 压缩与解压
来源：http://rll.guannengcc.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://zoy.hysaishi.cn

[R56] 远程拷贝
来源：http://bwq.hcnkem.com

scp file user@host:/path/
来源：http://ggp.yj202588.top

[R57] 远程执行命令
来源：http://yxh.yonumen.top

ssh user@host 'uptime'
来源：http://llx.xinyue.icu

[R58] 下载文件
来源：http://riv.nanxinkj.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://zmw.chenzaomai.com

[R59] 发 POST JSON
来源：http://xcm.sufxvd.cn


<!-- 参考信息 -->