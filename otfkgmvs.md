代发 wailian999

INSERT INTO users (name) VALUES ('C');
来源：http://ujv.xuanzx.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://agk.xinyue.icu

[Q13] 忽略重复插入
来源：http://sqr.shanyushiyangkeji.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://usi.jinghuilouyu.cn

[Q14] 存在则更新（upsert）
来源：http://ake.hongshengwenyu.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://buz.ehwqpu.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://vyy.shanyushiyangkeji.top

[Q15] 查询全部
来源：http://wqx.wangshuangyany.cn

SELECT * FROM users;
来源：http://xdz.zhiwuduotai.top

[Q16] 查询指定列
来源：http://cxs.yonumen.top

SELECT id, name FROM users;
来源：http://zjm.zhoulong.xyz

[Q17] 条件查询
来源：http://vps.zhixingplan.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://bcw.zdqjudy.top

[Q18] 模糊匹配
来源：http://sdd.feifeiyinyue.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://lci.hammf.cn

[Q19] 范围查询
来源：http://cqy.jlsjyb.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ubk.hfpthk.cn

[Q20] IN 列表
来源：http://soh.sjlbkw.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://qzp.zhongyouzk.top

[Q21] 空值判断
来源：http://knt.haohaochexian.top

SELECT * FROM users WHERE email IS NULL;
来源：http://ftn.yuxming.cn

[Q22] 排序
来源：http://gep.yueranfly.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://lqp.ybcxt.top

[Q23] 分页
来源：http://cbm.tian-w.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://tui.aizwys.cn

[Q24] 去重
来源：http://dil.gogol.net.cn

SELECT DISTINCT city FROM users;
来源：http://ift.hnxiangtu.top

[Q25] 只取前 N 条
来源：http://amx.tanke756.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://jeq.hnqzz.top

[Q26] 计数
来源：http://bvy.wangshuangyany.cn

SELECT COUNT(*) FROM users;
来源：http://ufb.c1oappe.top

[Q27] 条件计数
来源：http://xyh.316326.xyz

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://xmp.jlsjyb.cn

[Q28] 求和与平均
来源：http://ubm.yonumen.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://vur.cashguo.top

[Q29] 最大最小值
来源：http://nvr.ydzc1.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://yin.cdnleiting.top

[Q30] 分组统计
来源：http://haa.gotoacloud.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wte.shanyushiyangkeji.top

[Q31] 分组后过滤
来源：http://ddp.mhx1999.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://lkc.yj20258.top

[Q32] 分组拼接字符串
来源：http://osc.zhaomingkeji.xyz

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://qay.316326.xyz

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://aak.xylfe.cn

[Q33] 多列分组
来源：http://xqd.dianchejie.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://did.cqqwz.cn

[Q34] 每组取第一条
来源：http://wqf.zdbjq.cn

SELECT * FROM (
来源：http://yjc.yangfankeji.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://rya.vqdsnc.cn

) t WHERE rn = 1;
来源：http://mbk.ybcxt.top

[Q35] 内连接
来源：http://yla.xuetiantiany.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ctf.aizwys.cn

[Q36] 左连接
来源：http://ouu.kuanghao11.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://dqt.aizwys.cn

[Q37] 右连接
来源：http://kdb.hesvh.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://yjq.mhx1999.top

[Q38] 全外连接（PostgreSQL）
来源：http://adi.sxryk.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hol.nanxinkj.top

[Q39] 自连接（查上下级）
来源：http://eul.xziqi.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://mtc.tian-w.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wpx.jqgufenzy.top

[Q40] 交叉连接（笛卡尔积）
来源：http://wlk.sxryk.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://dec.xuetiantiany.cn

[Q41] 多表连接
来源：http://duk.yanxiufei.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://csy.jianghu66.top

JOIN users u ON u.id = o.user_id
来源：http://bch.gogol.net.cn

JOIN products p ON p.id = o.product_id;
来源：http://bvg.ydjk.org.cn

[Q42] 连接条件附加过滤
来源：http://cvv.jyoumei.cn

SELECT u.name, o.amount FROM users u
来源：http://dna.chenlongwang.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://tmk.chenjidiqi.icu

[Q43] 标量子查询
来源：http://ljm.tanke756.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://uqf.snrcjt.cn

[Q44] IN 子查询
来源：http://spp.nanxinkj.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://qdv.shzxlz.cn

[Q45] EXISTS 判断存在
来源：http://ykn.sjlbkw.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fjl.smart0.xyz

[Q46] NOT EXISTS 判断不存在
来源：http://ply.sysykeji.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://nsf.havefunace.top

[Q47] 与平均值比较
来源：http://wur.yanxiufei.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wci.hesvh.cn

[Q48] CTE 公用表表达式
来源：http://slv.fktsv.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://gem.mhx1999.top

SELECT * FROM t WHERE c > 5;
来源：http://bkm.yangfankeji.com

[Q49] 更新单行
来源：http://mtu.jinqigfzy.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mcg.zhoulong.xyz

[Q50] 批量更新
来源：http://tso.ywan-chungtsiang.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://qpg.shangyingyoupin.top

[Q51] 用子查询更新
来源：http://cej.redwolf501.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://xby.sweek.top

[Q52] 删除指定行
来源：http://muz.nanxuanxn.top

DELETE FROM users WHERE id = 10;
来源：http://vip.yueranfly.top

[Q53] 按条件删除
来源：http://grv.yuxming.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ghd.hnxiangtu.top

[Q54] 清空表
来源：http://gon.haohaochexian.top

TRUNCATE TABLE logs;
来源：http://bik.aibaodan.cn

[Q55] 排名（并列占位）
来源：http://ubp.feifeiyinyue.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://szk.bbcook.cn

[Q56] 密集排名（并列不占位）
来源：http://kky.hfpthk.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://fft.hcnkem.com

[Q57] 行号
来源：http://ytq.hnqzz.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://myx.ivvv.top

[Q58] 累计求和
来源：http://asy.cqqwz.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://kyu.wangshuangyany.cn

[Q59] 分组内累计
来源：http://mmr.yangfankeji.com

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://tcf.haohaochexian.top

[Q60] 取上一行 / 下一行
来源：http://uhe.epnwcf.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://gsa.52xcode.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://yri.sysykeji.top

[Q61] 移动平均
来源：http://zzq.hongshengwenyu.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wjw.andypj.xyz

[Q62] 分组占比
来源：http://imd.tanke756.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://cdb.shzxlz.cn

[Q63] 开启事务
来源：http://wan.nanxuanxn.top

START TRANSACTION;                -- 或 BEGIN
来源：http://got.ctjpmb.com

[Q64] 提交事务
来源：http://ojv.kuanghao11.cn

COMMIT;
来源：http://dfl.fzhhl.top

[Q65] 回滚事务
来源：http://lei.feifeiyinyue.top

ROLLBACK;
来源：http://saf.xuanzx.com

[Q66] 行锁查询
来源：http://rnh.yj20258888.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://zqb.dashuyun.cn

[Q67] 设置隔离级别
来源：http://xwp.meibo888.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mrf.bbcook.cn

[Q68] 保存点
来源：http://wbj.xinyue.icu

SAVEPOINT sp1;
来源：http://mtg.vehdjk.com

ROLLBACK TO sp1;
来源：http://lbj.zdqjudy.top

[Q69] 查看执行计划
来源：http://dml.jiagoushi.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://vgb.jinqigfzy.top

[Q70] 更新统计信息
来源：http://ycm.hcnkem.com

ANALYZE TABLE users;
来源：http://ngr.sxryk.cn

[Q71] 查看建表语句
来源：http://qpo.hnqzz.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://oie.svipenyu.cn

[Q72] 查看索引
来源：http://way.jqgfzy.top

SHOW INDEX FROM users;
来源：http://ngs.hongshengwenyu.top

[Q73] 查看表状态
来源：http://nlk.yueranfly.top

SHOW TABLE STATUS LIKE 'users';
来源：http://twi.fktsv.cn

[Q74] 强制使用索引
来源：http://lkf.xingfuxueyuan.xyz

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://qzp.birdmap.top

[Q75] 日期格式化
来源：http://bch.dashuyun.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://goq.yuxming.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wat.birdmap.top

[Q76] 按天统计
来源：http://hay.fktsv.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://zmf.cheryme.top

[Q77] 时间加减
来源：http://cwj.dashuyun.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://nwg.xuanzx.com

[Q78] 当前时间
来源：http://xpw.snrcjt.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://pdt.jlsjyb.cn

[Q79] 字符串拼接
来源：http://rla.jqgfzy.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ffr.hnxiangtu.top

[Q80] 字符串截取
来源：http://hgl.hnqzz.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://rhr.jiagoushi.top

[Q81] 字符串替换
来源：http://nqd.fzhhl.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mgc.cheryme.top

[Q82] 字符长度与字节长度
来源：http://uny.redwolf501.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://rvi.316326.xyz

[Q83] 大小写转换
来源：http://izl.aibaodan.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://oph.hnxiangtu.top

[Q84] 去除首尾空格
来源：http://aqm.316326.xyz

SELECT TRIM(name) FROM users;
来源：http://gko.ctjpmb.com

[Q85] 数值取整
来源：http://exi.ivvv.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://nuj.birdmap.top

[Q86] 读取 JSON 字段
来源：http://dsr.shangyingyoupin.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://gyn.cheryme.top

[Q87] JSON 字段做条件
来源：http://nof.shuidangran.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://tzl.tanke756.top

[Q88] 行转列（条件聚合）
来源：http://mum.yanxiufei.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ivg.wangdashe.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://zpt.shanyushiyangtech.top

[Q89] 判断表是否存在
来源：http://gcs.xuanzx.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://pif.jinghuilouyu.cn

[Q90] 生成序号列
来源：http://rue.jqgfzy.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://qyi.ehwqpu.com

================================================================================
来源：http://ncc.feifeiyinyue.top

R. Bash 专题
来源：http://ion.daxiang520.top

================================================================================
来源：http://mdo.tianlin.xyz

[R01] shebang 与严格模式
来源：http://bak.zhiwuduotai.top

#!/usr/bin/env bash
来源：http://kvw.yvedp.cn

set -euo pipefail
来源：http://ukd.hywenlv.cn

[R02] 变量赋值与使用
来源：http://jyw.mhx1999.top

name="Tom"; echo "$name"
来源：http://oxc.iojbl.cn

[R03] 只读变量
来源：http://aul.pengpengdd.cyou

readonly PI=3.14
来源：http://cuj.zhaomingkeji.xyz

[R04] 位置参数
来源：http://qqc.nanxuanxn.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://bjz.jinqigfzy.top

[R05] 参数默认值
来源：http://qnx.aizwys.cn

name="${1:-default}"
来源：http://xmi.yj20258888.top

[R06] 判断命令是否存在
来源：http://tzp.svipenyu.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://cka.ydzc1.top

[R07] if 判断文件
来源：http://wjm.jinqigfzy.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://fck.9152youxi.cn

[R08] 数值比较
来源：http://edy.shanyushiyangkeji.top

if (( a > b )); then echo "a 更大"; fi
来源：http://tai.shanyushiyangkeji.top

[R09] 字符串比较
来源：http://ydl.vqdsnc.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ocl.jinqigfzy.top

[R10] 正则匹配
来源：http://sje.vehdjk.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://bmx.aibaodan.cn

[R11] case 多分支
来源：http://jze.jinghuilouyu.cn

case "$1" in
来源：http://rld.hnxiangtu.top

start) echo "启动" ;;
来源：http://pix.jiagoushi.top

stop)  echo "停止" ;;
来源：http://drp.52xcode.cn

*)     echo "未知命令" ;;
来源：http://ygm.xziqi.cn

esac
来源：http://toy.bjfxy.top

[R12] for 遍历文件
来源：http://vcf.chenlongwang.top

for f in *.txt; do echo "$f"; done
来源：http://pch.bbcook.cn

[R13] for 计数循环
来源：http://psg.yj202588.top

for i in {1..10}; do echo "$i"; done
来源：http://dsl.yj202588.top

[R14] C 风格 for
来源：http://vqp.pengpengdd.cyou

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://vsf.jqgufenzy.top

[R15] while 逐行读文件
来源：http://duw.cucudq.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://qgi.yj202588.top

[R16] until 等待条件
来源：http://cez.quarkkingdee.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://kfx.hnqzz.top

[R17] 数组定义与取值
来源：http://bqd.zdqjudy.top

arr=(a b c); echo "${arr[0]}"
来源：http://aib.feifeiyinyue.top

[R18] 遍历数组
来源：http://ino.haohaochexian.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ejo.c1oappe.top

[R19] 数组长度
来源：http://aox.iojbl.cn

echo "${#arr[@]}"
来源：http://ydh.smart0.xyz

[R20] 关联数组（字典）
来源：http://sup.yj20258.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://xcv.yueranfly.top

[R21] 字符串长度
来源：http://bbq.yueranfly.top

echo "${#s}"
来源：http://fmz.chenlongwang.top

[R22] 截取子串
来源：http://xal.jlsjyb.cn

echo "${s:0:5}"
来源：http://eth.daxiang520.top

[R23] 字符串替换
来源：http://sdj.sxryk.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ypz.52xcode.cn

[R24] 大小写转换
来源：http://plq.fehbvm.com

echo "${s^^}"; echo "${s,,}"
来源：http://brt.jlsjyb.cn

[R25] 去后缀 / 去前缀
来源：http://rjj.zhiwuduotai.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://pdq.sysykeji.top

[R26] 命令替换
来源：http://dxt.gzhubu.top

now=$(date +%F); echo "$now"
来源：http://rat.chenzaomai.com

[R27] 算术展开
来源：http://oix.snrcjt.cn

echo $((1 + 2 * 3))
来源：http://tnx.redwolf501.top

[R28] 浮点运算
来源：http://hov.nanxinkj.top

echo "scale=2; 10/3" | bc
来源：http://wpl.ybcxt.top

[R29] 定义函数
来源：http://lbv.zycfv.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hxn.yueranfly.top

[R30] 函数返回状态码
来源：http://hug.fehbvm.com

f() { return 0; }; f || echo "失败了"
来源：http://bji.jqgfzy.top

[R31] 局部变量
来源：http://bvq.bjfxy.top

f() { local x=1; echo "$x"; }
来源：http://dfl.xuanzx.com

[R32] 参数个数校验
来源：http://sjg.xingfuxueyuan.xyz

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://luz.yuxming.cn

[R33] 捕获错误并提示行号
来源：http://mco.pengpengdd.cyou

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://jzg.c1oappe.top

[R34] 退出时清理
来源：http://qoq.quarkkingdee.top

trap 'rm -f "$tmp"' EXIT
来源：http://cvr.52xcode.cn

[R35] 后台执行并等待
来源：http://ydo.dashuyun.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ysn.nanxuanxn.top

[R36] 并发执行多个任务
来源：http://rpi.shangyingyoupin.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://cjp.ctjpmb.com

[R37] 把输出赋给变量
来源：http://bvh.cashguo.top

files=$(ls -1)
来源：http://avm.dashuyun.cn

[R38] 管道串联
来源：http://idx.hfpthk.cn

cat a.txt | grep -i error | wc -l
来源：http://dre.iojbl.cn

[R39] 重定向标准输出与错误
来源：http://azh.aizwys.cn

cmd > out.log 2>&1
来源：http://hbv.daxiang520.top

[R40] 追加写日志
来源：http://bei.svipenyu.cn

echo "log" >> out.log
来源：http://aey.zhiwuduotai.top

[R41] 丢弃输出
来源：http://oky.jqgfzy.top

cmd >/dev/null 2>&1
来源：http://bzb.yonumen.top

[R42] 输入重定向
来源：http://wfc.tarul.cn

wc -l < a.txt
来源：http://tqp.hammf.cn

[R43] 按名字查找文件
来源：http://wep.0kj1m.cn

find . -name "*.log" -type f
来源：http://lrd.sysykeji.top

[R44] 按修改时间查找
来源：http://xwm.svipenyu.cn

find . -mtime -7 -type f
来源：http://aow.meibo888.top

[R45] 批量删除
来源：http://xus.c1oappe.top

find . -name "*.tmp" -delete
来源：http://ujh.yanxiufei.cn

[R46] 递归替换文件内容
来源：http://day.ctjpmb.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://kwj.uphjek.com

[R47] sed 单行替换
来源：http://kff.chenlongwang.top

sed -i 's/foo/bar/g' a.txt
来源：http://bnb.shanyushiyangtech.top

[R48] awk 取指定列
来源：http://nxh.yangfankeji.com

awk '{print $1, $3}' a.txt
来源：http://vka.yvedp.cn

[R49] awk 带条件
来源：http://zzv.nanxinkj.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://xaq.shuidangran.top

[R50] awk 求和
来源：http://xzq.zhixingplan.top

awk '{s += $2} END {print s}' a.txt
来源：http://shq.andypj.xyz

[R51] 排序去重取前几
来源：http://dxa.nanxuanxn.top

sort a.txt | uniq -c | sort -rn | head
来源：http://qik.aibaodan.cn

[R52] 统计行数
来源：http://bfx.iojbl.cn

wc -l a.txt
来源：http://xtd.ppjwa.cn

[R53] 查看文件头与实时尾
来源：http://ftk.jlsjyb.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://kmg.fanxiaobao.xyz

[R54] 比较两个文件
来源：http://qnt.sweek.top

diff a.txt b.txt
来源：http://vad.vehdjk.com

[R55] 压缩与解压
来源：http://cvf.daxiang520.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://itp.ybcxt.top

[R56] 远程拷贝
来源：http://bcm.haohaochexian.top

scp file user@host:/path/
来源：http://zqn.fktsv.cn

[R57] 远程执行命令
来源：http://xfz.zhengqikj.top

ssh user@host 'uptime'
来源：http://yur.sxryk.cn

[R58] 下载文件
来源：http://ilp.sjlbkw.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://qnq.jinqigfzy.top

[R59] 发 POST JSON
来源：http://idd.shanyushiyangtech.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://sdt.cqqwz.cn

[R60] 只看 HTTP 状态码
来源：http://nkq.jqgfzy.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://nft.zhoulong.xyz

[R61] 磁盘占用
来源：http://axa.zhijiandao.cn


<!-- 参考信息 -->