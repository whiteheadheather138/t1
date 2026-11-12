代发 wailian999

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://fvy.iojbl.cn

[Q18] 模糊匹配
来源：http://zia.zdqjudy.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ols.aizwys.cn

[Q19] 范围查询
来源：http://uew.tian-w.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wgv.chenjidiqi.icu

[Q20] IN 列表
来源：http://izp.jinghuilouyu.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://zkp.tianlin.xyz

[Q21] 空值判断
来源：http://qco.meibo888.top

SELECT * FROM users WHERE email IS NULL;
来源：http://gve.jinqigfzy.top

[Q22] 排序
来源：http://chu.gzhubu.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://grv.dianchejie.cn

[Q23] 分页
来源：http://hjy.pycfn.com

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mdr.mhx1999.top

[Q24] 去重
来源：http://mvu.xingfuxueyuan.xyz

SELECT DISTINCT city FROM users;
来源：http://top.sweek.top

[Q25] 只取前 N 条
来源：http://uvx.jinqigfzy.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://goz.zhijiandao.cn

[Q26] 计数
来源：http://rfn.xylfe.cn

SELECT COUNT(*) FROM users;
来源：http://vqc.chenlongwang.top

[Q27] 条件计数
来源：http://aei.shanyushiyangkeji.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://jtj.yueranfly.top

[Q28] 求和与平均
来源：http://oiv.jqgfzy.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://bbi.zhaomingkeji.xyz

[Q29] 最大最小值
来源：http://ozp.jinqigfzy.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://urb.tian-w.cn

[Q30] 分组统计
来源：http://rtd.ydzc1.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mgy.yangfankeji.com

[Q31] 分组后过滤
来源：http://xnn.andypj.xyz

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wce.gotoacloud.top

[Q32] 分组拼接字符串
来源：http://bkw.smart0.xyz

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://gdj.ydjk.org.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ynb.cqqwz.cn

[Q33] 多列分组
来源：http://rzy.wangshuangyany.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://fwn.dianchejie.cn

[Q34] 每组取第一条
来源：http://gbk.shuidangran.top

SELECT * FROM (
来源：http://cmk.9152youxi.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://vum.pycfn.com

) t WHERE rn = 1;
来源：http://zqc.andypj.xyz

[Q35] 内连接
来源：http://joe.hcnkem.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://fax.aibaodan.cn

[Q36] 左连接
来源：http://qub.meibo888.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://cvs.guannengcc.top

[Q37] 右连接
来源：http://ouh.zdbjq.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://vkn.fktsv.cn

[Q38] 全外连接（PostgreSQL）
来源：http://lqg.cucudq.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://jhv.iojbl.cn

[Q39] 自连接（查上下级）
来源：http://dei.fzhhl.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://hzn.zdqjudy.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ory.shangyingyoupin.top

[Q40] 交叉连接（笛卡尔积）
来源：http://hjc.mhx1999.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://rlu.dianchejie.cn

[Q41] 多表连接
来源：http://kgg.cheryme.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://jwr.fanxiaobao.xyz

JOIN users u ON u.id = o.user_id
来源：http://qak.nwbrower.top

JOIN products p ON p.id = o.product_id;
来源：http://dvq.nwbrower.top

[Q42] 连接条件附加过滤
来源：http://mvs.zdqjudy.top

SELECT u.name, o.amount FROM users u
来源：http://qvp.zycfv.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://cwk.andypj.xyz

[Q43] 标量子查询
来源：http://jjz.ehwqpu.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://kbt.jlsjyb.cn

[Q44] IN 子查询
来源：http://gzw.shzxlz.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://alz.yongpay.top

[Q45] EXISTS 判断存在
来源：http://joo.gaohongyu789.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://csv.xinyue.icu

[Q46] NOT EXISTS 判断不存在
来源：http://apt.ppjwa.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qmu.xziqi.cn

[Q47] 与平均值比较
来源：http://vix.nanxinkj.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hcz.yj202588.top

[Q48] CTE 公用表表达式
来源：http://xpj.tarul.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://bge.wangdashe.top

SELECT * FROM t WHERE c > 5;
来源：http://rgs.jinghuilouyu.cn

[Q49] 更新单行
来源：http://bqh.cucudq.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://amz.yuxming.cn

[Q50] 批量更新
来源：http://swe.fanxiaobao.xyz

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://xyb.jinqigfzy.top

[Q51] 用子查询更新
来源：http://gyc.hammf.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://qep.gzhubu.top

[Q52] 删除指定行
来源：http://wzy.xingfuxueyuan.xyz

DELETE FROM users WHERE id = 10;
来源：http://myr.hfpthk.cn

[Q53] 按条件删除
来源：http://nov.jlsjyb.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://xdj.0kj1m.cn

[Q54] 清空表
来源：http://ibv.cqqwz.cn

TRUNCATE TABLE logs;
来源：http://fwh.quarkkingdee.top

[Q55] 排名（并列占位）
来源：http://pjd.jinqigfzy.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://lrr.yongpay.top

[Q56] 密集排名（并列不占位）
来源：http://sdk.ydjk.org.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://rfm.zhongyouzk.top

[Q57] 行号
来源：http://ipb.hysaishi.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://cys.9152youxi.cn

[Q58] 累计求和
来源：http://zdk.yangfankeji.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://grw.sjlbkw.cn

[Q59] 分组内累计
来源：http://kzi.cheryme.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://coy.ctjpmb.com

[Q60] 取上一行 / 下一行
来源：http://ngv.ywan-chungtsiang.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://yhw.0kj1m.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://smd.jlsjyb.cn

[Q61] 移动平均
来源：http://szk.dianchejie.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ydu.quarkkingdee.top

[Q62] 分组占比
来源：http://isa.smart0.xyz

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://zsp.nanxuanxn.top

[Q63] 开启事务
来源：http://gso.iojbl.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://jcj.tianlin.xyz

[Q64] 提交事务
来源：http://xtt.sweek.top

COMMIT;
来源：http://eym.hesvh.cn

[Q65] 回滚事务
来源：http://zzz.snrcjt.cn

ROLLBACK;
来源：http://uji.shanyushiyangkeji.top

[Q66] 行锁查询
来源：http://khx.9152youxi.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://jvj.zdqjudy.top

[Q67] 设置隔离级别
来源：http://pzj.0kj1m.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://fzm.jiagoushi.top

[Q68] 保存点
来源：http://nuj.yangfankeji.com

SAVEPOINT sp1;
来源：http://omq.yvedp.cn

ROLLBACK TO sp1;
来源：http://mnf.xingfuxueyuan.xyz

[Q69] 查看执行计划
来源：http://hrj.chenjidiqi.icu

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://nnv.ybcxt.top

[Q70] 更新统计信息
来源：http://iqg.cucudq.cn

ANALYZE TABLE users;
来源：http://wvz.gogol.net.cn

[Q71] 查看建表语句
来源：http://aqt.zhaomingkeji.xyz

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://kjs.hnxiangtu.top

[Q72] 查看索引
来源：http://hej.jinghuilouyu.cn

SHOW INDEX FROM users;
来源：http://uet.jqgufenzy.top

[Q73] 查看表状态
来源：http://uvl.chenjidiqi.icu

SHOW TABLE STATUS LIKE 'users';
来源：http://ccl.tarul.cn

[Q74] 强制使用索引
来源：http://mdq.fanxiaobao.xyz

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://agk.jinghuilouyu.cn

[Q75] 日期格式化
来源：http://zno.xinyue.icu

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://vnm.iojbl.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://yyg.jiagoushi.top

[Q76] 按天统计
来源：http://tnu.yuanzhike.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://bfu.tianlin.xyz

[Q77] 时间加减
来源：http://xik.sweek.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wfj.guowangkeji.top

[Q78] 当前时间
来源：http://gyd.jinqigfzy.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://clo.yj202588.top

[Q79] 字符串拼接
来源：http://dym.jinqigfzy.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://uka.kuanghao11.cn

[Q80] 字符串截取
来源：http://iwd.guowangkeji.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://gqg.hysaishi.cn

[Q81] 字符串替换
来源：http://ktl.zdbjq.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wpm.nanxinkj.top

[Q82] 字符长度与字节长度
来源：http://bvd.zhengqikj.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mqp.chenjidiqi.icu

[Q83] 大小写转换
来源：http://hhg.kuanghao11.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://adu.aibaodan.cn

[Q84] 去除首尾空格
来源：http://ddv.yongpay.top

SELECT TRIM(name) FROM users;
来源：http://woc.quarkkingdee.top

[Q85] 数值取整
来源：http://jtb.hesvh.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://rlc.pycfn.com

[Q86] 读取 JSON 字段
来源：http://xua.yongpay.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://lxv.sjlbkw.cn

[Q87] JSON 字段做条件
来源：http://knh.jinqigufen.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ekt.sxryk.cn

[Q88] 行转列（条件聚合）
来源：http://mpc.gogol.net.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://sqr.zhaomingkeji.xyz

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://lcv.kuanghao11.cn

[Q89] 判断表是否存在
来源：http://gcx.yueranfly.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://teq.sjlbkw.cn

[Q90] 生成序号列
来源：http://fnc.zycfv.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://fte.redwolf501.top

================================================================================
来源：http://loh.sweek.top

R. Bash 专题
来源：http://zhv.wangshuangyany.cn

================================================================================
来源：http://zmd.tarul.cn

[R01] shebang 与严格模式
来源：http://mxq.andypj.xyz

#!/usr/bin/env bash
来源：http://sdp.daria6918.cn

set -euo pipefail
来源：http://pby.uphjek.com

[R02] 变量赋值与使用
来源：http://siw.sweek.top

name="Tom"; echo "$name"
来源：http://mrt.wangshuangyany.cn

[R03] 只读变量
来源：http://kye.9152youxi.cn

readonly PI=3.14
来源：http://vdr.feifeiyinyue.top

[R04] 位置参数
来源：http://zke.c1oappe.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://sby.uphjek.com

[R05] 参数默认值
来源：http://mky.havefunace.top

name="${1:-default}"
来源：http://thi.birdmap.top

[R06] 判断命令是否存在
来源：http://znu.fanxiaobao.xyz

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://nfg.yj20258.top

[R07] if 判断文件
来源：http://sye.hesvh.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://yjf.fanxiaobao.xyz

[R08] 数值比较
来源：http://bhd.hcnkem.com

if (( a > b )); then echo "a 更大"; fi
来源：http://sum.jqgfzy.top

[R09] 字符串比较
来源：http://cfg.daria6918.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://aab.andypj.xyz

[R10] 正则匹配
来源：http://irf.svipenyu.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ouf.nwbrower.top

[R11] case 多分支
来源：http://ouv.feifeiyinyue.top

case "$1" in
来源：http://rrg.vqdsnc.cn

start) echo "启动" ;;
来源：http://eyo.zhiwuduotai.top

stop)  echo "停止" ;;
来源：http://xlp.birdmap.top

*)     echo "未知命令" ;;
来源：http://jeu.gzhubu.top

esac
来源：http://odv.yanxiufei.cn

[R12] for 遍历文件
来源：http://uhw.nwbrower.top

for f in *.txt; do echo "$f"; done
来源：http://gtm.birdmap.top

[R13] for 计数循环
来源：http://kcb.yj20258888.top

for i in {1..10}; do echo "$i"; done
来源：http://dds.shangyingyoupin.top

[R14] C 风格 for
来源：http://rwb.gotoacloud.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://kya.meibo888.top

[R15] while 逐行读文件
来源：http://wae.wangdashe.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://zqo.ydzc1.top

[R16] until 等待条件
来源：http://rjh.wangdashe.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://rgn.hysaishi.cn

[R17] 数组定义与取值
来源：http://nng.haohaochexian.top

arr=(a b c); echo "${arr[0]}"
来源：http://hkp.cqqwz.cn

[R18] 遍历数组
来源：http://spa.hysaishi.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://tof.sufxvd.cn

[R19] 数组长度
来源：http://dgv.yangfankeji.com

echo "${#arr[@]}"
来源：http://kda.nwbrower.top

[R20] 关联数组（字典）
来源：http://rov.chenlongwang.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://uuz.meibo888.top

[R21] 字符串长度
来源：http://ckh.haohaochexian.top

echo "${#s}"
来源：http://hry.bjfxy.top

[R22] 截取子串
来源：http://ibo.xuanzx.com

echo "${s:0:5}"
来源：http://eyt.gzhubu.top

[R23] 字符串替换
来源：http://qoi.cdnleiting.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://dkh.sysykeji.top

[R24] 大小写转换
来源：http://utr.jqgfzy.top

echo "${s^^}"; echo "${s,,}"
来源：http://pmr.wangdashe.top

[R25] 去后缀 / 去前缀
来源：http://gfb.hammf.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://uzu.tarul.cn

[R26] 命令替换
来源：http://mkz.hcnkem.com

now=$(date +%F); echo "$now"
来源：http://kbc.jqgufenzy.top

[R27] 算术展开
来源：http://bgb.smart0.xyz

echo $((1 + 2 * 3))
来源：http://xnk.ywan-chungtsiang.top

[R28] 浮点运算
来源：http://zdd.zycfv.cn

echo "scale=2; 10/3" | bc
来源：http://npu.hywenlv.cn

[R29] 定义函数
来源：http://fez.hnxiangtu.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://snd.ehwqpu.com

[R30] 函数返回状态码
来源：http://emt.andypj.xyz

f() { return 0; }; f || echo "失败了"
来源：http://rvy.zhixingplan.top

[R31] 局部变量
来源：http://btx.gaohongyu789.top

f() { local x=1; echo "$x"; }
来源：http://kmc.yvedp.cn

[R32] 参数个数校验
来源：http://sfi.fehbvm.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://lni.yuanzhike.top

[R33] 捕获错误并提示行号
来源：http://weq.hnxiangtu.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://kaf.yanxiufei.cn

[R34] 退出时清理
来源：http://fhm.shangyingyoupin.top

trap 'rm -f "$tmp"' EXIT
来源：http://olm.ydjk.org.cn

[R35] 后台执行并等待
来源：http://elo.tian-w.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://znd.shzxlz.cn

[R36] 并发执行多个任务
来源：http://hdy.nwbrower.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://awc.yanxiufei.cn

[R37] 把输出赋给变量
来源：http://kcz.xinyue.icu

files=$(ls -1)
来源：http://vfb.shangyingyoupin.top

[R38] 管道串联
来源：http://asr.dashuyun.cn

cat a.txt | grep -i error | wc -l
来源：http://efh.zhengqikj.top

[R39] 重定向标准输出与错误
来源：http://mxw.jlsjyb.cn

cmd > out.log 2>&1
来源：http://ufw.dianchejie.cn

[R40] 追加写日志
来源：http://dha.birdmap.top

echo "log" >> out.log
来源：http://fzg.shanyushiyangkeji.top

[R41] 丢弃输出
来源：http://sno.chenlongwang.top

cmd >/dev/null 2>&1
来源：http://rwu.shanyushiyangkeji.top

[R42] 输入重定向
来源：http://cdl.daria6918.cn

wc -l < a.txt
来源：http://gfb.yj202588.top

[R43] 按名字查找文件
来源：http://ers.zycfv.cn

find . -name "*.log" -type f
来源：http://jov.pycfn.com

[R44] 按修改时间查找
来源：http://fuk.fktsv.cn

find . -mtime -7 -type f
来源：http://mjc.nwbrower.top

[R45] 批量删除
来源：http://lwo.jianghu66.top

find . -name "*.tmp" -delete
来源：http://xcy.hammf.cn

[R46] 递归替换文件内容
来源：http://cem.ydjk.org.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://bum.fehbvm.com

[R47] sed 单行替换
来源：http://kgd.bjfxy.top

sed -i 's/foo/bar/g' a.txt
来源：http://vac.chenlongwang.top

[R48] awk 取指定列
来源：http://dlt.cucudq.cn

awk '{print $1, $3}' a.txt
来源：http://gbb.redwolf501.top

[R49] awk 带条件
来源：http://alx.redwolf501.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://imw.tarul.cn

[R50] awk 求和
来源：http://npr.aizwys.cn

awk '{s += $2} END {print s}' a.txt
来源：http://dhi.yongpay.top

[R51] 排序去重取前几
来源：http://leh.gzhubu.top

sort a.txt | uniq -c | sort -rn | head
来源：http://jtq.haohaochexian.top

[R52] 统计行数
来源：http://vbb.ydzc1.top

wc -l a.txt
来源：http://wld.ydjk.org.cn

[R53] 查看文件头与实时尾
来源：http://nrr.gotoacloud.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://uyd.chenlongwang.top

[R54] 比较两个文件
来源：http://gyk.daxiang520.top

diff a.txt b.txt
来源：http://yrj.hywenlv.cn

[R55] 压缩与解压
来源：http://xwq.jianghu66.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://kjp.hesvh.cn

[R56] 远程拷贝
来源：http://udr.yonumen.top

scp file user@host:/path/
来源：http://mvd.zhiwuduotai.top

[R57] 远程执行命令
来源：http://ctp.ctjpmb.com

ssh user@host 'uptime'
来源：http://abc.ivvv.top

[R58] 下载文件
来源：http://dye.316326.xyz

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://aqk.zhaomingkeji.xyz

[R59] 发 POST JSON
来源：http://kfh.ctjpmb.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://rhm.zhongyouzk.top

[R60] 只看 HTTP 状态码
来源：http://gnn.pengpengdd.cyou

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://cxr.sysykeji.top

[R61] 磁盘占用
来源：http://ngv.havefunace.top

df -h;  du -sh *
来源：http://acq.shanyushiyangkeji.top

[R62] 找最占空间的文件
来源：http://gkx.shzxlz.cn

du -ah . | sort -rh | head -10
来源：http://brx.hfpthk.cn

[R63] 内存与进程
来源：http://ehk.wangshuangyany.cn

free -h;  ps aux | grep nginx
来源：http://mtb.bbcook.cn

[R64] 结束进程
来源：http://rfr.yvedp.cn

kill -9 $(pgrep -f app.py)
来源：http://erb.sxryk.cn

[R65] 查看端口占用
来源：http://sxe.nanxinkj.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://zzu.haohaochexian.top

[R66] 定时任务
来源：http://niy.shzxlz.cn

crontab -e;  crontab -l
来源：http://cgk.meibo888.top

[R67] 生成随机十六进制串
来源：http://nku.jinghuilouyu.cn


<!-- 参考信息 -->